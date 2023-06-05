# Comparing `tmp/quickstats-0.6.8.3.tar.gz` & `tmp/quickstats-0.6.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.8.3.tar", last modified: Wed May 31 23:19:43 2023, max compression
+gzip compressed data, was "quickstats-0.6.8.4.tar", last modified: Mon Jun  5 21:18:20 2023, max compression
```

## Comparing `quickstats-0.6.8.3.tar` & `quickstats-0.6.8.4.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.3/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.3/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-05-31 20:15:22.000000 quickstats-0.6.8.3/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.3/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.3/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.3/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.3/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.3/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.3/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.3/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31665 2023-05-20 03:35:44.000000 quickstats-0.6.8.3/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8856 2023-05-20 03:36:01.000000 quickstats-0.6.8.3/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.3/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    35299 2023-05-31 19:41:46.000000 quickstats-0.6.8.3/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.3/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.3/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-05-03 13:28:30.000000 quickstats-0.6.8.3/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.3/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.3/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.3/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.3/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13395 2023-05-27 02:29:45.000000 quickstats-0.6.8.3/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.8.3/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.3/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-05-31 14:47:47.000000 quickstats-0.6.8.3/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    98139 2023-05-31 20:12:21.000000 quickstats-0.6.8.3/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.3/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15647 2023-05-25 18:13:48.000000 quickstats-0.6.8.3/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.3/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.3/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.3/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.3/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.3/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.3/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.3/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.3/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17291 2023-05-31 18:05:59.000000 quickstats-0.6.8.3/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12390 2023-05-31 15:55:13.000000 quickstats-0.6.8.3/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.3/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      937 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2204 2022-11-10 10:03:00.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      654 2022-07-19 21:53:28.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8953 2023-05-28 22:27:10.000000 quickstats-0.6.8.3/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.3/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6646 2023-05-20 03:08:06.000000 quickstats-0.6.8.3/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.3/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.3/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.3/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.3/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.3/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.3/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.3/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.3/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.3/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.3/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.3/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53138 2023-05-20 03:11:16.000000 quickstats-0.6.8.3/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.3/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.3/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.3/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3064 2023-05-31 15:10:38.000000 quickstats-0.6.8.3/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.3/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.3/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-05-31 15:28:21.000000 quickstats-0.6.8.3/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-05-31 15:28:38.000000 quickstats-0.6.8.3/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.3/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.3/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.3/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.3/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.3/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.3/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.3/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.3/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.3/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.3/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.3/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.3/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.3/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.3/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.3/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.3/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.3/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.3/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.3/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.3/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.3/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.3/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.3/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.3/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.3/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.3/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.3/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.8.3/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.3/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    24166 2023-05-20 11:38:14.000000 quickstats-0.6.8.3/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.3/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.3/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.3/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.3/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15883 2023-05-31 15:27:08.000000 quickstats-0.6.8.3/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.3/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12818 2023-04-27 22:46:00.000000 quickstats-0.6.8.3/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.3/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.3/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.3/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.3/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.3/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.3/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.3/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.3/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.3/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5834 2023-05-25 20:07:07.000000 quickstats-0.6.8.3/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.8.3/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.3/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.3/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.3/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.3/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.3/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.3/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.3/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.3/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28679 2023-05-20 03:29:27.000000 quickstats-0.6.8.3/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.3/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.3/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.3/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.3/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10949 2023-05-27 07:03:50.000000 quickstats-0.6.8.3/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.3/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16140 2023-03-25 23:04:40.000000 quickstats-0.6.8.3/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.3/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.3/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.3/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26227 2023-05-20 21:07:10.000000 quickstats-0.6.8.3/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.3/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.3/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.3/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.8.3/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9079 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.3/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.4/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.4/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-06-05 21:17:07.000000 quickstats-0.6.8.4/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.4/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.4/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.4/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.4/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.4/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.4/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.4/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32052 2023-06-03 14:05:32.000000 quickstats-0.6.8.4/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8856 2023-05-20 03:36:01.000000 quickstats-0.6.8.4/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:12.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:12.000000 quickstats-0.6.8.4/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.4/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    35299 2023-05-31 19:41:46.000000 quickstats-0.6.8.4/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.4/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.4/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.4/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.4/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.4/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:14.000000 quickstats-0.6.8.4/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.4/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.4/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13395 2023-05-27 02:29:45.000000 quickstats-0.6.8.4/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.8.4/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.4/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-05-31 14:47:47.000000 quickstats-0.6.8.4/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    98139 2023-05-31 20:12:21.000000 quickstats-0.6.8.4/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.4/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15647 2023-05-25 18:13:48.000000 quickstats-0.6.8.4/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:14.000000 quickstats-0.6.8.4/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.4/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.4/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.4/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.4/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.4/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.4/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.4/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.4/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17291 2023-05-31 18:05:59.000000 quickstats-0.6.8.4/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12390 2023-05-31 15:55:13.000000 quickstats-0.6.8.4/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:14.000000 quickstats-0.6.8.4/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.4/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:15.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8953 2023-05-28 22:27:10.000000 quickstats-0.6.8.4/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.4/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6772 2023-06-03 19:25:34.000000 quickstats-0.6.8.4/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.4/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.4/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.4/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.4/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.4/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.4/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.4/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.4/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.4/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.4/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.4/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53138 2023-05-20 03:11:16.000000 quickstats-0.6.8.4/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.4/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.4/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.4/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3064 2023-05-31 15:10:38.000000 quickstats-0.6.8.4/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.4/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-05-31 15:28:21.000000 quickstats-0.6.8.4/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-05-31 15:28:38.000000 quickstats-0.6.8.4/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.4/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.4/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.4/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.4/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.4/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.4/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.4/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.4/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:17.000000 quickstats-0.6.8.4/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.4/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.4/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.4/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.4/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.4/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.4/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.4/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.4/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.4/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.4/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.4/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.4/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.4/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.4/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.4/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.4/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.4/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.4/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:17.000000 quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:17.000000 quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.4/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.8.4/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.4/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25719 2023-06-05 15:09:16.000000 quickstats-0.6.8.4/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.4/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.4/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.4/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.4/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15883 2023-05-31 15:27:08.000000 quickstats-0.6.8.4/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.4/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12818 2023-04-27 22:46:00.000000 quickstats-0.6.8.4/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.4/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.4/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.4/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.4/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.4/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.4/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.4/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.4/quickstats/plots/histo_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.4/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5834 2023-05-25 20:07:07.000000 quickstats-0.6.8.4/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.8.4/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.4/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.4/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.4/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.4/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.4/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.4/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.4/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.4/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29805 2023-06-05 15:07:31.000000 quickstats-0.6.8.4/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.4/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.4/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.4/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.4/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10988 2023-06-03 14:56:07.000000 quickstats-0.6.8.4/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.4/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.4/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.4/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.4/quickstats/utils/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.4/quickstats/utils/process_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26227 2023-05-20 21:07:10.000000 quickstats-0.6.8.4/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.4/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.4/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.4/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.8.4/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9079 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.4/setup.py
```

### Comparing `quickstats-0.6.8.3/PKG-INFO` & `quickstats-0.6.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.3
+Version: 0.6.8.4
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.3/README.md` & `quickstats-0.6.8.4/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/bin/quickstats` & `quickstats-0.6.8.4/bin/quickstats`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/__init__.py` & `quickstats-0.6.8.4/quickstats/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/analysis_base.py` & `quickstats-0.6.8.4/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.8.4/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.8.4/quickstats/analysis/config_format_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/data_loading.py` & `quickstats-0.6.8.4/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.8.4/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/event_categorization.py` & `quickstats-0.6.8.4/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.8.4/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.8.4/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.6.8.4/quickstats/analysis/ntuple_process_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     @property
     def attribute_df(self):
         return self._attribute_df
     
     def __init__(self, sample_config:Union[Dict, str], outdir:str='output',
                  processor_config:Optional[str]=None,
                  processor_flags:Optional[List[str]]=None,
+                 cache:bool=True,
                  use_template:bool=False,
                  multithread:bool=True,
                  disable_config_message:bool=False,
                  verbosity:Optional[Union[int, str]]="INFO",
                  **kwargs):
         
         super().__init__(disable_config_message=disable_config_message,
@@ -77,14 +78,15 @@
         self.path_manager.set_directory("cutflow", "cutflow")
         
         self.load_sample_config(sample_config)
         
         self.processor = None        
         if processor_config is not None:
             self.load_processor_config(processor_config,
+                                       cache=cache,
                                        use_template=use_template,
                                        multithread=multithread)
             
         if processor_flags is not None:
             self.processor_flags = list(processor_flags)
         else:
             self.processor_flags = []
@@ -95,14 +97,19 @@
         if isinstance(config_source, str):
             if not os.path.exists(config_source):
                 raise FileNotFoundError(f'config file "{config_source}" does not exist')
             config_path = os.path.abspath(config_source)
             self.path_manager.set_file("sample_config", config_path)
         self.load_config(config_source)
         
+        if 'systematic_samples' not in self.config:
+            self.config['systematic_samples'] = {}
+        if 'systematics' not in self.config:
+            self.config['systematics'] = {}
+            
         if 'Nominal' in self.sample_config['systematic_samples']:
             raise ValueError('Nominal samples should be placed in the "samples" key '
                              '(instead of "systematic_samples")')
         sample_list = list(self.sample_config['samples'])
         self._syst_theme_list = list(self.sample_config['systematic_samples'])
         for syst_theme in self.syst_theme_list:
             sample_list.extend(list(self.sample_config['systematic_samples'][syst_theme]))
@@ -170,21 +177,23 @@
                     attribute_data['sample'].append(sample)
                     attribute_data['syst_name'].append(syst_name)
                     attribute_data['syst_var'].append(syst_var)
                     attribute_data['sample_type'].append(sample_type)
         import pandas as pd
         index_list = ['syst_theme', 'sample', 'syst_name', 'sample_type', 'syst_var']
         attribute_df = pd.DataFrame(attribute_data).set_index(index_list)
-        return attribute_df  
+        return attribute_df
     
     def load_processor_config(self, config_path:str,
+                              cache:bool=True,
                               multithread:bool=True,
                               use_template:bool=False):
         from quickstats.components.processors import RooProcessor
         self.processor = RooProcessor(config_path,
+                                      cache=cache,
                                       use_template=use_template,
                                       multithread=multithread,
                                       verbosity=self.stdout.verbosity)
         self.path_manager.set_file("processor_config", os.path.abspath(config_path))
         
     def get_validated_syst_themes(self, syst_themes:Optional[List[str]]=None):
         if syst_themes is None:
```

### Comparing `quickstats-0.6.8.3/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.8.4/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.6.8.4/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.6.8.4/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.6.8.4/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.6.8.4/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/clis/core.py` & `quickstats-0.6.8.4/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.8.4/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/clis/inspect_ws.py` & `quickstats-0.6.8.4/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.8.4/quickstats/clis/likelihood_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @click.option('-s', '--snapshot', 'snapshot_name', default=None, show_default=True,
               help='Name of initial snapshot')
 @click.option('-r', '--profile', 'profile_param', default="", show_default=True,
               help='Parameters to profile')
 @click.option('-f', '--fix', 'fix_param', default="", show_default=True,
               help='Parameters to fix')
 @click.option('--pois', default="", show_default=True,
-              help='Define the set of POIs (separated by commas) sed for calculating Minos errors.')
+              help='Define the set of POIs (separated by commas) set for calculating Minos errors.')
 @click.option('--constrain/--no-constrain', 'constrain_nuis', default=True, show_default=True,
               help='Use constrained NLL (i.e. include systematics)')
 @click.option('-t', '--minimizer_type', default="Minuit2", show_default=True,
               help='Minimizer type')
 @click.option('-a', '--minimizer_algo', default="Migrad", show_default=True,
               help='Minimizer algorithm')
 @click.option('-c', '--num_cpu', type=int, default=1, show_default=True,
```

### Comparing `quickstats-0.6.8.3/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.8.4/quickstats/clis/likelihood_scan.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/clis/limit_setting.py` & `quickstats-0.6.8.4/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/clis/processor_cli.py` & `quickstats-0.6.8.4/quickstats/clis/processor_cli.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/clis/workspace_tools.py` & `quickstats-0.6.8.4/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/__init__.py` & `quickstats-0.6.8.4/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/analysis_base.py` & `quickstats-0.6.8.4/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/analysis_object.py` & `quickstats-0.6.8.4/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/asimov_generator.py` & `quickstats-0.6.8.4/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.8.4/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/basics.py` & `quickstats-0.6.8.4/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/extended_minimizer.py` & `quickstats-0.6.8.4/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/extended_model.py` & `quickstats-0.6.8.4/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/extended_rfile.py` & `quickstats-0.6.8.4/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/likelihood.py` & `quickstats-0.6.8.4/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/modelling/component_source.py` & `quickstats-0.6.8.4/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.8.4/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/modelling/model_source.py` & `quickstats-0.6.8.4/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.8.4/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.8.4/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.8.4/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.8.4/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.8.4/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.6.8.4/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_export.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from typing import Optional, List, Dict
 import os
 import json
 
 from .rooproc_helper_action import RooProcHelperAction
 
+from quickstats.utils.common_utils import is_valid_file
+
 class RooProcExport(RooProcHelperAction):
     def __init__(self, filename:str):
         super().__init__(filename=filename)
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
         kwargs = cls.parse_as_kwargs(main_text)
         return cls(**kwargs)
     
     def _execute(self, processor:"quickstats.RooProcessor", **params):
         filename = params['filename']
+        if processor.cache and is_valid_file(filename):
+            processor.stdout.info(f"INFO: Cached output `{filename}`.")
+            return processor   
         data = {k:v.GetValue() for k,v in processor.external_variables.items()}
         dirname = os.path.dirname(filename)
         if dirname and (not os.path.exists(dirname)):
             os.makedirs(dirname)
         with open(filename, 'w') as outfile:
             processor.stdout.info(f'INFO: Writing auxiliary data to "{filename}".')
             json.dump(data, outfile, indent=2)
```

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from typing import Optional, List
 import fnmatch
 
 from .rooproc_hybrid_action import RooProcHybridAction
 
-from quickstats.utils.common_utils import is_valid_file
+from quickstats.utils.common_utils import is_valid_file, filter_by_wildcards
 
 class RooProcSave(RooProcHybridAction):
     
     def __init__(self, treename:str, filename:str, 
                  columns:Optional[List[str]]=None,
+                 exclude:Optional[List[str]]=None,
                  frame:Optional[str]=None):
         super().__init__(treename=treename,
                          filename=filename,
                          columns=columns,
+                         exclude=exclude,
                          frame=frame)
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
         kwargs = cls.parse_as_kwargs(main_text)
         return cls(**kwargs)
     
     def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
         treename = params['treename']
         filename = params['filename']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'INFO: Cached output from "{filename}".')
             return rdf, processor
+        all_columns = [str(c) for c in rdf.GetColumnNames()]
         columns = params.get('columns', None)
+        exclude = params.get('exclude', None)
+        self.makedirs(filename)
         if isinstance(columns, str):
             columns = self.parse_as_list(columns)
         if columns is None:
-            if processor.use_template:
-                from quickstats.utils.root_utils import templated_rdf_snapshot
-                rdf_next = templated_rdf_snapshot(rdf)(treename, filename)
-            else:
-                rdf_next = rdf.Snapshot(treename, filename)
+            columns = list(all_columns)
+        if exclude is None:
+            exclude = []
+        save_columns = filter_by_wildcards(all_columns, columns)
+        save_columns = filter_by_wildcards(save_columns, exclude, exclusion=True)
+        save_columns = list(set(save_columns))
+        if processor.use_template:
+            from quickstats.utils.root_utils import templated_rdf_snapshot 
+            rdf_next = templated_rdf_snapshot(rdf, save_columns)(treename, filename, save_columns)
         else:
-            all_columns = [str(c) for c in rdf.GetColumnNames()]
-            save_columns = []
-            for column in columns:
-                save_columns += [c for c in all_columns if fnmatch.fnmatch(c, column)]
-            save_columns = list(set(save_columns))
-            self.makedirs(filename)
-            if processor.use_template:
-                from quickstats.utils.root_utils import templated_rdf_snapshot 
-                rdf_next = templated_rdf_snapshot(rdf, save_columns)(treename, filename, save_columns)
-            else:
-                rdf_next = rdf.Snapshot(treename, filename, save_columns)
-        processor.stdout.info(f'INFO: Writing output to "{filename}".')
+            rdf_next = rdf.Snapshot(treename, filename, save_columns)
+        processor.stdout.info(f'Writing output to "{filename}".')
         return rdf_next, processor
```

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,10 +9,10 @@
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
         return cls(name=main_text)
     
     def _execute(self, processor:"quickstats.RooProcessor", **params):
         frame_name = params['name']
         if frame_name in processor.rdf_frames:
-            processor.stdout.warning(f"WARNING: Overriding existing rdf frame `{frame_name}`")
+            processor.stdout.warning(f'Overriding existing rdf frame "{frame_name}"')
         processor.rdf_frames[frame_name] = processor.rdf
         return processor
```

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/builtin_methods.py` & `quickstats-0.6.8.4/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.8.4/quickstats/components/processors/roo_config_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.8.4/quickstats/components/processors/roo_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,18 @@
             return None
         if self.treename is None:
             raise RuntimeError("tree name is undefined")
     
     def run(self, filename:Union[List[str], str]):
         self.sanity_check()
         all_files = self._get_all_files(filename)
-        if len(all_files) == 1:
+        if len(all_files) == 0:
+            self.stdout.info(f'No files to be processed. Skipped.')
+            return None
+        elif len(all_files) == 1:
             self.stdout.info(f'Processing file "{all_files[0]}".')
         else:
             self.stdout.info(f"Professing files")
             for f in all_files:
                 self.stdout.info(f'\t"{f}"', bare=True)  
         with Timer() as t:
             self.rdf = ROOT.RDataFrame(self.treename, all_files)
```

### Comparing `quickstats-0.6.8.3/quickstats/components/pvalue_toys.py` & `quickstats-0.6.8.4/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/roo_inspector.py` & `quickstats-0.6.8.4/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/root_object.py` & `quickstats-0.6.8.4/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.8.4/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/sample.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/settings.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.8.4/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/concurrent/logging.py` & `quickstats-0.6.8.4/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.6.8.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.8.4/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.8.4/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.8.4/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/abstract_object.py` & `quickstats-0.6.8.4/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/configs.py` & `quickstats-0.6.8.4/quickstats/core/configs.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/configurable_object.py` & `quickstats-0.6.8.4/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/dataclass_object.py` & `quickstats-0.6.8.4/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/decorators.py` & `quickstats-0.6.8.4/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/enums.py` & `quickstats-0.6.8.4/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/methods.py` & `quickstats-0.6.8.4/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/path_manager.py` & `quickstats-0.6.8.4/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/core/virtual_trees.py` & `quickstats-0.6.8.4/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/cppyy/core.py` & `quickstats-0.6.8.4/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/cppyy/macros.py` & `quickstats-0.6.8.4/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.8.4/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.8.4/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.6.8.4/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/RooCategory.py` & `quickstats-0.6.8.4/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.8.4/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.8.4/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.8.4/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/TF1.py` & `quickstats-0.6.8.4/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/TFile.py` & `quickstats-0.6.8.4/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/TH1.py` & `quickstats-0.6.8.4/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/TH2.py` & `quickstats-0.6.8.4/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/TObject.py` & `quickstats-0.6.8.4/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/__init__.py` & `quickstats-0.6.8.4/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/helper.py` & `quickstats-0.6.8.4/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/inspection.py` & `quickstats-0.6.8.4/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/macros.py` & `quickstats-0.6.8.4/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.8.4/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/maths/interpolation.py` & `quickstats-0.6.8.4/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/maths/numerics.py` & `quickstats-0.6.8.4/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/maths/statistics.py` & `quickstats-0.6.8.4/quickstats/maths/statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,21 +198,33 @@
 
 def min_max_to_range(min_val:Optional[float]=None, max_val:Optional[float]=None):
     if (min_val is None) and (max_val is None):
         return None
     if (min_val is not None) and (max_val is not None):
         return (min_val, max_val)
     raise ValueError("min and max values must be all None or all float")
+    
+def get_clipped_data(x:np.ndarray,
+                     bin_range:Optional[Sequence]=None,
+                     clip_lower:bool=True,
+                     clip_upper:bool=True):
+    if (bin_range is None) or ((clip_lower == False) and (clip_upper == False)):
+        return np.array(x)
+    xmin = bin_range[0] if clip_lower else None
+    xmax = bin_range[1] if clip_upper else None
+    return np.clip(x, xmin, xmax)
 
 def histogram(x:np.ndarray, weights:Optional[np.ndarray]=None,
               bins:Union[int, Sequence]=10,
               bin_range:Optional[Sequence]=None,
+              underflow:bool=False,
+              overflow:bool=False,
               normalize:bool=True,
               clip_weight:bool=False,
-              evaluate_error:bool=True,
+              evaluate_error:bool=False,
               error_option:Union[BinErrorOption, str]="auto"):
     """
         Compute the histogram of a data array.
         
         Arguments:
         -------------------------------------------------------------------------------
         x: ndarray
@@ -224,22 +236,27 @@
             If integer, it defines the number of equal-width bins in the
             given range.
             If sequence, it defines a monotonically increasing array of bin edges,
             including the rightmost edge.
        bin_range: (optional) sequence of the form (float, float)
            The lower and upper range of the bins.  If not provided, range is simply 
            ``(x.min(), x.max())``.  Values outside the range are ignored.
+       underflow: bool, default = False
+           Include undeflow data in the first bin.
+       overflow: bool, default = False
+           Include overflow data in the last bin.
        normalize: bool, default = True
-           If True, the sum of bin contents is normalized to one.
-       clip_weight: bool, default = True
-           If True, ignore data outside given range when evaluating total weight
+           Normalize the sum of weights to one. Weights outside the bin range will
+           not be counted if ``clip_weight`` is set to false, so the sum of bin
+           content could be less than one.
+       clip_weight: bool, default = False
+           Ignore data outside given range when evaluating total weight
            used in normalization.
        evaluate_error: bool, default = True
-           If True, evaluate the error of the bin contents using the given error
-           option.
+           Evaluate the error of the bin contents using the given error option.
        error_option: BinErrorOption or str, default = "auto"
            How to evaluate bin errors. If "sumw2", symmetric errors from the Wald
            approximation is used (square root of sum of squares of weights). If
            "poisson", asymmetric errors from Poisson interval at one sigma is
            used. If "auto", it will use sumw2 error if data has unit weights,
            else Poisson error will be used.
            
@@ -248,15 +265,16 @@
        bin_content: np.ndarray
            The bin content of the histogram.
        bin_edges: np.ndarray
            The bin edges of the histogram.
        bin_errors: np.ndarray
            The bin errors of the histogram.
     """
-    x = np.array(x)
+    x = get_clipped_data(x, bin_range=bin_range, clip_lower=underflow,
+                         clip_upper=overflow)
     
     if weights is None:
         weights = np.ones(x.shape)
     else:
         # fix overflow bugs
         weights = np.array(weights, dtype=float)
         
@@ -266,22 +284,23 @@
             norm_factor = weights[(x >= first_edge) & (x <= last_edge)].sum()
         else:
             norm_factor = weights.sum()
     else:
         norm_factor = 1
         
     bin_content, bin_edges = np.histogram(x, bins=bins, range=bin_range, weights=weights)
+    
     if evaluate_error:
         error_option = BinErrorOption.parse(error_option)
         if error_option == BinErrorOption.AUTO:
             unit_weight = np.allclose(weights, np.ones(weights.shape))
             error_option = BinErrorOption.POISSON if unit_weight else BinErrorOption.SUMW2
         if error_option == BinErrorOption.POISSON:
             pois_interval = get_poisson_interval(bin_content)
-            bin_errors =  (pois_interval["lo"] / norm_factor, pois_interval["hi"] / norm_factor)
+            bin_errors =  (pois_interval["lo"], pois_interval["hi"])
         elif error_option == BinErrorOption.SUMW2:
             bin_content_weight2, _ = np.histogram(x, bins=bins, range=bin_range, weights=weights**2)
             bin_errors = np.sqrt(bin_content_weight2)
         if norm_factor != 1:
             if isinstance(bin_errors, tuple):
                 bin_errors = (bin_errors[0] / norm_factor, bin_errors[1] / norm_factor)
             else:
@@ -293,14 +312,16 @@
         bin_content /= norm_factor
     
     return bin_content, bin_edges, bin_errors
         
 def get_hist_data(x:np.ndarray, weights:Optional[np.ndarray]=None,
                   bins:Union[int, Sequence]=10,
                   bin_range:Optional[Sequence]=None,
+                  underflow:bool=False,
+                  overflow:bool=False,
                   normalize:bool=True,
                   clip_weight:bool=False,
                   xerr:bool=True,
                   yerr:bool=True,
                   error_option:Union[BinErrorOption, str]="auto"):
     """
         Extract histogram data from a data array.
@@ -316,16 +337,22 @@
             If integer, it defines the number of equal-width bins in the
             given range.
             If sequence, it defines a monotonically increasing array of bin edges,
             including the rightmost edge.
        bin_range: (optional) sequence of the form (float, float)
            The lower and upper range of the bins.  If not provided, range is simply 
            ``(x.min(), x.max())``.  Values outside the range are ignored.
+       underflow: bool, default = False
+           Include undeflow data in the first bin.
+       overflow: bool, default = False
+           Include overflow data in the last bin.
        normalize: bool, default = True
-           If True, the sum of bin contents is normalized to one.
+           Normalize the sum of weights to one. Weights outside the bin range will
+           not be counted if ``clip_weight`` is set to false, so the sum of bin
+           content could be less than one.
        clip_weight: bool, default = True
            If True, ignore data outside given range when evaluating total weight
            used in normalization.
        xerr: bool, default = True
            If True, evaluate the error of the bin centers (= bin widths / 2).
        yerr: bool, default = True
            If True, evaluate the error of the bin contents using the given error
@@ -341,14 +368,16 @@
        -------------------------------------------------------------------------------
        hist_data: dict
            A dictionary with the keys "x", "y", "xerr", "yerr" with the bin centers,
            bin content, half bin widths and bin errors as values.
     """
     y, bin_edges, yerr = histogram(x, weights=weights,
                                    bins=bins, bin_range=bin_range,
+                                   underflow=underflow,
+                                   overflow=overflow,
                                    normalize=normalize,
                                    clip_weight=clip_weight,
                                    evaluate_error=yerr,
                                    error_option=error_option)
     x = bin_edge_to_bin_center(bin_edges)
     if xerr:
         # todo do not hard-code number of digits to keep
@@ -363,27 +392,31 @@
     }
     return hist_data
 
 def get_stacked_hist_data(x:List[np.ndarray],
                           weights:List[Optional[np.ndarray]]=None,
                           bins:Union[int, Sequence]=10,
                           bin_range:Optional[Sequence]=None,
+                          underflow:bool=False,
+                          overflow:bool=False,
                           normalize:bool=True,
                           clip_weight:bool=False,
                           xerr:bool=True,
                           yerr:bool=True,
                           error_option:Union[BinErrorOption, str]="auto"):
     x = np.concatenate(x)
     if weights is not None:
         weights = np.concatenate(weights)
         assert x.shape == weights.shape
     if bin_range is None:
         bin_range = (np.min(x), np.max(x))
     return get_hist_data(x=x, weights=weights,
                          bins=bins, bin_range=bin_range,
+                         underflow=underflow,
+                         overflow=overflow,
                          normalize=normalize,
                          clip_weight=clip_weight,
                          xerr=xerr, yerr=yerr,
                          error_option=error_option)
 
 def get_sumw2(weights:np.ndarray):
     return np.sqrt(np.sum(weights ** 2))
```

### Comparing `quickstats-0.6.8.3/quickstats/maths/statistics_jitted.py` & `quickstats-0.6.8.4/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/maths/symbolics.py` & `quickstats-0.6.8.4/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/parsers/param_parser.py` & `quickstats-0.6.8.4/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/__init__.py` & `quickstats-0.6.8.4/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/abstract_plot.py` & `quickstats-0.6.8.4/quickstats/plots/abstract_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.6.8.4/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.8.4/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/color_schemes.py` & `quickstats-0.6.8.4/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/core.py` & `quickstats-0.6.8.4/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/correlation_plot.py` & `quickstats-0.6.8.4/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.8.4/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.8.4/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/histo_1D_plot.py` & `quickstats-0.6.8.4/quickstats/plots/histo_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.8.4/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.6.8.4/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.6.8.4/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.8.4/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.8.4/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.8.4/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.8.4/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.8.4/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/template.py` & `quickstats-0.6.8.4/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.8.4/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.8.4/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.8.4/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.6.8.4/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.6.8.4/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.6.8.4/quickstats/plots/variable_distribution_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from quickstats.plots import AbstractPlot, get_color_cycle
 from quickstats.plots.template import ratio_frames, suggest_markersize, centralize_axis
 from quickstats.utils.common_utils import combine_dict
 from quickstats.maths.numerics import safe_div
 from quickstats.maths.statistics import (HistComparisonMode,
                                          min_max_to_range, get_hist_data,
                                          get_stacked_hist_data,
-                                         get_hist_comparison_data)
+                                         get_hist_comparison_data,
+                                         get_clipped_data)
 
 from .core import PlotFormat, ErrorDisplayFormat
 
 class VariableDistributionPlot(AbstractPlot):
     
     COLOR_CYCLE = "simple_contrast"
     
@@ -344,14 +345,16 @@
             weights = weights * weight_scale            
         return x, weights
     
     def draw_stacked(self, ax, plot_options:Dict,
                      column_name:str, weight_name:Optional[str]=None,
                      bins:Union[int, Sequence]=25,
                      bin_range:Optional[Sequence]=None,
+                     underflow:bool=False,
+                     overflow:bool=False,
                      normalize:bool=True,
                      show_error:bool=False,
                      variable_scale:Optional[float]=None):
         stacked_data = {
             'x'       : [],
             'weights' : [],
             'color'   : [],
@@ -363,14 +366,15 @@
             samples, styles = options['samples'], options['styles']
             label, color = styles['label'], styles['color']
             weight_scale = options['weight_scale']
             x, weights = self.get_sample_data(samples, column_name,
                                               variable_scale=variable_scale,
                                               weight_scale=weight_scale,
                                               weight_name=weight_name)
+            x = get_clipped_data(x, bin_range=bin_range, clip_lower=underflow, clip_upper=overflow)
             stacked_data['x'].append(x)
             stacked_data['weights'].append(weights)
             stacked_data['color'].append(color)
             stacked_data['label'].append(label)
             stacked_styles.append(styles)
         if normalize:
             norm_factor = np.sum([np.sum(weights) for weights in stacked_data['weights']])
@@ -382,26 +386,29 @@
                                             stacked=True,
                                             **stacked_styles)
         for i, target in enumerate(plot_options):
             self.update_legend_handles({target:handle[i]})
         bin_edges = np.histogram_bin_edges(np.concatenate(stacked_data['x']).flatten(),
                                            bins=bins, range=bin_range)
         hist_data = get_stacked_hist_data(stacked_data['x'], stacked_data['weights'],
+                                          underflow=underflow,
+                                          overflow=overflow,
                                           normalize=normalize,
                                           bin_range=bin_range, bins=bins,
                                           clip_weight=False,
                                           xerr=show_error and self.config['show_xerr'],
                                           yerr=show_error,
                                           error_option='auto')
         return bin_edges, hist_data
             
     def draw(self, column_name:str, weight_name:Optional[str]=None,
              targets:Optional[List[str]]=None,
              xlabel:str="", ylabel:str="Fraction of Events / {bin_width:.2f}",
              bins:Union[int, Sequence]=25, bin_range:Optional[Sequence]=None,
+             underflow:bool=False, overflow:bool=False,
              normalize:bool=True, show_error:bool=False, show_error_legend:bool=False,
              stacked:bool=False, xmin:Optional[float]=None, xmax:Optional[float]=None,
              ymin:Optional[float]=None, ymax:Optional[float]=None, ypad:float=0.3,
              variable_scale:Optional[float]=None, logy:bool=False,
              comparison_options:Optional[Union[Dict, List[Dict]]]=None,
              legend_order:Optional[List[str]]=None):
         """
@@ -423,16 +430,22 @@
                 If specified, draw score boundaries at given values.
             bins: int or sequence of scalars, default = 25
                 If integer, it defines the number of equal-width bins in the given range.
                 If sequence, it defines a monotonically increasing array of bin edges,
                 including the rightmost edge.
             bin_range: (optional) (float, float)
                 Range of histogram bins.
+            underflow: bool, default = False
+                Include undeflow data in the first bin.
+            overflow: bool, default = False
+                Include overflow data in the last bin.
             normalize: bool, default = True
-                Normalize the sum of histogram to unity.
+                Normalize the sum of weights to one. Weights outside the bin range will
+                not be counted if ``clip_weight`` is set to false, so the sum of bin
+                content could be less than one.
             show_error: bool, default = False
                 Whether to display data error.
             show_error_legend: bool, default = False
                 Whether to include legend for the error artists.
             xmin: (optional) float
                 Minimum range of x-axis.
             xmax: (optional) float
@@ -491,14 +504,16 @@
                     stacked_plot_options[stack_index] = {}
                 stacked_plot_options[stack_index][target] = options
             for stack_index, stacked_plot_options_i in stacked_plot_options.items():
                 bin_edges, hist_data = self.draw_stacked(ax, stacked_plot_options_i,
                                                          column_name=column_name,
                                                          weight_name=weight_name,
                                                          bins=bins, bin_range=bin_range,
+                                                         underflow=underflow,
+                                                         overflow=overflow,
                                                          normalize=normalize,
                                                          variable_scale=variable_scale)
                 label = self.config['stacked_label'].format(index=stack_index)
                 binned_data[label] = hist_data
                 target_bin_edges[label] = bin_edges
 
         for target, options in plot_options.items():
@@ -507,26 +522,28 @@
             weight_scale = options['weight_scale']
             plot_format, error_format = options['plot_format'], options['error_format']
             x, weights = self.get_sample_data(samples, column_name,
                                               variable_scale=variable_scale,
                                               weight_scale=weight_scale,
                                               weight_name=weight_name)
             bin_edges = np.histogram_bin_edges(x, bins=bins, range=bin_range)
-            hist_data = get_hist_data(x, weights, normalize=normalize,
+            hist_data = get_hist_data(x, weights, underflow=underflow,
+                                      overflow=overflow, normalize=normalize,
                                       bin_range=bin_range, bins=bins,
                                       clip_weight=False,
                                       xerr=show_error and self.config['show_xerr'],
                                       yerr=show_error,
                                       error_option='auto')
             binned_data[target] = hist_data
             target_bin_edges[target] = bin_edges
             if plot_format == PlotFormat.HIST:
                 if normalize:
                     weights /= weights.sum()
-                hist_y, _, handle = ax.hist(x, bins, range=bin_range,
+                x_ = get_clipped_data(x, bin_range=bin_range, clip_lower=underflow, clip_upper=overflow)
+                hist_y, _, handle = ax.hist(x_, bins, range=bin_range,
                                             weights=weights, **styles)
                 assert np.allclose(hist_data['y'], hist_y)
                 _, error_handle = self.draw_binned_data(ax, hist_data,
                                                         bin_edges=bin_edges,
                                                         draw_data=False,
                                                         draw_error=show_error,
                                                         error_format=error_format,
```

### Comparing `quickstats-0.6.8.3/quickstats/root_checker.py` & `quickstats-0.6.8.4/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/utils/common_utils.py` & `quickstats-0.6.8.4/quickstats/utils/common_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,16 @@
         os.environ["PYTHONPATH"].replace(scripts_path+":","")
         
     if (scripts_path not in sys.path) and (undo==False):
         sys.path.insert(0, scripts_path)
         os.environ["PYTHONPATH"] = scripts_path + ":" + os.environ.get("PYTHONPATH", "")
         
 def is_valid_file(fname:str):
+    if not fname:
+        return False
     if not os.path.exists(fname):
         return False
     ext = os.path.splitext(fname)[-1]
     if ext == ".root":
         from quickstats.utils.root_utils import is_corrupt
         return not is_corrupt(fname)
     return (os.path.isfile(fname)) and (os.path.getsize(fname) > 0)
```

### Comparing `quickstats-0.6.8.3/quickstats/utils/data_conversion.py` & `quickstats-0.6.8.4/quickstats/utils/data_conversion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Optional, Dict, List
+from typing import Union, Optional, Dict, List, Sequence
 import os
 import re
 import glob
 import uuid
 
 import numpy as np
 
@@ -46,15 +46,15 @@
     import pandas as pd
     fcols = df.select_dtypes('float').columns
     icols = df.select_dtypes('integer').columns
 
     df[fcols] = df[fcols].apply(pd.to_numeric, downcast='float')
     df[icols] = df[icols].apply(pd.to_numeric, downcast='integer')
 
-def array2root(array_data:Dict[str, np.ndarray], fname:str, treename:str,
+def array2root(array_data:Dict[str, np.ndarray], filename:str, treename:str,
                library:str="auto", multithread:bool=True):
     if library.lower() == "auto":
         library = get_default_library()
     if library == "root":
         from quickstats.interface.root.helper import RMultithreadEnv
         from quickstats.interface.cppyy.vectorize import np_type_str_maps
         with RMultithreadEnv(multithread):
@@ -68,22 +68,22 @@
                 if template_type == "bool":
                     template_type = "int"
                     array_data[column] = array_data[column].astype("int32")
                 snapshot_templates.append(template_type)
             snapshot_templates = tuple(snapshot_templates)
             import ROOT
             df = ROOT.RDF.MakeNumpyDataFrame(array_data)
-            df.Snapshot.__getitem__(snapshot_templates)(treename, fname, columns)
+            df.Snapshot.__getitem__(snapshot_templates)(treename, filename, columns)
     elif library == "uproot":
         import uproot
         from packaging import version
         uproot_version = uproot.__version__
         if version.parse(uproot_version) < version.parse("4.2.0"):
             raise RuntimeError("uproot version too old (requires 4.2.0+)")
-        file = uproot.recreate(fname)
+        file = uproot.recreate(filename)
         file[treename] = array_data
         file.close()
     else:
         raise RuntimeError(f'unknown library "{library}" for root data conversion')            
         
 numpy2root = array2root
 
@@ -103,19 +103,19 @@
             array_shallow_copy[key] = list(array)
     import pandas as pd
     df = pd.DataFrame(array_shallow_copy)
     return df
 
 array2dataframe = numpy2dataframe
 
-def dataframe2root(df:"pandas.DataFrame", fname:str, treename:str,
+def dataframe2root(df:"pandas.DataFrame", filename:str, treename:str,
                    columns:Optional[List[str]]=None,
                    library:str="auto", multithread:bool=True):
     array_data = dataframe2numpy(df, columns)
-    array2root(array_data, fname, treename, library=library,
+    array2root(array_data, filename, treename, library=library,
                multithread=multithread)
     
 def uproot_get_standard_columns(uproot_tree):
     typenames = uproot_tree.typenames()
     columns = list(typenames.keys())
     column_types = list(typenames.values())
     return np.array(columns)[np.where(np.isin(column_types, uproot_datatypes))]
@@ -141,14 +141,73 @@
             reduced_column_types.append(match(vec_expr1, column_type))
         elif column_type.startswith("vector"):
             reduced_column_types.append(match(vec_expr2, column_type))
         else:
             reduced_column_types.append(column_type)
     reduced_column_types = np.array(reduced_column_types)
     return reduced_column_types
+
+
+def make_iter_result(results, downcast:bool=False):
+    if downcast:
+        for result in results:
+            downcast_dataframe(result)
+            yield result
+    for result in results:
+        yield result
+        
+def iterate_uproot(files:List[str], columns:Optional[Union[str, List[str], Dict]]=None,
+                   filter_typename=None, step_size:Union[str, int]='100 MB',
+                   cut:Optional[str]=None, iterate:bool=False, library:str='numpy',
+                   downcast:bool=True):
+    import uproot
+    assert library in ['numpy', 'pandas']
+    if columns is None:
+        expressions = None
+        aliases = None
+    elif isinstance(columns, str):
+        expressions = columns
+        aliases = None
+    elif isinstance(columns, Sequence):
+        expressions = list(columns)
+        aliases = None
+    elif isinstance(columns, dict):
+        expressions = list(columns)
+        aliases = {k:v for k, v in columns.items() if k != v}
+    else:
+        raise TypeError('columns must be a string, list of strings or a dictionary')
+    results = uproot.iterate(files, expressions=expressions,
+                             filter_typename=filter_typename,
+                             step_size=step_size,
+                             aliases=aliases,
+                             cut=cut, library=library)
+    if not iterate:
+        if library == 'numpy':
+            result = {}
+            for batch in results:
+                for column in batch:
+                    if column not in result:
+                        result[column] = batch[column]
+                    else:
+                        result[column] = np.concatenate([result[column], batch[column]])
+            return result
+        else:
+            result = None
+            for batch in results:
+                if downcast:
+                    downcast_dataframe(batch)
+                if result is None:
+                    result = batch
+                else:
+                    result = pd.concat([result, batch])
+            return result
+    else:
+        if (library == 'pandas') and (downcast):
+            return make_iter_result(results, downcast=True)
+        return make_iter_result(results, downcast=False)
     
 def rdf2numpy(rdf, columns:Union[Dict[str, str], List[str]]=None,
               cut:Optional[str]=None, convert_vectors:bool=True,
               mode:Union[str, int, ConversionMode]=1):
     if cut is not None:
         rdf = rdf.Filter(cut)     
     rename_columns = {}
@@ -224,14 +283,15 @@
         result = {column: result[column] for column in columns if column in result}
     return result
     
 def root2numpy(filename:Union[str, List[str]], treename:str,
                columns:Union[Dict[str, str], List[str]]=None,
                cut:Optional[str]=None, convert_vectors:bool=True,
                mode:Union[str, int, ConversionMode]=1,
+               step_size:Union[str, int]='100 MB', iterate:bool=False,
                library:str="auto", multithread:bool=True):
     if isinstance(filename, str) and os.path.isdir(filename):
         filename = glob.glob(os.path.join(filename, "*.root"))
     conversion_mode = ConversionMode.parse(mode)
     if conversion_mode == ConversionMode.REMOVE_NON_ARRAY_TYPE:
         library = "root"
     if library.lower() == "auto":
@@ -241,99 +301,73 @@
         with RMultithreadEnv(multithread):
             import ROOT
             rdf = ROOT.RDataFrame(treename, filename)
             return rdf2numpy(rdf, columns=columns, cut=cut,
                              convert_vectors=convert_vectors,
                              mode=mode)
     elif library.lower() == "uproot":
-        if isinstance(columns, dict):
-            raise RuntimeError('defining new columns are not supported when using "uproot" as the library')
         import uproot
-        if isinstance(filename, str):
-            f = uproot.open(filename)
-            t = f[treename]
-            if conversion_mode == ConversionMode.REMOVE_NON_STANDARD_TYPE:
-                standard_columns = uproot_get_standard_columns(t)
-                if columns is None:
-                    columns = standard_columns
-                else:
-                    columns = [column for column in columns if column in standard_columns]
-            return f[treename].arrays(columns, library="numpy", cut=cut)
+        if not isinstance(filename, list):
+            filename = [filename]
+        # iterate over multiple files
+        files = {f:treename for f in filename}
+        if conversion_mode == ConversionMode.REMOVE_NON_STANDARD_TYPE:
+            filter_typename = list(uproot_datatypes)
         else:
-            # iterate over multiple files
-            files = {f:treename for f in filename}
-            if conversion_mode == ConversionMode.REMOVE_NON_STANDARD_TYPE:
-                filter_typename = list(uproot_datatypes)
-            else:
-                filter_typename = None
-            result = {}
-            for batch in uproot.iterate(files, expressions=columns,
-                                        filter_typename=filter_typename,
-                                        cut=cut, library="numpy"):
-                for column in batch:
-                    if column not in result:
-                        result[column] = batch[column]
-                    else:
-                        result[column] = np.concatenate([result[column], batch[column]])
-            return result
+            filter_typename = None
+        result = iterate_uproot(files, columns=columns,
+                                filter_typename=filter_typename,
+                                step_size=step_size,
+                                cut=cut, library='numpy',
+                                iterate=iterate,
+                                downcast=False)
+        return result
     else:
         raise RuntimeError(f'unknown library "{library}" for root data conversion')
 
 root2array = root2numpy
         
 def root2dataframe(filename:Union[str, List[str]], treename:str,
                    columns:Union[Dict[str, str], List[str]]=None,
                    cut:Optional[str]=None,
                    mode:Union[str, int, ConversionMode]=1,
-                   downcast:bool=True,
+                   downcast:bool=True, iterate:bool=False,
+                   step_size:Union[str, int]='100 MB',
                    library:str="auto", multithread:bool=True):
     conversion_mode = ConversionMode.parse(mode)
     if conversion_mode == ConversionMode.REMOVE_NON_ARRAY_TYPE:
         library = "root"    
     if library.lower() == "auto":
         library = get_default_library(custom_columns=isinstance(columns,dict))
     if library.lower() == "root":
         numpy_data = root2numpy(filename, treename, columns=columns, cut=cut,
                                 convert_vectors=True,
                                 mode=mode,
                                 library=library,
                                 multithread=multithread)
         result = numpy2dataframe(numpy_data)
+        if downcast:
+            downcast_dataframe(result)
     elif library.lower() == "uproot":
-        if isinstance(columns, dict):
-            raise RuntimeError('defining new columns are not supported when using "uproot" as the library')
         import uproot
-        if isinstance(filename, str):
-            f = uproot.open(filename)
-            t = f[treename]
-            if conversion_mode == ConversionMode.REMOVE_NON_STANDARD_TYPE:
-                standard_columns = uproot_get_standard_columns(t)
-                if columns is None:
-                    columns = standard_columns
-                else:
-                    columns = [column for column in columns if column in standard_columns]
-            result = f[treename].arrays(columns, library="pandas")
+        if not isinstance(filename, list):
+            filename = [filename]
+        import pandas as pd
+        # iterate over multiple files
+        files = {f:treename for f in filename}
+        if conversion_mode == ConversionMode.REMOVE_NON_STANDARD_TYPE:
+            filter_typename = list(uproot_datatypes)
         else:
-            import pandas as pd
-            # iterate over multiple files
-            files = {f:treename for f in filename}
-            if conversion_mode == ConversionMode.REMOVE_NON_STANDARD_TYPE:
-                filter_typename = list(uproot_datatypes)
-            else:
-                filter_typename = None
-            result = None
-            for batch in uproot.iterate(files, expressions=columns,
-                                        filter_typename=filter_typename,
-                                        cut=cut, library="pandas"):
-                if result is None:
-                    result = batch
-                else:
-                    result = pd.concat([result, batch])
-    if downcast:
-        downcast_dataframe(result)
+            filter_typename = None
+        result = iterate_uproot(files, columns=columns,
+                                filter_typename=filter_typename,
+                                step_size=step_size,
+                                cut=cut, library='pandas',
+                                iterate=iterate,
+                                downcast=False)
     return result
 
 def root2rdataset(filename:Union[str, List[str], "quickstats.PathManager"], treename:str,
                   observable:Union[str, dict, "ROOT.RooRealVar",
                                    "quickstats.interface.root.RooRealVar"],
                   weight_name:Optional[str]=None,
                   dataset_name:str="obsData"):
```

### Comparing `quickstats-0.6.8.3/quickstats/utils/hep_utils.py` & `quickstats-0.6.8.4/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/utils/io.py` & `quickstats-0.6.8.4/quickstats/utils/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/utils/roofit_utils.py` & `quickstats-0.6.8.4/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/utils/roostats_utils.py` & `quickstats-0.6.8.4/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/utils/root_utils.py` & `quickstats-0.6.8.4/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/utils/string_utils.py` & `quickstats-0.6.8.4/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats/utils/xml_tools.py` & `quickstats-0.6.8.4/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.8.4/quickstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.3
+Version: 0.6.8.4
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.3/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.8.4/quickstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.3/setup.py` & `quickstats-0.6.8.4/setup.py`

 * *Files identical despite different names*

