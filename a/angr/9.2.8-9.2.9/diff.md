# Comparing `tmp/angr-9.2.8.tar.gz` & `tmp/angr-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angr-9.2.8.tar", last modified: Tue Jun 28 17:04:05 2022, max compression
+gzip compressed data, was "angr-9.2.9.tar", last modified: Tue Jul  5 17:03:21 2022, max compression
```

## Comparing `angr-9.2.8.tar` & `angr-9.2.9.tar`

### file list

```diff
@@ -1,1243 +1,1244 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.277489 angr-9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-06-28 17:01:19.000000 angr-9.2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-06-28 17:01:19.000000 angr-9.2.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     3181 2022-06-28 17:04:05.277489 angr-9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2641 2022-06-28 17:01:19.000000 angr-9.2.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.021468 angr-9.2.8/angr/
--rw-r--r--   0 vsts      (1001) docker     (121)     2774 2022-06-28 17:01:35.000000 angr-9.2.8/angr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.025469 angr-9.2.8/angr/analyses/
--rw-r--r--   0 vsts      (1001) docker     (121)     1751 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10185 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (121)    27512 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/backward_slice.py
--rw-r--r--   0 vsts      (1001) docker     (121)    26401 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/binary_optimizer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    52237 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/bindiff.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2233 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/boyscout.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2724 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/callee_cleanup_finder.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25838 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/calling_convention.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6418 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cdg.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.025469 angr-9.2.8/angr/analyses/cfg/
--rw-r--r--   0 vsts      (1001) docker     (121)      354 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14692 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfb.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3125 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3155 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg_arch_options.py
--rw-r--r--   0 vsts      (1001) docker     (121)   114825 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)   155853 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg_emulated.py
--rw-r--r--   0 vsts      (1001) docker     (121)   212555 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg_fast.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25948 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg_fast_soot.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5737 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg_job_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7746 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/cfg_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.025469 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/
--rw-r--r--   0 vsts      (1001) docker     (121)      317 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1747 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3146 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2938 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1194 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py
--rw-r--r--   0 vsts      (1001) docker     (121)    77780 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8493 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2794 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/resolver.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2916 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1283 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20414 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg/segment_list.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.029469 angr-9.2.8/angr/analyses/cfg_slice_to_sink/
--rw-r--r--   0 vsts      (1001) docker     (121)      120 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg_slice_to_sink/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4072 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3656 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg_slice_to_sink/graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/cfg_slice_to_sink/transitions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3334 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/class_identifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3673 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/code_tagging.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12684 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/complete_calling_conventions.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16352 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/congruency_check.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.029469 angr-9.2.8/angr/analyses/data_dep/
--rw-r--r--   0 vsts      (1001) docker     (121)      180 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/data_dep/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25414 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/data_dep/data_dependency_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4649 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/data_dep/dep_nodes.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1522 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/data_dep/sim_act_location.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3348 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/datagraph_meta.py
--rw-r--r--   0 vsts      (1001) docker     (121)    63069 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/ddg.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.029469 angr-9.2.8/angr/analyses/decompiler/
--rw-r--r--   0 vsts      (1001) docker     (121)      549 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    39491 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/ail_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16416 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/ailblock_walker.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1603 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/ailgraph_walker.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12835 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/block_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14084 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/callsite_maker.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.029469 angr-9.2.8/angr/analyses/decompiler/ccall_rewriters/
--rw-r--r--   0 vsts      (1001) docker     (121)      102 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/ccall_rewriters/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5965 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py
--rw-r--r--   0 vsts      (1001) docker     (121)      438 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/ccall_rewriters/rewriter_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)    43724 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/clinic.py
--rw-r--r--   0 vsts      (1001) docker     (121)    44213 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/condition_processor.py
--rw-r--r--   0 vsts      (1001) docker     (121)      841 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/decompilation_cache.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/decompilation_options.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12805 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/decompiler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6691 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/empty_node_remover.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3568 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/expression_narrower.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6077 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/graph_region.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.033469 angr-9.2.8/angr/analyses/decompiler/optimization_passes/
--rw-r--r--   0 vsts      (1001) docker     (121)     2144 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5320 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9478 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/const_derefs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16857 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/div_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8906 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/eager_returns.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10177 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7528 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2950 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/mod_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10466 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/multi_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5622 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/optimization_pass.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7466 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6207 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11678 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2961 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.037470 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/
--rw-r--r--   0 vsts      (1001) docker     (121)     2109 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1865 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1475 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py
--rw-r--r--   0 vsts      (1001) docker     (121)      999 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1272 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1289 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py
--rw-r--r--   0 vsts      (1001) docker     (121)      611 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2491 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/base.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1043 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py
--rw-r--r--   0 vsts      (1001) docker     (121)      956 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py
--rw-r--r--   0 vsts      (1001) docker     (121)      936 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3275 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/bswap.py
--rw-r--r--   0 vsts      (1001) docker     (121)      908 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py
--rw-r--r--   0 vsts      (1001) docker     (121)      967 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2452 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1432 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/conv_const_mull_a_shift.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2062 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/eager_eval.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1937 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1042 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py
--rw-r--r--   0 vsts      (1001) docker     (121)      525 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1157 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1545 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3480 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1152 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py
--rw-r--r--   0 vsts      (1001) docker     (121)      531 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1441 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1331 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py
--rw-r--r--   0 vsts      (1001) docker     (121)      941 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py
--rw-r--r--   0 vsts      (1001) docker     (121)    33401 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_identifier.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.037470 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/
--rw-r--r--   0 vsts      (1001) docker     (121)       48 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3894 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2593 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14125 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/expr_folding.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3609 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/goto.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5022 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/if_.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2546 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/ifelse.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5065 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/loop.py
--rw-r--r--   0 vsts      (1001) docker     (121)      564 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/node_address_finder.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4943 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_simplifiers/region_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)      716 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/region_walker.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5929 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/sequence_walker.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.041470 angr-9.2.8/angr/analyses/decompiler/structured_codegen/
--rw-r--r--   0 vsts      (1001) docker     (121)      284 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/structured_codegen/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3848 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/structured_codegen/base.py
--rw-r--r--   0 vsts      (1001) docker     (121)   100865 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/structured_codegen/c.py
--rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/structured_codegen/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6705 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/structured_codegen/dwarf_import.py
--rw-r--r--   0 vsts      (1001) docker     (121)    72110 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/structurer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7923 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/structurer_nodes.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9436 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/decompiler/utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)    38206 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/disassembly.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2988 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/disassembly_utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1247 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/dominance_frontier.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10823 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/find_objects_static.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7803 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/flirt.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.041470 angr-9.2.8/angr/analyses/forward_analysis/
--rw-r--r--   0 vsts      (1001) docker     (121)      144 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18933 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/forward_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1502 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/job_info.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.041470 angr-9.2.8/angr/analyses/forward_analysis/visitors/
--rw-r--r--   0 vsts      (1001) docker     (121)      174 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/visitors/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      732 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/visitors/call_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1338 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/visitors/function_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7811 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/visitors/graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)      725 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/visitors/loop.py
--rw-r--r--   0 vsts      (1001) docker     (121)      779 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/forward_analysis/visitors/single_node_graph.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.041470 angr-9.2.8/angr/analyses/identifier/
--rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4538 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/custom_callable.py
--rw-r--r--   0 vsts      (1001) docker     (121)      158 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/errors.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1714 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/func.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.045470 angr-9.2.8/angr/analyses/identifier/functions/
--rw-r--r--   0 vsts      (1001) docker     (121)     1062 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2121 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/atoi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3317 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/based_atoi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4343 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/fdprintf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1944 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/free.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8760 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/int2str.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3854 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/malloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1963 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/memcmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3153 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/memcpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1193 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/memset.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4295 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/printf.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11558 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/recv_until.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2363 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/skip_calloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3192 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/skip_realloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2910 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/skip_recv_n.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4189 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/snprintf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4130 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/sprintf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      821 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/strcasecmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3509 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/strcmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1193 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)      751 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/strlen.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3347 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/strncmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2014 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/strncpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2435 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/functions/strtol.py
--rw-r--r--   0 vsts      (1001) docker     (121)    33116 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/identify.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13825 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/identifier/runner.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8604 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/init_finder.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9333 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/loop_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7214 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/loopfinder.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.049471 angr-9.2.8/angr/analyses/propagator/
--rw-r--r--   0 vsts      (1001) docker     (121)       44 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      551 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/call_expr_finder.py
--rw-r--r--   0 vsts      (1001) docker     (121)    39786 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1134 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8736 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6116 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/outdated_definition_walker.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7136 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/prop_value.py
--rw-r--r--   0 vsts      (1001) docker     (121)    27240 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/propagator.py
--rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/top_checker_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/values.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1401 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/propagator/vex_vars.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15285 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/proximity_graph.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.049471 angr-9.2.8/angr/analyses/reaching_definitions/
--rw-r--r--   0 vsts      (1001) docker     (121)     1258 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2232 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/call_trace.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7785 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/dep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)    41873 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (121)    51117 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (121)      242 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/external_codeloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5958 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/function_handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2632 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/heap_allocator.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19861 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/rd_state.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16703 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/reaching_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reaching_definitions/subject.py
--rw-r--r--   0 vsts      (1001) docker     (121)   100773 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/reassembler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8942 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/soot_class_hierarchy.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19938 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/stack_pointer_tracker.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1709 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/static_hooker.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.049471 angr-9.2.8/angr/analyses/typehoon/
--rw-r--r--   0 vsts      (1001) docker     (121)       32 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/typehoon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1676 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/typehoon/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25122 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/typehoon/simple_solver.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8340 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/typehoon/translator.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3688 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/typehoon/typeconsts.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8717 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/typehoon/typehoon.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13526 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/typehoon/typevars.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.053471 angr-9.2.8/angr/analyses/variable_recovery/
--rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/annotations.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20317 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (121)    38254 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14919 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (121)    23287 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/variable_recovery.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13000 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/variable_recovery_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21420 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/variable_recovery/variable_recovery_fast.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25486 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/veritesting.py
--rw-r--r--   0 vsts      (1001) docker     (121)    73710 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/vfg.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16358 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/vsa_ddg.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4142 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/vtable.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9479 2022-06-28 17:01:19.000000 angr-9.2.8/angr/analyses/xrefs.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.053471 angr-9.2.8/angr/angrdb/
--rw-r--r--   0 vsts      (1001) docker     (121)      243 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6401 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/db.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4939 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/models.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.053471 angr-9.2.8/angr/angrdb/serializers/
--rw-r--r--   0 vsts      (1001) docker     (121)       78 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1323 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/cfg_model.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1514 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/comments.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1700 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/funcs.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3689 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/kb.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1408 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/labels.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2125 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/loader.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4380 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/structured_code.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2453 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/variables.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1287 2022-06-28 17:01:19.000000 angr-9.2.8/angr/angrdb/serializers/xrefs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10929 2022-06-28 17:01:19.000000 angr-9.2.8/angr/annocfg.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15184 2022-06-28 17:01:19.000000 angr-9.2.8/angr/blade.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14018 2022-06-28 17:01:19.000000 angr-9.2.8/angr/block.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5539 2022-06-28 17:01:19.000000 angr-9.2.8/angr/callable.py
--rw-r--r--   0 vsts      (1001) docker     (121)    85459 2022-06-28 17:01:19.000000 angr-9.2.8/angr/calling_conventions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3526 2022-06-28 17:01:19.000000 angr-9.2.8/angr/code_location.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3828 2022-06-28 17:01:19.000000 angr-9.2.8/angr/codenode.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.053471 angr-9.2.8/angr/concretization_strategies/
--rw-r--r--   0 vsts      (1001) docker     (121)     3724 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      440 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/any.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/controlled_data.py
--rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/eval.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1039 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/max.py
--rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/nonzero.py
--rw-r--r--   0 vsts      (1001) docker     (121)      825 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/nonzero_range.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1464 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/norepeats.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1633 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/norepeats_range.py
--rw-r--r--   0 vsts      (1001) docker     (121)      587 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/range.py
--rw-r--r--   0 vsts      (1001) docker     (121)      357 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/single.py
--rw-r--r--   0 vsts      (1001) docker     (121)      570 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/solutions.py
--rw-r--r--   0 vsts      (1001) docker     (121)      526 2022-06-28 17:01:19.000000 angr-9.2.8/angr/concretization_strategies/unlimited_range.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.053471 angr-9.2.8/angr/distributed/
--rw-r--r--   0 vsts      (1001) docker     (121)      141 2022-06-28 17:01:19.000000 angr-9.2.8/angr/distributed/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6501 2022-06-28 17:01:19.000000 angr-9.2.8/angr/distributed/server.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6076 2022-06-28 17:01:19.000000 angr-9.2.8/angr/distributed/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.057471 angr-9.2.8/angr/engines/
--rw-r--r--   0 vsts      (1001) docker     (121)     1066 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7379 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/concrete.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7910 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/engine.py
--rw-r--r--   0 vsts      (1001) docker     (121)      992 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/failure.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2472 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/hook.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.057471 angr-9.2.8/angr/engines/light/
--rw-r--r--   0 vsts      (1001) docker     (121)      187 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/light/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16743 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/light/data.py
--rw-r--r--   0 vsts      (1001) docker     (121)    37154 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/light/engine.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.057471 angr-9.2.8/angr/engines/pcode/
--rw-r--r--   0 vsts      (1001) docker     (121)       64 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/pcode/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4119 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/pcode/arch.py
--rw-r--r--   0 vsts      (1001) docker     (121)    28477 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/pcode/behavior.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13837 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/pcode/emulate.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9493 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/pcode/engine.py
--rw-r--r--   0 vsts      (1001) docker     (121)    49058 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/pcode/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2473 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/procedure.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.057471 angr-9.2.8/angr/engines/soot/
--rw-r--r--   0 vsts      (1001) docker     (121)       31 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17456 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/engine.py
--rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.061472 angr-9.2.8/angr/engines/soot/expressions/
--rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      859 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/arrayref.py
--rw-r--r--   0 vsts      (1001) docker     (121)      508 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/base.py
--rw-r--r--   0 vsts      (1001) docker     (121)      781 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/binop.py
--rw-r--r--   0 vsts      (1001) docker     (121)      903 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/cast.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1252 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/condition.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1390 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/constants.py
--rw-r--r--   0 vsts      (1001) docker     (121)      314 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/instanceOf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/instancefieldref.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4884 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/invoke.py
--rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/length.py
--rw-r--r--   0 vsts      (1001) docker     (121)      216 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/local.py
--rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/new.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2036 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/newArray.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3326 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/newMultiArray.py
--rw-r--r--   0 vsts      (1001) docker     (121)      225 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/paramref.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1163 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/phi.py
--rw-r--r--   0 vsts      (1001) docker     (121)      233 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/staticfieldref.py
--rw-r--r--   0 vsts      (1001) docker     (121)      150 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/thisref.py
--rw-r--r--   0 vsts      (1001) docker     (121)      114 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/expressions/unsupported.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1958 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/field_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1834 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/method_dispatcher.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.061472 angr-9.2.8/angr/engines/soot/statements/
--rw-r--r--   0 vsts      (1001) docker     (121)      884 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1272 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/assign.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2115 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/base.py
--rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/goto.py
--rw-r--r--   0 vsts      (1001) docker     (121)      422 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/identity.py
--rw-r--r--   0 vsts      (1001) docker     (121)      583 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/if_.py
--rw-r--r--   0 vsts      (1001) docker     (121)      285 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/invoke.py
--rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/return_.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1325 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/switch.py
--rw-r--r--   0 vsts      (1001) docker     (121)      384 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/statements/throw.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.061472 angr-9.2.8/angr/engines/soot/values/
--rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4365 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/arrayref.py
--rw-r--r--   0 vsts      (1001) docker     (121)      123 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/base.py
--rw-r--r--   0 vsts      (1001) docker     (121)      436 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/constants.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1603 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/instancefieldref.py
--rw-r--r--   0 vsts      (1001) docker     (121)      413 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/local.py
--rw-r--r--   0 vsts      (1001) docker     (121)      417 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/paramref.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1250 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/staticfieldref.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1146 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/strref.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6133 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/soot/values/thisref.py
--rw-r--r--   0 vsts      (1001) docker     (121)    23140 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/successors.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2027 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/syscall.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20693 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/unicorn.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.061472 angr-9.2.8/angr/engines/vex/
--rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.065472 angr-9.2.8/angr/engines/vex/claripy/
--rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/claripy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    82545 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/claripy/ccall.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5097 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/claripy/datalayer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    44882 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/claripy/irop.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.065472 angr-9.2.8/angr/engines/vex/heavy/
--rw-r--r--   0 vsts      (1001) docker     (121)      200 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/heavy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8349 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/heavy/actions.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18700 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/heavy/dirty.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14793 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/heavy/heavy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2290 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/heavy/inspect.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3417 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/heavy/resilience.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1180 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/heavy/super_fastpath.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16862 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/lifter.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.065472 angr-9.2.8/angr/engines/vex/light/
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/light/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21607 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/light/light.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1928 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/light/resilience.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2120 2022-06-28 17:01:19.000000 angr-9.2.8/angr/engines/vex/light/slicing.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8096 2022-06-28 17:01:19.000000 angr-9.2.8/angr/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.073473 angr-9.2.8/angr/exploration_techniques/
--rw-r--r--   0 vsts      (1001) docker     (121)     8784 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2579 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/bucketizer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5144 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/cacher.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2210 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/common.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1175 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/dfs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18009 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/director.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3448 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/driller_core.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6155 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/explorer.py
--rw-r--r--   0 vsts      (1001) docker     (121)      568 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/lengthlimiter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2583 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/local_loop_seer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11393 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/loop_seer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3055 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/manual_mergepoint.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1286 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/memory_watcher.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3597 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/oppologist.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5141 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/slicecutor.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9304 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/spiller.py
--rw-r--r--   0 vsts      (1001) docker     (121)      725 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/spiller_db.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2081 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/stochastic.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3183 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/symbion.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/tech_builder.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1531 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/threading.py
--rw-r--r--   0 vsts      (1001) docker     (121)      922 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/timeout.py
--rw-r--r--   0 vsts      (1001) docker     (121)    49118 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/tracer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4408 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/unique.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1394 2022-06-28 17:01:19.000000 angr-9.2.8/angr/exploration_techniques/veritesting.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15873 2022-06-28 17:01:19.000000 angr-9.2.8/angr/factory.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.073473 angr-9.2.8/angr/flirt/
--rw-r--r--   0 vsts      (1001) docker     (121)     4166 2022-06-28 17:01:19.000000 angr-9.2.8/angr/flirt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10375 2022-06-28 17:01:19.000000 angr-9.2.8/angr/flirt/build_sig.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17205 2022-06-28 17:01:19.000000 angr-9.2.8/angr/keyed_region.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.073473 angr-9.2.8/angr/knowledge_base/
--rw-r--r--   0 vsts      (1001) docker     (121)       43 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_base/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4463 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_base/knowledge_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.073473 angr-9.2.8/angr/knowledge_plugins/
--rw-r--r--   0 vsts      (1001) docker     (121)      548 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.077473 angr-9.2.8/angr/knowledge_plugins/cfg/
--rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/cfg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2341 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/cfg/cfg_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18789 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/cfg/cfg_model.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18238 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/cfg/cfg_node.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1998 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/cfg/indirect_jump.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3390 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/cfg/memory_data.py
--rw-r--r--   0 vsts      (1001) docker     (121)      330 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/comments.py
--rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/data.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.077473 angr-9.2.8/angr/knowledge_plugins/functions/
--rw-r--r--   0 vsts      (1001) docker     (121)       78 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/functions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    64306 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/functions/function.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17366 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/functions/function_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11598 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/functions/function_parser.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4977 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/functions/soot_function.py
--rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/indirect_jumps.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.081473 angr-9.2.8/angr/knowledge_plugins/key_definitions/
--rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6654 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/atoms.py
--rw-r--r--   0 vsts      (1001) docker     (121)      457 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/constants.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2640 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/definition.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3315 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/environment.py
--rw-r--r--   0 vsts      (1001) docker     (121)      912 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/heap_address.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3267 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/key_definition_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25708 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/live_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1093 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/rd_model.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1711 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/tag.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1234 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/undefined.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1508 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/unknown_size.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6273 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/key_definitions/uses.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2983 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/labels.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3920 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/patches.py
--rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/plugin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1548 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/propagations.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.081473 angr-9.2.8/angr/knowledge_plugins/structured_code/
--rw-r--r--   0 vsts      (1001) docker     (121)       43 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/structured_code/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2133 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/structured_code/manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.081473 angr-9.2.8/angr/knowledge_plugins/sync/
--rw-r--r--   0 vsts      (1001) docker     (121)       45 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/sync/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9467 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/sync/sync_controller.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1910 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/types.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.081473 angr-9.2.8/angr/knowledge_plugins/variables/
--rw-r--r--   0 vsts      (1001) docker     (121)       61 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/variables/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3685 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/variables/variable_access.py
--rw-r--r--   0 vsts      (1001) docker     (121)    38042 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/variables/variable_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.081473 angr-9.2.8/angr/knowledge_plugins/xrefs/
--rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/xrefs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4360 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/xrefs/xref.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3991 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/xrefs/xref_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)      272 2022-06-28 17:01:19.000000 angr-9.2.8/angr/knowledge_plugins/xrefs/xref_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.085474 angr-9.2.8/angr/misc/
--rw-r--r--   0 vsts      (1001) docker     (121)      237 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2335 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/autoimport.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3950 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/bug_report.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3775 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/hookset.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/import_hooks.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2929 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/loggers.py
--rw-r--r--   0 vsts      (1001) docker     (121)      642 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/picklable_lock.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9553 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/plugins.py
--rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/range.py
--rw-r--r--   0 vsts      (1001) docker     (121)      480 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/testing.py
--rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/ux.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1446 2022-06-28 17:01:19.000000 angr-9.2.8/angr/misc/weakpatch.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.085474 angr-9.2.8/angr/procedures/
--rw-r--r--   0 vsts      (1001) docker     (121)       97 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.085474 angr-9.2.8/angr/procedures/advapi32/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/advapi32/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.089474 angr-9.2.8/angr/procedures/cgc/
--rw-r--r--   0 vsts      (1001) docker     (121)       76 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      218 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/_terminate.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2148 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/allocate.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1857 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/deallocate.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2661 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/fdwait.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2309 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/random.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3718 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/receive.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2285 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/cgc/transmit.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.189482 angr-9.2.8/angr/procedures/definitions/
--rw-r--r--   0 vsts      (1001) docker     (121)    27701 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      460 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (121)   379211 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/glibc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      701 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/libstdcpp.py
--rw-r--r--   0 vsts      (1001) docker     (121)   238847 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/linux_kernel.py
--rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/linux_loader.py
--rw-r--r--   0 vsts      (1001) docker     (121)      601 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/msvcr.py
--rw-r--r--   0 vsts      (1001) docker     (121)      404 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/ntdll.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1816 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/parse_syscalls_from_local_system.py
--rw-r--r--   0 vsts      (1001) docker     (121)    84675 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/parse_win32json.py
--rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/user32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1451 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_aclui.py
--rw-r--r--   0 vsts      (1001) docker     (121)    58240 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_activeds.py
--rw-r--r--   0 vsts      (1001) docker     (121)   570046 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_advapi32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24565 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_advpack.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2856 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_amsi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4595 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3002 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (121)      882 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1091 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1030 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1063 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (121)      933 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3151 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5854 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1021 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2631 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1388 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6054 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3243 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8278 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1499 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1177 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1571 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)      891 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1081 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1364 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1434 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3279 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3785 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3237 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1163 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)      902 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1697 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11013 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1551 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1531 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13539 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12396 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)      796 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1100 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1245 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4664 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5935 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2610 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4262 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1103 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6979 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1380 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py
--rw-r--r--   0 vsts      (1001) docker     (121)      937 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)      996 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1185 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1240 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2446 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1820 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3488 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1013 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_apphelp.py
--rw-r--r--   0 vsts      (1001) docker     (121)    36371 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_authz.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2783 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_avicap32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    33016 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_avifil32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    30164 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_bcrypt.py
--rw-r--r--   0 vsts      (1001) docker     (121)    27283 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_bluetoothapis.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10956 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_bthprops.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24192 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_cabinet.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7474 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_certadm.py
--rw-r--r--   0 vsts      (1001) docker     (121)    61551 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_certpoleng.py
--rw-r--r--   0 vsts      (1001) docker     (121)   109314 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_cfgmgr32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    35359 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_chakra.py
--rw-r--r--   0 vsts      (1001) docker     (121)    37001 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_cldapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    48485 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_clfsw32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    94767 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_clusapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    61003 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_comctl32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    37039 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_comdlg32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4756 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_compstui.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2143 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_comsvcs.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1202 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_coremessaging.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14165 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_credui.py
--rw-r--r--   0 vsts      (1001) docker     (121)   812991 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_crypt32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10937 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_cryptnet.py
--rw-r--r--   0 vsts      (1001) docker     (121)    68321 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_cryptui.py
--rw-r--r--   0 vsts      (1001) docker     (121)    55382 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_cryptxml.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1668 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_cscapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10555 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d2d1.py
--rw-r--r--   0 vsts      (1001) docker     (121)    33031 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d3d10.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3157 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d3d10_1.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5142 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d3d11.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11588 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d3d12.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2195 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d3d9.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14129 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d3dcompiler_47.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7420 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_d3dcsx.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10538 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_davclnt.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dbgeng.py
--rw-r--r--   0 vsts      (1001) docker     (121)   199381 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dbghelp.py
--rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dbgmodel.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25071 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dciman32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2932 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dcomp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4041 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ddraw.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1030 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_deviceaccess.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1041 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dflayout.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11910 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dhcpcsvc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6875 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dhcpcsvc6.py
--rw-r--r--   0 vsts      (1001) docker     (121)   305741 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dhcpsapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18915 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_diagnosticdataquery.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1139 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dinput8.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_directml.py
--rw-r--r--   0 vsts      (1001) docker     (121)   852503 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dnsapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12646 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_drt.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21806 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_drtprov.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1342 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_drttransport.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6425 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dsound.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11496 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dsparse.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15688 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dsprop.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14000 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dssec.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3746 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dsuiext.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15005 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dwmapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)      994 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dwrite.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1381 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dxcompiler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1971 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dxgi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15994 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_dxva2.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32201 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_eappcfg.py
--rw-r--r--   0 vsts      (1001) docker     (121)    23845 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_eappprxy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_efswrt.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14361 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_elscore.py
--rw-r--r--   0 vsts      (1001) docker     (121)   171669 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_esent.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3048 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_evr.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5746 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_faultrep.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2303 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_fhsvcctl.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13027 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_fltlib.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4002 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_fontsub.py
--rw-r--r--   0 vsts      (1001) docker     (121)  4212258 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_fwpuclnt.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1026 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_fxsutility.py
--rw-r--r--   0 vsts      (1001) docker     (121)   329482 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_gdi32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2794 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_gpedit.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32104 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_hid.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13835 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_hlink.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1465 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_hrtfapo.py
--rw-r--r--   0 vsts      (1001) docker     (121)    42362 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_httpapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24371 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_icm32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4102 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_icmui.py
--rw-r--r--   0 vsts      (1001) docker     (121)   657006 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_icu.py
--rw-r--r--   0 vsts      (1001) docker     (121)    39627 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_imm32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13194 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_inkobjcore.py
--rw-r--r--   0 vsts      (1001) docker     (121)   280179 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_iphlpapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    62614 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_iscsidsc.py
--rw-r--r--   0 vsts      (1001) docker     (121)   745684 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_kernel32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2085 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_keycredmgr.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8081 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ksuser.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21401 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ktmw32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4241 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_loadperf.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10814 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_magnification.py
--rw-r--r--   0 vsts      (1001) docker     (121)      850 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mapi32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4161 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mdmregistration.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25448 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1255 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mfcore.py
--rw-r--r--   0 vsts      (1001) docker     (121)   111647 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mfplat.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1222 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mfplay.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2329 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mfreadwrite.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2595 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mfsensorgroup.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1348 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mfsrcsnk.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12409 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mgmtapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5783 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9206 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mmdevapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32688 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mpr.py
--rw-r--r--   0 vsts      (1001) docker     (121)   100899 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mprapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12038 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mrmsupport.py
--rw-r--r--   0 vsts      (1001) docker     (121)    49258 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msacm32.py
--rw-r--r--   0 vsts      (1001) docker     (121)   210992 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msajapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    59783 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mscms.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1225 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msctfmonitor.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8951 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msdmo.py
--rw-r--r--   0 vsts      (1001) docker     (121)    45691 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msdrm.py
--rw-r--r--   0 vsts      (1001) docker     (121)   111815 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3202 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msimg32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2746 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msports.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mstask.py
--rw-r--r--   0 vsts      (1001) docker     (121)    54511 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_msvfw32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16406 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mswsock.py
--rw-r--r--   0 vsts      (1001) docker     (121)      869 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_mtxdm.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25997 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ncrypt.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11663 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ndfapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    99774 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_netapi32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10790 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_netsh.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7336 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_newdev.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19123 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ninput.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1581 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_normaliz.py
--rw-r--r--   0 vsts      (1001) docker     (121)    56589 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ntdll.py
--rw-r--r--   0 vsts      (1001) docker     (121)    44385 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ntdsapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4854 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ntlanman.py
--rw-r--r--   0 vsts      (1001) docker     (121)   184451 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ole32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20592 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_oleacc.py
--rw-r--r--   0 vsts      (1001) docker     (121)   579265 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_oleaut32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    38261 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_oledlg.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3385 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ondemandconnroutehelper.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8663 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_opengl32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    86868 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_p2p.py
--rw-r--r--   0 vsts      (1001) docker     (121)    34539 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_p2pgraph.py
--rw-r--r--   0 vsts      (1001) docker     (121)    57625 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_pdh.py
--rw-r--r--   0 vsts      (1001) docker     (121)    23974 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_peerdist.py
--rw-r--r--   0 vsts      (1001) docker     (121)    70509 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_powrprof.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10390 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_prntvpt.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25479 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_projectedfslib.py
--rw-r--r--   0 vsts      (1001) docker     (121)  1186372 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_propsys.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1259 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_quartz.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1950 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_query.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8167 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_qwave.py
--rw-r--r--   0 vsts      (1001) docker     (121)    81892 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_rasapi32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7251 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_rasdlg.py
--rw-r--r--   0 vsts      (1001) docker     (121)    98994 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_resutils.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1013 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_rometadata.py
--rw-r--r--   0 vsts      (1001) docker     (121)    31967 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_rpcns4.py
--rw-r--r--   0 vsts      (1001) docker     (121)  2012152 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_rpcrt4.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6369 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_rstrtmgr.py
--rw-r--r--   0 vsts      (1001) docker     (121)    74486 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_rtm.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13526 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_scarddlg.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5357 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_schannel.py
--rw-r--r--   0 vsts      (1001) docker     (121)   103333 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_secur32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1863 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_sensapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)   224522 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_setupapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3484 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_sfc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2651 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_shdocvw.py
--rw-r--r--   0 vsts      (1001) docker     (121)   155923 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_shell32.py
--rw-r--r--   0 vsts      (1001) docker     (121)   112605 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_shlwapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14906 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_slc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2882 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_slcext.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1234 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_slwga.py
--rw-r--r--   0 vsts      (1001) docker     (121)    29411 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_snmpapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    23360 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_spoolss.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4362 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_srpapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3503 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_sspicli.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11528 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_t2embed.py
--rw-r--r--   0 vsts      (1001) docker     (121)   256358 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_tapi32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4829 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_tbs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    44132 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_tdh.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7224 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_tokenbinding.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15494 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_traffic.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6469 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_txfw32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3161 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ualapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    97380 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_uiautomationcore.py
--rw-r--r--   0 vsts      (1001) docker     (121)    38971 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_urlmon.py
--rw-r--r--   0 vsts      (1001) docker     (121)   406278 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_user32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25501 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_userenv.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32504 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_usp10.py
--rw-r--r--   0 vsts      (1001) docker     (121)    43347 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_uxtheme.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1475 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_verifier.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7144 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_version.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1417 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_vertdll.py
--rw-r--r--   0 vsts      (1001) docker     (121)    35559 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_virtdisk.py
--rw-r--r--   0 vsts      (1001) docker     (121)      883 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_vssapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3316 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wcmapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3241 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wdsbp.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14784 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wdsclientapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2747 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wdsmc.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15830 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wdspxe.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5146 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wdstptc.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13831 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_webauthn.py
--rw-r--r--   0 vsts      (1001) docker     (121)   205619 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_webservices.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10108 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_websocket.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10469 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wecapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16649 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    52832 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wevtapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    66198 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winbio.py
--rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_windows_ai_machinelearning.py
--rw-r--r--   0 vsts      (1001) docker     (121)      930 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_windows_data_pdf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      861 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_windows_networking.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1619 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_windows_ui_xaml.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4801 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_windowscodecs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    57342 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winfax.py
--rw-r--r--   0 vsts      (1001) docker     (121)    30571 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winhttp.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22445 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winhvemulation.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25856 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winhvplatform.py
--rw-r--r--   0 vsts      (1001) docker     (121)   246872 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wininet.py
--rw-r--r--   0 vsts      (1001) docker     (121)      865 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winml.py
--rw-r--r--   0 vsts      (1001) docker     (121)    94474 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winmm.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32020 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winscard.py
--rw-r--r--   0 vsts      (1001) docker     (121)   114827 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winspool.py
--rw-r--r--   0 vsts      (1001) docker     (121)   169418 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wintrust.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22890 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_winusb.py
--rw-r--r--   0 vsts      (1001) docker     (121)    42226 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wlanapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wlanui.py
--rw-r--r--   0 vsts      (1001) docker     (121)   507152 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wldap32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2778 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wldp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3145 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wmvcore.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2326 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wnvapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7202 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wofutil.py
--rw-r--r--   0 vsts      (1001) docker     (121)   154580 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_ws2_32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2176 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wscapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1645 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wsclient.py
--rw-r--r--   0 vsts      (1001) docker     (121)    33500 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wsdapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    91209 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wsmsvc.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22469 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wsnmp32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    40300 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_wtsapi32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1775 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_xaudio2_8.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4581 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_xinputuap.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3002 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_xmllite.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2284 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/definitions/win32_xpsprint.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.193482 angr-9.2.8/angr/procedures/glibc/
--rw-r--r--   0 vsts      (1001) docker     (121)      861 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/__ctype_b_loc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/__ctype_tolower_loc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/__ctype_toupper_loc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      253 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/__errno_location.py
--rw-r--r--   0 vsts      (1001) docker     (121)      110 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1560 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/__libc_init.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11523 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/__libc_start_main.py
--rw-r--r--   0 vsts      (1001) docker     (121)      653 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/dynamic_loading.py
--rw-r--r--   0 vsts      (1001) docker     (121)      145 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/scanf.py
--rw-r--r--   0 vsts      (1001) docker     (121)       74 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/glibc/sscanf.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.193482 angr-9.2.8/angr/procedures/java/
--rw-r--r--   0 vsts      (1001) docker     (121)     1226 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3413 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java/unconstrained.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.193482 angr-9.2.8/angr/procedures/java_io/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_io/read.py
--rw-r--r--   0 vsts      (1001) docker     (121)      627 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_io/write.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.197483 angr-9.2.8/angr/procedures/java_jni/
--rw-r--r--   0 vsts      (1001) docker     (121)    21522 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10404 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/array_operations.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1056 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/class_and_interface_operations.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5343 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/field_access.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1093 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/global_and_local_refs.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9682 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/method_calls.py
--rw-r--r--   0 vsts      (1001) docker     (121)      951 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/not_implemented.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2797 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/object_operations.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2683 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/string_operations.py
--rw-r--r--   0 vsts      (1001) docker     (121)      230 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_jni/version_information.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.197483 angr-9.2.8/angr/procedures/java_lang/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1030 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/character.py
--rw-r--r--   0 vsts      (1001) docker     (121)      757 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/double.py
--rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/exit.py
--rw-r--r--   0 vsts      (1001) docker     (121)      521 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/getsimplename.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1587 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/integer.py
--rw-r--r--   0 vsts      (1001) docker     (121)      256 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/load_library.py
--rw-r--r--   0 vsts      (1001) docker     (121)      360 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/math.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3358 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/string.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1635 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/stringbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (121)      428 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_lang/system.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.201483 angr-9.2.8/angr/procedures/java_util/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1348 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_util/collection.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1762 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_util/iterator.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3912 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_util/list.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5018 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_util/map.py
--rw-r--r--   0 vsts      (1001) docker     (121)      388 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_util/random.py
--rw-r--r--   0 vsts      (1001) docker     (121)      810 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/java_util/scanner_nextline.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.217484 angr-9.2.8/angr/procedures/libc/
--rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/abort.py
--rw-r--r--   0 vsts      (1001) docker     (121)      373 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/access.py
--rw-r--r--   0 vsts      (1001) docker     (121)      361 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/atoi.py
--rw-r--r--   0 vsts      (1001) docker     (121)      294 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/atol.py
--rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/calloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/closelog.py
--rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/err.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/error.py
--rw-r--r--   0 vsts      (1001) docker     (121)      279 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/exit.py
--rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fclose.py
--rw-r--r--   0 vsts      (1001) docker     (121)      655 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/feof.py
--rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fflush.py
--rw-r--r--   0 vsts      (1001) docker     (121)      665 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fgetc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2826 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fgets.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2489 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fopen.py
--rw-r--r--   0 vsts      (1001) docker     (121)      818 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fprintf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      620 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fputc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      745 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fputs.py
--rw-r--r--   0 vsts      (1001) docker     (121)      697 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fread.py
--rw-r--r--   0 vsts      (1001) docker     (121)      242 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/free.py
--rw-r--r--   0 vsts      (1001) docker     (121)      646 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fscanf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1178 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fseek.py
--rw-r--r--   0 vsts      (1001) docker     (121)      599 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/ftell.py
--rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/fwrite.py
--rw-r--r--   0 vsts      (1001) docker     (121)      402 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/getchar.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4069 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/getdelim.py
--rw-r--r--   0 vsts      (1001) docker     (121)      214 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/getegid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      214 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/geteuid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      212 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/getgid.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2639 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/gets.py
--rw-r--r--   0 vsts      (1001) docker     (121)      212 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/getuid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/malloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3007 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/memcmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1446 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/memcpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2495 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/memset.py
--rw-r--r--   0 vsts      (1001) docker     (121)      294 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/openlog.py
--rw-r--r--   0 vsts      (1001) docker     (121)      419 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/perror.py
--rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/printf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      362 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/putchar.py
--rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/puts.py
--rw-r--r--   0 vsts      (1001) docker     (121)      195 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/rand.py
--rw-r--r--   0 vsts      (1001) docker     (121)      254 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/realloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      323 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/rewind.py
--rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/scanf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      149 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/setbuf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      109 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/setvbuf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1359 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/snprintf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      739 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/sprintf.py
--rw-r--r--   0 vsts      (1001) docker     (121)       89 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/srand.py
--rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/sscanf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strcat.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1873 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strchr.py
--rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strcmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)      408 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3112 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strlen.py
--rw-r--r--   0 vsts      (1001) docker     (121)      516 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strncat.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7392 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strncmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)      598 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strncpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)      381 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strnlen.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3149 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strstr.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11680 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strtol.py
--rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/strtoul.py
--rw-r--r--   0 vsts      (1001) docker     (121)      337 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/system.py
--rw-r--r--   0 vsts      (1001) docker     (121)      262 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/time.py
--rw-r--r--   0 vsts      (1001) docker     (121)      630 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/tmpnam.py
--rw-r--r--   0 vsts      (1001) docker     (121)      230 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/tolower.py
--rw-r--r--   0 vsts      (1001) docker     (121)      231 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/toupper.py
--rw-r--r--   0 vsts      (1001) docker     (121)      709 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/ungetc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/vsnprintf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libc/wchar.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.217484 angr-9.2.8/angr/procedures/libstdcpp/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libstdcpp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      274 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libstdcpp/_unwind_resume.py
--rw-r--r--   0 vsts      (1001) docker     (121)      422 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libstdcpp/std____throw_bad_alloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      420 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libstdcpp/std____throw_bad_cast.py
--rw-r--r--   0 vsts      (1001) docker     (121)      481 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libstdcpp/std____throw_length_error.py
--rw-r--r--   0 vsts      (1001) docker     (121)      479 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libstdcpp/std____throw_logic_error.py
--rw-r--r--   0 vsts      (1001) docker     (121)      361 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/libstdcpp/std__terminate.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.225485 angr-9.2.8/angr/procedures/linux_kernel/
--rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1127 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/arch_prctl.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1550 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/arm_user_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (121)      327 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/brk.py
--rw-r--r--   0 vsts      (1001) docker     (121)      717 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/cwd.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5013 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/fstat.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6188 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/fstat64.py
--rw-r--r--   0 vsts      (1001) docker     (121)      608 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/futex.py
--rw-r--r--   0 vsts      (1001) docker     (121)      464 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/getegid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      463 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/geteuid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      461 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/getgid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      227 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/getpid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      832 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/getrlimit.py
--rw-r--r--   0 vsts      (1001) docker     (121)      139 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/gettid.py
--rw-r--r--   0 vsts      (1001) docker     (121)      460 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/getuid.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1429 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/iovec.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1186 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/lseek.py
--rw-r--r--   0 vsts      (1001) docker     (121)      507 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/mmap.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1395 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/mprotect.py
--rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/munmap.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1197 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/openat.py
--rw-r--r--   0 vsts      (1001) docker     (121)      300 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/set_tid_address.py
--rw-r--r--   0 vsts      (1001) docker     (121)      610 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/sigaction.py
--rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/sigprocmask.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1147 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/stat.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (121)      234 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/tgkill.py
--rw-r--r--   0 vsts      (1001) docker     (121)      998 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/time.py
--rw-r--r--   0 vsts      (1001) docker     (121)      760 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/uid.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1132 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/uname.py
--rw-r--r--   0 vsts      (1001) docker     (121)      792 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/unlink.py
--rw-r--r--   0 vsts      (1001) docker     (121)      490 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_kernel/vsyscall.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.225485 angr-9.2.8/angr/procedures/linux_loader/
--rw-r--r--   0 vsts      (1001) docker     (121)      115 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      128 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_loader/_dl_initial_error_catch_tsd.py
--rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_loader/_dl_rtld_lock.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1798 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_loader/sim_loader.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1547 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/linux_loader/tls.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.229485 angr-9.2.8/angr/procedures/msvcr/
--rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/msvcr/__getmainargs.py
--rw-r--r--   0 vsts      (1001) docker     (121)      116 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/msvcr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1429 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/msvcr/_initterm.py
--rw-r--r--   0 vsts      (1001) docker     (121)      748 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/msvcr/fmode.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.229485 angr-9.2.8/angr/procedures/ntdll/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/ntdll/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2687 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/ntdll/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.237486 angr-9.2.8/angr/procedures/posix/
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/accept.py
--rw-r--r--   0 vsts      (1001) docker     (121)      413 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/bind.py
--rw-r--r--   0 vsts      (1001) docker     (121)      173 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/bzero.py
--rw-r--r--   0 vsts      (1001) docker     (121)      286 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/close.py
--rw-r--r--   0 vsts      (1001) docker     (121)       63 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/closedir.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2128 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/dup.py
--rw-r--r--   0 vsts      (1001) docker     (121)      399 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/fcntl.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2262 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/fdopen.py
--rw-r--r--   0 vsts      (1001) docker     (121)      500 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/fileno.py
--rw-r--r--   0 vsts      (1001) docker     (121)      276 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/fork.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/getenv.py
--rw-r--r--   0 vsts      (1001) docker     (121)      911 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/gethostbyname.py
--rw-r--r--   0 vsts      (1001) docker     (121)      571 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/getpass.py
--rw-r--r--   0 vsts      (1001) docker     (121)      278 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/getsockopt.py
--rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/htonl.py
--rw-r--r--   0 vsts      (1001) docker     (121)      393 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/htons.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/inet_ntoa.py
--rw-r--r--   0 vsts      (1001) docker     (121)      414 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/listen.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4996 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/mmap.py
--rw-r--r--   0 vsts      (1001) docker     (121)      619 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/open.py
--rw-r--r--   0 vsts      (1001) docker     (121)      289 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/opendir.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2116 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/poll.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1354 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/pread64.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2823 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/pthread.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1361 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/pwrite64.py
--rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/read.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/readdir.py
--rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/recv.py
--rw-r--r--   0 vsts      (1001) docker     (121)      387 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/recvfrom.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/select.py
--rw-r--r--   0 vsts      (1001) docker     (121)      855 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/send.py
--rw-r--r--   0 vsts      (1001) docker     (121)      257 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/setsockopt.py
--rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/sigaction.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1622 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/sim_time.py
--rw-r--r--   0 vsts      (1001) docker     (121)      143 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/sleep.py
--rw-r--r--   0 vsts      (1001) docker     (121)      728 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/socket.py
--rw-r--r--   0 vsts      (1001) docker     (121)      581 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/strcasecmp.py
--rw-r--r--   0 vsts      (1001) docker     (121)      485 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/strdup.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2552 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/strtok_r.py
--rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/syslog.py
--rw-r--r--   0 vsts      (1001) docker     (121)      259 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/tz.py
--rw-r--r--   0 vsts      (1001) docker     (121)      368 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/unlink.py
--rw-r--r--   0 vsts      (1001) docker     (121)      138 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/usleep.py
--rw-r--r--   0 vsts      (1001) docker     (121)      339 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/posix/write.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1822 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/procedure_dict.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.241486 angr-9.2.8/angr/procedures/stubs/
--rw-r--r--   0 vsts      (1001) docker     (121)      218 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/CallReturn.py
--rw-r--r--   0 vsts      (1001) docker     (121)      492 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/NoReturnUnconstrained.py
--rw-r--r--   0 vsts      (1001) docker     (121)      171 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/Nop.py
--rw-r--r--   0 vsts      (1001) docker     (121)      205 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/PathTerminator.py
--rw-r--r--   0 vsts      (1001) docker     (121)      565 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/Redirect.py
--rw-r--r--   0 vsts      (1001) docker     (121)      437 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/ReturnChar.py
--rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/ReturnUnconstrained.py
--rw-r--r--   0 vsts      (1001) docker     (121)      256 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/UnresolvableCallTarget.py
--rw-r--r--   0 vsts      (1001) docker     (121)      255 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/UnresolvableJumpTarget.py
--rw-r--r--   0 vsts      (1001) docker     (121)      558 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/UserHook.py
--rw-r--r--   0 vsts      (1001) docker     (121)       67 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1579 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/b64_decode.py
--rw-r--r--   0 vsts      (1001) docker     (121)      432 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/caller.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1036 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/crazy_scanf.py
--rw-r--r--   0 vsts      (1001) docker     (121)    27862 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/format_parser.py
--rw-r--r--   0 vsts      (1001) docker     (121)      984 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/stubs/syscall_stub.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.241486 angr-9.2.8/angr/procedures/testing/
--rw-r--r--   0 vsts      (1001) docker     (121)      106 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)       99 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/testing/manyargs.py
--rw-r--r--   0 vsts      (1001) docker     (121)      169 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/testing/retreg.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.241486 angr-9.2.8/angr/procedures/tracer/
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/tracer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1079 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/tracer/random.py
--rw-r--r--   0 vsts      (1001) docker     (121)      586 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/tracer/receive.py
--rw-r--r--   0 vsts      (1001) docker     (121)      723 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/tracer/transmit.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.245487 angr-9.2.8/angr/procedures/uclibc/
--rw-r--r--   0 vsts      (1001) docker     (121)       88 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/uclibc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      363 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/uclibc/__uClibc_main.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.249487 angr-9.2.8/angr/procedures/win32/
--rw-r--r--   0 vsts      (1001) docker     (121)       96 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/EncodePointer.py
--rw-r--r--   0 vsts      (1001) docker     (121)      132 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/ExitProcess.py
--rw-r--r--   0 vsts      (1001) docker     (121)      226 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/GetCommandLine.py
--rw-r--r--   0 vsts      (1001) docker     (121)      104 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/GetCurrentProcessId.py
--rw-r--r--   0 vsts      (1001) docker     (121)      103 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/GetCurrentThreadId.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1092 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/GetLastInputInfo.py
--rw-r--r--   0 vsts      (1001) docker     (121)      938 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/GetModuleHandle.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1137 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/GetProcessAffinityMask.py
--rw-r--r--   0 vsts      (1001) docker     (121)      525 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/InterlockedExchange.py
--rw-r--r--   0 vsts      (1001) docker     (121)      198 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/IsProcessorFeaturePresent.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3923 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/VirtualAlloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/VirtualProtect.py
--rw-r--r--   0 vsts      (1001) docker     (121)       86 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      275 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/critical_section.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3430 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/dynamic_loading.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1454 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/file_handles.py
--rw-r--r--   0 vsts      (1001) docker     (121)      316 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/gethostbyname.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1588 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/heap.py
--rw-r--r--   0 vsts      (1001) docker     (121)      748 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/is_bad_ptr.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/local_storage.py
--rw-r--r--   0 vsts      (1001) docker     (121)      174 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/mutex.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5271 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/sim_time.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1184 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win32/system_paths.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.249487 angr-9.2.8/angr/procedures/win_user32/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win_user32/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win_user32/chars.py
--rw-r--r--   0 vsts      (1001) docker     (121)      376 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win_user32/keyboard.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1733 2022-06-28 17:01:19.000000 angr-9.2.8/angr/procedures/win_user32/messagebox.py
--rw-r--r--   0 vsts      (1001) docker     (121)    34536 2022-06-28 17:01:19.000000 angr-9.2.8/angr/project.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.253487 angr-9.2.8/angr/protos/
--rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-06-28 17:01:19.000000 angr-9.2.8/angr/protos/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3090 2022-06-28 17:01:19.000000 angr-9.2.8/angr/protos/cfg_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2170 2022-06-28 17:01:19.000000 angr-9.2.8/angr/protos/function_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8551 2022-06-28 17:01:19.000000 angr-9.2.8/angr/protos/primitives_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8136 2022-06-28 17:01:19.000000 angr-9.2.8/angr/protos/variables_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1271 2022-06-28 17:01:19.000000 angr-9.2.8/angr/protos/xrefs_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (121)        7 2022-06-28 17:01:19.000000 angr-9.2.8/angr/py.typed
--rw-r--r--   0 vsts      (1001) docker     (121)     1508 2022-06-28 17:01:19.000000 angr-9.2.8/angr/serializable.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-06-28 17:01:19.000000 angr-9.2.8/angr/service.py
--rw-r--r--   0 vsts      (1001) docker     (121)    36818 2022-06-28 17:01:19.000000 angr-9.2.8/angr/sim_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17256 2022-06-28 17:01:19.000000 angr-9.2.8/angr/sim_options.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24894 2022-06-28 17:01:19.000000 angr-9.2.8/angr/sim_procedure.py
--rw-r--r--   0 vsts      (1001) docker     (121)    38075 2022-06-28 17:01:19.000000 angr-9.2.8/angr/sim_state.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12710 2022-06-28 17:01:19.000000 angr-9.2.8/angr/sim_state_options.py
--rw-r--r--   0 vsts      (1001) docker     (121)   116179 2022-06-28 17:01:19.000000 angr-9.2.8/angr/sim_type.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17184 2022-06-28 17:01:19.000000 angr-9.2.8/angr/sim_variable.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.253487 angr-9.2.8/angr/simos/
--rw-r--r--   0 vsts      (1001) docker     (121)      672 2022-06-28 17:01:19.000000 angr-9.2.8/angr/simos/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5769 2022-06-28 17:01:19.000000 angr-9.2.8/angr/simos/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22136 2022-06-28 17:01:19.000000 angr-9.2.8/angr/simos/javavm.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22806 2022-06-28 17:01:19.000000 angr-9.2.8/angr/simos/linux.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18474 2022-06-28 17:01:19.000000 angr-9.2.8/angr/simos/simos.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7283 2022-06-28 17:01:19.000000 angr-9.2.8/angr/simos/userland.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25786 2022-06-28 17:01:19.000000 angr-9.2.8/angr/simos/windows.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10044 2022-06-28 17:01:19.000000 angr-9.2.8/angr/slicer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8064 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_hierarchy.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.261488 angr-9.2.8/angr/state_plugins/
--rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12019 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/callstack.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4192 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13003 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/concrete.py
--rw-r--r--   0 vsts      (1001) docker     (121)    25841 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/filesystem.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5087 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/gdb.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1528 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/globals.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.261488 angr-9.2.8/angr/state_plugins/heap/
--rw-r--r--   0 vsts      (1001) docker     (121)      135 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/heap/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6439 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/heap/heap_base.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5423 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/heap/heap_brk.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9280 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/heap/heap_freelist.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2140 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/heap/heap_libc.py
--rw-r--r--   0 vsts      (1001) docker     (121)    28904 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/heap/heap_ptmalloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      792 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/heap/utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20424 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/history.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11451 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/inspect.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5707 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/javavm_classloader.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3453 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/jni_references.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16309 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/libc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6488 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/light_registers.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2362 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/log.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4222 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/loop_data.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5933 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/plugin.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24620 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/posix.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7873 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/preconstrainer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5937 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/scratch.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9933 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/sim_action.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4235 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/sim_action_object.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1044 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/sim_event.py
--rw-r--r--   0 vsts      (1001) docker     (121)    39588 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/solver.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10896 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/symbolizer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    30329 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/trace_additions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2631 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/uc_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    75935 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/unicorn_engine.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11444 2022-06-28 17:01:19.000000 angr-9.2.8/angr/state_plugins/view.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.265488 angr-9.2.8/angr/storage/
--rw-r--r--   0 vsts      (1001) docker     (121)      182 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    46286 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/file.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.269489 angr-9.2.8/angr/storage/memory_mixins/
--rw-r--r--   0 vsts      (1001) docker     (121)    11649 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3535 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/actions_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17030 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/address_concretization_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2897 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/bvv_conversion_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5440 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/clouseau_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      929 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/conditional_store_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10208 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/convenient_mappings_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5611 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/default_filler_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      314 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/dirty_addrs_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3692 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/hex_dumper_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.269489 angr-9.2.8/angr/storage/memory_mixins/javavm_memory/
--rw-r--r--   0 vsts      (1001) docker     (121)       51 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/javavm_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15550 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.269489 angr-9.2.8/angr/storage/memory_mixins/keyvalue_memory/
--rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/keyvalue_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      894 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      857 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/label_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1197 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/multi_value_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2925 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/name_resolution_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.269489 angr-9.2.8/angr/storage/memory_mixins/paged_memory/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10022 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py
--rw-r--r--   0 vsts      (1001) docker     (121)    26936 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.273489 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/
--rw-r--r--   0 vsts      (1001) docker     (121)     1468 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10649 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/cooperation.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2720 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2049 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13755 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/list_page.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5355 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/multi_values.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15447 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py
--rw-r--r--   0 vsts      (1001) docker     (121)      828 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1679 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18500 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1534 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/privileged_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3182 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.273489 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/
--rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1096 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1314 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      129 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/region_category_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9201 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/region_data.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4554 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4962 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18546 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2184 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2483 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/simple_interface_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      492 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/simplification_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5667 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/size_resolution_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4732 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/slotted_memory.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5423 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/smart_find_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/symbolic_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)      657 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/top_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2467 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/underconstrained_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1088 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_mixins/unwrapper_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5516 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/memory_object.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1948 2022-06-28 17:01:19.000000 angr-9.2.8/angr/storage/pcap.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3240 2022-06-28 17:01:19.000000 angr-9.2.8/angr/tablespecs.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4206 2022-06-28 17:01:19.000000 angr-9.2.8/angr/type_backend.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.273489 angr-9.2.8/angr/utils/
--rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/algo.py
--rw-r--r--   0 vsts      (1001) docker     (121)      133 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/constants.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2079 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/cowdict.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2093 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/enums_conv.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4482 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/formatting.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15164 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7160 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/library.py
--rw-r--r--   0 vsts      (1001) docker     (121)      425 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/mp.py
--rw-r--r--   0 vsts      (1001) docker     (121)      820 2022-06-28 17:01:19.000000 angr-9.2.8/angr/utils/timing.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9651 2022-06-28 17:01:19.000000 angr-9.2.8/angr/vaults.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.021468 angr-9.2.8/angr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     3181 2022-06-28 17:04:04.000000 angr-9.2.8/angr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    48887 2022-06-28 17:04:05.000000 angr-9.2.8/angr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-28 17:04:04.000000 angr-9.2.8/angr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      402 2022-06-28 17:04:04.000000 angr-9.2.8/angr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        5 2022-06-28 17:04:04.000000 angr-9.2.8/angr.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:05.277489 angr-9.2.8/native/
--rw-r--r--   0 vsts      (1001) docker     (121)      946 2022-06-28 17:01:19.000000 angr-9.2.8/native/Makefile
--rw-r--r--   0 vsts      (1001) docker     (121)      312 2022-06-28 17:01:19.000000 angr-9.2.8/native/Makefile-win
--rw-r--r--   0 vsts      (1001) docker     (121)     1297 2022-06-28 17:01:19.000000 angr-9.2.8/native/angr_native.def
--rw-r--r--   0 vsts      (1001) docker     (121)     3940 2022-06-28 17:01:19.000000 angr-9.2.8/native/log.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2754 2022-06-28 17:01:19.000000 angr-9.2.8/native/log.h
--rw-r--r--   0 vsts      (1001) docker     (121)   110001 2022-06-28 17:01:19.000000 angr-9.2.8/native/sim_unicorn.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    27677 2022-06-28 17:01:19.000000 angr-9.2.8/native/sim_unicorn.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)      131 2022-06-28 17:01:35.000000 angr-9.2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     1169 2022-06-28 17:04:05.277489 angr-9.2.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     3322 2022-06-28 17:01:19.000000 angr-9.2.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.433720 angr-9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-07-05 17:01:25.000000 angr-9.2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-07-05 17:01:25.000000 angr-9.2.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     3181 2022-07-05 17:03:21.433720 angr-9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     2641 2022-07-05 17:01:25.000000 angr-9.2.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.057673 angr-9.2.9/angr/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2774 2022-07-05 17:01:34.000000 angr-9.2.9/angr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.065674 angr-9.2.9/angr/analyses/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1751 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10185 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    27512 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/backward_slice.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    26401 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/binary_optimizer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    52237 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/bindiff.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2233 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/boyscout.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2724 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/callee_cleanup_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25838 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/calling_convention.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6418 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cdg.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.065674 angr-9.2.9/angr/analyses/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (121)      354 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14692 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfb.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3125 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3155 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg_arch_options.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   114824 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   155853 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg_emulated.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   212828 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25948 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg_fast_soot.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5737 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg_job_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7746 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/cfg_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.069674 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/
+-rw-r--r--   0 vsts      (1001) docker     (121)      317 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1747 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3146 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2938 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1194 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    77780 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8493 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2794 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2916 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1283 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20414 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg/segment_list.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.069674 angr-9.2.9/angr/analyses/cfg_slice_to_sink/
+-rw-r--r--   0 vsts      (1001) docker     (121)      120 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg_slice_to_sink/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4072 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3656 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg_slice_to_sink/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/cfg_slice_to_sink/transitions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3334 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/class_identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3673 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/code_tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12684 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/complete_calling_conventions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16352 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/congruency_check.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.069674 angr-9.2.9/angr/analyses/data_dep/
+-rw-r--r--   0 vsts      (1001) docker     (121)      180 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/data_dep/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25414 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/data_dep/data_dependency_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4649 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/data_dep/dep_nodes.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1522 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/data_dep/sim_act_location.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3348 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/datagraph_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    63069 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/ddg.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.073675 angr-9.2.9/angr/analyses/decompiler/
+-rw-r--r--   0 vsts      (1001) docker     (121)      549 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    39491 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/ail_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16416 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/ailblock_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1603 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/ailgraph_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12835 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/block_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14084 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/callsite_maker.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.073675 angr-9.2.9/angr/analyses/decompiler/ccall_rewriters/
+-rw-r--r--   0 vsts      (1001) docker     (121)      102 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/ccall_rewriters/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5965 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      438 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/ccall_rewriters/rewriter_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    43724 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/clinic.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    44213 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/condition_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      841 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/decompilation_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/decompilation_options.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12805 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/decompiler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6691 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/empty_node_remover.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3568 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/expression_narrower.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6077 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/graph_region.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.077675 angr-9.2.9/angr/analyses/decompiler/optimization_passes/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2144 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5320 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9478 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/const_derefs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16857 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/div_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8906 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/eager_returns.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10177 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7528 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2950 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/mod_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10466 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/multi_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5622 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/optimization_pass.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7466 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6207 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11678 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2961 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.081676 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2109 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1865 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1475 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      999 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1272 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1289 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      611 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2491 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1043 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      956 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      936 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3275 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/bswap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      908 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      967 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2452 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1432 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/conv_const_mull_a_shift.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2062 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/eager_eval.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1937 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1042 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      525 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1157 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1545 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3480 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1152 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      531 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1441 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1331 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      941 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    33401 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_identifier.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.081676 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/
+-rw-r--r--   0 vsts      (1001) docker     (121)       48 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3894 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2593 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14125 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/expr_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3609 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/goto.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5022 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/if_.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2546 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/ifelse.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5065 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/loop.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      564 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/node_address_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4943 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_simplifiers/region_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      716 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/region_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5929 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/sequence_walker.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.085676 angr-9.2.9/angr/analyses/decompiler/structured_codegen/
+-rw-r--r--   0 vsts      (1001) docker     (121)      284 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/structured_codegen/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3848 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/structured_codegen/base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   100865 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/structured_codegen/c.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/structured_codegen/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6705 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/structured_codegen/dwarf_import.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    72110 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/structurer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7923 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/structurer_nodes.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9436 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/decompiler/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    38206 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/disassembly.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2988 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/disassembly_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1247 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/dominance_frontier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10823 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/find_objects_static.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7803 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/flirt.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.085676 angr-9.2.9/angr/analyses/forward_analysis/
+-rw-r--r--   0 vsts      (1001) docker     (121)      144 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18933 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/forward_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1529 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/job_info.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.085676 angr-9.2.9/angr/analyses/forward_analysis/visitors/
+-rw-r--r--   0 vsts      (1001) docker     (121)      174 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/visitors/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      732 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/visitors/call_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1338 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/visitors/function_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7811 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/visitors/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      725 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/visitors/loop.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      779 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/forward_analysis/visitors/single_node_graph.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.085676 angr-9.2.9/angr/analyses/identifier/
+-rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4538 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/custom_callable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      158 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1714 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/func.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.089677 angr-9.2.9/angr/analyses/identifier/functions/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1062 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2121 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3317 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/based_atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4343 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/fdprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1944 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/free.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8760 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/int2str.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3854 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/malloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1963 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/memcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3153 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/memcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1193 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/memset.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4295 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/printf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11558 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/recv_until.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2363 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/skip_calloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3192 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/skip_realloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2910 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/skip_recv_n.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4189 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/snprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4130 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/sprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      821 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/strcasecmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3509 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/strcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1193 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      751 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/strlen.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3347 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/strncmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2014 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/strncpy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2435 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/functions/strtol.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    33116 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13825 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/identifier/runner.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8604 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/init_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9333 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/loop_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7214 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/loopfinder.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.089677 angr-9.2.9/angr/analyses/propagator/
+-rw-r--r--   0 vsts      (1001) docker     (121)       44 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      551 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/call_expr_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    39786 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1134 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8736 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6116 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/outdated_definition_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7136 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/prop_value.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    27240 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/propagator.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/top_checker_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/values.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1401 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/propagator/vex_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15285 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/proximity_graph.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.093677 angr-9.2.9/angr/analyses/reaching_definitions/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1258 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2232 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/call_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7785 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/dep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    41873 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    51117 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      242 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/external_codeloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5958 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/function_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2632 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/heap_allocator.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19861 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/rd_state.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16703 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/reaching_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reaching_definitions/subject.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   100773 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/reassembler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8942 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/soot_class_hierarchy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19938 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/stack_pointer_tracker.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1709 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/static_hooker.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.093677 angr-9.2.9/angr/analyses/typehoon/
+-rw-r--r--   0 vsts      (1001) docker     (121)       32 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/typehoon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1676 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/typehoon/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25122 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/typehoon/simple_solver.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8340 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/typehoon/translator.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3688 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/typehoon/typeconsts.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8717 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/typehoon/typehoon.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13526 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/typehoon/typevars.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.097678 angr-9.2.9/angr/analyses/variable_recovery/
+-rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/annotations.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20374 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    38254 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16299 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    23287 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/variable_recovery.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13000 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/variable_recovery_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22126 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/variable_recovery/variable_recovery_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25486 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/veritesting.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    73710 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/vfg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16358 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/vsa_ddg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4142 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/vtable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9479 2022-07-05 17:01:25.000000 angr-9.2.9/angr/analyses/xrefs.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.097678 angr-9.2.9/angr/angrdb/
+-rw-r--r--   0 vsts      (1001) docker     (121)      243 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6401 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/db.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4939 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/models.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.097678 angr-9.2.9/angr/angrdb/serializers/
+-rw-r--r--   0 vsts      (1001) docker     (121)       78 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1323 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/cfg_model.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1514 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/comments.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1700 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/funcs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3689 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/kb.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1408 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/labels.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2125 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/loader.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4380 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/structured_code.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2453 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/variables.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1287 2022-07-05 17:01:25.000000 angr-9.2.9/angr/angrdb/serializers/xrefs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10929 2022-07-05 17:01:25.000000 angr-9.2.9/angr/annocfg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15184 2022-07-05 17:01:25.000000 angr-9.2.9/angr/blade.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14018 2022-07-05 17:01:25.000000 angr-9.2.9/angr/block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5539 2022-07-05 17:01:25.000000 angr-9.2.9/angr/callable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    85459 2022-07-05 17:01:25.000000 angr-9.2.9/angr/calling_conventions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3766 2022-07-05 17:01:25.000000 angr-9.2.9/angr/code_location.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3828 2022-07-05 17:01:25.000000 angr-9.2.9/angr/codenode.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.101678 angr-9.2.9/angr/concretization_strategies/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3724 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      440 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/any.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/controlled_data.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/eval.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1039 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/max.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/nonzero.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      825 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/nonzero_range.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1464 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/norepeats.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1633 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/norepeats_range.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      587 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/range.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      357 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/single.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      570 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/solutions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      526 2022-07-05 17:01:25.000000 angr-9.2.9/angr/concretization_strategies/unlimited_range.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.101678 angr-9.2.9/angr/distributed/
+-rw-r--r--   0 vsts      (1001) docker     (121)      141 2022-07-05 17:01:25.000000 angr-9.2.9/angr/distributed/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6501 2022-07-05 17:01:25.000000 angr-9.2.9/angr/distributed/server.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6076 2022-07-05 17:01:25.000000 angr-9.2.9/angr/distributed/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.105679 angr-9.2.9/angr/engines/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1066 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7379 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/concrete.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7910 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      992 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/failure.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2472 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/hook.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.105679 angr-9.2.9/angr/engines/light/
+-rw-r--r--   0 vsts      (1001) docker     (121)      187 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/light/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16743 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/light/data.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    37169 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/light/engine.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.105679 angr-9.2.9/angr/engines/pcode/
+-rw-r--r--   0 vsts      (1001) docker     (121)       64 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/pcode/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4119 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/pcode/arch.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    28477 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/pcode/behavior.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13837 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/pcode/emulate.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9493 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/pcode/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    49058 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/pcode/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2473 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/procedure.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.109679 angr-9.2.9/angr/engines/soot/
+-rw-r--r--   0 vsts      (1001) docker     (121)       31 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17456 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.113680 angr-9.2.9/angr/engines/soot/expressions/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      859 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/arrayref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      508 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      781 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/binop.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      903 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/cast.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1252 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/condition.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1390 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      314 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/instanceOf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/instancefieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4884 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/invoke.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/length.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      216 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/local.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/new.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2036 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/newArray.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3326 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/newMultiArray.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      225 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/paramref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1163 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/phi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      233 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/staticfieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      150 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/thisref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      114 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/expressions/unsupported.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1958 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/field_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1834 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/method_dispatcher.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.117680 angr-9.2.9/angr/engines/soot/statements/
+-rw-r--r--   0 vsts      (1001) docker     (121)      884 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1272 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/assign.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2115 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/goto.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      422 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/identity.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      583 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/if_.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      285 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/invoke.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/return_.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1325 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/switch.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      384 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/statements/throw.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.117680 angr-9.2.9/angr/engines/soot/values/
+-rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4365 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/arrayref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      123 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      436 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1603 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/instancefieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      413 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/local.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      417 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/paramref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1250 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/staticfieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1146 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/strref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6133 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/soot/values/thisref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    23140 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/successors.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2027 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/syscall.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20693 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/unicorn.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.117680 angr-9.2.9/angr/engines/vex/
+-rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.121681 angr-9.2.9/angr/engines/vex/claripy/
+-rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/claripy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    82545 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/claripy/ccall.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5097 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/claripy/datalayer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    44882 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/claripy/irop.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.121681 angr-9.2.9/angr/engines/vex/heavy/
+-rw-r--r--   0 vsts      (1001) docker     (121)      200 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/heavy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8349 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/heavy/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18700 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/heavy/dirty.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14816 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/heavy/heavy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2290 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/heavy/inspect.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3417 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/heavy/resilience.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1180 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/heavy/super_fastpath.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16862 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/lifter.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.121681 angr-9.2.9/angr/engines/vex/light/
+-rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/light/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21607 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/light/light.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1928 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/light/resilience.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2120 2022-07-05 17:01:25.000000 angr-9.2.9/angr/engines/vex/light/slicing.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8096 2022-07-05 17:01:25.000000 angr-9.2.9/angr/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.129682 angr-9.2.9/angr/exploration_techniques/
+-rw-r--r--   0 vsts      (1001) docker     (121)     8784 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2579 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/bucketizer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5144 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/cacher.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2210 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/common.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1175 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/dfs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18009 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/director.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3448 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/driller_core.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6155 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/explorer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      568 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/lengthlimiter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2583 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/local_loop_seer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11393 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/loop_seer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3055 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/manual_mergepoint.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1286 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/memory_watcher.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3597 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/oppologist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5141 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/slicecutor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9304 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/spiller.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      725 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/spiller_db.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2081 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/stochastic.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3183 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/symbion.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/tech_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1531 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/threading.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      922 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/timeout.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    49983 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4408 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/unique.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1394 2022-07-05 17:01:25.000000 angr-9.2.9/angr/exploration_techniques/veritesting.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15873 2022-07-05 17:01:25.000000 angr-9.2.9/angr/factory.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.129682 angr-9.2.9/angr/flirt/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4166 2022-07-05 17:01:25.000000 angr-9.2.9/angr/flirt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10375 2022-07-05 17:01:25.000000 angr-9.2.9/angr/flirt/build_sig.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17205 2022-07-05 17:01:25.000000 angr-9.2.9/angr/keyed_region.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.129682 angr-9.2.9/angr/knowledge_base/
+-rw-r--r--   0 vsts      (1001) docker     (121)       43 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_base/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4463 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_base/knowledge_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.137683 angr-9.2.9/angr/knowledge_plugins/
+-rw-r--r--   0 vsts      (1001) docker     (121)      548 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.137683 angr-9.2.9/angr/knowledge_plugins/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/cfg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2341 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/cfg/cfg_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19073 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/cfg/cfg_model.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18238 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/cfg/cfg_node.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1998 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/cfg/indirect_jump.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3617 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/cfg/memory_data.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      330 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/comments.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/data.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.141683 angr-9.2.9/angr/knowledge_plugins/functions/
+-rw-r--r--   0 vsts      (1001) docker     (121)       78 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/functions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    64298 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/functions/function.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17366 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/functions/function_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11598 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/functions/function_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4977 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/functions/soot_function.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/indirect_jumps.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.145684 angr-9.2.9/angr/knowledge_plugins/key_definitions/
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6654 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/atoms.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      457 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2640 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/definition.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3315 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      912 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/heap_address.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3267 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/key_definition_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    26281 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/live_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1093 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/rd_model.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1711 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/tag.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1234 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/undefined.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1508 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/unknown_size.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6273 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/key_definitions/uses.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2983 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/labels.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3920 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/patches.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1548 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/propagations.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.145684 angr-9.2.9/angr/knowledge_plugins/structured_code/
+-rw-r--r--   0 vsts      (1001) docker     (121)       43 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/structured_code/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2133 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/structured_code/manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.145684 angr-9.2.9/angr/knowledge_plugins/sync/
+-rw-r--r--   0 vsts      (1001) docker     (121)       45 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/sync/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9467 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/sync/sync_controller.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1910 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/types.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.145684 angr-9.2.9/angr/knowledge_plugins/variables/
+-rw-r--r--   0 vsts      (1001) docker     (121)       61 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/variables/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3685 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/variables/variable_access.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    38042 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/variables/variable_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.145684 angr-9.2.9/angr/knowledge_plugins/xrefs/
+-rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/xrefs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4360 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/xrefs/xref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3991 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/xrefs/xref_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      272 2022-07-05 17:01:25.000000 angr-9.2.9/angr/knowledge_plugins/xrefs/xref_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.149684 angr-9.2.9/angr/misc/
+-rw-r--r--   0 vsts      (1001) docker     (121)      237 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2335 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/autoimport.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3950 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/bug_report.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3775 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/hookset.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/import_hooks.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2929 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/loggers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      642 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/picklable_lock.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9553 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/plugins.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/range.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      480 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/testing.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/ux.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1446 2022-07-05 17:01:25.000000 angr-9.2.9/angr/misc/weakpatch.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.149684 angr-9.2.9/angr/procedures/
+-rw-r--r--   0 vsts      (1001) docker     (121)       97 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.149684 angr-9.2.9/angr/procedures/advapi32/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/advapi32/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.153685 angr-9.2.9/angr/procedures/cgc/
+-rw-r--r--   0 vsts      (1001) docker     (121)       76 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      218 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/_terminate.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2148 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/allocate.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1857 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/deallocate.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2661 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/fdwait.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2309 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/random.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3718 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/receive.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2285 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/cgc/transmit.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.317705 angr-9.2.9/angr/procedures/definitions/
+-rw-r--r--   0 vsts      (1001) docker     (121)    27701 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      460 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   379370 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/glibc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      701 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/libstdcpp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   238847 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/linux_kernel.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/linux_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      601 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/msvcr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      404 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/ntdll.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1816 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/parse_syscalls_from_local_system.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    84675 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/parse_win32json.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/user32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1451 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_aclui.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    58240 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_activeds.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   570046 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_advapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24565 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_advpack.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2856 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_amsi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4595 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3002 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      882 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1091 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1030 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1063 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      933 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3151 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5854 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1021 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2631 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1388 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6054 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3243 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8278 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1499 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1177 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1571 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      891 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1081 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1364 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1434 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3279 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3785 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3237 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1163 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      902 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1697 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11013 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1551 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1531 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13539 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12396 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      796 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1100 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1245 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4664 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5935 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2610 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4262 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1103 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6979 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1380 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      937 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      996 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1185 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1240 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2446 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1820 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3488 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1013 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_apphelp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    36371 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_authz.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2783 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_avicap32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    33016 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_avifil32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    30164 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_bcrypt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    27283 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_bluetoothapis.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10956 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_bthprops.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24192 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_cabinet.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7474 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_certadm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    61551 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_certpoleng.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   109314 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_cfgmgr32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    35359 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_chakra.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    37001 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_cldapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    48485 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_clfsw32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    94767 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_clusapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    61003 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_comctl32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    37039 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_comdlg32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4756 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_compstui.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2143 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_comsvcs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1202 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_coremessaging.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14165 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_credui.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   812991 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_crypt32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10937 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_cryptnet.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    68321 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_cryptui.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    55382 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_cryptxml.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1668 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_cscapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10555 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d2d1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    33031 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d3d10.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3157 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d3d10_1.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5142 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d3d11.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11588 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d3d12.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2195 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d3d9.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14129 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d3dcompiler_47.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7420 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_d3dcsx.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10538 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_davclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dbgeng.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   199381 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dbghelp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dbgmodel.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25071 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dciman32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2932 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dcomp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4041 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ddraw.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1030 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_deviceaccess.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1041 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dflayout.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11910 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dhcpcsvc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6875 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dhcpcsvc6.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   305741 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dhcpsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18915 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_diagnosticdataquery.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1139 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dinput8.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_directml.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   852503 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dnsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12646 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_drt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21806 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_drtprov.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1342 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_drttransport.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6425 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dsound.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11496 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dsparse.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15688 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dsprop.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14000 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dssec.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3746 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dsuiext.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15005 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dwmapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      994 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1381 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dxcompiler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1971 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dxgi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15994 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_dxva2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    32201 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_eappcfg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    23845 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_eappprxy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_efswrt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14361 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_elscore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   171669 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_esent.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3048 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_evr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5746 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_faultrep.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2303 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_fhsvcctl.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13027 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_fltlib.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4002 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_fontsub.py
+-rw-r--r--   0 vsts      (1001) docker     (121)  4212258 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_fwpuclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1026 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_fxsutility.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   329482 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_gdi32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2794 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_gpedit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    32104 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_hid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13835 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_hlink.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1465 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_hrtfapo.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    42362 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_httpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24371 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_icm32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4102 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_icmui.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   657006 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_icu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    39627 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_imm32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13194 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_inkobjcore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   280179 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_iphlpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    62614 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_iscsidsc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   745684 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_kernel32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2085 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_keycredmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8081 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ksuser.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21401 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ktmw32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4241 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_loadperf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10814 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_magnification.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      850 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4161 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mdmregistration.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25448 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1255 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mfcore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   111647 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mfplat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1222 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mfplay.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2329 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mfreadwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2595 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mfsensorgroup.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1348 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mfsrcsnk.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12409 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mgmtapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5783 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9206 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mmdevapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    32688 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mpr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   100899 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mprapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12038 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mrmsupport.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    49258 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msacm32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   210992 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msajapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    59783 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mscms.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1225 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msctfmonitor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8951 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msdmo.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    45691 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msdrm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   111815 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3202 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msimg32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2746 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msports.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mstask.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    54511 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_msvfw32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16406 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mswsock.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      869 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_mtxdm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25997 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ncrypt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11663 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ndfapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    99774 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_netapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10790 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_netsh.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7336 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_newdev.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19123 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ninput.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1581 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_normaliz.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    56589 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ntdll.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    44385 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ntdsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4854 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ntlanman.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   184451 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ole32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20592 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_oleacc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   579265 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_oleaut32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    38261 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_oledlg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3385 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ondemandconnroutehelper.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8663 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_opengl32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    86868 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_p2p.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    34539 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_p2pgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    57625 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_pdh.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    23974 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_peerdist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    70509 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_powrprof.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10390 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_prntvpt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25479 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_projectedfslib.py
+-rw-r--r--   0 vsts      (1001) docker     (121)  1186372 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_propsys.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1259 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_quartz.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1950 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_query.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8167 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_qwave.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    81892 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_rasapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7251 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_rasdlg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    98994 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_resutils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1013 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_rometadata.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    31967 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_rpcns4.py
+-rw-r--r--   0 vsts      (1001) docker     (121)  2012152 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_rpcrt4.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6369 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_rstrtmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    74486 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_rtm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13526 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_scarddlg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5357 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_schannel.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   103333 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_secur32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1863 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_sensapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   224522 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_setupapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3484 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_sfc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2651 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_shdocvw.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   155923 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_shell32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   112605 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_shlwapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14906 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_slc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2882 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_slcext.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1234 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_slwga.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    29411 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_snmpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    23360 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_spoolss.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4362 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_srpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3503 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_sspicli.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11528 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_t2embed.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   256358 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_tapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4829 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_tbs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    44132 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_tdh.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7224 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_tokenbinding.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15494 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_traffic.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6469 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_txfw32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3161 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ualapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    97380 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_uiautomationcore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    38971 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_urlmon.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   406278 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_user32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25501 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_userenv.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    32504 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_usp10.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    43347 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_uxtheme.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1475 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_verifier.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7144 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_version.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1417 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_vertdll.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    35559 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_virtdisk.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      883 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_vssapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3316 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wcmapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3241 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wdsbp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14784 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wdsclientapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2747 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wdsmc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15830 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wdspxe.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5146 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wdstptc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13831 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_webauthn.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   205619 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_webservices.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10108 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_websocket.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10469 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wecapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16649 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    52832 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wevtapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    66198 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winbio.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_windows_ai_machinelearning.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      930 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_windows_data_pdf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      861 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_windows_networking.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1619 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_windows_ui_xaml.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4801 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_windowscodecs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    57342 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winfax.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    30571 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22445 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winhvemulation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25856 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winhvplatform.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   246872 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wininet.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      865 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winml.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    94474 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winmm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    32020 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winscard.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   114827 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winspool.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   169418 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wintrust.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22890 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_winusb.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    42226 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wlanapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wlanui.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   507152 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wldap32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2778 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wldp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3145 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wmvcore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2326 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wnvapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7202 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wofutil.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   154580 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_ws2_32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2176 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wscapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1645 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wsclient.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    33500 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wsdapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    91209 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wsmsvc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22469 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wsnmp32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    40300 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_wtsapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1775 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_xaudio2_8.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4581 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_xinputuap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3002 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_xmllite.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2284 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/definitions/win32_xpsprint.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.325707 angr-9.2.9/angr/procedures/glibc/
+-rw-r--r--   0 vsts      (1001) docker     (121)      861 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/__ctype_b_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/__ctype_tolower_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/__ctype_toupper_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      253 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/__errno_location.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      110 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1560 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/__libc_init.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11523 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/__libc_start_main.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      653 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/dynamic_loading.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      145 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       74 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/glibc/sscanf.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.325707 angr-9.2.9/angr/procedures/java/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1226 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3413 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java/unconstrained.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.329707 angr-9.2.9/angr/procedures/java_io/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_io/read.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      627 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_io/write.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.333707 angr-9.2.9/angr/procedures/java_jni/
+-rw-r--r--   0 vsts      (1001) docker     (121)    21522 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10404 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/array_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1056 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/class_and_interface_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5343 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/field_access.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1093 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/global_and_local_refs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9682 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/method_calls.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      951 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/not_implemented.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2797 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/object_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2683 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/string_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      230 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_jni/version_information.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.337708 angr-9.2.9/angr/procedures/java_lang/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1030 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/character.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      757 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/double.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/exit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      521 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/getsimplename.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1587 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/integer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      256 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/load_library.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      360 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/math.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3358 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/string.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1635 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/stringbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      428 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_lang/system.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.337708 angr-9.2.9/angr/procedures/java_util/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1348 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_util/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1762 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_util/iterator.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3912 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_util/list.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5018 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_util/map.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      388 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_util/random.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      810 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/java_util/scanner_nextline.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.357710 angr-9.2.9/angr/procedures/libc/
+-rw-r--r--   0 vsts      (1001) docker     (121)       95 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/abort.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      373 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/access.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      361 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      294 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/atol.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/calloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/closelog.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/err.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/error.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      279 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/exit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fclose.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      655 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/feof.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fflush.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      665 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fgetc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2826 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fgets.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2489 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fopen.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      818 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      620 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fputc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      745 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fputs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      697 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fread.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      242 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/free.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      646 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fscanf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1178 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fseek.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      599 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/ftell.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/fwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      402 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/getchar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4069 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/getdelim.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      214 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/getegid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      214 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/geteuid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      212 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/getgid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2639 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/gets.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      212 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/getuid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/malloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3007 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/memcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1446 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/memcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2495 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/memset.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      294 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/openlog.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      419 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/perror.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/printf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      362 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/putchar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/puts.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      195 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/rand.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      254 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/realloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      323 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/rewind.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      149 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/setbuf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      109 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/setvbuf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1359 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/snprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      739 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/sprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       89 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/srand.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/sscanf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strcat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1873 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strchr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      408 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3112 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strlen.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      516 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strncat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7392 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strncmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      598 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strncpy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      381 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strnlen.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3149 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strstr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11680 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strtol.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      271 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/strtoul.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      337 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/system.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      262 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/time.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      630 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/tmpnam.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      230 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/tolower.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      231 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/toupper.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      709 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/ungetc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/vsnprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libc/wchar.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.361711 angr-9.2.9/angr/procedures/libstdcpp/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libstdcpp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      274 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libstdcpp/_unwind_resume.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      422 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libstdcpp/std____throw_bad_alloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      420 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libstdcpp/std____throw_bad_cast.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      481 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libstdcpp/std____throw_length_error.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      479 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libstdcpp/std____throw_logic_error.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      361 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/libstdcpp/std__terminate.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.373712 angr-9.2.9/angr/procedures/linux_kernel/
+-rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      656 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/access.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1127 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/arch_prctl.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1550 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/arm_user_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      327 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/brk.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      717 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/cwd.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5013 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/fstat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6188 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/fstat64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      608 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/futex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      464 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/getegid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      463 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/geteuid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      461 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/getgid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      227 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/getpid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      832 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/getrlimit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      139 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/gettid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      460 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/getuid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1429 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/iovec.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1186 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/lseek.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      507 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/mmap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1395 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/mprotect.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/munmap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1197 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/openat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      300 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/set_tid_address.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      610 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/sigaction.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/sigprocmask.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1147 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/stat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      234 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/tgkill.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      998 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/time.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      760 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1132 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/uname.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      792 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/unlink.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      490 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_kernel/vsyscall.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.373712 angr-9.2.9/angr/procedures/linux_loader/
+-rw-r--r--   0 vsts      (1001) docker     (121)      115 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      128 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_loader/_dl_initial_error_catch_tsd.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_loader/_dl_rtld_lock.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1798 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_loader/sim_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1547 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/linux_loader/tls.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.373712 angr-9.2.9/angr/procedures/msvcr/
+-rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/msvcr/__getmainargs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      116 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/msvcr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1429 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/msvcr/_initterm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      748 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/msvcr/fmode.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.373712 angr-9.2.9/angr/procedures/ntdll/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/ntdll/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2687 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/ntdll/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.389715 angr-9.2.9/angr/procedures/posix/
+-rw-r--r--   0 vsts      (1001) docker     (121)       66 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/accept.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      413 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/bind.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      173 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/bzero.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      286 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/close.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       63 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/closedir.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2128 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/dup.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      399 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/fcntl.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2262 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/fdopen.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      500 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/fileno.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      276 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/fork.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/getenv.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      911 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/gethostbyname.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      571 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/getpass.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      278 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/getsockopt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/htonl.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      393 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/htons.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/inet_ntoa.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      414 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/listen.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4996 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/mmap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      619 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/open.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      289 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/opendir.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2116 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/poll.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1354 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/pread64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2823 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/pthread.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1361 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/pwrite64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      336 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/read.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/readdir.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/recv.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      387 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/recvfrom.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/select.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      855 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/send.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      257 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/setsockopt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/sigaction.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1622 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/sim_time.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      143 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/sleep.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      728 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/socket.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      581 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/strcasecmp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      485 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/strdup.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2552 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/strtok_r.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/syslog.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      259 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/tz.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      368 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/unlink.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      138 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/usleep.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      339 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/posix/write.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1822 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/procedure_dict.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.393715 angr-9.2.9/angr/procedures/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (121)      218 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/CallReturn.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      492 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/NoReturnUnconstrained.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      171 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/Nop.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      205 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/PathTerminator.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      565 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/Redirect.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      437 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/ReturnChar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/ReturnUnconstrained.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      256 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/UnresolvableCallTarget.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      255 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/UnresolvableJumpTarget.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      558 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/UserHook.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       67 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1579 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/b64_decode.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      432 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/caller.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1036 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/crazy_scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    27862 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/format_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      984 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/stubs/syscall_stub.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.393715 angr-9.2.9/angr/procedures/testing/
+-rw-r--r--   0 vsts      (1001) docker     (121)      106 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       99 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/testing/manyargs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      169 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/testing/retreg.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.397715 angr-9.2.9/angr/procedures/tracer/
+-rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/tracer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1079 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/tracer/random.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      586 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/tracer/receive.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      723 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/tracer/transmit.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.397715 angr-9.2.9/angr/procedures/uclibc/
+-rw-r--r--   0 vsts      (1001) docker     (121)       88 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/uclibc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      363 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/uclibc/__uClibc_main.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.401716 angr-9.2.9/angr/procedures/win32/
+-rw-r--r--   0 vsts      (1001) docker     (121)       96 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/EncodePointer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      132 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/ExitProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      226 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/GetCommandLine.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      104 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/GetCurrentProcessId.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      103 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/GetCurrentThreadId.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1092 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/GetLastInputInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      938 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/GetModuleHandle.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1137 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/GetProcessAffinityMask.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      525 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/InterlockedExchange.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      198 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/IsProcessorFeaturePresent.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3923 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/VirtualAlloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/VirtualProtect.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       86 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      275 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/critical_section.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3430 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/dynamic_loading.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1454 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/file_handles.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      316 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/gethostbyname.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1588 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/heap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      748 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/is_bad_ptr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/local_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      174 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/mutex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5271 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/sim_time.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1184 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win32/system_paths.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.401716 angr-9.2.9/angr/procedures/win_user32/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win_user32/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win_user32/chars.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      376 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win_user32/keyboard.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1733 2022-07-05 17:01:25.000000 angr-9.2.9/angr/procedures/win_user32/messagebox.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    34536 2022-07-05 17:01:25.000000 angr-9.2.9/angr/project.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.405717 angr-9.2.9/angr/protos/
+-rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-07-05 17:01:25.000000 angr-9.2.9/angr/protos/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3090 2022-07-05 17:01:25.000000 angr-9.2.9/angr/protos/cfg_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2170 2022-07-05 17:01:25.000000 angr-9.2.9/angr/protos/function_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8551 2022-07-05 17:01:25.000000 angr-9.2.9/angr/protos/primitives_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8136 2022-07-05 17:01:25.000000 angr-9.2.9/angr/protos/variables_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1271 2022-07-05 17:01:25.000000 angr-9.2.9/angr/protos/xrefs_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        7 2022-07-05 17:01:25.000000 angr-9.2.9/angr/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (121)     1508 2022-07-05 17:01:25.000000 angr-9.2.9/angr/serializable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-07-05 17:01:25.000000 angr-9.2.9/angr/service.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    36818 2022-07-05 17:01:25.000000 angr-9.2.9/angr/sim_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17256 2022-07-05 17:01:25.000000 angr-9.2.9/angr/sim_options.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24894 2022-07-05 17:01:25.000000 angr-9.2.9/angr/sim_procedure.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    38075 2022-07-05 17:01:25.000000 angr-9.2.9/angr/sim_state.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12710 2022-07-05 17:01:25.000000 angr-9.2.9/angr/sim_state_options.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   116179 2022-07-05 17:01:25.000000 angr-9.2.9/angr/sim_type.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17184 2022-07-05 17:01:25.000000 angr-9.2.9/angr/sim_variable.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.405717 angr-9.2.9/angr/simos/
+-rw-r--r--   0 vsts      (1001) docker     (121)      672 2022-07-05 17:01:25.000000 angr-9.2.9/angr/simos/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5769 2022-07-05 17:01:25.000000 angr-9.2.9/angr/simos/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22136 2022-07-05 17:01:25.000000 angr-9.2.9/angr/simos/javavm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22806 2022-07-05 17:01:25.000000 angr-9.2.9/angr/simos/linux.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18474 2022-07-05 17:01:25.000000 angr-9.2.9/angr/simos/simos.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7283 2022-07-05 17:01:25.000000 angr-9.2.9/angr/simos/userland.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25786 2022-07-05 17:01:25.000000 angr-9.2.9/angr/simos/windows.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10044 2022-07-05 17:01:25.000000 angr-9.2.9/angr/slicer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8064 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_hierarchy.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.413718 angr-9.2.9/angr/state_plugins/
+-rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12019 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/callstack.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4192 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13003 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/concrete.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    25841 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5087 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1528 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/globals.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.413718 angr-9.2.9/angr/state_plugins/heap/
+-rw-r--r--   0 vsts      (1001) docker     (121)      135 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/heap/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6439 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/heap/heap_base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5423 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/heap/heap_brk.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9280 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/heap/heap_freelist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2140 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/heap/heap_libc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    28904 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/heap/heap_ptmalloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      792 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/heap/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20424 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/history.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11451 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/inspect.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5707 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/javavm_classloader.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3453 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/jni_references.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16309 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/libc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6488 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/light_registers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2362 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/log.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4222 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/loop_data.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5933 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24672 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/posix.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7873 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/preconstrainer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5937 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/scratch.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9933 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/sim_action.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4235 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/sim_action_object.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1044 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/sim_event.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    39588 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/solver.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10896 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/symbolizer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    30329 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/trace_additions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2631 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/uc_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    75935 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/unicorn_engine.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11444 2022-07-05 17:01:25.000000 angr-9.2.9/angr/state_plugins/view.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.417718 angr-9.2.9/angr/storage/
+-rw-r--r--   0 vsts      (1001) docker     (121)      182 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    46286 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/file.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.421718 angr-9.2.9/angr/storage/memory_mixins/
+-rw-r--r--   0 vsts      (1001) docker     (121)    11649 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3535 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/actions_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17030 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/address_concretization_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2897 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/bvv_conversion_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5440 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/clouseau_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      929 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/conditional_store_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10208 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/convenient_mappings_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5611 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/default_filler_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      314 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/dirty_addrs_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3692 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/hex_dumper_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.421718 angr-9.2.9/angr/storage/memory_mixins/javavm_memory/
+-rw-r--r--   0 vsts      (1001) docker     (121)       51 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/javavm_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15550 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.425719 angr-9.2.9/angr/storage/memory_mixins/keyvalue_memory/
+-rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/keyvalue_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      894 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      857 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/label_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1197 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/multi_value_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2925 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/name_resolution_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.425719 angr-9.2.9/angr/storage/memory_mixins/paged_memory/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10022 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    26936 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.429720 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1468 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10649 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/cooperation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2720 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2049 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13755 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/list_page.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5355 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/multi_values.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15447 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      828 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1679 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18500 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1534 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/privileged_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3182 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.429720 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/
+-rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1096 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1314 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      129 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/region_category_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9201 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/region_data.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4554 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4962 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18546 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2184 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2483 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/simple_interface_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      492 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/simplification_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5667 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/size_resolution_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4732 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/slotted_memory.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5423 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/smart_find_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/symbolic_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      657 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/top_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2467 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/underconstrained_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1088 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_mixins/unwrapper_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5516 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/memory_object.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1948 2022-07-05 17:01:25.000000 angr-9.2.9/angr/storage/pcap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3240 2022-07-05 17:01:25.000000 angr-9.2.9/angr/tablespecs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4206 2022-07-05 17:01:25.000000 angr-9.2.9/angr/type_backend.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.433720 angr-9.2.9/angr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/algo.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      133 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2079 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/cowdict.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2093 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/enums_conv.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4482 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/formatting.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15164 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7160 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/library.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      425 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/mp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      820 2022-07-05 17:01:25.000000 angr-9.2.9/angr/utils/timing.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9651 2022-07-05 17:01:25.000000 angr-9.2.9/angr/vaults.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.057673 angr-9.2.9/angr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3181 2022-07-05 17:03:20.000000 angr-9.2.9/angr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)    48926 2022-07-05 17:03:21.000000 angr-9.2.9/angr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-05 17:03:20.000000 angr-9.2.9/angr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      402 2022-07-05 17:03:20.000000 angr-9.2.9/angr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        5 2022-07-05 17:03:20.000000 angr-9.2.9/angr.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:21.433720 angr-9.2.9/native/
+-rw-r--r--   0 vsts      (1001) docker     (121)      946 2022-07-05 17:01:25.000000 angr-9.2.9/native/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (121)      312 2022-07-05 17:01:25.000000 angr-9.2.9/native/Makefile-win
+-rw-r--r--   0 vsts      (1001) docker     (121)     1297 2022-07-05 17:01:25.000000 angr-9.2.9/native/angr_native.def
+-rw-r--r--   0 vsts      (1001) docker     (121)     3940 2022-07-05 17:01:25.000000 angr-9.2.9/native/log.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2754 2022-07-05 17:01:25.000000 angr-9.2.9/native/log.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   110001 2022-07-05 17:01:25.000000 angr-9.2.9/native/sim_unicorn.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    27677 2022-07-05 17:01:25.000000 angr-9.2.9/native/sim_unicorn.hpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      131 2022-07-05 17:01:34.000000 angr-9.2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1169 2022-07-05 17:03:21.433720 angr-9.2.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)     3322 2022-07-05 17:01:25.000000 angr-9.2.9/setup.py
```

### Comparing `angr-9.2.8/LICENSE` & `angr-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/PKG-INFO` & `angr-9.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr
-Version: 9.2.8
+Version: 9.2.9
 Summary: A multi-architecture binary analysis toolkit, with the ability to perform dynamic symbolic execution and various static analyses on binaries
 Home-page: https://github.com/angr/angr
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `angr-9.2.8/README.md` & `angr-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/__init__.py` & `angr-9.2.9/angr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=wildcard-import
 # pylint: disable=wrong-import-position
 
-__version__ = "9.2.8"
+__version__ = "9.2.9"
 
 if bytes is str:
     raise Exception("""
 
 =-=-=-=-=-=-=-=-=-=-=-=-=  WELCOME TO THE FUTURE!  =-=-=-=-=-=-=-=-=-=-=-=-=-=
 
 angr has transitioned to python 3. Due to the small size of the team behind it,
```

### Comparing `angr-9.2.8/angr/analyses/__init__.py` & `angr-9.2.9/angr/analyses/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/analysis.py` & `angr-9.2.9/angr/analyses/analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/backward_slice.py` & `angr-9.2.9/angr/analyses/backward_slice.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/binary_optimizer.py` & `angr-9.2.9/angr/analyses/binary_optimizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/bindiff.py` & `angr-9.2.9/angr/analyses/bindiff.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/boyscout.py` & `angr-9.2.9/angr/analyses/boyscout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/callee_cleanup_finder.py` & `angr-9.2.9/angr/analyses/callee_cleanup_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/calling_convention.py` & `angr-9.2.9/angr/analyses/calling_convention.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cdg.py` & `angr-9.2.9/angr/analyses/cdg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/cfb.py` & `angr-9.2.9/angr/analyses/cfg/cfb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg.py` & `angr-9.2.9/angr/analyses/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg_arch_options.py` & `angr-9.2.9/angr/analyses/cfg/cfg_arch_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg_base.py` & `angr-9.2.9/angr/analyses/cfg/cfg_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1441,15 +1441,15 @@
             if node.addr not in blockaddr_to_function:
                 secondary_function_nodes.add(node)
 
         missing_cfg_nodes = set(self.graph.nodes()) - traversed_cfg_nodes
         missing_cfg_nodes = { node for node in missing_cfg_nodes if node.function_address is not None }
         if missing_cfg_nodes:
             l.debug('%d CFGNodes are missing in the first traversal.', len(missing_cfg_nodes))
-            secondary_function_nodes |=  missing_cfg_nodes
+            secondary_function_nodes |= missing_cfg_nodes
 
         min_stage_3_progress = 90.0
         max_stage_3_progress = 99.9
 
         nodes_count = len(secondary_function_nodes)
         for i, fn in enumerate(sorted(secondary_function_nodes, key=lambda n: n.addr)):
```

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg_emulated.py` & `angr-9.2.9/angr/analyses/cfg/cfg_emulated.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg_fast.py` & `angr-9.2.9/angr/analyses/cfg/cfg_fast.py`

 * *Files 0% similar despite different names*

```diff
@@ -2779,14 +2779,19 @@
                         if data[i*2-2] == 0 and data[i*2-1] == 0:
                             break
                     else:
                         running_failures += 1
                         if running_failures > 3:
                             break
 
+                if content_holder is not None:
+                    string_data = data[:last_success * 2]
+                    if string_data.endswith(b'\x00\x00'):
+                        string_data = string_data[:-2]
+                    content_holder.append(string_data)
                 return MemoryDataSort.UnicodeString, last_success
 
         if data:
             try:
                 zero_pos = data.index(0)
             except ValueError:
                 zero_pos = None
```

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg_fast_soot.py` & `angr-9.2.9/angr/analyses/cfg/cfg_fast_soot.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg_job_base.py` & `angr-9.2.9/angr/analyses/cfg/cfg_job_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/cfg_utils.py` & `angr-9.2.9/angr/analyses/cfg/cfg_utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/resolver.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/resolver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py` & `angr-9.2.9/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg/segment_list.py` & `angr-9.2.9/angr/analyses/cfg/segment_list.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py` & `angr-9.2.9/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg_slice_to_sink/graph.py` & `angr-9.2.9/angr/analyses/cfg_slice_to_sink/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/cfg_slice_to_sink/transitions.py` & `angr-9.2.9/angr/analyses/cfg_slice_to_sink/transitions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/class_identifier.py` & `angr-9.2.9/angr/analyses/class_identifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/code_tagging.py` & `angr-9.2.9/angr/analyses/code_tagging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/complete_calling_conventions.py` & `angr-9.2.9/angr/analyses/complete_calling_conventions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/congruency_check.py` & `angr-9.2.9/angr/analyses/congruency_check.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/data_dep/data_dependency_analysis.py` & `angr-9.2.9/angr/analyses/data_dep/data_dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/data_dep/dep_nodes.py` & `angr-9.2.9/angr/analyses/data_dep/dep_nodes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/data_dep/sim_act_location.py` & `angr-9.2.9/angr/analyses/data_dep/sim_act_location.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/datagraph_meta.py` & `angr-9.2.9/angr/analyses/datagraph_meta.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/ddg.py` & `angr-9.2.9/angr/analyses/ddg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/__init__.py` & `angr-9.2.9/angr/analyses/decompiler/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/ail_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/ail_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/ailblock_walker.py` & `angr-9.2.9/angr/analyses/decompiler/ailblock_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/ailgraph_walker.py` & `angr-9.2.9/angr/analyses/decompiler/ailgraph_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/block_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/block_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/callsite_maker.py` & `angr-9.2.9/angr/analyses/decompiler/callsite_maker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py` & `angr-9.2.9/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/clinic.py` & `angr-9.2.9/angr/analyses/decompiler/clinic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/condition_processor.py` & `angr-9.2.9/angr/analyses/decompiler/condition_processor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/decompilation_cache.py` & `angr-9.2.9/angr/analyses/decompiler/decompilation_cache.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/decompilation_options.py` & `angr-9.2.9/angr/analyses/decompiler/decompilation_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/decompiler.py` & `angr-9.2.9/angr/analyses/decompiler/decompiler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/empty_node_remover.py` & `angr-9.2.9/angr/analyses/decompiler/empty_node_remover.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/expression_narrower.py` & `angr-9.2.9/angr/analyses/decompiler/expression_narrower.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/graph_region.py` & `angr-9.2.9/angr/analyses/decompiler/graph_region.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py` & `angr-9.2.9/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/__init__.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/const_derefs.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/const_derefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/div_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/div_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/eager_returns.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/eager_returns.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/engine_base.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/mod_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/mod_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/multi_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/multi_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/optimization_pass.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/optimization_pass.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/__init__.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/base.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/bswap.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/bswap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/conv_const_mull_a_shift.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/conv_const_mull_a_shift.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/eager_eval.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/eager_eval.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py` & `angr-9.2.9/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_identifier.py` & `angr-9.2.9/angr/analyses/decompiler/region_identifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/expr_folding.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/expr_folding.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/goto.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/goto.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/if_.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/if_.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/ifelse.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/ifelse.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/loop.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/loop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/node_address_finder.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/node_address_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_simplifiers/region_simplifier.py` & `angr-9.2.9/angr/analyses/decompiler/region_simplifiers/region_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/region_walker.py` & `angr-9.2.9/angr/analyses/decompiler/region_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/sequence_walker.py` & `angr-9.2.9/angr/analyses/decompiler/sequence_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/structured_codegen/base.py` & `angr-9.2.9/angr/analyses/decompiler/structured_codegen/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/structured_codegen/c.py` & `angr-9.2.9/angr/analyses/decompiler/structured_codegen/c.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/structured_codegen/dummy.py` & `angr-9.2.9/angr/analyses/decompiler/structured_codegen/dummy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/structured_codegen/dwarf_import.py` & `angr-9.2.9/angr/analyses/decompiler/structured_codegen/dwarf_import.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/structurer.py` & `angr-9.2.9/angr/analyses/decompiler/structurer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/structurer_nodes.py` & `angr-9.2.9/angr/analyses/decompiler/structurer_nodes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/decompiler/utils.py` & `angr-9.2.9/angr/analyses/decompiler/utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/disassembly.py` & `angr-9.2.9/angr/analyses/disassembly.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/disassembly_utils.py` & `angr-9.2.9/angr/analyses/disassembly_utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/dominance_frontier.py` & `angr-9.2.9/angr/analyses/dominance_frontier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/find_objects_static.py` & `angr-9.2.9/angr/analyses/find_objects_static.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/flirt.py` & `angr-9.2.9/angr/analyses/flirt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/forward_analysis/forward_analysis.py` & `angr-9.2.9/angr/analyses/forward_analysis/forward_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/forward_analysis/job_info.py` & `angr-9.2.9/angr/analyses/forward_analysis/job_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,18 @@
     def __init__(self, key: BlockID, job: CFGJobBase):
         self.key = key
         self.jobs = [(job, '')]
 
         self.narrowing_count = 0  # not used
 
     def __hash__(self):
-        return hash(self.key)
+        return hash((self.key,) + tuple(self.jobs))
 
     def __eq__(self, o):
-        return type(self) == type(o) and \
-               self.key == o.key
+        return type(self) == type(o) and self.key == o.key and self.job == o.job
 
     def __repr__(self):
         s = "<JobInfo %s>" % (str(self.key))
         return s
 
     @property
     def job(self) -> CFGJobBase:
```

### Comparing `angr-9.2.8/angr/analyses/forward_analysis/visitors/call_graph.py` & `angr-9.2.9/angr/analyses/forward_analysis/visitors/call_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/forward_analysis/visitors/function_graph.py` & `angr-9.2.9/angr/analyses/forward_analysis/visitors/function_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/forward_analysis/visitors/graph.py` & `angr-9.2.9/angr/analyses/forward_analysis/visitors/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/forward_analysis/visitors/loop.py` & `angr-9.2.9/angr/analyses/forward_analysis/visitors/loop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/forward_analysis/visitors/single_node_graph.py` & `angr-9.2.9/angr/analyses/forward_analysis/visitors/single_node_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/custom_callable.py` & `angr-9.2.9/angr/analyses/identifier/custom_callable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/func.py` & `angr-9.2.9/angr/analyses/identifier/func.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/__init__.py` & `angr-9.2.9/angr/analyses/identifier/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/atoi.py` & `angr-9.2.9/angr/analyses/identifier/functions/atoi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/based_atoi.py` & `angr-9.2.9/angr/analyses/identifier/functions/based_atoi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/fdprintf.py` & `angr-9.2.9/angr/analyses/identifier/functions/fdprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/free.py` & `angr-9.2.9/angr/analyses/identifier/functions/free.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/int2str.py` & `angr-9.2.9/angr/analyses/identifier/functions/int2str.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/malloc.py` & `angr-9.2.9/angr/analyses/identifier/functions/malloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/memcmp.py` & `angr-9.2.9/angr/analyses/identifier/functions/memcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/memcpy.py` & `angr-9.2.9/angr/analyses/identifier/functions/memcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/memset.py` & `angr-9.2.9/angr/analyses/identifier/functions/memset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/printf.py` & `angr-9.2.9/angr/analyses/identifier/functions/printf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/recv_until.py` & `angr-9.2.9/angr/analyses/identifier/functions/recv_until.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/skip_calloc.py` & `angr-9.2.9/angr/analyses/identifier/functions/skip_calloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/skip_realloc.py` & `angr-9.2.9/angr/analyses/identifier/functions/skip_realloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/skip_recv_n.py` & `angr-9.2.9/angr/analyses/identifier/functions/skip_recv_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/snprintf.py` & `angr-9.2.9/angr/analyses/identifier/functions/snprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/sprintf.py` & `angr-9.2.9/angr/analyses/identifier/functions/sprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/strcasecmp.py` & `angr-9.2.9/angr/analyses/identifier/functions/strcasecmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/strcmp.py` & `angr-9.2.9/angr/analyses/identifier/functions/strcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/strcpy.py` & `angr-9.2.9/angr/analyses/identifier/functions/strcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/strlen.py` & `angr-9.2.9/angr/analyses/identifier/functions/strlen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/strncmp.py` & `angr-9.2.9/angr/analyses/identifier/functions/strncmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/strncpy.py` & `angr-9.2.9/angr/analyses/identifier/functions/strncpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/functions/strtol.py` & `angr-9.2.9/angr/analyses/identifier/functions/strtol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/identify.py` & `angr-9.2.9/angr/analyses/identifier/identify.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/identifier/runner.py` & `angr-9.2.9/angr/analyses/identifier/runner.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/init_finder.py` & `angr-9.2.9/angr/analyses/init_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/loop_analysis.py` & `angr-9.2.9/angr/analyses/loop_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/loopfinder.py` & `angr-9.2.9/angr/analyses/loopfinder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/call_expr_finder.py` & `angr-9.2.9/angr/analyses/propagator/call_expr_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/engine_ail.py` & `angr-9.2.9/angr/analyses/propagator/engine_ail.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/engine_base.py` & `angr-9.2.9/angr/analyses/propagator/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/engine_vex.py` & `angr-9.2.9/angr/analyses/propagator/engine_vex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/outdated_definition_walker.py` & `angr-9.2.9/angr/analyses/propagator/outdated_definition_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/prop_value.py` & `angr-9.2.9/angr/analyses/propagator/prop_value.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/propagator.py` & `angr-9.2.9/angr/analyses/propagator/propagator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/values.py` & `angr-9.2.9/angr/analyses/propagator/values.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/propagator/vex_vars.py` & `angr-9.2.9/angr/analyses/propagator/vex_vars.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/proximity_graph.py` & `angr-9.2.9/angr/analyses/proximity_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/__init__.py` & `angr-9.2.9/angr/analyses/reaching_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/call_trace.py` & `angr-9.2.9/angr/analyses/reaching_definitions/call_trace.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/dep_graph.py` & `angr-9.2.9/angr/analyses/reaching_definitions/dep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/engine_ail.py` & `angr-9.2.9/angr/analyses/reaching_definitions/engine_ail.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/engine_vex.py` & `angr-9.2.9/angr/analyses/reaching_definitions/engine_vex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/function_handler.py` & `angr-9.2.9/angr/analyses/reaching_definitions/function_handler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/heap_allocator.py` & `angr-9.2.9/angr/analyses/reaching_definitions/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/rd_state.py` & `angr-9.2.9/angr/analyses/reaching_definitions/rd_state.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/reaching_definitions.py` & `angr-9.2.9/angr/analyses/reaching_definitions/reaching_definitions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reaching_definitions/subject.py` & `angr-9.2.9/angr/analyses/reaching_definitions/subject.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/reassembler.py` & `angr-9.2.9/angr/analyses/reassembler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/soot_class_hierarchy.py` & `angr-9.2.9/angr/analyses/soot_class_hierarchy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/stack_pointer_tracker.py` & `angr-9.2.9/angr/analyses/stack_pointer_tracker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/static_hooker.py` & `angr-9.2.9/angr/analyses/static_hooker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/typehoon/lifter.py` & `angr-9.2.9/angr/analyses/typehoon/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/typehoon/simple_solver.py` & `angr-9.2.9/angr/analyses/typehoon/simple_solver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/typehoon/translator.py` & `angr-9.2.9/angr/analyses/typehoon/translator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/typehoon/typeconsts.py` & `angr-9.2.9/angr/analyses/typehoon/typeconsts.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/typehoon/typehoon.py` & `angr-9.2.9/angr/analyses/typehoon/typehoon.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/typehoon/typevars.py` & `angr-9.2.9/angr/analyses/typehoon/typevars.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/variable_recovery/annotations.py` & `angr-9.2.9/angr/analyses/variable_recovery/annotations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/variable_recovery/engine_ail.py` & `angr-9.2.9/angr/analyses/variable_recovery/engine_ail.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 
 class SimEngineVRAIL(
     SimEngineLightAILMixin,
     SimEngineVRBase,
 ):
     state: 'VariableRecoveryFastState'
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, call_info=None, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._reference_spoffset: bool = False
+        self.call_info = call_info or {}
 
     # Statement handlers
 
     def _ail_handle_Assignment(self, stmt):
         dst_type = type(stmt.dst)
 
         if dst_type is ailment.Expr.Register:
```

### Comparing `angr-9.2.8/angr/analyses/variable_recovery/engine_base.py` & `angr-9.2.9/angr/analyses/variable_recovery/engine_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         existing_vars: Set[Tuple[SimVariable,int]]
         if not existing_vars:
             variable = SimRegisterVariable(offset, size,
                                            ident=self.variable_manager[self.func_addr].next_variable_ident(
                                                'register'),
                                            region=self.func_addr
                                            )
-            self.variable_manager[self.func_addr].set_variable('register', offset, variable)
+            self.variable_manager[self.func_addr].add_variable('register', offset, variable)
         else:
             variable, _ = next(iter(existing_vars))
 
         # FIXME: The offset does not have to be 0
         annotated_data = self.state.annotate_with_variables(data, [(0, variable)])
         v = MultiValues(offset_to_values={0: {annotated_data}})
         self.state.register_region.store(offset, v)
```

### Comparing `angr-9.2.8/angr/analyses/variable_recovery/engine_vex.py` & `angr-9.2.9/angr/analyses/variable_recovery/engine_vex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 # pylint:disable=unused-argument
 from typing import TYPE_CHECKING
 
 import claripy
 import pyvex
 from archinfo.arch_arm import is_arm_arch
 
+from ...errors import SimMemoryMissingError
+from ...calling_conventions import SimRegArg, SimStackArg
 from ...engines.vex.claripy.datalayer import value as claripy_value
 from ...engines.light import SimEngineLightVEXMixin
 from ..typehoon import typevars, typeconsts
 from .engine_base import SimEngineVRBase, RichR
+from ...knowledge_plugins import Function
+from ...storage.memory_mixins.paged_memory.pages.multi_values import MultiValues
 
 if TYPE_CHECKING:
     from .variable_recovery_base import VariableRecoveryStateBase
 
 
 class SimEngineVRVEX(
     SimEngineLightVEXMixin,
     SimEngineVRBase,
 ):
     """
     Implements the VEX engine for variable recovery analysis.
     """
     state: 'VariableRecoveryStateBase'
 
+    def __init__(self, *args, call_info=None, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.call_info = call_info or {}
+
     # Statement handlers
 
     def _handle_Put(self, stmt):
         offset = stmt.offset
         r = self._expr(stmt.data)
         size = stmt.data.result_size(self.tyenv) // 8
 
@@ -133,16 +142,37 @@
         return RichR(self.state.top(expr.result_size(self.tyenv)))
 
     def _handle_Conversion(self, expr: pyvex.IRExpr.Unop) -> RichR:
         return RichR(self.state.top(expr.result_size(self.tyenv)))
 
     # Function handlers
 
-    def _handle_function(self, func_addr):  # pylint:disable=unused-argument,no-self-use,useless-return
-        return None
+    def _handle_function_concrete(self, func: Function):
+        if func.prototype is None or func.calling_convention is None:
+            return
+
+        for arg_loc in func.calling_convention.arg_locs(func.prototype):
+            for loc in arg_loc.get_footprint():
+                if isinstance(loc, SimRegArg):
+                    self._read_from_register(self.arch.registers[loc.reg_name][0] + loc.reg_offset, loc.size)
+                elif isinstance(loc, SimStackArg):
+                    try:
+                        sp: MultiValues = self.state.register_region.load(self.arch.sp_offset, self.arch.bytes)
+                    except SimMemoryMissingError:
+                        pass
+                    else:
+                        one_sp = sp.one_value()
+                        if one_sp is not None:
+                            addr = RichR(loc.stack_offset + one_sp)
+                            self._load(addr, loc.size)
+
+    def _process_block_end(self):
+        current_addr = self.state.block_addr
+        for target_func in self.call_info.get(current_addr, []):
+            self._handle_function_concrete(target_func)
 
     def _handle_Const(self, expr):
         return RichR(claripy_value(expr.con.type, expr.con.value, size=expr.con.size),
                      typevar=typeconsts.int_type(expr.con.size))
 
     def _handle_Add(self, expr):
         arg0, arg1 = expr.args
```

### Comparing `angr-9.2.8/angr/analyses/variable_recovery/variable_recovery.py` & `angr-9.2.9/angr/analyses/variable_recovery/variable_recovery.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/variable_recovery/variable_recovery_base.py` & `angr-9.2.9/angr/analyses/variable_recovery/variable_recovery_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/variable_recovery/variable_recovery_fast.py` & `angr-9.2.9/angr/analyses/variable_recovery/variable_recovery_fast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pylint:disable=wrong-import-position,wrong-import-order
 from typing import Optional, List, Tuple
 import logging
 from collections import defaultdict
 
+import networkx
+
 import claripy
 import pyvex
 import ailment
 
 import angr.errors
 from ...storage.memory_mixins.paged_memory.pages.multi_values import MultiValues
 from ...block import Block
@@ -187,25 +189,37 @@
 
 
 class VariableRecoveryFast(ForwardAnalysis, VariableRecoveryBase):  #pylint:disable=abstract-method
     """
     Recover "variables" from a function by keeping track of stack pointer offsets and pattern matching VEX statements.
 
     If calling conventions are recovered prior to running VariableRecoveryFast, variables can be recognized more
-    accurately. However, it is not a requirement.
+    accurately. However, it is not a requirement. In this case, the function graph you pass must contain information
+    indicating the call-out sites inside the analyzed function. These graph edges must be annotated with either
+    ``"type": "call"`` or ``"outside": True``.
     """
 
-    def __init__(self, func, func_graph=None, max_iterations=2, low_priority=False, track_sp=True,
-                 func_args: Optional[List[SimVariable]]=None, store_live_variables=False):
-        """
-
-        :param knowledge.Function func:  The function to analyze.
-        :param int max_iterations:
-        :param clinic:
-        """
+    def __init__(
+            self,
+            func: Function,
+            func_graph: Optional[networkx.DiGraph]=None,
+            max_iterations: int=2,
+            low_priority=False,
+            track_sp=True,
+            func_args: Optional[List[SimVariable]]=None,
+            store_live_variables=False
+    ):
+        func_graph_with_calls = func_graph or func.transition_graph
+        call_info = defaultdict(list)
+        for node_from, node_to, data in func_graph_with_calls.edges(data=True):
+            if data.get('type', None) == 'call' or data.get('outside', False):
+                try:
+                    call_info[node_from.addr].append(self.kb.functions.get_by_addr(node_to.addr))
+                except KeyError:
+                    pass
 
         function_graph_visitor = FunctionGraphVisitor(func, graph=func_graph)
 
         # Make sure the function is not empty
         if not func.block_addrs_set or func.startpoint is None:
             raise AngrVariableRecoveryError("Function %s is empty." % repr(func))
 
@@ -214,16 +228,16 @@
                                  graph_visitor=function_graph_visitor)
 
         self._low_priority = low_priority
         self._job_ctr = 0
         self._track_sp = track_sp and self.project.arch.sp_offset is not None
         self._func_args = func_args
 
-        self._ail_engine = SimEngineVRAIL(self.project, self.kb)
-        self._vex_engine = SimEngineVRVEX(self.project, self.kb)
+        self._ail_engine = SimEngineVRAIL(self.project, self.kb, call_info=call_info)
+        self._vex_engine = SimEngineVRVEX(self.project, self.kb, call_info=call_info)
 
         self._node_iterations = defaultdict(int)
 
         self._node_to_cc = { }
         self.var_to_typevars = defaultdict(set)
         self.type_constraints = None
```

### Comparing `angr-9.2.8/angr/analyses/veritesting.py` & `angr-9.2.9/angr/analyses/veritesting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/vfg.py` & `angr-9.2.9/angr/analyses/vfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/vsa_ddg.py` & `angr-9.2.9/angr/analyses/vsa_ddg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/vtable.py` & `angr-9.2.9/angr/analyses/vtable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/analyses/xrefs.py` & `angr-9.2.9/angr/analyses/xrefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/db.py` & `angr-9.2.9/angr/angrdb/db.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/models.py` & `angr-9.2.9/angr/angrdb/models.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/cfg_model.py` & `angr-9.2.9/angr/angrdb/serializers/cfg_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/comments.py` & `angr-9.2.9/angr/angrdb/serializers/comments.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/funcs.py` & `angr-9.2.9/angr/angrdb/serializers/funcs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/kb.py` & `angr-9.2.9/angr/angrdb/serializers/kb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/labels.py` & `angr-9.2.9/angr/angrdb/serializers/labels.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/loader.py` & `angr-9.2.9/angr/angrdb/serializers/loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/structured_code.py` & `angr-9.2.9/angr/angrdb/serializers/structured_code.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/variables.py` & `angr-9.2.9/angr/angrdb/serializers/variables.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/angrdb/serializers/xrefs.py` & `angr-9.2.9/angr/angrdb/serializers/xrefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/annocfg.py` & `angr-9.2.9/angr/annocfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/blade.py` & `angr-9.2.9/angr/blade.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/block.py` & `angr-9.2.9/angr/block.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/callable.py` & `angr-9.2.9/angr/callable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/calling_conventions.py` & `angr-9.2.9/angr/calling_conventions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/code_location.py` & `angr-9.2.9/angr/code_location.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,27 +76,31 @@
     def __eq__(self, other):
         """
         Check if self is the same as other.
         """
         return type(self) is type(other) and self.block_addr == other.block_addr and \
                 self.stmt_idx == other.stmt_idx and self.sim_procedure is other.sim_procedure and \
                 self.context == other.context and \
-                self.block_idx == other.block_idx
+                self.block_idx == other.block_idx and \
+                self.ins_addr == other.ins_addr
 
     def __lt__(self, other):
         if self.block_addr != other.block_addr:
             return self.block_addr < other.block_addr
+        if self.ins_addr is not None and other.ins_addr is not None:
+            if self.ins_addr != other.ins_addr:
+                return self.ins_addr < other.ins_addr
         if self.stmt_idx != other.stmt_idx:
             return self.stmt_idx < other.stmt_idx
         return False
 
     def __hash__(self):
         """
         returns the hash value of self.
         """
-        return hash((self.block_addr, self.stmt_idx, self.sim_procedure, self.context, self.block_idx))
+        return hash((self.block_addr, self.stmt_idx, self.sim_procedure, self.ins_addr, self.context, self.block_idx))
 
     def _store_kwargs(self, **kwargs):
         if self.info is None:
             self.info = { }
         for k, v in kwargs.items():
             self.info[k] = v
```

### Comparing `angr-9.2.8/angr/codenode.py` & `angr-9.2.9/angr/codenode.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/__init__.py` & `angr-9.2.9/angr/concretization_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/controlled_data.py` & `angr-9.2.9/angr/concretization_strategies/controlled_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/eval.py` & `angr-9.2.9/angr/concretization_strategies/eval.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/max.py` & `angr-9.2.9/angr/concretization_strategies/max.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/nonzero.py` & `angr-9.2.9/angr/concretization_strategies/nonzero.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/nonzero_range.py` & `angr-9.2.9/angr/concretization_strategies/nonzero_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/norepeats.py` & `angr-9.2.9/angr/concretization_strategies/norepeats.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/norepeats_range.py` & `angr-9.2.9/angr/concretization_strategies/norepeats_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/range.py` & `angr-9.2.9/angr/concretization_strategies/range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/solutions.py` & `angr-9.2.9/angr/concretization_strategies/solutions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/concretization_strategies/unlimited_range.py` & `angr-9.2.9/angr/concretization_strategies/unlimited_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/distributed/server.py` & `angr-9.2.9/angr/distributed/server.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/distributed/worker.py` & `angr-9.2.9/angr/distributed/worker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/__init__.py` & `angr-9.2.9/angr/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/concrete.py` & `angr-9.2.9/angr/engines/concrete.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/engine.py` & `angr-9.2.9/angr/engines/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/failure.py` & `angr-9.2.9/angr/engines/failure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/hook.py` & `angr-9.2.9/angr/engines/hook.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/light/data.py` & `angr-9.2.9/angr/engines/light/data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/light/engine.py` & `angr-9.2.9/angr/engines/light/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def __init__(self):
 
         logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
         super(SimEngineLight, self).__init__(logger=logger)
 
         # local variables
         self.state = None
-        self.arch = None
+        self.arch: archinfo.Arch = None
         self.block = None
         self._call_stack = None
 
         self.stmt_idx = None
         self.ins_addr = None
         self.tmps = None
```

### Comparing `angr-9.2.8/angr/engines/pcode/arch.py` & `angr-9.2.9/angr/engines/pcode/arch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/pcode/behavior.py` & `angr-9.2.9/angr/engines/pcode/behavior.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/pcode/emulate.py` & `angr-9.2.9/angr/engines/pcode/emulate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/pcode/engine.py` & `angr-9.2.9/angr/engines/pcode/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/pcode/lifter.py` & `angr-9.2.9/angr/engines/pcode/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/procedure.py` & `angr-9.2.9/angr/engines/procedure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/engine.py` & `angr-9.2.9/angr/engines/soot/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/__init__.py` & `angr-9.2.9/angr/engines/soot/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/arrayref.py` & `angr-9.2.9/angr/engines/soot/expressions/arrayref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/binop.py` & `angr-9.2.9/angr/engines/soot/expressions/binop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/cast.py` & `angr-9.2.9/angr/engines/soot/expressions/cast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/condition.py` & `angr-9.2.9/angr/engines/soot/expressions/condition.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/constants.py` & `angr-9.2.9/angr/engines/soot/expressions/constants.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/invoke.py` & `angr-9.2.9/angr/engines/soot/expressions/invoke.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/new.py` & `angr-9.2.9/angr/engines/soot/expressions/new.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/newArray.py` & `angr-9.2.9/angr/engines/soot/expressions/newArray.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/newMultiArray.py` & `angr-9.2.9/angr/engines/soot/expressions/newMultiArray.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/expressions/phi.py` & `angr-9.2.9/angr/engines/soot/expressions/phi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/field_dispatcher.py` & `angr-9.2.9/angr/engines/soot/field_dispatcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/method_dispatcher.py` & `angr-9.2.9/angr/engines/soot/method_dispatcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/statements/__init__.py` & `angr-9.2.9/angr/engines/soot/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/statements/assign.py` & `angr-9.2.9/angr/engines/soot/statements/assign.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/statements/base.py` & `angr-9.2.9/angr/engines/soot/statements/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/statements/if_.py` & `angr-9.2.9/angr/engines/soot/statements/if_.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/statements/return_.py` & `angr-9.2.9/angr/engines/soot/statements/return_.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/statements/switch.py` & `angr-9.2.9/angr/engines/soot/statements/switch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/values/__init__.py` & `angr-9.2.9/angr/engines/soot/values/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/values/arrayref.py` & `angr-9.2.9/angr/engines/soot/values/arrayref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/values/instancefieldref.py` & `angr-9.2.9/angr/engines/soot/values/instancefieldref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/values/staticfieldref.py` & `angr-9.2.9/angr/engines/soot/values/staticfieldref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/values/strref.py` & `angr-9.2.9/angr/engines/soot/values/strref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/soot/values/thisref.py` & `angr-9.2.9/angr/engines/soot/values/thisref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/successors.py` & `angr-9.2.9/angr/engines/successors.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/syscall.py` & `angr-9.2.9/angr/engines/syscall.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/unicorn.py` & `angr-9.2.9/angr/engines/unicorn.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/claripy/ccall.py` & `angr-9.2.9/angr/engines/vex/claripy/ccall.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/claripy/datalayer.py` & `angr-9.2.9/angr/engines/vex/claripy/datalayer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/claripy/irop.py` & `angr-9.2.9/angr/engines/vex/claripy/irop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/heavy/actions.py` & `angr-9.2.9/angr/engines/vex/heavy/actions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/heavy/dirty.py` & `angr-9.2.9/angr/engines/vex/heavy/dirty.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/heavy/heavy.py` & `angr-9.2.9/angr/engines/vex/heavy/heavy.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             o.UNICORN_HANDLE_SYMBOLIC_CONDITIONS in self.state.options) and data.symbolic:
             # Update the concrete memory value before updating symbolic value so that correct values are mapped into
             # native interface
             concrete_data = claripy.BVV(self.state.solver.eval(data), data.size())
             self.state.memory.store(addr, concrete_data, endness=endness, action=None, inspect=False,
                                     condition=condition)
 
-        self.state.memory.store(addr, data, endness=endness, action=action, inspect=inspect, condition=condition)
+        self.state.memory.store(addr, data, size=data.size() // 8, endness=endness, action=action, inspect=inspect, condition=condition)
 
     def _perform_vex_stmt_WrTmp(self, tmp, data, deps=None):
         self.state.scratch.store_tmp(tmp, data, deps=deps)
 
 
 # pylint:disable=arguments-differ
 class HeavyVEXMixin(SuccessorsMixin, ClaripyDataMixin, SimStateStorageMixin, VEXMixin, VEXLifter):
```

### Comparing `angr-9.2.8/angr/engines/vex/heavy/inspect.py` & `angr-9.2.9/angr/engines/vex/heavy/inspect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/heavy/resilience.py` & `angr-9.2.9/angr/engines/vex/heavy/resilience.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/heavy/super_fastpath.py` & `angr-9.2.9/angr/engines/vex/heavy/super_fastpath.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/lifter.py` & `angr-9.2.9/angr/engines/vex/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/light/light.py` & `angr-9.2.9/angr/engines/vex/light/light.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/light/resilience.py` & `angr-9.2.9/angr/engines/vex/light/resilience.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/engines/vex/light/slicing.py` & `angr-9.2.9/angr/engines/vex/light/slicing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/errors.py` & `angr-9.2.9/angr/errors.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/__init__.py` & `angr-9.2.9/angr/exploration_techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/bucketizer.py` & `angr-9.2.9/angr/exploration_techniques/bucketizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/cacher.py` & `angr-9.2.9/angr/exploration_techniques/cacher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/common.py` & `angr-9.2.9/angr/exploration_techniques/common.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/dfs.py` & `angr-9.2.9/angr/exploration_techniques/dfs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/director.py` & `angr-9.2.9/angr/exploration_techniques/director.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/driller_core.py` & `angr-9.2.9/angr/exploration_techniques/driller_core.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/explorer.py` & `angr-9.2.9/angr/exploration_techniques/explorer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/lengthlimiter.py` & `angr-9.2.9/angr/exploration_techniques/lengthlimiter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/local_loop_seer.py` & `angr-9.2.9/angr/exploration_techniques/local_loop_seer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/loop_seer.py` & `angr-9.2.9/angr/exploration_techniques/loop_seer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/manual_mergepoint.py` & `angr-9.2.9/angr/exploration_techniques/manual_mergepoint.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/memory_watcher.py` & `angr-9.2.9/angr/exploration_techniques/memory_watcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/oppologist.py` & `angr-9.2.9/angr/exploration_techniques/oppologist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/slicecutor.py` & `angr-9.2.9/angr/exploration_techniques/slicecutor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/spiller.py` & `angr-9.2.9/angr/exploration_techniques/spiller.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/spiller_db.py` & `angr-9.2.9/angr/exploration_techniques/spiller_db.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/stochastic.py` & `angr-9.2.9/angr/exploration_techniques/stochastic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/symbion.py` & `angr-9.2.9/angr/exploration_techniques/symbion.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/tech_builder.py` & `angr-9.2.9/angr/exploration_techniques/tech_builder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/threading.py` & `angr-9.2.9/angr/exploration_techniques/threading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/timeout.py` & `angr-9.2.9/angr/exploration_techniques/timeout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/tracer.py` & `angr-9.2.9/angr/exploration_techniques/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,28 @@
     """
     Strict = 'strict'
     Permissive = 'permissive'
     CatchDesync = 'catch_desync'
 
 
 class TracerDesyncError(AngrTracerError):
+    """
+    An error class to report tracing Tracing desyncronization error
+    """
     def __init__(self, msg, deviating_addr=None, deviating_trace_idx=None):
         super().__init__(msg)
         self.deviating_addr = deviating_addr
         self.deviating_trace_idx = deviating_trace_idx
 
 
 class RepHook:
+    """
+    Hook rep movs/stos to speed up constraint solving
+    TODO: This should be made an exploration technique later
+    """
     def __init__(self, mnemonic):
         self.mnemonic = mnemonic
 
     @staticmethod
     def _inline_call(state, procedure, *arguments, **kwargs):
         e_args = [state.solver.BVV(a, state.arch.bits) if isinstance(a, int) else a for a in arguments]
         p = procedure(project=state.project, **kwargs)
@@ -234,19 +241,21 @@
                     else:
                         possibilities.intersection_update(slides)
 
                 if possibilities is None:
                     continue
 
                 if len(possibilities) == 0:
-                    raise AngrTracerError("Trace does not seem to contain object initializers for %s. Do you want to have a Tracer(aslr=False)?" % obj)
+                    raise AngrTracerError("Trace does not seem to contain object initializers for %s. "
+                                          "Do you want to have a Tracer(aslr=False)?" % obj)
                 if len(possibilities) == 1:
                     self._aslr_slides[obj] = next(iter(possibilities))
                 else:
-                    raise AngrTracerError("Trace seems ambiguous with respect to what the ASLR slides are for %s. This is surmountable, please open an issue." % obj)
+                    raise AngrTracerError("Trace seems ambiguous with respect to what the ASLR slides are for %s. "
+                                          "This is surmountable, please open an issue." % obj)
         else:
             # if we know there is no slides, just trust the address in the loader
             for obj in self.project.loader.all_objects:
                 # do not analyze pseudo-objects
                 if obj.binary_basename.startswith('cle##'):
                     continue
                 self._aslr_slides[obj] = 0
@@ -286,15 +295,16 @@
             idx = self._trace.index(self._translate_state_addr(self.project.entry))
             # step to entry point
             while simgr.one_active.addr != self.project.entry:
                 simgr.step(extra_stop_points={self.project.entry})
                 if len(simgr.active) == 0:
                     raise AngrTracerError("Could not step to the first address of the trace - simgr is empty")
                 if len(simgr.active) > 1:
-                    raise AngrTracerError("Could not step to the first address of the trace - state split. Do you want to have a Tracer(fast_forward_to_entry=False)?")
+                    raise AngrTracerError("Could not step to the first address of the trace - state split. "
+                                          "Do you want to have a Tracer(fast_forward_to_entry=False)?")
                 simgr.drop(stash='unsat')
         else:
             idx = 0
 
         # initialize the state info
         simgr.one_active.globals['trace_idx'] = idx
         simgr.one_active.globals['sync_idx'] = None
@@ -516,15 +526,16 @@
                         # Found the address in trace. Start normal trace checks from next address
                         idx = sync + 1
                         state.globals['sync_idx'] = None
                         sync = None
 
                     continue
 
-                if self._compare_addr(self._trace[idx], addr) or self._check_qemu_unicorn_large_block_split(state, idx, addr_idx):
+                if self._compare_addr(self._trace[idx], addr) or \
+                   self._check_qemu_unicorn_large_block_split(state, idx, addr_idx):
                     idx += 1
                 else:
                     is_contained, increment = self._check_qemu_block_in_unicorn_block(state, idx, addr_idx)
                     if is_contained:
                         idx += increment
                         # Big block is now skipped in qemu trace. Perform compare at correct index again.
                         if self._compare_addr(self._trace[idx], addr):
@@ -548,38 +559,41 @@
             if self._compare_addr(self._trace[sync], state.addr):
                 state.globals['trace_idx'] = sync
                 state.globals['sync_idx'] = None
                 state.globals['sync_timer'] = 0
             elif timer > 0:
                 state.globals['sync_timer'] = timer
             else:
-                raise Exception("Trace failed to synchronize! We expected it to hit %#x (trace addr), but it failed to do this within a timeout" % self._trace[sync])
+                raise Exception("Trace failed to synchronize! We expected it to hit %#x (trace addr), "
+                                "but it failed to do this within a timeout" % self._trace[sync])
 
         elif state.history.jumpkind.startswith('Ijk_Exit'):
             # termination! will be handled by filter
             pass
         elif self.project.is_hooked(state.addr) and not self.project.loader.extern_object.contains_addr(state.addr):
             # handle simprocedures
             self._sync_return(state, idx)
         elif self._compare_addr(self._trace[idx + 1], state.addr):
             # normal case
             state.globals['trace_idx'] = idx + 1
-        elif self.project.loader._extern_object is not None and self.project.loader.extern_object.contains_addr(state.addr):
+        elif self.project.loader._extern_object is not None \
+             and self.project.loader.extern_object.contains_addr(state.addr):
             # externs
             proc = self.project.hooked_by(state.addr)
             if proc is None:
                 raise Exception("Extremely bad news: we're executing an unhooked address in the externs space")
             if proc.display_name == 'LinuxLoader':
                 state.globals['sync_idx'] = 'entry'
             elif proc.is_continuation:
                 orig_addr = self.project.loader.find_symbol(proc.display_name).rebased_addr
                 obj = self.project.loader.find_object_containing(orig_addr)
                 orig_trace_addr = self._translate_state_addr(orig_addr, obj)
                 if 0 <= self._trace[idx + 1] - orig_trace_addr <= 0x10000:
-                    # this is fine. we do nothing and then next round it'll get handled by the is_hooked(state.history.addr) case
+                    # this is fine. we do nothing and then next round
+                    # it'll get handled by the is_hooked(state.history.addr) case
                     pass
                 else:
                     # this may also be triggered as a consequence of the unicorn issue linked above
                     raise Exception("BUG: State is returning to a continuation that isn't its own???")
             elif state.addr == getattr(self.project.simos, 'vsyscall_addr', None):
                 if not self._sync_callsite(state, idx, state.history.addr):
                     raise AngrTracerError("Could not synchronize following vsyscall")
@@ -598,41 +612,42 @@
             self._fast_forward(state)
         elif state.addr == self._trace[-1]:
             # we may have prematurely stopped because of setting stop points. try to resync.
             state.globals['sync_idx'] = idx + 1
             state.globals['sync_timer'] = 1
         elif self.project.is_hooked(state.addr) and \
                 self.project.loader.find_symbol(self.project.hooked_by(state.addr).display_name) is not None and \
-                self.project.loader.find_symbol(self.project.hooked_by(state.addr).display_name).subtype.value[0] == 10:  # STT_GNU_IFUNC
+                self.project.loader.find_symbol(self.project.hooked_by(state.addr).display_name).subtype.value[0] == 10:  # STT_GNU_IFUNC #pylint:disable=line-too-long
             if not self._sync_return(state, idx):
                 raise AngrTracerError("Could not synchronize at ifunc return address")
         elif self._analyze_misfollow(state, idx):
             # misfollow analysis will set a sync point somewhere if it succeeds
             pass
         else:
             raise TracerDesyncError("Oops! angr did not follow the trace",
                                     deviating_addr=state.addr,
                                     deviating_trace_idx=idx+1)
 
         if state.globals['sync_idx'] is not None:
-            l.debug("Trace: %s-%s/%s synchronizing %s", state.globals['trace_idx'], state.globals['sync_idx'], len(self._trace), state.globals['sync_timer'])
+            l.debug("Trace: %s-%s/%s synchronizing %s", state.globals['trace_idx'], state.globals['sync_idx'],
+                                                        len(self._trace), state.globals['sync_timer'])
         else:
             l.debug("Trace: %s/%s", state.globals['trace_idx'], len(self._trace))
 
     def _translate_state_addr(self, state_addr, obj=None):
         if obj is None:
             obj = self.project.loader.find_object_containing(state_addr)
         if obj not in self._aslr_slides:
             raise Exception("Internal error: cannot translate address")
         return state_addr + self._aslr_slides[obj]
 
     def _translate_trace_addr(self, trace_addr, obj=None):
         if obj is None:
-            for obj in self._aslr_slides:  # pylint: disable=redefined-argument-from-local
-                if obj.contains_addr(trace_addr - self._aslr_slides[obj]):
+            for obj, slide in self._aslr_slides.items():  # pylint: disable=redefined-argument-from-local
+                if obj.contains_addr(trace_addr - slide):
                     break
             else:
                 raise Exception("Can't figure out which object this address belongs to")
         if obj not in self._aslr_slides:
             raise Exception("Internal error: object is untranslated")
         return trace_addr - self._aslr_slides[obj]
 
@@ -647,15 +662,16 @@
             self._current_slide = self._aslr_slides[current_bin]
             return trace_addr == state_addr + self._current_slide
         elif ((trace_addr - state_addr) & 0xfff) == 0:
             self._aslr_slides[current_bin] = self._current_slide = trace_addr - state_addr
             return True
         # error handling
         elif current_bin:
-            raise AngrTracerError("Trace desynced on jumping into %s. Did you load the right version of this library?" % current_bin.provides)
+            raise AngrTracerError("Trace desynced on jumping into %s. "
+                                  "Did you load the right version of this library?" % current_bin.provides)
         else:
             raise AngrTracerError("Trace desynced on jumping into %#x, where no library is mapped!" % state_addr)
 
     def _check_qemu_block_in_unicorn_block(self, state: 'angr.SimState', trace_curr_idx, state_desync_block_idx):
         """
         Check if desync occurred because unicorn block was split into multiple blocks in qemu tracer. If yes, find the
         correct increment for trace index
@@ -900,24 +916,29 @@
             target_idx = self._trace.index(target_addr, state.globals['trace_idx'])
         except ValueError as e:
             # if the user wants to catch desync caused by sim_procedure,
             # mark this state as a desync state and then end the tracing prematurely
             if self._mode == TracingMode.CatchDesync:
                 state.globals['is_desync'] = True
                 return
-            raise AngrTracerError("Trace failed to synchronize during fast forward? You might want to unhook %s." % (self.project.hooked_by(state.history.addr).display_name)) from e
+            raise AngrTracerError("Trace failed to synchronize during fast forward? You might want to unhook %s." %
+                                             (self.project.hooked_by(state.history.addr).display_name)) from e
         else:
             state.globals['trace_idx'] = target_idx
 
     @classmethod
     def crash_windup(cls, state, crash_addr):
         # first check: are we just executing user-controlled code?
         if not state.ip.symbolic and state.mem[state.ip].char.resolved.symbolic:
             l.debug("executing input-related code")
             return state, state
+        # second check: is this code mapped and executable?
+        section = state.project.loader.find_section_containing(state.addr)
+        if not section or not (section.flags & 0x4): # pylint:disable=superfluous-parens
+            return state, state
         # in case we can't unwind, we return the state itself
         if state.addr == crash_addr:
             return state, state
 
         state = state.copy()
         state.options.add(sim_options.COPY_STATES)
         state.options.discard(sim_options.STRICT_PAGE_ACCESS)
```

### Comparing `angr-9.2.8/angr/exploration_techniques/unique.py` & `angr-9.2.9/angr/exploration_techniques/unique.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/exploration_techniques/veritesting.py` & `angr-9.2.9/angr/exploration_techniques/veritesting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/factory.py` & `angr-9.2.9/angr/factory.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/flirt/__init__.py` & `angr-9.2.9/angr/flirt/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/flirt/build_sig.py` & `angr-9.2.9/angr/flirt/build_sig.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/keyed_region.py` & `angr-9.2.9/angr/keyed_region.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_base/knowledge_base.py` & `angr-9.2.9/angr/knowledge_base/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/__init__.py` & `angr-9.2.9/angr/knowledge_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/cfg/cfg_manager.py` & `angr-9.2.9/angr/knowledge_plugins/cfg/cfg_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/cfg/cfg_model.py` & `angr-9.2.9/angr/knowledge_plugins/cfg/cfg_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,21 @@
             pos = bisect.bisect_left(self._node_addrs, node.addr)
             if pos >= len(self._node_addrs):
                 self._node_addrs.append(node.addr)
             elif self._node_addrs[pos] != node.addr:
                 self._node_addrs.insert(pos, node.addr)
 
     def remove_node(self, block_id: int, node: CFGNode) -> None:
+        """
+        Remove the given CFGNode instance. Note that this method *does not* remove the node from the graph.
+
+        :param block_id:    The Unique ID of the CFGNode.
+        :param node:        The CFGNode instance to remove.
+        :return:            None
+        """
         if block_id in self._nodes:
             del self._nodes[block_id]
 
         if node.addr in self._nodes_by_addr and node in self._nodes_by_addr[node.addr]:
             self._nodes_by_addr[node.addr].remove(node)
             if not self._nodes_by_addr[node.addr]:
                 del self._nodes_by_addr[node.addr]
```

### Comparing `angr-9.2.8/angr/knowledge_plugins/cfg/cfg_node.py` & `angr-9.2.9/angr/knowledge_plugins/cfg/cfg_node.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/cfg/indirect_jump.py` & `angr-9.2.9/angr/knowledge_plugins/cfg/indirect_jump.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/cfg/memory_data.py` & `angr-9.2.9/angr/knowledge_plugins/cfg/memory_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,14 +81,18 @@
         :return:        None
         """
 
         if self.sort == MemoryDataSort.String:
             self.content = loader.memory.load(self.addr, self.size)
             if self.content.endswith(b"\x00"):
                 self.content = self.content.strip(b"\x00")
+        elif self.sort == MemoryDataSort.UnicodeString:
+            self.content = loader.memory.load(self.addr, self.size)
+            while self.content.endswith(b"\x00\x00"):
+                self.content = self.content[:-2]
         else:
             # FIXME: Other types are not supported yet
             return
 
     #
     # Serialization
     #
```

### Comparing `angr-9.2.8/angr/knowledge_plugins/functions/function.py` & `angr-9.2.9/angr/knowledge_plugins/functions/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self.alignment = alignment
 
         # These properties are set by VariableManager
         self.bp_on_stack = False
         self.retaddr_on_stack = False
         self.sp_delta = 0
         # Calling convention
-        self.calling_convention = None  # type: Optional[SimCC]
+        self.calling_convention: Optional[SimCC] = None
         # Function prototype
         self.prototype = None  # type: Optional[SimTypeFunction]
         self.is_prototype_guessed: bool = True
         # Whether this function returns or not. `None` means it's not determined yet
         self._returning = None
         self.prepared_registers = set()
         self.prepared_stack_variables = set()
```

### Comparing `angr-9.2.8/angr/knowledge_plugins/functions/function_manager.py` & `angr-9.2.9/angr/knowledge_plugins/functions/function_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/functions/function_parser.py` & `angr-9.2.9/angr/knowledge_plugins/functions/function_parser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/functions/soot_function.py` & `angr-9.2.9/angr/knowledge_plugins/functions/soot_function.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/indirect_jumps.py` & `angr-9.2.9/angr/knowledge_plugins/indirect_jumps.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/atoms.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/atoms.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/definition.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/definition.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/environment.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/environment.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/heap_address.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/heap_address.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/key_definition_manager.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/key_definition_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/live_definitions.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/live_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import weakref
 from typing import Optional, Iterable, Dict, Set, Generator, Tuple, Union, Any, TYPE_CHECKING
 import logging
 
+from collections import defaultdict
+
 import claripy
 from claripy.annotation import Annotation
 import archinfo
 
-from collections import defaultdict
-
 from ...errors import SimMemoryMissingError, SimMemoryError
 from ...storage.memory_mixins import MultiValuedMemory
 from ...storage.memory_mixins.paged_memory.pages.multi_values import MultiValues
 from ...engines.light import SpOffset
 from ...code_location import CodeLocation
 from .atoms import Atom, Register, MemoryLocation, Tmp, FunctionCall, ConstantSrc
 from .definition import Definition, Tag
@@ -210,25 +210,35 @@
         return base
 
     @staticmethod
     def is_stack_address(addr: claripy.ast.Base) -> bool:
         return "stack_base" in addr.variables
 
     @staticmethod
-    def get_stack_offset(addr: claripy.ast.Base) -> Optional[int]:
+    def get_stack_offset(addr: claripy.ast.Base, had_stack_base=False) -> Optional[int]:
+        if had_stack_base and addr.op == "BVV":
+            return addr._model_concrete.value
+        if "TOP" in addr.variables:
+            return None
         if "stack_base" in addr.variables:
             if addr.op == "BVS":
                 return 0
             elif addr.op == "__add__":
-                if len(addr.args) == 2 and addr.args[1].op == "BVV":
-                    return addr.args[1]._model_concrete.value
-                if len(addr.args) == 1:
+                if len(addr.args) == 2:
+                    off0 = LiveDefinitions.get_stack_offset(addr.args[0], had_stack_base=True)
+                    off1 = LiveDefinitions.get_stack_offset(addr.args[1], had_stack_base=True)
+                    if off0 is not None and off1 is not None:
+                        return off0 + off1
+                elif len(addr.args) == 1:
                     return 0
-            elif addr.op == "__sub__" and len(addr.args) == 2 and addr.args[1].op == "BVV":
-                return -addr.args[1]._model_concrete.value
+            elif addr.op == "__sub__" and len(addr.args) == 2:
+                off0 = LiveDefinitions.get_stack_offset(addr.args[0], had_stack_base=True)
+                off1 = LiveDefinitions.get_stack_offset(addr.args[1], had_stack_base=True)
+                if off0 is not None and off1 is not None:
+                    return off0 - off1
         return None
 
     @staticmethod
     def annotate_with_def(symvar: claripy.ast.Base, definition: Definition):
         """
 
         :param symvar:
```

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/rd_model.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/rd_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/tag.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/tag.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/undefined.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/undefined.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/unknown_size.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/unknown_size.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/key_definitions/uses.py` & `angr-9.2.9/angr/knowledge_plugins/key_definitions/uses.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/labels.py` & `angr-9.2.9/angr/knowledge_plugins/labels.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/patches.py` & `angr-9.2.9/angr/knowledge_plugins/patches.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/propagations.py` & `angr-9.2.9/angr/knowledge_plugins/propagations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/structured_code/manager.py` & `angr-9.2.9/angr/knowledge_plugins/structured_code/manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/sync/sync_controller.py` & `angr-9.2.9/angr/knowledge_plugins/sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/types.py` & `angr-9.2.9/angr/knowledge_plugins/types.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/variables/variable_access.py` & `angr-9.2.9/angr/knowledge_plugins/variables/variable_access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/variables/variable_manager.py` & `angr-9.2.9/angr/knowledge_plugins/variables/variable_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/xrefs/xref.py` & `angr-9.2.9/angr/knowledge_plugins/xrefs/xref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/knowledge_plugins/xrefs/xref_manager.py` & `angr-9.2.9/angr/knowledge_plugins/xrefs/xref_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/autoimport.py` & `angr-9.2.9/angr/misc/autoimport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/bug_report.py` & `angr-9.2.9/angr/misc/bug_report.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/hookset.py` & `angr-9.2.9/angr/misc/hookset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/import_hooks.py` & `angr-9.2.9/angr/misc/import_hooks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/loggers.py` & `angr-9.2.9/angr/misc/loggers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/picklable_lock.py` & `angr-9.2.9/angr/misc/picklable_lock.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/plugins.py` & `angr-9.2.9/angr/misc/plugins.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/range.py` & `angr-9.2.9/angr/misc/range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/ux.py` & `angr-9.2.9/angr/misc/ux.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/misc/weakpatch.py` & `angr-9.2.9/angr/misc/weakpatch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/cgc/allocate.py` & `angr-9.2.9/angr/procedures/cgc/allocate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/cgc/deallocate.py` & `angr-9.2.9/angr/procedures/cgc/deallocate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/cgc/fdwait.py` & `angr-9.2.9/angr/procedures/cgc/fdwait.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/cgc/random.py` & `angr-9.2.9/angr/procedures/cgc/random.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/cgc/receive.py` & `angr-9.2.9/angr/procedures/cgc/receive.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/cgc/transmit.py` & `angr-9.2.9/angr/procedures/cgc/transmit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/__init__.py` & `angr-9.2.9/angr/procedures/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/glibc.py` & `angr-9.2.9/angr/procedures/definitions/glibc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2751,16 +2751,16 @@
         "vfork": SimTypeFunction([], SimTypeInt(signed=True, label="pid_t")),
         # int execv (const char *FILENAME, char *const ARGV[]);
         "execv": SimTypeFunction([SimTypePointer(SimTypeChar(), offset=0), SimTypeFixedSizeArray(SimTypePointer(SimTypeChar(), offset=0), 0)], SimTypeInt(signed=True), arg_names=["filename", "argv"]),
         # int execl (const char *FILENAME, const char *ARG0, ...);
         "execl": SimTypeFunction([SimTypePointer(SimTypeChar(), offset=0), SimTypePointer(SimTypeChar(), offset=0)], SimTypeInt(signed=True), arg_names=["filename", "arg0"], variadic=True),
         # int execve (const char *FILENAME, char *const ARGV[], char *const ENV[]);
         "execve": SimTypeFunction([SimTypePointer(SimTypeChar(), offset=0), SimTypeFixedSizeArray(SimTypePointer(SimTypeChar(), offset=0), 0), SimTypeFixedSizeArray(SimTypePointer(SimTypeChar(), offset=0), 0)], SimTypeInt(signed=True), arg_names=["filename", "argv", "env"]),
-        # int execle (const char *FILENAME, const char *ARG0, ..., char *const ENV[]);
-        "execle": None,
+        # int execle (const char *FILENAME, const char *ARG0, ...);
+        "execle": SimTypeFunction([SimTypePointer(SimTypeChar(), offset=0), SimTypeFixedSizeArray(SimTypePointer(SimTypeChar(), offset=0), 0)], SimTypeInt(signed=True), arg_names=["filename", "argv"]),
         # int execvp (const char *FILENAME, char *const ARGV[]);
         "execvp": SimTypeFunction([SimTypePointer(SimTypeChar(), offset=0), SimTypeFixedSizeArray(SimTypePointer(SimTypeChar(), offset=0), 0)], SimTypeInt(signed=True), arg_names=["filename", "argv"]),
         # int execvpe (const char *FILENAME, char *const ARGV[], char *const ENV[]);,
         "execvpe": SimTypeFunction([SimTypePointer(SimTypeChar(), offset=0), SimTypeFixedSizeArray(SimTypePointer(SimTypeChar(), offset=0), 0), SimTypeFixedSizeArray(SimTypePointer(SimTypeChar(), offset=0), 0)], SimTypeInt(signed=True), arg_names=["filename", "argv", "env"]),
         # int execlp (const char *FILENAME, const char *ARG0, ...);
         "execlp": SimTypeFunction([SimTypePointer(SimTypeChar(), offset=0), SimTypePointer(SimTypeChar(), offset=0)], SimTypeInt(signed=True), arg_names=["filename", "arg0"], variadic=True),
         # pid_t waitpid (pid_t PID, int *STATUS_PTR, int OPTIONS);
```

### Comparing `angr-9.2.8/angr/procedures/definitions/libstdcpp.py` & `angr-9.2.9/angr/procedures/definitions/libstdcpp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/linux_kernel.py` & `angr-9.2.9/angr/procedures/definitions/linux_kernel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/msvcr.py` & `angr-9.2.9/angr/procedures/definitions/msvcr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/parse_syscalls_from_local_system.py` & `angr-9.2.9/angr/procedures/definitions/parse_syscalls_from_local_system.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/parse_win32json.py` & `angr-9.2.9/angr/procedures/definitions/parse_win32json.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_aclui.py` & `angr-9.2.9/angr/procedures/definitions/win32_aclui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_activeds.py` & `angr-9.2.9/angr/procedures/definitions/win32_activeds.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_advapi32.py` & `angr-9.2.9/angr/procedures/definitions/win32_advapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_advpack.py` & `angr-9.2.9/angr/procedures/definitions/win32_advpack.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_amsi.py` & `angr-9.2.9/angr/procedures/definitions/win32_amsi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py` & `angr-9.2.9/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_apphelp.py` & `angr-9.2.9/angr/procedures/definitions/win32_apphelp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_authz.py` & `angr-9.2.9/angr/procedures/definitions/win32_authz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_avicap32.py` & `angr-9.2.9/angr/procedures/definitions/win32_avicap32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_avifil32.py` & `angr-9.2.9/angr/procedures/definitions/win32_avifil32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_bcrypt.py` & `angr-9.2.9/angr/procedures/definitions/win32_bcrypt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_bluetoothapis.py` & `angr-9.2.9/angr/procedures/definitions/win32_bluetoothapis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_bthprops.py` & `angr-9.2.9/angr/procedures/definitions/win32_bthprops.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_cabinet.py` & `angr-9.2.9/angr/procedures/definitions/win32_cabinet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_certadm.py` & `angr-9.2.9/angr/procedures/definitions/win32_certadm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_certpoleng.py` & `angr-9.2.9/angr/procedures/definitions/win32_certpoleng.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_cfgmgr32.py` & `angr-9.2.9/angr/procedures/definitions/win32_cfgmgr32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_chakra.py` & `angr-9.2.9/angr/procedures/definitions/win32_chakra.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_cldapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_cldapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_clfsw32.py` & `angr-9.2.9/angr/procedures/definitions/win32_clfsw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_clusapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_clusapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_comctl32.py` & `angr-9.2.9/angr/procedures/definitions/win32_comctl32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_comdlg32.py` & `angr-9.2.9/angr/procedures/definitions/win32_comdlg32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_compstui.py` & `angr-9.2.9/angr/procedures/definitions/win32_compstui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_comsvcs.py` & `angr-9.2.9/angr/procedures/definitions/win32_comsvcs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_coremessaging.py` & `angr-9.2.9/angr/procedures/definitions/win32_coremessaging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_credui.py` & `angr-9.2.9/angr/procedures/definitions/win32_credui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_crypt32.py` & `angr-9.2.9/angr/procedures/definitions/win32_crypt32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_cryptnet.py` & `angr-9.2.9/angr/procedures/definitions/win32_cryptnet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_cryptui.py` & `angr-9.2.9/angr/procedures/definitions/win32_cryptui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_cryptxml.py` & `angr-9.2.9/angr/procedures/definitions/win32_cryptxml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_cscapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_cscapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d2d1.py` & `angr-9.2.9/angr/procedures/definitions/win32_d2d1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d3d10.py` & `angr-9.2.9/angr/procedures/definitions/win32_d3d10.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d3d10_1.py` & `angr-9.2.9/angr/procedures/definitions/win32_d3d10_1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d3d11.py` & `angr-9.2.9/angr/procedures/definitions/win32_d3d11.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d3d12.py` & `angr-9.2.9/angr/procedures/definitions/win32_d3d12.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d3d9.py` & `angr-9.2.9/angr/procedures/definitions/win32_d3d9.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d3dcompiler_47.py` & `angr-9.2.9/angr/procedures/definitions/win32_d3dcompiler_47.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_d3dcsx.py` & `angr-9.2.9/angr/procedures/definitions/win32_d3dcsx.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_davclnt.py` & `angr-9.2.9/angr/procedures/definitions/win32_davclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dbgeng.py` & `angr-9.2.9/angr/procedures/definitions/win32_dbgeng.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dbghelp.py` & `angr-9.2.9/angr/procedures/definitions/win32_dbghelp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dbgmodel.py` & `angr-9.2.9/angr/procedures/definitions/win32_dbgmodel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dciman32.py` & `angr-9.2.9/angr/procedures/definitions/win32_dciman32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dcomp.py` & `angr-9.2.9/angr/procedures/definitions/win32_dcomp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ddraw.py` & `angr-9.2.9/angr/procedures/definitions/win32_ddraw.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_deviceaccess.py` & `angr-9.2.9/angr/procedures/definitions/win32_deviceaccess.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dflayout.py` & `angr-9.2.9/angr/procedures/definitions/win32_dflayout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dhcpcsvc.py` & `angr-9.2.9/angr/procedures/definitions/win32_dhcpcsvc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dhcpcsvc6.py` & `angr-9.2.9/angr/procedures/definitions/win32_dhcpcsvc6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dhcpsapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_dhcpsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_diagnosticdataquery.py` & `angr-9.2.9/angr/procedures/definitions/win32_diagnosticdataquery.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dinput8.py` & `angr-9.2.9/angr/procedures/definitions/win32_dinput8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_directml.py` & `angr-9.2.9/angr/procedures/definitions/win32_directml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dnsapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_dnsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_drt.py` & `angr-9.2.9/angr/procedures/definitions/win32_drt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_drtprov.py` & `angr-9.2.9/angr/procedures/definitions/win32_drtprov.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_drttransport.py` & `angr-9.2.9/angr/procedures/definitions/win32_drttransport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dsound.py` & `angr-9.2.9/angr/procedures/definitions/win32_dsound.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dsparse.py` & `angr-9.2.9/angr/procedures/definitions/win32_dsparse.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dsprop.py` & `angr-9.2.9/angr/procedures/definitions/win32_dsprop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dssec.py` & `angr-9.2.9/angr/procedures/definitions/win32_dssec.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dsuiext.py` & `angr-9.2.9/angr/procedures/definitions/win32_dsuiext.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dwmapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_dwmapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dwrite.py` & `angr-9.2.9/angr/procedures/definitions/win32_dwrite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dxcompiler.py` & `angr-9.2.9/angr/procedures/definitions/win32_dxcompiler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dxgi.py` & `angr-9.2.9/angr/procedures/definitions/win32_dxgi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_dxva2.py` & `angr-9.2.9/angr/procedures/definitions/win32_dxva2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_eappcfg.py` & `angr-9.2.9/angr/procedures/definitions/win32_eappcfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_eappprxy.py` & `angr-9.2.9/angr/procedures/definitions/win32_eappprxy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_efswrt.py` & `angr-9.2.9/angr/procedures/definitions/win32_efswrt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_elscore.py` & `angr-9.2.9/angr/procedures/definitions/win32_elscore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_esent.py` & `angr-9.2.9/angr/procedures/definitions/win32_esent.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_evr.py` & `angr-9.2.9/angr/procedures/definitions/win32_evr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_faultrep.py` & `angr-9.2.9/angr/procedures/definitions/win32_faultrep.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_fhsvcctl.py` & `angr-9.2.9/angr/procedures/definitions/win32_fhsvcctl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_fltlib.py` & `angr-9.2.9/angr/procedures/definitions/win32_fltlib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_fontsub.py` & `angr-9.2.9/angr/procedures/definitions/win32_fontsub.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_fwpuclnt.py` & `angr-9.2.9/angr/procedures/definitions/win32_fwpuclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_fxsutility.py` & `angr-9.2.9/angr/procedures/definitions/win32_fxsutility.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_gdi32.py` & `angr-9.2.9/angr/procedures/definitions/win32_gdi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_gpedit.py` & `angr-9.2.9/angr/procedures/definitions/win32_gpedit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_hid.py` & `angr-9.2.9/angr/procedures/definitions/win32_hid.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_hlink.py` & `angr-9.2.9/angr/procedures/definitions/win32_hlink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_hrtfapo.py` & `angr-9.2.9/angr/procedures/definitions/win32_hrtfapo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_httpapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_httpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_icm32.py` & `angr-9.2.9/angr/procedures/definitions/win32_icm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_icmui.py` & `angr-9.2.9/angr/procedures/definitions/win32_icmui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_icu.py` & `angr-9.2.9/angr/procedures/definitions/win32_icu.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_imm32.py` & `angr-9.2.9/angr/procedures/definitions/win32_imm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_inkobjcore.py` & `angr-9.2.9/angr/procedures/definitions/win32_inkobjcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_iphlpapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_iphlpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_iscsidsc.py` & `angr-9.2.9/angr/procedures/definitions/win32_iscsidsc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_kernel32.py` & `angr-9.2.9/angr/procedures/definitions/win32_kernel32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_keycredmgr.py` & `angr-9.2.9/angr/procedures/definitions/win32_keycredmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ksuser.py` & `angr-9.2.9/angr/procedures/definitions/win32_ksuser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ktmw32.py` & `angr-9.2.9/angr/procedures/definitions/win32_ktmw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_loadperf.py` & `angr-9.2.9/angr/procedures/definitions/win32_loadperf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_magnification.py` & `angr-9.2.9/angr/procedures/definitions/win32_magnification.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mapi32.py` & `angr-9.2.9/angr/procedures/definitions/win32_mapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mdmregistration.py` & `angr-9.2.9/angr/procedures/definitions/win32_mdmregistration.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mf.py` & `angr-9.2.9/angr/procedures/definitions/win32_mf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mfcore.py` & `angr-9.2.9/angr/procedures/definitions/win32_mfcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mfplat.py` & `angr-9.2.9/angr/procedures/definitions/win32_mfplat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mfplay.py` & `angr-9.2.9/angr/procedures/definitions/win32_mfplay.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mfreadwrite.py` & `angr-9.2.9/angr/procedures/definitions/win32_mfreadwrite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mfsensorgroup.py` & `angr-9.2.9/angr/procedures/definitions/win32_mfsensorgroup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mfsrcsnk.py` & `angr-9.2.9/angr/procedures/definitions/win32_mfsrcsnk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mgmtapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_mgmtapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mi.py` & `angr-9.2.9/angr/procedures/definitions/win32_mi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mmdevapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_mmdevapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mpr.py` & `angr-9.2.9/angr/procedures/definitions/win32_mpr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mprapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_mprapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mrmsupport.py` & `angr-9.2.9/angr/procedures/definitions/win32_mrmsupport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msacm32.py` & `angr-9.2.9/angr/procedures/definitions/win32_msacm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msajapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_msajapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mscms.py` & `angr-9.2.9/angr/procedures/definitions/win32_mscms.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msctfmonitor.py` & `angr-9.2.9/angr/procedures/definitions/win32_msctfmonitor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msdmo.py` & `angr-9.2.9/angr/procedures/definitions/win32_msdmo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msdrm.py` & `angr-9.2.9/angr/procedures/definitions/win32_msdrm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msi.py` & `angr-9.2.9/angr/procedures/definitions/win32_msi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msimg32.py` & `angr-9.2.9/angr/procedures/definitions/win32_msimg32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msports.py` & `angr-9.2.9/angr/procedures/definitions/win32_msports.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mstask.py` & `angr-9.2.9/angr/procedures/definitions/win32_mstask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_msvfw32.py` & `angr-9.2.9/angr/procedures/definitions/win32_msvfw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mswsock.py` & `angr-9.2.9/angr/procedures/definitions/win32_mswsock.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_mtxdm.py` & `angr-9.2.9/angr/procedures/definitions/win32_mtxdm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ncrypt.py` & `angr-9.2.9/angr/procedures/definitions/win32_ncrypt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ndfapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_ndfapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_netapi32.py` & `angr-9.2.9/angr/procedures/definitions/win32_netapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_netsh.py` & `angr-9.2.9/angr/procedures/definitions/win32_netsh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_newdev.py` & `angr-9.2.9/angr/procedures/definitions/win32_newdev.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ninput.py` & `angr-9.2.9/angr/procedures/definitions/win32_ninput.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_normaliz.py` & `angr-9.2.9/angr/procedures/definitions/win32_normaliz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ntdll.py` & `angr-9.2.9/angr/procedures/definitions/win32_ntdll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ntdsapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_ntdsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ntlanman.py` & `angr-9.2.9/angr/procedures/definitions/win32_ntlanman.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ole32.py` & `angr-9.2.9/angr/procedures/definitions/win32_ole32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_oleacc.py` & `angr-9.2.9/angr/procedures/definitions/win32_oleacc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_oleaut32.py` & `angr-9.2.9/angr/procedures/definitions/win32_oleaut32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_oledlg.py` & `angr-9.2.9/angr/procedures/definitions/win32_oledlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ondemandconnroutehelper.py` & `angr-9.2.9/angr/procedures/definitions/win32_ondemandconnroutehelper.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_opengl32.py` & `angr-9.2.9/angr/procedures/definitions/win32_opengl32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_p2p.py` & `angr-9.2.9/angr/procedures/definitions/win32_p2p.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_p2pgraph.py` & `angr-9.2.9/angr/procedures/definitions/win32_p2pgraph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_pdh.py` & `angr-9.2.9/angr/procedures/definitions/win32_pdh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_peerdist.py` & `angr-9.2.9/angr/procedures/definitions/win32_peerdist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_powrprof.py` & `angr-9.2.9/angr/procedures/definitions/win32_powrprof.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_prntvpt.py` & `angr-9.2.9/angr/procedures/definitions/win32_prntvpt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_projectedfslib.py` & `angr-9.2.9/angr/procedures/definitions/win32_projectedfslib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_propsys.py` & `angr-9.2.9/angr/procedures/definitions/win32_propsys.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_quartz.py` & `angr-9.2.9/angr/procedures/definitions/win32_quartz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_query.py` & `angr-9.2.9/angr/procedures/definitions/win32_query.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_qwave.py` & `angr-9.2.9/angr/procedures/definitions/win32_qwave.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_rasapi32.py` & `angr-9.2.9/angr/procedures/definitions/win32_rasapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_rasdlg.py` & `angr-9.2.9/angr/procedures/definitions/win32_rasdlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_resutils.py` & `angr-9.2.9/angr/procedures/definitions/win32_resutils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_rometadata.py` & `angr-9.2.9/angr/procedures/definitions/win32_rometadata.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_rpcns4.py` & `angr-9.2.9/angr/procedures/definitions/win32_rpcns4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_rpcrt4.py` & `angr-9.2.9/angr/procedures/definitions/win32_rpcrt4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_rstrtmgr.py` & `angr-9.2.9/angr/procedures/definitions/win32_rstrtmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_rtm.py` & `angr-9.2.9/angr/procedures/definitions/win32_rtm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_scarddlg.py` & `angr-9.2.9/angr/procedures/definitions/win32_scarddlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_schannel.py` & `angr-9.2.9/angr/procedures/definitions/win32_schannel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_secur32.py` & `angr-9.2.9/angr/procedures/definitions/win32_secur32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_sensapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_sensapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_setupapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_setupapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_sfc.py` & `angr-9.2.9/angr/procedures/definitions/win32_sfc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_shdocvw.py` & `angr-9.2.9/angr/procedures/definitions/win32_shdocvw.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_shell32.py` & `angr-9.2.9/angr/procedures/definitions/win32_shell32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_shlwapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_shlwapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_slc.py` & `angr-9.2.9/angr/procedures/definitions/win32_slc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_slcext.py` & `angr-9.2.9/angr/procedures/definitions/win32_slcext.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_slwga.py` & `angr-9.2.9/angr/procedures/definitions/win32_slwga.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_snmpapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_snmpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_spoolss.py` & `angr-9.2.9/angr/procedures/definitions/win32_spoolss.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_srpapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_srpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_sspicli.py` & `angr-9.2.9/angr/procedures/definitions/win32_sspicli.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_t2embed.py` & `angr-9.2.9/angr/procedures/definitions/win32_t2embed.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_tapi32.py` & `angr-9.2.9/angr/procedures/definitions/win32_tapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_tbs.py` & `angr-9.2.9/angr/procedures/definitions/win32_tbs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_tdh.py` & `angr-9.2.9/angr/procedures/definitions/win32_tdh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_tokenbinding.py` & `angr-9.2.9/angr/procedures/definitions/win32_tokenbinding.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_traffic.py` & `angr-9.2.9/angr/procedures/definitions/win32_traffic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_txfw32.py` & `angr-9.2.9/angr/procedures/definitions/win32_txfw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ualapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_ualapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_uiautomationcore.py` & `angr-9.2.9/angr/procedures/definitions/win32_uiautomationcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_urlmon.py` & `angr-9.2.9/angr/procedures/definitions/win32_urlmon.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_user32.py` & `angr-9.2.9/angr/procedures/definitions/win32_user32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_userenv.py` & `angr-9.2.9/angr/procedures/definitions/win32_userenv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_usp10.py` & `angr-9.2.9/angr/procedures/definitions/win32_usp10.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_uxtheme.py` & `angr-9.2.9/angr/procedures/definitions/win32_uxtheme.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_verifier.py` & `angr-9.2.9/angr/procedures/definitions/win32_verifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_version.py` & `angr-9.2.9/angr/procedures/definitions/win32_version.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_vertdll.py` & `angr-9.2.9/angr/procedures/definitions/win32_vertdll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_virtdisk.py` & `angr-9.2.9/angr/procedures/definitions/win32_virtdisk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_vssapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_vssapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wcmapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wcmapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wdsbp.py` & `angr-9.2.9/angr/procedures/definitions/win32_wdsbp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wdsclientapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wdsclientapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wdsmc.py` & `angr-9.2.9/angr/procedures/definitions/win32_wdsmc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wdspxe.py` & `angr-9.2.9/angr/procedures/definitions/win32_wdspxe.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wdstptc.py` & `angr-9.2.9/angr/procedures/definitions/win32_wdstptc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_webauthn.py` & `angr-9.2.9/angr/procedures/definitions/win32_webauthn.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_webservices.py` & `angr-9.2.9/angr/procedures/definitions/win32_webservices.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_websocket.py` & `angr-9.2.9/angr/procedures/definitions/win32_websocket.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wecapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wecapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wer.py` & `angr-9.2.9/angr/procedures/definitions/win32_wer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wevtapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wevtapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winbio.py` & `angr-9.2.9/angr/procedures/definitions/win32_winbio.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_windows_ai_machinelearning.py` & `angr-9.2.9/angr/procedures/definitions/win32_windows_ai_machinelearning.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_windows_data_pdf.py` & `angr-9.2.9/angr/procedures/definitions/win32_windows_data_pdf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_windows_networking.py` & `angr-9.2.9/angr/procedures/definitions/win32_windows_networking.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_windows_ui_xaml.py` & `angr-9.2.9/angr/procedures/definitions/win32_windows_ui_xaml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_windowscodecs.py` & `angr-9.2.9/angr/procedures/definitions/win32_windowscodecs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winfax.py` & `angr-9.2.9/angr/procedures/definitions/win32_winfax.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winhttp.py` & `angr-9.2.9/angr/procedures/definitions/win32_winhttp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winhvemulation.py` & `angr-9.2.9/angr/procedures/definitions/win32_winhvemulation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winhvplatform.py` & `angr-9.2.9/angr/procedures/definitions/win32_winhvplatform.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wininet.py` & `angr-9.2.9/angr/procedures/definitions/win32_wininet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winml.py` & `angr-9.2.9/angr/procedures/definitions/win32_winml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winmm.py` & `angr-9.2.9/angr/procedures/definitions/win32_winmm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winscard.py` & `angr-9.2.9/angr/procedures/definitions/win32_winscard.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winspool.py` & `angr-9.2.9/angr/procedures/definitions/win32_winspool.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wintrust.py` & `angr-9.2.9/angr/procedures/definitions/win32_wintrust.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_winusb.py` & `angr-9.2.9/angr/procedures/definitions/win32_winusb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wlanapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wlanapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wlanui.py` & `angr-9.2.9/angr/procedures/definitions/win32_wlanui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wldap32.py` & `angr-9.2.9/angr/procedures/definitions/win32_wldap32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wldp.py` & `angr-9.2.9/angr/procedures/definitions/win32_wldp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wmvcore.py` & `angr-9.2.9/angr/procedures/definitions/win32_wmvcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wnvapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wnvapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wofutil.py` & `angr-9.2.9/angr/procedures/definitions/win32_wofutil.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_ws2_32.py` & `angr-9.2.9/angr/procedures/definitions/win32_ws2_32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wscapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wscapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wsclient.py` & `angr-9.2.9/angr/procedures/definitions/win32_wsclient.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wsdapi.py` & `angr-9.2.9/angr/procedures/definitions/win32_wsdapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wsmsvc.py` & `angr-9.2.9/angr/procedures/definitions/win32_wsmsvc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wsnmp32.py` & `angr-9.2.9/angr/procedures/definitions/win32_wsnmp32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_wtsapi32.py` & `angr-9.2.9/angr/procedures/definitions/win32_wtsapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_xaudio2_8.py` & `angr-9.2.9/angr/procedures/definitions/win32_xaudio2_8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_xinputuap.py` & `angr-9.2.9/angr/procedures/definitions/win32_xinputuap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_xmllite.py` & `angr-9.2.9/angr/procedures/definitions/win32_xmllite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/definitions/win32_xpsprint.py` & `angr-9.2.9/angr/procedures/definitions/win32_xpsprint.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/glibc/__ctype_b_loc.py` & `angr-9.2.9/angr/procedures/glibc/__ctype_b_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/glibc/__ctype_tolower_loc.py` & `angr-9.2.9/angr/procedures/glibc/__ctype_tolower_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/glibc/__ctype_toupper_loc.py` & `angr-9.2.9/angr/procedures/glibc/__ctype_toupper_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/glibc/__libc_init.py` & `angr-9.2.9/angr/procedures/glibc/__libc_init.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/glibc/__libc_start_main.py` & `angr-9.2.9/angr/procedures/glibc/__libc_start_main.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/glibc/dynamic_loading.py` & `angr-9.2.9/angr/procedures/glibc/dynamic_loading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java/__init__.py` & `angr-9.2.9/angr/procedures/java/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java/unconstrained.py` & `angr-9.2.9/angr/procedures/java/unconstrained.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_io/write.py` & `angr-9.2.9/angr/procedures/java_io/write.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/__init__.py` & `angr-9.2.9/angr/procedures/java_jni/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/array_operations.py` & `angr-9.2.9/angr/procedures/java_jni/array_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/class_and_interface_operations.py` & `angr-9.2.9/angr/procedures/java_jni/class_and_interface_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/field_access.py` & `angr-9.2.9/angr/procedures/java_jni/field_access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/global_and_local_refs.py` & `angr-9.2.9/angr/procedures/java_jni/global_and_local_refs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/method_calls.py` & `angr-9.2.9/angr/procedures/java_jni/method_calls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/not_implemented.py` & `angr-9.2.9/angr/procedures/java_jni/not_implemented.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/object_operations.py` & `angr-9.2.9/angr/procedures/java_jni/object_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_jni/string_operations.py` & `angr-9.2.9/angr/procedures/java_jni/string_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_lang/character.py` & `angr-9.2.9/angr/procedures/java_lang/character.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_lang/double.py` & `angr-9.2.9/angr/procedures/java_lang/double.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_lang/getsimplename.py` & `angr-9.2.9/angr/procedures/java_lang/getsimplename.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_lang/integer.py` & `angr-9.2.9/angr/procedures/java_lang/integer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_lang/string.py` & `angr-9.2.9/angr/procedures/java_lang/string.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_lang/stringbuilder.py` & `angr-9.2.9/angr/procedures/java_lang/stringbuilder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_util/collection.py` & `angr-9.2.9/angr/procedures/java_util/collection.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_util/iterator.py` & `angr-9.2.9/angr/procedures/java_util/iterator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_util/list.py` & `angr-9.2.9/angr/procedures/java_util/list.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_util/map.py` & `angr-9.2.9/angr/procedures/java_util/map.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/java_util/scanner_nextline.py` & `angr-9.2.9/angr/procedures/java_util/scanner_nextline.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/error.py` & `angr-9.2.9/angr/procedures/libc/error.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fclose.py` & `angr-9.2.9/angr/procedures/libc/fclose.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/feof.py` & `angr-9.2.9/angr/procedures/libc/feof.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fgetc.py` & `angr-9.2.9/angr/procedures/libc/fgetc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fgets.py` & `angr-9.2.9/angr/procedures/libc/fgets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fopen.py` & `angr-9.2.9/angr/procedures/libc/fopen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fprintf.py` & `angr-9.2.9/angr/procedures/libc/fprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fputc.py` & `angr-9.2.9/angr/procedures/libc/fputc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fputs.py` & `angr-9.2.9/angr/procedures/libc/fputs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fread.py` & `angr-9.2.9/angr/procedures/libc/fread.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fscanf.py` & `angr-9.2.9/angr/procedures/libc/fscanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fseek.py` & `angr-9.2.9/angr/procedures/libc/fseek.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/ftell.py` & `angr-9.2.9/angr/procedures/libc/ftell.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/fwrite.py` & `angr-9.2.9/angr/procedures/libc/fwrite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/getdelim.py` & `angr-9.2.9/angr/procedures/libc/getdelim.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/gets.py` & `angr-9.2.9/angr/procedures/libc/gets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/memcmp.py` & `angr-9.2.9/angr/procedures/libc/memcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/memcpy.py` & `angr-9.2.9/angr/procedures/libc/memcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/memset.py` & `angr-9.2.9/angr/procedures/libc/memset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/printf.py` & `angr-9.2.9/angr/procedures/libc/printf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/puts.py` & `angr-9.2.9/angr/procedures/libc/puts.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/snprintf.py` & `angr-9.2.9/angr/procedures/libc/snprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/sprintf.py` & `angr-9.2.9/angr/procedures/libc/sprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strchr.py` & `angr-9.2.9/angr/procedures/libc/strchr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strcmp.py` & `angr-9.2.9/angr/procedures/libc/strcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strlen.py` & `angr-9.2.9/angr/procedures/libc/strlen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strncat.py` & `angr-9.2.9/angr/procedures/libc/strncat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strncmp.py` & `angr-9.2.9/angr/procedures/libc/strncmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strncpy.py` & `angr-9.2.9/angr/procedures/libc/strncpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strstr.py` & `angr-9.2.9/angr/procedures/libc/strstr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/strtol.py` & `angr-9.2.9/angr/procedures/libc/strtol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/tmpnam.py` & `angr-9.2.9/angr/procedures/libc/tmpnam.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/ungetc.py` & `angr-9.2.9/angr/procedures/libc/ungetc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/vsnprintf.py` & `angr-9.2.9/angr/procedures/libc/vsnprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/libc/wchar.py` & `angr-9.2.9/angr/procedures/libc/wchar.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/arch_prctl.py` & `angr-9.2.9/angr/procedures/linux_kernel/arch_prctl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/arm_user_helpers.py` & `angr-9.2.9/angr/procedures/linux_kernel/arm_user_helpers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/cwd.py` & `angr-9.2.9/angr/procedures/linux_kernel/cwd.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/fstat.py` & `angr-9.2.9/angr/procedures/linux_kernel/fstat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/fstat64.py` & `angr-9.2.9/angr/procedures/linux_kernel/fstat64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/futex.py` & `angr-9.2.9/angr/procedures/linux_kernel/futex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/getrlimit.py` & `angr-9.2.9/angr/procedures/linux_kernel/getrlimit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/iovec.py` & `angr-9.2.9/angr/procedures/linux_kernel/iovec.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/lseek.py` & `angr-9.2.9/angr/procedures/linux_kernel/lseek.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/mprotect.py` & `angr-9.2.9/angr/procedures/linux_kernel/mprotect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/openat.py` & `angr-9.2.9/angr/procedures/linux_kernel/openat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/sigaction.py` & `angr-9.2.9/angr/procedures/linux_kernel/sigaction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/sigprocmask.py` & `angr-9.2.9/angr/procedures/linux_kernel/sigprocmask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/stat.py` & `angr-9.2.9/angr/procedures/linux_kernel/stat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/sysinfo.py` & `angr-9.2.9/angr/procedures/linux_kernel/sysinfo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/time.py` & `angr-9.2.9/angr/procedures/linux_kernel/time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/uid.py` & `angr-9.2.9/angr/procedures/linux_kernel/uid.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/uname.py` & `angr-9.2.9/angr/procedures/linux_kernel/uname.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_kernel/unlink.py` & `angr-9.2.9/angr/procedures/linux_kernel/unlink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_loader/sim_loader.py` & `angr-9.2.9/angr/procedures/linux_loader/sim_loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/linux_loader/tls.py` & `angr-9.2.9/angr/procedures/linux_loader/tls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/msvcr/__getmainargs.py` & `angr-9.2.9/angr/procedures/msvcr/__getmainargs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/msvcr/_initterm.py` & `angr-9.2.9/angr/procedures/msvcr/_initterm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/msvcr/fmode.py` & `angr-9.2.9/angr/procedures/msvcr/fmode.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/ntdll/exceptions.py` & `angr-9.2.9/angr/procedures/ntdll/exceptions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/accept.py` & `angr-9.2.9/angr/procedures/posix/accept.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/dup.py` & `angr-9.2.9/angr/procedures/posix/dup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/fdopen.py` & `angr-9.2.9/angr/procedures/posix/fdopen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/getenv.py` & `angr-9.2.9/angr/procedures/posix/getenv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/gethostbyname.py` & `angr-9.2.9/angr/procedures/posix/gethostbyname.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/getpass.py` & `angr-9.2.9/angr/procedures/posix/getpass.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/inet_ntoa.py` & `angr-9.2.9/angr/procedures/posix/inet_ntoa.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/mmap.py` & `angr-9.2.9/angr/procedures/posix/mmap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/open.py` & `angr-9.2.9/angr/procedures/posix/open.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/poll.py` & `angr-9.2.9/angr/procedures/posix/poll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/pread64.py` & `angr-9.2.9/angr/procedures/posix/pread64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/pthread.py` & `angr-9.2.9/angr/procedures/posix/pthread.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/pwrite64.py` & `angr-9.2.9/angr/procedures/posix/pwrite64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/readdir.py` & `angr-9.2.9/angr/procedures/posix/readdir.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/select.py` & `angr-9.2.9/angr/procedures/posix/select.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/send.py` & `angr-9.2.9/angr/procedures/posix/send.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/sigaction.py` & `angr-9.2.9/angr/procedures/posix/sigaction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/sim_time.py` & `angr-9.2.9/angr/procedures/posix/sim_time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/socket.py` & `angr-9.2.9/angr/procedures/posix/socket.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/strcasecmp.py` & `angr-9.2.9/angr/procedures/posix/strcasecmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/posix/strtok_r.py` & `angr-9.2.9/angr/procedures/posix/strtok_r.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/procedure_dict.py` & `angr-9.2.9/angr/procedures/procedure_dict.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/stubs/Redirect.py` & `angr-9.2.9/angr/procedures/stubs/Redirect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/stubs/ReturnUnconstrained.py` & `angr-9.2.9/angr/procedures/stubs/ReturnUnconstrained.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/stubs/UserHook.py` & `angr-9.2.9/angr/procedures/stubs/UserHook.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/stubs/b64_decode.py` & `angr-9.2.9/angr/procedures/stubs/b64_decode.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/stubs/crazy_scanf.py` & `angr-9.2.9/angr/procedures/stubs/crazy_scanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/stubs/format_parser.py` & `angr-9.2.9/angr/procedures/stubs/format_parser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/stubs/syscall_stub.py` & `angr-9.2.9/angr/procedures/stubs/syscall_stub.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/tracer/random.py` & `angr-9.2.9/angr/procedures/tracer/random.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/tracer/receive.py` & `angr-9.2.9/angr/procedures/tracer/receive.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/tracer/transmit.py` & `angr-9.2.9/angr/procedures/tracer/transmit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/GetLastInputInfo.py` & `angr-9.2.9/angr/procedures/win32/GetLastInputInfo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/GetModuleHandle.py` & `angr-9.2.9/angr/procedures/win32/GetModuleHandle.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/GetProcessAffinityMask.py` & `angr-9.2.9/angr/procedures/win32/GetProcessAffinityMask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/InterlockedExchange.py` & `angr-9.2.9/angr/procedures/win32/InterlockedExchange.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/VirtualAlloc.py` & `angr-9.2.9/angr/procedures/win32/VirtualAlloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/VirtualProtect.py` & `angr-9.2.9/angr/procedures/win32/VirtualProtect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/dynamic_loading.py` & `angr-9.2.9/angr/procedures/win32/dynamic_loading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/file_handles.py` & `angr-9.2.9/angr/procedures/win32/file_handles.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/heap.py` & `angr-9.2.9/angr/procedures/win32/heap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/is_bad_ptr.py` & `angr-9.2.9/angr/procedures/win32/is_bad_ptr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/local_storage.py` & `angr-9.2.9/angr/procedures/win32/local_storage.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/sim_time.py` & `angr-9.2.9/angr/procedures/win32/sim_time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win32/system_paths.py` & `angr-9.2.9/angr/procedures/win32/system_paths.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/procedures/win_user32/messagebox.py` & `angr-9.2.9/angr/procedures/win_user32/messagebox.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/project.py` & `angr-9.2.9/angr/project.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/protos/cfg_pb2.py` & `angr-9.2.9/angr/protos/cfg_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/protos/function_pb2.py` & `angr-9.2.9/angr/protos/function_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/protos/primitives_pb2.py` & `angr-9.2.9/angr/protos/primitives_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/protos/variables_pb2.py` & `angr-9.2.9/angr/protos/variables_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/protos/xrefs_pb2.py` & `angr-9.2.9/angr/protos/xrefs_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/serializable.py` & `angr-9.2.9/angr/serializable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/service.py` & `angr-9.2.9/angr/service.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/sim_manager.py` & `angr-9.2.9/angr/sim_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/sim_options.py` & `angr-9.2.9/angr/sim_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/sim_procedure.py` & `angr-9.2.9/angr/sim_procedure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/sim_state.py` & `angr-9.2.9/angr/sim_state.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/sim_state_options.py` & `angr-9.2.9/angr/sim_state_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/sim_type.py` & `angr-9.2.9/angr/sim_type.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/sim_variable.py` & `angr-9.2.9/angr/sim_variable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/simos/__init__.py` & `angr-9.2.9/angr/simos/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/simos/cgc.py` & `angr-9.2.9/angr/simos/cgc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/simos/javavm.py` & `angr-9.2.9/angr/simos/javavm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/simos/linux.py` & `angr-9.2.9/angr/simos/linux.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/simos/simos.py` & `angr-9.2.9/angr/simos/simos.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/simos/userland.py` & `angr-9.2.9/angr/simos/userland.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/simos/windows.py` & `angr-9.2.9/angr/simos/windows.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/slicer.py` & `angr-9.2.9/angr/slicer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_hierarchy.py` & `angr-9.2.9/angr/state_hierarchy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/__init__.py` & `angr-9.2.9/angr/state_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/callstack.py` & `angr-9.2.9/angr/state_plugins/callstack.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/cgc.py` & `angr-9.2.9/angr/state_plugins/cgc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/concrete.py` & `angr-9.2.9/angr/state_plugins/concrete.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/filesystem.py` & `angr-9.2.9/angr/state_plugins/filesystem.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/gdb.py` & `angr-9.2.9/angr/state_plugins/gdb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/globals.py` & `angr-9.2.9/angr/state_plugins/globals.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/heap/heap_base.py` & `angr-9.2.9/angr/state_plugins/heap/heap_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/heap/heap_brk.py` & `angr-9.2.9/angr/state_plugins/heap/heap_brk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/heap/heap_freelist.py` & `angr-9.2.9/angr/state_plugins/heap/heap_freelist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/heap/heap_libc.py` & `angr-9.2.9/angr/state_plugins/heap/heap_libc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/heap/heap_ptmalloc.py` & `angr-9.2.9/angr/state_plugins/heap/heap_ptmalloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/heap/utils.py` & `angr-9.2.9/angr/state_plugins/heap/utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/history.py` & `angr-9.2.9/angr/state_plugins/history.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/inspect.py` & `angr-9.2.9/angr/state_plugins/inspect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/javavm_classloader.py` & `angr-9.2.9/angr/state_plugins/javavm_classloader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/jni_references.py` & `angr-9.2.9/angr/state_plugins/jni_references.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/libc.py` & `angr-9.2.9/angr/state_plugins/libc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/light_registers.py` & `angr-9.2.9/angr/state_plugins/light_registers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/log.py` & `angr-9.2.9/angr/state_plugins/log.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/loop_data.py` & `angr-9.2.9/angr/state_plugins/loop_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/plugin.py` & `angr-9.2.9/angr/state_plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/posix.py` & `angr-9.2.9/angr/state_plugins/posix.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,25 +457,27 @@
         # if it is mounted, let the filesystem figure out the stat
         if guest_path is not None and mount is not None:
             stat = mount._get_stat(guest_path, dereference=True)
             if stat is None:
                 raise SimPosixError("file %s does not exist on mount %s" % (guest_path, mount))
             size = stat.st_size
             mode = stat.st_mode
+            ino = stat.st_ino
         else:
             # now we know it is not mounted, do the same as before
             if not fd:
                 mode = self.state.solver.BVS('st_mode', 32, key=('api', 'fstat', 'st_mode'))
             else:
                 mode = self.state.solver.BVS('st_mode', 32, key=('api', 'fstat', 'st_mode')) if fd > 2 else self.state.solver.BVV(0, 32)
             size = self.state.solver.BVS('st_size', 64, key=('api', 'fstat', 'st_size')) # st_size
+            ino = 0
 
         # return this weird bogus zero value to keep code paths in libc simple :\
         return Stat(self.state.solver.BVV(0, 64), # st_dev
-                    self.state.solver.BVV(0, 64), # st_ino
+                    self.state.solver.BVV(ino, 64), # st_ino
                     self.state.solver.BVV(0, 64), # st_nlink
                     mode, # st_mode
                     self.state.solver.BVV(0, 32), # st_uid (lol root)
                     self.state.solver.BVV(0, 32), # st_gid
                     self.state.solver.BVV(0, 64), # st_rdev
                     size, # st_size
                     self.state.solver.BVV(0x400, 64), # st_blksize
```

### Comparing `angr-9.2.8/angr/state_plugins/preconstrainer.py` & `angr-9.2.9/angr/state_plugins/preconstrainer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/scratch.py` & `angr-9.2.9/angr/state_plugins/scratch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/sim_action.py` & `angr-9.2.9/angr/state_plugins/sim_action.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/sim_action_object.py` & `angr-9.2.9/angr/state_plugins/sim_action_object.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/sim_event.py` & `angr-9.2.9/angr/state_plugins/sim_event.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/solver.py` & `angr-9.2.9/angr/state_plugins/solver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/symbolizer.py` & `angr-9.2.9/angr/state_plugins/symbolizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/trace_additions.py` & `angr-9.2.9/angr/state_plugins/trace_additions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/uc_manager.py` & `angr-9.2.9/angr/state_plugins/uc_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/unicorn_engine.py` & `angr-9.2.9/angr/state_plugins/unicorn_engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/state_plugins/view.py` & `angr-9.2.9/angr/state_plugins/view.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/file.py` & `angr-9.2.9/angr/storage/file.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/__init__.py` & `angr-9.2.9/angr/storage/memory_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/actions_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/actions_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/address_concretization_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/address_concretization_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/bvv_conversion_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/bvv_conversion_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/clouseau_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/clouseau_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/conditional_store_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/conditional_store_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/convenient_mappings_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/convenient_mappings_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/default_filler_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/default_filler_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/hex_dumper_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/hex_dumper_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/label_merger_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/label_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/multi_value_merger_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/multi_value_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/name_resolution_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/name_resolution_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/__init__.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/cooperation.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/cooperation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/list_page.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/list_page.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/multi_values.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/multi_values.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/privileged_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/privileged_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py` & `angr-9.2.9/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/regioned_memory/region_data.py` & `angr-9.2.9/angr/storage/memory_mixins/regioned_memory/region_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/simple_interface_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/simple_interface_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/size_resolution_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/size_resolution_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/slotted_memory.py` & `angr-9.2.9/angr/storage/memory_mixins/slotted_memory.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/smart_find_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/smart_find_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/top_merger_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/top_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/underconstrained_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/underconstrained_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_mixins/unwrapper_mixin.py` & `angr-9.2.9/angr/storage/memory_mixins/unwrapper_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/memory_object.py` & `angr-9.2.9/angr/storage/memory_object.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/storage/pcap.py` & `angr-9.2.9/angr/storage/pcap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/tablespecs.py` & `angr-9.2.9/angr/tablespecs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/type_backend.py` & `angr-9.2.9/angr/type_backend.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/__init__.py` & `angr-9.2.9/angr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/algo.py` & `angr-9.2.9/angr/utils/algo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/cowdict.py` & `angr-9.2.9/angr/utils/cowdict.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/enums_conv.py` & `angr-9.2.9/angr/utils/enums_conv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/formatting.py` & `angr-9.2.9/angr/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/graph.py` & `angr-9.2.9/angr/utils/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/library.py` & `angr-9.2.9/angr/utils/library.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/utils/timing.py` & `angr-9.2.9/angr/utils/timing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr/vaults.py` & `angr-9.2.9/angr/vaults.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/angr.egg-info/PKG-INFO` & `angr-9.2.9/angr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr
-Version: 9.2.8
+Version: 9.2.9
 Summary: A multi-architecture binary analysis toolkit, with the ability to perform dynamic symbolic execution and various static analyses on binaries
 Home-page: https://github.com/angr/angr
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `angr-9.2.8/angr.egg-info/SOURCES.txt` & `angr-9.2.9/angr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -893,14 +893,15 @@
 angr/procedures/libstdcpp/_unwind_resume.py
 angr/procedures/libstdcpp/std____throw_bad_alloc.py
 angr/procedures/libstdcpp/std____throw_bad_cast.py
 angr/procedures/libstdcpp/std____throw_length_error.py
 angr/procedures/libstdcpp/std____throw_logic_error.py
 angr/procedures/libstdcpp/std__terminate.py
 angr/procedures/linux_kernel/__init__.py
+angr/procedures/linux_kernel/access.py
 angr/procedures/linux_kernel/arch_prctl.py
 angr/procedures/linux_kernel/arm_user_helpers.py
 angr/procedures/linux_kernel/brk.py
 angr/procedures/linux_kernel/cwd.py
 angr/procedures/linux_kernel/fstat.py
 angr/procedures/linux_kernel/fstat64.py
 angr/procedures/linux_kernel/futex.py
```

### Comparing `angr-9.2.8/native/Makefile` & `angr-9.2.9/native/Makefile`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/native/angr_native.def` & `angr-9.2.9/native/angr_native.def`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/native/log.c` & `angr-9.2.9/native/log.c`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/native/log.h` & `angr-9.2.9/native/log.h`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/native/sim_unicorn.cpp` & `angr-9.2.9/native/sim_unicorn.cpp`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/native/sim_unicorn.hpp` & `angr-9.2.9/native/sim_unicorn.hpp`

 * *Files identical despite different names*

### Comparing `angr-9.2.8/setup.cfg` & `angr-9.2.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 	dpkt
 	mulpyplexer
 	networkx >= 2.0, != 2.8.1
 	progressbar2 >= 3
 	rpyc
 	cffi >= 1.14.0
 	unicorn == 1.0.2rc4
-	archinfo == 9.2.8
-	claripy == 9.2.8
-	cle == 9.2.8
-	pyvex == 9.2.8
-	ailment == 9.2.8
+	archinfo == 9.2.9
+	claripy == 9.2.9
+	cle == 9.2.9
+	pyvex == 9.2.9
+	ailment == 9.2.9
 	GitPython
 	psutil
 	pycparser >= 2.18
 	itanium_demangler
 	CppHeaderParser
 	protobuf >= 3.19.0
 	nampa
```

### Comparing `angr-9.2.8/setup.py` & `angr-9.2.9/setup.py`

 * *Files identical despite different names*

