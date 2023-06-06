# Comparing `tmp/raesl-0.12.1.tar.gz` & `tmp/raesl-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raesl-0.12.1.tar", max compression
+gzip compressed data, was "raesl-0.12.2.tar", max compression
```

## Comparing `raesl-0.12.1.tar` & `raesl-0.12.2.tar`

### file list

```diff
@@ -1,108 +1,107 @@
--rw-r--r--   0        0        0    35400 2023-02-28 12:07:23.463315 raesl-0.12.1/LICENSE.rst
--rw-r--r--   0        0        0     1820 2023-02-28 12:07:23.463315 raesl-0.12.1/README.rst
--rw-r--r--   0        0        0     3000 2023-02-28 12:07:23.465315 raesl-0.12.1/pyproject.toml
--rw-r--r--   0        0        0      155 2023-02-28 12:07:23.465315 raesl-0.12.1/raesl/__init__.py
--rw-r--r--   0        0        0       64 2023-02-28 12:07:23.465315 raesl-0.12.1/raesl/__main__.py
--rw-r--r--   0        0        0      903 2023-02-28 12:07:23.465315 raesl-0.12.1/raesl/cli.py
--rw-r--r--   0        0        0     1307 2023-02-28 12:07:23.465315 raesl-0.12.1/raesl/compile/__init__.py
--rw-r--r--   0        0        0       45 2023-02-28 12:07:23.465315 raesl-0.12.1/raesl/compile/ast/__init__.py
--rw-r--r--   0        0        0    17189 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/comment_storage.py
--rw-r--r--   0        0        0    16232 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/components.py
--rw-r--r--   0        0        0     6405 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/exprs.py
--rw-r--r--   0        0        0     6216 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/nodes.py
--rw-r--r--   0        0        0     1324 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/relations.py
--rw-r--r--   0        0        0    19717 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/specification.py
--rw-r--r--   0        0        0     2829 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/types.py
--rw-r--r--   0        0        0      649 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/ast/verbs.py
--rw-r--r--   0        0        0     3546 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/cli.py
--rw-r--r--   0        0        0    21094 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/diagnostics.py
--rw-r--r--   0        0        0    10311 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/esl_lines.py
--rw-r--r--   0        0        0       54 2023-02-28 12:07:23.466315 raesl-0.12.1/raesl/compile/instantiating/__init__.py
--rw-r--r--   0        0        0    67112 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/instantiating/edge_building.py
--rw-r--r--   0        0        0     1919 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/instantiating/graph_building.py
--rw-r--r--   0        0        0     1903 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/instantiating/graph_data.py
--rw-r--r--   0        0        0    16947 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/instantiating/instantation_graph_structure.yml
--rw-r--r--   0        0        0    29988 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/instantiating/node_building.py
--rw-r--r--   0        0        0     1666 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/machine_files/__init__.py
--rw-r--r--   0        0        0      663 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/machine_files/argument_list.py
--rw-r--r--   0        0        0     8862 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/machine_files/behavior.py
--rw-r--r--   0        0        0     9610 2023-02-28 12:07:23.467315 raesl-0.12.1/raesl/compile/machine_files/builder.py
--rw-r--r--   0        0        0     1191 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/comments.py
--rw-r--r--   0        0        0     1272 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/component_definitions.py
--rw-r--r--   0        0        0     2908 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/component_instances.py
--rw-r--r--   0        0        0     2805 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/designs.py
--rw-r--r--   0        0        0     3962 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/goals.py
--rw-r--r--   0        0        0     1790 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/groups.py
--rw-r--r--   0        0        0     5372 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/machine_parts.py
--rw-r--r--   0        0        0     1422 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/needs.py
--rw-r--r--   0        0        0     1817 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/parameters.py
--rw-r--r--   0        0        0     3072 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/relation_definitions.py
--rw-r--r--   0        0        0     2584 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/relation_instances.py
--rw-r--r--   0        0        0     3728 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/sub_clause.py
--rw-r--r--   0        0        0     4593 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/transforms.py
--rw-r--r--   0        0        0    12155 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/type_defs.py
--rw-r--r--   0        0        0      566 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/typing.py
--rw-r--r--   0        0        0     1726 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/utils.py
--rw-r--r--   0        0        0     1485 2023-02-28 12:07:23.468315 raesl-0.12.1/raesl/compile/machine_files/variables.py
--rw-r--r--   0        0        0     1183 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/machine_files/verb_defs.py
--rw-r--r--   0        0        0    11202 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/parser.py
--rw-r--r--   0        0        0    16395 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/scanner.py
--rw-r--r--   0        0        0     7456 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/state_machine.py
--rw-r--r--   0        0        0       29 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/__init__.py
--rw-r--r--   0        0        0     6601 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/ast_builder.py
--rw-r--r--   0        0        0    12287 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/compdef_behavior_builder.py
--rw-r--r--   0        0        0    18542 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/compdef_builder.py
--rw-r--r--   0        0        0     3523 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/compdef_comment_builder.py
--rw-r--r--   0        0        0     6853 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/compdef_compinst_builder.py
--rw-r--r--   0        0        0     3045 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/compdef_design_builder.py
--rw-r--r--   0        0        0     3885 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/compdef_goal_builder.py
--rw-r--r--   0        0        0     3617 2023-02-28 12:07:23.469315 raesl-0.12.1/raesl/compile/typechecking/compdef_need_builder.py
--rw-r--r--   0        0        0    16768 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/compdef_relinst_builder.py
--rw-r--r--   0        0        0     4451 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/compdef_transform_builder.py
--rw-r--r--   0        0        0     6410 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/compdef_vargroup_builder.py
--rw-r--r--   0        0        0     4031 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/compdef_varparam_builder.py
--rw-r--r--   0        0        0     6804 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/expr_checker.py
--rw-r--r--   0        0        0     8336 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/goal_transform_base.py
--rw-r--r--   0        0        0     6034 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/orderer.py
--rw-r--r--   0        0        0     7514 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/reldef_builder.py
--rw-r--r--   0        0        0    18722 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/type_builder.py
--rw-r--r--   0        0        0     9826 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/type_checker.py
--rw-r--r--   0        0        0     9226 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/utils.py
--rw-r--r--   0        0        0     2184 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/compile/typechecking/verb_builder.py
--rw-r--r--   0        0        0     1577 2023-02-28 12:07:23.470315 raesl-0.12.1/raesl/datasets/__init__.py
--rw-r--r--   0        0        0     2455 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/__init__.py
--rw-r--r--   0        0        0     2543 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/cli.py
--rw-r--r--   0        0        0    14087 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/doc.py
--rw-r--r--   0        0        0     8359 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/lines.py
--rw-r--r--   0        0        0     1472 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/locales/__init__.py
--rw-r--r--   0        0        0     7678 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/locales/en.py
--rw-r--r--   0        0        0    18488 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/locales/nl.py
--rw-r--r--   0        0        0     3806 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/rich.py
--rw-r--r--   0        0        0    18356 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/sections.py
--rw-r--r--   0        0        0     1073 2023-02-28 12:07:23.471315 raesl-0.12.1/raesl/doc/templates/background.pdf
--rw-r--r--   0        0        0    30867 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/doc/templates/eisvogel.latex
--rw-r--r--   0        0        0     4466 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/doc/utils.py
--rw-r--r--   0        0        0     2205 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/excel/__init__.py
--rw-r--r--   0        0        0     1460 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/excel/cli.py
--rw-r--r--   0        0        0     3577 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/excel/defaults.py
--rw-r--r--   0        0        0    18718 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/excel/sheets.py
--rw-r--r--   0        0        0     6565 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/excel/text.py
--rw-r--r--   0        0        0     3418 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/excel/utils.py
--rw-r--r--   0        0        0       79 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/jupyter/__init__.py
--rw-r--r--   0        0        0     2700 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/jupyter/cli.py
--rw-r--r--   0        0        0     3208 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/jupyter/kernel.py
--rw-r--r--   0        0        0      463 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/plot/__init__.py
--rw-r--r--   0        0        0    12639 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/plot/diagrams.py
--rw-r--r--   0        0        0     3834 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/plot/generic.py
--rw-r--r--   0        0        0     2452 2023-02-28 12:07:23.472315 raesl-0.12.1/raesl/plot/matrix.py
--rw-r--r--   0        0        0    16723 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/plot/utils.py
--rw-r--r--   0        0        0    12731 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/plot/view_funcs.py
--rw-r--r--   0        0        0     2474 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/pygments.py
--rw-r--r--   0        0        0      154 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/server/__init__.py
--rw-r--r--   0        0        0      843 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/server/cli.py
--rw-r--r--   0        0        0     2594 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/server/config.py
--rw-r--r--   0        0        0     6131 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/server/server.py
--rw-r--r--   0        0        0     7724 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/types.py
--rw-r--r--   0        0        0     5062 2023-02-28 12:07:23.473316 raesl-0.12.1/raesl/utils.py
--rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 raesl-0.12.1/setup.py
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 raesl-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0    35400 2023-06-06 12:34:20.460014 raesl-0.12.2/LICENSE.rst
+-rw-r--r--   0        0        0     1827 2023-06-06 12:34:20.460014 raesl-0.12.2/README.rst
+-rw-r--r--   0        0        0     3015 2023-06-06 12:34:20.463014 raesl-0.12.2/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/__main__.py
+-rw-r--r--   0        0        0      903 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/cli.py
+-rw-r--r--   0        0        0     1307 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/__init__.py
+-rw-r--r--   0        0        0    17153 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/comment_storage.py
+-rw-r--r--   0        0        0    16196 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/components.py
+-rw-r--r--   0        0        0     6375 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/exprs.py
+-rw-r--r--   0        0        0     6202 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/nodes.py
+-rw-r--r--   0        0        0     1324 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/relations.py
+-rw-r--r--   0        0        0    19201 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/specification.py
+-rw-r--r--   0        0        0     2829 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/types.py
+-rw-r--r--   0        0        0      649 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/verbs.py
+-rw-r--r--   0        0        0     3540 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/cli.py
+-rw-r--r--   0        0        0    20854 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/diagnostics.py
+-rw-r--r--   0        0        0    10311 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/esl_lines.py
+-rw-r--r--   0        0        0       54 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/__init__.py
+-rw-r--r--   0        0        0    63030 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/edge_building.py
+-rw-r--r--   0        0        0     1897 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/graph_building.py
+-rw-r--r--   0        0        0     1903 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/graph_data.py
+-rw-r--r--   0        0        0    16947 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/instantation_graph_structure.yml
+-rw-r--r--   0        0        0    29622 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/node_building.py
+-rw-r--r--   0        0        0     1666 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/argument_list.py
+-rw-r--r--   0        0        0     8794 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/behavior.py
+-rw-r--r--   0        0        0     9514 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/builder.py
+-rw-r--r--   0        0        0     1179 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/comments.py
+-rw-r--r--   0        0        0     1266 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/component_definitions.py
+-rw-r--r--   0        0        0     2896 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/component_instances.py
+-rw-r--r--   0        0        0     2787 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/designs.py
+-rw-r--r--   0        0        0     3938 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/goals.py
+-rw-r--r--   0        0        0     1772 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/groups.py
+-rw-r--r--   0        0        0     5360 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/machine_parts.py
+-rw-r--r--   0        0        0     1416 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/needs.py
+-rw-r--r--   0        0        0     1805 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/parameters.py
+-rw-r--r--   0        0        0     3066 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/relation_definitions.py
+-rw-r--r--   0        0        0     2558 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/relation_instances.py
+-rw-r--r--   0        0        0     3682 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/sub_clause.py
+-rw-r--r--   0        0        0     4531 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/transforms.py
+-rw-r--r--   0        0        0    12065 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/type_defs.py
+-rw-r--r--   0        0        0      566 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/typing.py
+-rw-r--r--   0        0        0     1700 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/machine_files/utils.py
+-rw-r--r--   0        0        0     1473 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/machine_files/variables.py
+-rw-r--r--   0        0        0     1171 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/machine_files/verb_defs.py
+-rw-r--r--   0        0        0    11112 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/parser.py
+-rw-r--r--   0        0        0    16347 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/scanner.py
+-rw-r--r--   0        0        0     7418 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/state_machine.py
+-rw-r--r--   0        0        0       29 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/__init__.py
+-rw-r--r--   0        0        0     6565 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/ast_builder.py
+-rw-r--r--   0        0        0    12213 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_behavior_builder.py
+-rw-r--r--   0        0        0    18324 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_builder.py
+-rw-r--r--   0        0        0     3461 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_comment_builder.py
+-rw-r--r--   0        0        0     6757 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_compinst_builder.py
+-rw-r--r--   0        0        0     3009 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_design_builder.py
+-rw-r--r--   0        0        0     3775 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_goal_builder.py
+-rw-r--r--   0        0        0     3565 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_need_builder.py
+-rw-r--r--   0        0        0    16463 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_relinst_builder.py
+-rw-r--r--   0        0        0     4355 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_transform_builder.py
+-rw-r--r--   0        0        0     6282 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_vargroup_builder.py
+-rw-r--r--   0        0        0     3925 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_varparam_builder.py
+-rw-r--r--   0        0        0     6796 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/expr_checker.py
+-rw-r--r--   0        0        0     8086 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/goal_transform_base.py
+-rw-r--r--   0        0        0     6020 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/orderer.py
+-rw-r--r--   0        0        0     7348 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/reldef_builder.py
+-rw-r--r--   0        0        0    18482 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/type_builder.py
+-rw-r--r--   0        0        0     9826 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/type_checker.py
+-rw-r--r--   0        0        0     9158 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/utils.py
+-rw-r--r--   0        0        0     2184 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/verb_builder.py
+-rw-r--r--   0        0        0     1577 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/datasets/__init__.py
+-rw-r--r--   0        0        0     2455 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/__init__.py
+-rw-r--r--   0        0        0     2523 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/cli.py
+-rw-r--r--   0        0        0    13934 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/doc.py
+-rw-r--r--   0        0        0     8301 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/lines.py
+-rw-r--r--   0        0        0     1456 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/locales/__init__.py
+-rw-r--r--   0        0        0     7442 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/locales/en.py
+-rw-r--r--   0        0        0    17968 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/locales/nl.py
+-rw-r--r--   0        0        0     3710 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/rich.py
+-rw-r--r--   0        0        0    18255 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/sections.py
+-rw-r--r--   0        0        0     1073 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/templates/background.pdf
+-rw-r--r--   0        0        0    31025 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/doc/templates/eisvogel.latex
+-rw-r--r--   0        0        0     4318 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/doc/utils.py
+-rw-r--r--   0        0        0     2169 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/__init__.py
+-rw-r--r--   0        0        0     1454 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/cli.py
+-rw-r--r--   0        0        0     3197 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/defaults.py
+-rw-r--r--   0        0        0    18454 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/sheets.py
+-rw-r--r--   0        0        0     6367 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/text.py
+-rw-r--r--   0        0        0     3380 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/utils.py
+-rw-r--r--   0        0        0       79 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/jupyter/__init__.py
+-rw-r--r--   0        0        0     2700 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/jupyter/cli.py
+-rw-r--r--   0        0        0     3108 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/jupyter/kernel.py
+-rw-r--r--   0        0        0      463 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/__init__.py
+-rw-r--r--   0        0        0    12489 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/diagrams.py
+-rw-r--r--   0        0        0     3834 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/generic.py
+-rw-r--r--   0        0        0     2438 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/matrix.py
+-rw-r--r--   0        0        0    16381 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/plot/utils.py
+-rw-r--r--   0        0        0    12565 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/plot/view_funcs.py
+-rw-r--r--   0        0        0     2474 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/pygments.py
+-rw-r--r--   0        0        0      154 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/__init__.py
+-rw-r--r--   0        0        0      821 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/cli.py
+-rw-r--r--   0        0        0     2594 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/config.py
+-rw-r--r--   0        0        0     6109 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/server.py
+-rw-r--r--   0        0        0     7628 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/types.py
+-rw-r--r--   0        0        0     5030 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/utils.py
+-rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 raesl-0.12.2/PKG-INFO
```

### Comparing `raesl-0.12.1/LICENSE.rst` & `raesl-0.12.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/README.rst` & `raesl-0.12.2/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -8,58 +8,58 @@
 **********
 Quickstart
 **********
 
 Installation
 ============
 
-RaESL can be installed using ``pip install raesl`` for any Python version >=3.9. Or,
-for Poetry managed projects, use ``poetry add raesl`` to add it as a dependency.
+RaESL can be installed using ``pip install raesl[all]`` for any Python version >=3.9. Or,
+for Poetry managed projects, use ``poetry add raesl -E all`` to add it as a dependency.
 
-For RaESL's different subcommands and functionality, the wheel provides extras:
+For RaESL's different subcommands and functionality, the wheel provides extras which you could
+provide instead of the ``all`` used above:
 
-* doc: documentation generation using pandoc, Markdown and optionally LaTeX.
-* jupyter: a Jupyter ESL kernel.
-* pygments: an ESL syntax highlighter for pygments.
-* rich: Rich doc output in the form of Plotly images.
-* server: A language server to parse documents.
+* ``doc``: documentation generation using pandoc, Markdown and optionally LaTeX.
+* ``jupyter``: a Jupyter ESL kernel.
+* ``pygments``: an ESL syntax highlighter for pygments.
+* ``rich``: Rich doc output in the form of Plotly images.
+* ``server``: A language server to parse documents.
 
 
 The default ``compile`` command is always available.
 
 Please refer to the `usage documentation <https://raesl.ratio-case.nl>`_ for more info
 on how to use RaESL.
 
-
 ***************
 Developer guide
 ***************
 
 Python packaging information
 ============================
 
 This project is packaged using `poetry <https://python-poetry.org/>`_. Packaging
 information as well as dependencies are stored in `pyproject.toml <./pyproject.toml>`_.
 
-Installing the project and its development dependencies can be done using ``poetry install``.
-
-
-Invoke tasks
-============
-
-Most elemental maintenance tasks can be accomplished using
-[Invoke](https://www.pyinvoke.org/). After installing using ``poetry install`` and
-enabling the environment using ``poetry shell``, you can run all tasks using ``inv
-[taskname]`` or ``invoke [taskname]``. E.g. ``inv docs`` builds the documentation.
-
+Installing the project and its development dependencies can be done using ``poetry install -E all``.
 
 Versioning
 ==========
 
 This project uses `semantic versioning <https://semver.org>`_. Version increments are
 checked using `Raver <https://raver.ratio-case.nl>`_.
 
-
 Changelog
 =========
 
-Changelog format as described by https://keepachangelog.com/ has been adopted.
+Changelog format as described by https://keepachangelog.com/ has been adopted and can be reviewed
+`on this page <https://raesl.ratio-case.nl/changelog.html>`.
+
+Tests
+=====
+
+Tests can be run using ``poetry run pytest``.
+
+Linting
+=======
+
+Linting config is included in `pyproject.toml <./pyproject.toml>`_ for both Black and Ruff.
```

### Comparing `raesl-0.12.1/pyproject.toml` & `raesl-0.12.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "raesl"
-version = "0.12.1"
+version = "0.12.2"
 description = "Ratio ESL support in Python."
 authors = ["Ratio Innovations B.V. <info@ratio-case.nl>"]
 license = "GPL-3.0-or-later"
 documentation = "https://raesl.ratio-case.nl"
 readme = "README.rst"
-repository = "https://gitlab.com/ratio-case/python/raesl"
-homepage = "https://gitlab.com/ratio-case/python/raesl"
+repository = "https://gitlab.com/ratio-case-os/python/raesl"
+homepage = "https://raesl.ratio-case.nl"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-click = { version = "^8.0.0" }
-click-log = { version = "^0.3.2" }
-numpy = { version = "^1.21.1" }
-openpyxl = { version = "^3.0.8" }
+click = { version = "^8" }
+click-log = { version = "^0.3" }
+numpy = { version = "^1" }
+openpyxl = { version = "^3" }
 graphviz = { version = "^0.17" }
-ragraph = { version = "^1.15.1" }
-sly = { version = "^0.4.0" }
-ipykernel = { version = "^6.4.1", optional = true }
-IPython = { version = "^7.13.0", optional = true }
-ipywidgets = { version = "^7.5", optional = true }
-jupyter_client = { version = "^7.0.6", optional = true }
+ragraph = { version = "^1" }
+sly = { version = "^0.4" }
+ipykernel = { version = "^6", optional = true }
+IPython = { version = "^7", optional = true }
+ipywidgets = { version = "^7", optional = true }
+jupyter_client = { version = "^7", optional = true }
 kaleido = { version = "0.2.1", optional = true }
-notebook = { version = "^6.0.0", optional = true }
-pandoc_fignos = { version = "^2.4.0", optional = true }
-plotly = { version = "^5.0.0", optional = true }
-pluggy = { version = "^1.0.0", optional = true }
-pygls = { version = "^0.11.0", optional = true }
-pypandoc = { version = "^1.4.0", optional = true }
+notebook = { version = "^6", optional = true }
+pandoc_fignos = { version = "^2", optional = true }
+plotly = { version = "^5", optional = true }
+pluggy = { version = "^1", optional = true }
+pygls = { version = "^0.11", optional = true }
+pypandoc = { version = "^1", optional = true }
 
 [tool.poetry.extras]
 doc = ["pandoc_fignos", "pluggy", "pypandoc"]
 jupyter = ["ipykernel", "IPython", "ipywidgets", "jupyter_client", "notebook"]
 pygments = ["pygments"]
 rich = ["plotly", "kaleido"]
 server = ["pygls"]
@@ -53,36 +53,43 @@
     "pygls",
     "pygments",
     "pypandoc",
 ]
 
 [tool.poetry.dev-dependencies]
 black = "*"
-invoke = "^1.7.1"
 jupyterlab = "^3"
-pandas = "^1.4.3"
+pandas = "^1"
 pydata-sphinx-theme = { version = "*" }
 pytest = "*"
 pytest-cov = "*"
 pytest-doctestplus = "*"
 pygments-csv-lexer = { version = "*" }
-raver = { version = "^3.0.1" }
+raver = { version = "^3" }
 Sphinx = { version = "*" }
 sphinx-autoapi = { version = "*" }
 sphinx-copybutton = { version = "*" }
 sphinx-prompt = { version = "*" }
 sphinxcontrib-bibtex = { version = "*" }
 sphinxemoji = { version = "*" }
 
 [tool.poetry.scripts]
 raesl = "raesl.cli:cli"
 
 [tool.black]
-line-length = 88
-target-version = ["py38"]
+line-length = 100
+target-version = ["py39"]
+
+[tool.ruff]
+line-length = 100
+select = [
+  "E",   # pycodestyle
+  "F",   # pyflakes
+]
+target-version = "py39"
 
 [tool.pytest.ini_options]
 addopts = "-s --cov --cov-report xml:./.pytest_cache/coverage.xml --cov-report term-missing --doctest-plus --doctest-rst --basetemp ./tests/.temp"
 testpaths = ["docs", "tests"]
 
 [tool.coverage.run]
 source = [
```

### Comparing `raesl-0.12.1/raesl/cli.py` & `raesl-0.12.2/raesl/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/__init__.py` & `raesl-0.12.2/raesl/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/ast/comment_storage.py` & `raesl-0.12.2/raesl/compile/ast/comment_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,18 +427,15 @@
 
         if elm.doc_tok.offset > element.doc_tok.offset:
             yield element
             element = elm
             continue
 
         assert elm.doc_tok.offset == element.doc_tok.offset
-        if (
-            isinstance(element, DummyElement)
-            and elm.doc_tok.fname == element.doc_tok.fname
-        ):
+        if isinstance(element, DummyElement) and elm.doc_tok.fname == element.doc_tok.fname:
             element = elm  # 'element' is not useful, 'elm' cannot be worse!
             continue
 
     if element is not None:
         yield element
```

### Comparing `raesl-0.12.1/raesl/compile/ast/components.py` & `raesl-0.12.2/raesl/compile/ast/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,17 +144,15 @@
 
     def __repr__(self):
         if self.is_variable:
             kind = "Variable"
         else:
             kind = "Parameter"
         text = "{}[{}, {}, {}]"
-        return text.format(
-            kind, self.name_tok.tok_text, self.type_tok.tok_text, self.is_property
-        )
+        return text.format(kind, self.name_tok.tok_text, self.type_tok.tok_text, self.is_property)
 
 
 class VariableGroup:
     """One variable group in ESL (a named group of variables).
 
     It has no documentation comment, as its only purpose is to enable interfacing
     to child components.
@@ -391,17 +389,15 @@
         self.cases: List[BehaviorCase] = []
         self.default_results: Optional[List[BehaviorResult]] = None
 
 
 class BehaviorCondition:
     """A condition of a case."""
 
-    def __init__(
-        self, name_tok: "Token", comparison: Union["Disjunction", "RelationComparison"]
-    ):
+    def __init__(self, name_tok: "Token", comparison: Union["Disjunction", "RelationComparison"]):
         self.name_tok = name_tok
         self.comparison = comparison
 
 
 class BehaviorResult:
     """A result of a case."""
```

### Comparing `raesl-0.12.1/raesl/compile/ast/exprs.py` & `raesl-0.12.2/raesl/compile/ast/exprs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,15 @@
         assert self.unit is None or self.unit.tok_text not in ("", "[]")
 
     def get_units(self) -> Optional[Set[str]]:
         # Updates self._unit_cache on first call.
         if self._unit_cache is None:
             if self.unit is None:
                 self._unit_cache = set(["-"])
-            elif self.unit.tok_text.startswith("[") and self.unit.tok_text.endswith(
-                "]"
-            ):
+            elif self.unit.tok_text.startswith("[") and self.unit.tok_text.endswith("]"):
                 self._unit_cache = set([self.unit.tok_text[1:-1]])
             else:
                 self._unit_cache = set([self.unit.tok_text])
 
         return self._unit_cache
 
     def __eq__(self, other):
```

### Comparing `raesl-0.12.1/raesl/compile/ast/nodes.py` & `raesl-0.12.2/raesl/compile/ast/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,17 +124,15 @@
         the_type: Type of the variable or parameter.
         child_nodes: Child nodes of the group.
 
     Attributes:
         name_index: Mapping of name to the associated VarNode instance.
     """
 
-    def __init__(
-        self, name_tok: "Token", the_type: "BaseType", child_nodes: List[VarNode]
-    ):
+    def __init__(self, name_tok: "Token", the_type: "BaseType", child_nodes: List[VarNode]):
         super(CompoundVarNode, self).__init__(name_tok, the_type)
         self.child_nodes = child_nodes
         self.name_index = dict((cn.name_tok.tok_text, cn) for cn in child_nodes)
 
         assert isinstance(self.child_nodes, list)
 
         # Bundle doesn't have duplicate child names.
```

### Comparing `raesl-0.12.1/raesl/compile/ast/relations.py` & `raesl-0.12.2/raesl/compile/ast/relations.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/ast/specification.py` & `raesl-0.12.2/raesl/compile/ast/specification.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,24 @@
         self.world: Optional[components.ComponentDefinition] = None
 
 
 class _DumpSpec:
     """Class for dumping the specification to an output stream."""
 
     def __init__(self, output_stream: Optional[TextIO] = None):
-        self.stream = (
-            click.get_text_stream("stdout") if output_stream is None else output_stream
-        )
+        self.stream = click.get_text_stream("stdout") if output_stream is None else output_stream
         self.done_types: Dict[types.BaseType, int] = {}
 
     def dump(self, spec: Specification):
         """Write the specification symbolically onto the output stream. Intended use is
         verifying content or debugging.
         """
         self.stream.write("\nTYPES:\n")
         if spec.types:
-            text_tdefs = [
-                (tdef.name, self._dump_type(tdef.type)) for tdef in spec.types.values()
-            ]
+            text_tdefs = [(tdef.name, self._dump_type(tdef.type)) for tdef in spec.types.values()]
             self.stream.write("\n")
             for name, tname in text_tdefs:
                 self.stream.write("typedef {}: {}\n".format(name.tok_text, tname))
 
         self.stream.write("\nVERBS:\n")
         for verbdef in spec.verb_prepos:
             self.stream.write("    {}\n".format(verbdef))
@@ -63,17 +59,15 @@
         self.stream.write("\nRELATION-DEFINITIONS:\n")
         for rel_def in spec.rel_defs:
             self.stream.write("    def {}:\n".format(rel_def.name.tok_text))
             self._dump_docs(rel_def, "    ")
             for param in rel_def.params:
                 tnumber = self.done_types[param.type]
                 param_type = "type#{}".format(tnumber)
-                text = "{} {}: {}".format(
-                    param.direction, param.name.tok_text, param_type
-                )
+                text = "{} {}: {}".format(param.direction, param.name.tok_text, param_type)
                 if param.multi:
                     text = "multi " + text
 
                 self.stream.write("        {}\n".format(text))
 
         self.stream.write("\nCOMPONENTS:\n")
         if spec.world is not None:
@@ -92,51 +86,43 @@
             name = compdef.name_tok.tok_text
             self.stream.write("    def component {}:\n".format(name))
         self._dump_docs(compdef, "    ")
 
         # Dump variables of a component definition.
         leading = "        "
         for vdef in compdef.variables:
-            self.stream.write(
-                "{}var {}\n{}  ".format(leading, vdef.name_tok.tok_text, leading)
-            )
+            self.stream.write("{}var {}\n{}  ".format(leading, vdef.name_tok.tok_text, leading))
             self._dump_nodes(vdef.node, prefixes=[leading + "  "])
 
         # Dump parameters of a component definition.
         for pdef in compdef.parameters:
             prop_text = {False: "", True: ": property"}[pdef.is_property]
             text = "param {}{}".format(pdef.name_tok.tok_text, prop_text)
             self.stream.write(leading + text + "\n  " + leading)
             self._dump_nodes(pdef.node, prefixes=[leading + "  "])
 
         # Dump variable groups of a component definition.
         for vgroup in compdef.var_groups:
-            content = ", ".join(
-                varpart.tok_text for varpart in vgroup.variablepart_names
-            )
+            content = ", ".join(varpart.tok_text for varpart in vgroup.variablepart_names)
             text = "vgroup {}: {}".format(vgroup.name_tok.tok_text, content)
             self.stream.write(leading + text + "\n  " + leading)
             self._dump_nodes(vgroup.node, prefixes=[leading + "  "])
 
         # Dump component instances of a component definition.
         for compinst in compdef.component_instances:
             def_name = compinst.compdef.name_tok.tok_text
-            text = "child-component {}: def={}".format(
-                compinst.inst_name_tok.tok_text, def_name
-            )
+            text = "child-component {}: def={}".format(compinst.inst_name_tok.tok_text, def_name)
             self.stream.write("        " + text + "\n")
             self._dump_docs(compinst, "        ")
             self._dump_compinst_params(compinst)
 
         # Dump relation instances of a component definition.
         for relinst in compdef.relations:
             def_name = relinst.reldef.name.tok_text
-            text = "relation-instance {}: def={}".format(
-                relinst.inst_name_tok.tok_text, def_name
-            )
+            text = "relation-instance {}: def={}".format(relinst.inst_name_tok.tok_text, def_name)
             self.stream.write("        " + text + "\n")
             self._dump_docs(relinst, "        ")
             self._dump_relinst_params(relinst)
 
         # Dump goals
         leading = "        "
         for goal in compdef.goals:
@@ -158,38 +144,32 @@
                 self.stream.write(indent + "  ")
                 self._dump_nodes(f.flow_node, prefixes=[indent + "  "])
 
             self._dump_subclauses(goal.sub_clauses)
 
         # Dump transformations
         for trans in compdef.transforms:
-            name = "{} transform {}:".format(
-                trans.transform_kind, trans.label_tok.tok_text
-            )
+            name = "{} transform {}:".format(trans.transform_kind, trans.label_tok.tok_text)
             comptext = "  {} ({} {})"
             comptext = comptext.format(
                 trans.doesaux_tok.tok_text,
                 trans.verb_tok.tok_text,
                 trans.prepos_tok.tok_text,
             )
 
             indent = "        "
             self.stream.write(indent + name + "\n")
             self._dump_docs(trans, indent)
             self.stream.write(indent + comptext + "\n")
             for f in trans.in_flows:
-                self.stream.write(
-                    indent + "  in-flow '{}':\n".format(f.name_tok.tok_text)
-                )
+                self.stream.write(indent + "  in-flow '{}':\n".format(f.name_tok.tok_text))
                 self.stream.write(indent + "  ")
                 self._dump_nodes(f.flow_node, prefixes=[indent + "  "])
             for f in trans.out_flows:
-                self.stream.write(
-                    indent + "  out-flow '{}':\n".format(f.name_tok.tok_text)
-                )
+                self.stream.write(indent + "  out-flow '{}':\n".format(f.name_tok.tok_text))
                 self.stream.write(indent + "  ")
                 self._dump_nodes(f.flow_node, prefixes=[indent + "  "])
             self._dump_subclauses(trans.sub_clauses)
 
         # Dump needs
         for need in compdef.needs:
             if need.subject is None:
@@ -209,17 +189,15 @@
             self.stream.write(indent + name + "\n")
             self._dump_docs(design, indent)
             self._dump_expr(design.expr, indent + "    ")
             self._dump_subclauses(design.sub_clauses)
 
         # Dump behavior
         for behavior in compdef.behaviors:
-            name = "{} behavior {}:".format(
-                behavior.behavior_kind, behavior.name_tok.tok_text
-            )
+            name = "{} behavior {}:".format(behavior.behavior_kind, behavior.name_tok.tok_text)
             self.stream.write("        " + name + "\n")
             self._dump_docs(behavior, "        ")
             for case in behavior.cases:
                 self.stream.write("            case " + case.name_tok.tok_text + ":\n")
                 self._dump_conds(case.conditions)
                 self._dump_results(case.results)
             if behavior.default_results is None:
@@ -237,17 +215,15 @@
             else:
                 self.stream.write("{}or ".format(indent))
 
             if isinstance(ex, exprs.RelationComparison):
                 # Construct text and node for RHS
                 rv = ex.rhs_varval
                 if isinstance(rv, Value):
-                    rhs_text = "{}[{}]".format(
-                        rv.value.tok_text, next(iter(rv.get_units()))
-                    )
+                    rhs_text = "{}[{}]".format(rv.value.tok_text, next(iter(rv.get_units())))
                     rhs_node = None
                 else:
                     assert isinstance(rv, VariableValue)
                     rhs_text = rv.var_tok.tok_text
                     rhs_node = rv.var_node
 
                 text = "{} {} {} {}".format(
@@ -363,48 +339,42 @@
 
         if isinstance(btp, types.Compound):
             indent = "    "
 
             type_names = [self._dump_type(field.type) for field in btp.fields]
             self.stream.write("{} = bundle\n".format(my_typename))
             for field, tname in zip(btp.fields, type_names):
-                self.stream.write(
-                    indent + "{}: {}\n".format(field.name.tok_text, tname)
-                )
+                self.stream.write(indent + "{}: {}\n".format(field.name.tok_text, tname))
             self.stream.write("{} end\n".format(my_typename))
             self.stream.write("\n")
 
         else:
             assert isinstance(btp, types.ElementaryType)
             if btp.parent is not None:
                 parent_name = self._dump_type(btp.parent)
                 self.stream.write("{} = type <-- {}\n".format(my_typename, parent_name))
             else:
                 self.stream.write("{} = type\n".format(my_typename))
 
             if btp.units:
-                self.stream.write(
-                    "    units: " + ", ".join(u.tok_text for u in btp.units) + "\n"
-                )
+                self.stream.write("    units: " + ", ".join(u.tok_text for u in btp.units) + "\n")
 
             if btp.intervals:
                 prefix = "    intervals: "
                 for ival in btp.intervals:
                     if ival[0] is None:
                         lbound = "*"
                     else:
                         lbound = str(ival[0])
                     if ival[1] is None:
                         ubound = "*"
                     else:
                         ubound = str(ival[1])
 
-                    self.stream.write(
-                        prefix + "(=> {}, <= {})\n".format(lbound, ubound)
-                    )
+                    self.stream.write(prefix + "(=> {}, <= {})\n".format(lbound, ubound))
                     prefix = " " * len(prefix)
 
         return my_typename
 
     def _dump_compinst_params(self, compinst):
         """Dump the arguments of the component instance."""
         if not compinst.arguments:
```

### Comparing `raesl-0.12.1/raesl/compile/ast/types.py` & `raesl-0.12.2/raesl/compile/ast/types.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/ast/verbs.py` & `raesl-0.12.2/raesl/compile/ast/verbs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/cli.py` & `raesl-0.12.2/raesl/compile/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,15 @@
 
         to_json(graph, path=out_file)
 
     return diag_store, spec, graph
 
 
 @click.command("compile")
-@click.argument(
-    "paths", nargs=-1, type=click.Path(exists=True, file_okay=True, dir_okay=True)
-)
+@click.argument("paths", nargs=-1, type=click.Path(exists=True, file_okay=True, dir_okay=True))
 @click.option(
     "--output",
     "-o",
     default=None,
     type=click.Path(file_okay=True, dir_okay=False),
     help="Graph output file.",
 )
```

### Comparing `raesl-0.12.1/raesl/compile/diagnostics.py` & `raesl-0.12.2/raesl/compile/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,15 @@
         location=location,
         severity=ERROR,
         code="E100",
         source="ESL parser",
     )
 
 
-def E101(
-    acceptors: Iterable[str], location: Location = utils.get_location()
-) -> EslDiagnostic:
+def E101(acceptors: Iterable[str], location: Location = utils.get_location()) -> EslDiagnostic:
     """Best line match is ambiguous. Found multiple acceptors: {ambi_acceptors}. This
     is an internal error.
     """
     enum = "', '".join(acceptors)
     return EslDiagnostic(
         (
             f"Best line match is ambiguous. Found multiple acceptors: '{enum}'. "
@@ -203,23 +201,19 @@
     dupes = [] if dupes is None else dupes
     return EslDiagnostic(
         f"Multiple {kind}s named '{name}'.",
         location=location,
         severity=ERROR,
         code="E200",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(dupe, f"Duplicate {kind} '{name}'.") for dupe in dupes
-        ],
+        related_information=[EslRelated(dupe, f"Duplicate {kind} '{name}'.") for dupe in dupes],
     )
 
 
-def E201(
-    section: str, context: str, location: Location = utils.get_location()
-) -> EslDiagnostic:
+def E201(section: str, context: str, location: Location = utils.get_location()) -> EslDiagnostic:
     """This '{section}' section is not allowed in the '{context}' context."""
     return EslDiagnostic(
         f"This '{section}' section is not allowed in the '{context}' context.",
         location=location,
         severity=ERROR,
         code="E201",
         source="ESL typechecker",
@@ -279,17 +273,15 @@
         source="ESL typechecker",
         related_information=[
             EslRelated(entry, f"Cycle {i+1}/{length}.") for i, entry in enumerate(cycle)
         ],
     )
 
 
-def E205(
-    name: str, context: str, location: Location = utils.get_location()
-) -> EslDiagnostic:
+def E205(name: str, context: str, location: Location = utils.get_location()) -> EslDiagnostic:
     """Cannot find {name} in {context}."""
     return EslDiagnostic(
         f"Cannot find {name} in {context}.",
         location=location,
         severity=ERROR,
         code="E205",
         source="ESL typechecker",
@@ -311,17 +303,15 @@
             f"Found {kind} block(s), "
             + f"but the relation definition {name} has no such parameters."
         ),
         location=location,
         severity=ERROR,
         code="E206",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(block, f"Relation {kind} block") for block in blocks
-        ],
+        related_information=[EslRelated(block, f"Relation {kind} block") for block in blocks],
     )
 
 
 def E207(
     name: str,
     kind: str,
     location: Location = utils.get_location(),
@@ -330,17 +320,15 @@
     """Relation instance '{name}' is missing a '{kind}' parameters section."""
     return EslDiagnostic(
         f"Relation instance '{name}' is missing a '{kind}' parameters section.",
         location=location,
         severity=ERROR,
         code="E207",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(definition, "Corresponding relation definition.")
-        ],
+        related_information=[EslRelated(definition, "Corresponding relation definition.")],
     )
 
 
 def E208(
     name: str,
     kind: str,
     num: int,
@@ -350,17 +338,15 @@
     """Relation instance '{name}' is missing at least {num} '{kind}' parameters."""
     return EslDiagnostic(
         f"Relation instance '{name}' is missing at least {num} '{kind}' parameters.",
         location=location,
         severity=ERROR,
         code="E208",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(definition, "Corresponding relation definition.")
-        ],
+        related_information=[EslRelated(definition, "Corresponding relation definition.")],
     )
 
 
 def E209(
     name: str,
     kind: str,
     other_kind: str,
@@ -371,23 +357,19 @@
     others = [] if others is None else others
     return EslDiagnostic(
         f"'{name}' is both a {kind} and a {other_kind}.",
         location=location,
         severity=ERROR,
         code="E209",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(other, f"{other_kind} location.") for other in others
-        ],
+        related_information=[EslRelated(other, f"{other_kind} location.") for other in others],
     )
 
 
-def E210(
-    lhs: Location, rhs: Location, reason: str = "are not compatible"
-) -> EslDiagnostic:
+def E210(lhs: Location, rhs: Location, reason: str = "are not compatible") -> EslDiagnostic:
     """Values cannot be compared, they {reason}."""
     return EslDiagnostic(
         f"Values cannot be compared, they {reason}.",
         location=lhs,
         severity=ERROR,
         code="E210",
         source="ESL typechecker",
@@ -442,17 +424,15 @@
     occurrences = [] if occurrences is None else occurrences
     return EslDiagnostic(
         f"Found {num} {kind}(s), but there should be {allowed}.",
         location=location,
         severity=ERROR,
         code="E213",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(occ, f"{kind.capitalize()}") for occ in occurrences
-        ],
+        related_information=[EslRelated(occ, f"{kind.capitalize()}") for occ in occurrences],
     )
 
 
 def E214(
     name: str,
     location: Location = utils.get_location(),
     def_location: Optional[Location] = None,
@@ -461,17 +441,15 @@
     def_locs = [] if def_location is None else [def_location]
     return EslDiagnostic(
         f"Definition of type '{name}' failed with an error.",
         location=location,
         severity=ERROR,
         code="E214",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(loc, "Related type definition.") for loc in def_locs
-        ],
+        related_information=[EslRelated(loc, "Related type definition.") for loc in def_locs],
     )
 
 
 def E215(
     name: str,
     location: Location = utils.get_location(),
 ) -> EslDiagnostic:
@@ -530,17 +508,15 @@
         location=location,
         severity=ERROR,
         code="E219",
         source="ESL typechecker",
     )
 
 
-def E220(
-    name: str, kind: str, location: Location = utils.get_location()
-) -> EslDiagnostic:
+def E220(name: str, kind: str, location: Location = utils.get_location()) -> EslDiagnostic:
     """Element '{name}' does not match with a {kind}."""
     return EslDiagnostic(
         f"Element '{name}' does not match with a {kind}.",
         location=location,
         severity=ERROR,
         code="E220",
         source="ESL typechecker",
@@ -559,16 +535,15 @@
     return EslDiagnostic(
         f"Number of {kind}s does not match. Found {num}, expected {expected}.",
         location=location,
         severity=ERROR,
         code="E221",
         source="ESL typechecker",
         related_information=[
-            EslRelated(ref, f"Reference with {expected} {kind}(s).")
-            for ref in references
+            EslRelated(ref, f"Reference with {expected} {kind}(s).") for ref in references
         ],
     )
 
 
 def E222(
     name: str,
     other: str,
@@ -643,17 +618,15 @@
     """Need '{name}' is not allowed to reference a bundle."""
     return EslDiagnostic(
         f"Need '{name}' is not allowed to reference a bundle.",
         location=location,
         severity=ERROR,
         code="E226",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(location, "Only elementary variables, try its fields.")
-        ],
+        related_information=[EslRelated(location, "Only elementary variables, try its fields.")],
     )
 
 
 def E227(
     name: str,
     scope: str,
     location: Location = utils.get_location(),
@@ -663,17 +636,15 @@
     dupes = [] if dupes is None else dupes
     return EslDiagnostic(
         f"Duplicate identifier '{name}' within the scope of '{scope}'.",
         location=location,
         severity=ERROR,
         code="E200",
         source="ESL typechecker",
-        related_information=[
-            EslRelated(dupe, f"Duplicate identifier '{name}'.") for dupe in dupes
-        ],
+        related_information=[EslRelated(dupe, f"Duplicate identifier '{name}'.") for dupe in dupes],
     )
 
 
 def E400(
     name: str,
     location: Location = utils.get_location(),
     owners: Optional[List[Location]] = None,
```

### Comparing `raesl-0.12.1/raesl/compile/esl_lines.py` & `raesl-0.12.2/raesl/compile/esl_lines.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/instantiating/edge_building.py` & `raesl-0.12.2/raesl/compile/instantiating/edge_building.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,15 @@
         diag_store: diagnostics.DiagnosticStore,
         node_store: Optional[NodeStore] = None,
     ):
         self.diag_store = diag_store
         self.node_store = node_store
 
         # Set categories dynamically.
-        EdgeStore.categories = ["edges"] + [
-            i[6:] for i in dir(self) if i.startswith("_make_")
-        ]
+        EdgeStore.categories = ["edges"] + [i[6:] for i in dir(self) if i.startswith("_make_")]
         self.edge_store = EdgeStore()
 
     def _add(self, edge: Edge, *args):
         """Proxy for :obj:`EdgeStore.add`."""
         self.edge_store.add(edge, *args)
 
     def _consume(self, edges: Iterable[Edge], *args):
@@ -107,17 +105,15 @@
                     self._add(
                         Edge(
                             source=nodes[vi],
                             target=nodes[vj],
                             kind="functional_dependency",
                             labels=[nodes[vi].annotations.esl_info["type_ref"]],
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(function_specifications=[t.name])
-                                )
+                                esl_info=dict(reason=dict(function_specifications=[t.name]))
                             ),
                         ),
                         "evf",
                     )
 
     def _make_evb(self):
         """Compute logical dependencies between variables for behavior specs."""
@@ -189,17 +185,15 @@
                     self._add(
                         Edge(
                             source=nodes[vi],
                             target=nodes[vj],
                             kind="design_dependency",
                             labels=[nodes[vi].annotations.esl_info["type_ref"]],
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(relation_specifications=[r.name])
-                                )
+                                esl_info=dict(reason=dict(relation_specifications=[r.name]))
                             ),
                         ),
                         "evd",
                     )
 
     def _make_ecf(self):
         """Compute function dependencies between component nodes."""
@@ -222,30 +216,26 @@
 
             self._add(
                 Edge(
                     source=src,
                     target=trg,
                     kind="functional_dependency",
                     labels=lbs,
-                    annotations=dict(
-                        esl_info=dict(reason=dict(function_specifications=[g.name]))
-                    ),
+                    annotations=dict(esl_info=dict(reason=dict(function_specifications=[g.name]))),
                 ),
                 "ecf",
             )
 
             self._add(
                 Edge(
                     source=trg,
                     target=src,
                     kind="functional_dependency",
                     labels=lbs,
-                    annotations=dict(
-                        esl_info=dict(reason=dict(function_specifications=[g.name]))
-                    ),
+                    annotations=dict(esl_info=dict(reason=dict(function_specifications=[g.name]))),
                 ),
                 "ecf",
             )
 
             gvars = set(g.annotations.esl_info["body"]["variables"])
             for c in src.descendants:
                 for t in nt_dict[c.name]:
@@ -259,36 +249,28 @@
                     self._add(
                         Edge(
                             source=c,
                             target=trg,
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[g.name, t.name]
-                                    )
-                                )
+                                esl_info=dict(reason=dict(function_specifications=[g.name, t.name]))
                             ),
                         ),
                         "ecf",
                     )
 
                     self._add(
                         Edge(
                             source=trg,
                             target=c,
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[g.name, t.name]
-                                    )
-                                )
+                                esl_info=dict(reason=dict(function_specifications=[g.name, t.name]))
                             ),
                         ),
                         "ecf",
                     )
 
             for c in trg.descendants:
                 for t in nt_dict[c.name]:
@@ -302,36 +284,28 @@
                     self._add(
                         Edge(
                             source=src,
                             target=c,
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[t.name, g.name]
-                                    )
-                                )
+                                esl_info=dict(reason=dict(function_specifications=[t.name, g.name]))
                             ),
                         ),
                         "ecf",
                     )
 
                     self._add(
                         Edge(
                             source=c,
                             target=src,
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[t.name, g.name]
-                                    )
-                                )
+                                esl_info=dict(reason=dict(function_specifications=[t.name, g.name]))
                             ),
                         ),
                         "ecf",
                     )
 
         for ti in transforms:
             for tj in transforms:
@@ -345,85 +319,71 @@
                 ti_out_vars = set(ti.annotations.esl_info["body"]["output_variables"])
                 tj_in_vars = set(tj.annotations.esl_info["body"]["input_variables"])
                 tj_out_vars = set(tj.annotations.esl_info["body"]["output_variables"])
                 shared_vars_ij = ti_out_vars.intersection(tj_in_vars)
                 shared_vars_ji = tj_out_vars.intersection(ti_in_vars)
 
                 if shared_vars_ij:
-                    lbs = [
-                        nodes[v].annotations.esl_info["type_ref"]
-                        for v in shared_vars_ij
-                    ]
+                    lbs = [nodes[v].annotations.esl_info["type_ref"] for v in shared_vars_ij]
                     self._add(
                         Edge(
                             source=nodes[ci],
                             target=nodes[cj],
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
                                 esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[ti.name, tj.name]
-                                    )
+                                    reason=dict(function_specifications=[ti.name, tj.name])
                                 )
                             ),
                         ),
                         "ecf",
                     )
 
                     self._add(
                         Edge(
                             source=nodes[cj],
                             target=nodes[ci],
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
                                 esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[ti.name, tj.name]
-                                    )
+                                    reason=dict(function_specifications=[ti.name, tj.name])
                                 )
                             ),
                         ),
                         "ecf",
                     )
 
                 if shared_vars_ji:
-                    lbs = [
-                        nodes[v].annotations.esl_info["type_ref"]
-                        for v in shared_vars_ji
-                    ]
+                    lbs = [nodes[v].annotations.esl_info["type_ref"] for v in shared_vars_ji]
                     self._add(
                         Edge(
                             source=nodes[cj],
                             target=nodes[ci],
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
                                 esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[tj.name, ti.name]
-                                    )
+                                    reason=dict(function_specifications=[tj.name, ti.name])
                                 )
                             ),
                         ),
                         "ecf",
                     )
 
                     self._add(
                         Edge(
                             source=nodes[ci],
                             target=nodes[cj],
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
                                 esl_info=dict(
-                                    reason=dict(
-                                        function_specifications=[tj.name, ti.name]
-                                    )
+                                    reason=dict(function_specifications=[tj.name, ti.name])
                                 )
                             ),
                         ),
                         "ecf",
                     )
 
     def _make_ecb(self):
@@ -478,22 +438,20 @@
                                 if ai == aj:
                                     continue
                                 self._add(
                                     Edge(
                                         source=ai,
                                         target=aj,
                                         kind="design_dependency",
-                                        labels=[
-                                            nodes[pi].annotations.esl_info["type_ref"]
-                                        ],
+                                        labels=[nodes[pi].annotations.esl_info["type_ref"]],
                                         annotations=dict(
                                             esl_info=dict(
-                                                reason=e_dict[
-                                                    (pi, pj)
-                                                ].annotations.esl_info["reason"]
+                                                reason=e_dict[(pi, pj)].annotations.esl_info[
+                                                    "reason"
+                                                ]
                                             )
                                         ),
                                     ),
                                     "ecd",
                                 )
 
     def _make_eft(self):
@@ -529,28 +487,22 @@
                         evf_c.append(
                             Edge(
                                 source=nodes[vi],
                                 target=nodes[vj],
                                 kind="functional_dependency",
                                 labels=[nodes[vi].annotations.esl_info["type_ref"]],
                                 annotations=dict(
-                                    esl_info=dict(
-                                        reason=dict(function_specifications=[t.name])
-                                    )
+                                    esl_info=dict(reason=dict(function_specifications=[t.name]))
                                 ),
                             )
                         )
 
             for t in ctd[c.name]:
-                srcs = [
-                    nodes[v] for v in t.annotations.esl_info["body"]["input_variables"]
-                ]
-                trgs = [
-                    nodes[v] for v in t.annotations.esl_info["body"]["output_variables"]
-                ]
+                srcs = [nodes[v] for v in t.annotations.esl_info["body"]["input_variables"]]
+                trgs = [nodes[v] for v in t.annotations.esl_info["body"]["output_variables"]]
 
                 paths = _get_paths_between_all(srcs=srcs, trgs=set(trgs), edges=evf_c)
 
                 pathvars = set()
                 for path in paths:
                     pathvars.update(set(path))
 
@@ -562,17 +514,15 @@
                         self._add(
                             Edge(
                                 source=t,
                                 target=child_t,
                                 kind="traceability_dependency",
                                 annotations=dict(
                                     esl_info=dict(
-                                        reason=dict(
-                                            path_variables=list(shared_path_variables)
-                                        )
+                                        reason=dict(path_variables=list(shared_path_variables))
                                     )
                                 ),
                             ),
                             "eft",
                         )
 
                 for child_g in child_gs:
@@ -583,17 +533,15 @@
                         self._add(
                             Edge(
                                 source=t,
                                 target=child_g,
                                 kind="traceability_dependency",
                                 annotations=dict(
                                     esl_info=dict(
-                                        reason=dict(
-                                            path_variables=list(shared_path_variables)
-                                        )
+                                        reason=dict(path_variables=list(shared_path_variables))
                                     )
                                 ),
                             ),
                             "eft",
                         )
 
     def _make_eff(self):
@@ -634,46 +582,38 @@
             for g in gls:
                 tvin = set(t1.annotations.esl_info["body"]["input_variables"])
                 tvout = set(t1.annotations.esl_info["body"]["output_variables"])
                 gv = set(g.annotations.esl_info["body"]["variables"])
 
                 vin_shared = tvin.intersection(gv)
                 if vin_shared:
-                    lbs = [
-                        nodes[v].annotations.esl_info["type_ref"] for v in vin_shared
-                    ]
+                    lbs = [nodes[v].annotations.esl_info["type_ref"] for v in vin_shared]
                     self._add(
                         Edge(
                             source=g,
                             target=t1,
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(shared_variables=list(vin_shared))
-                                )
+                                esl_info=dict(reason=dict(shared_variables=list(vin_shared)))
                             ),
                         ),
                         "eff",
                     )
                 vout_shared = tvout.intersection(gv)
                 if vout_shared:
-                    lbs = [
-                        nodes[v].annotations.esl_info["type_ref"] for v in vout_shared
-                    ]
+                    lbs = [nodes[v].annotations.esl_info["type_ref"] for v in vout_shared]
                     self._add(
                         Edge(
                             source=t1,
                             target=g,
                             kind="functional_dependency",
                             labels=lbs,
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(shared_variables=list(vout_shared))
-                                )
+                                esl_info=dict(reason=dict(shared_variables=list(vout_shared)))
                             ),
                         ),
                         "eff",
                     )
 
     def _make_efb(self):
         """Compute behavior dependencies between goal- and transformation specs."""
@@ -748,17 +688,15 @@
                     Edge(
                         source=bi,
                         target=bj,
                         kind="logical_dependency",
                         labels=lbs,
                         annotations=dict(
                             esl_info=dict(
-                                reason=dict(
-                                    shared_variables=[v.name for v in shared_vars]
-                                )
+                                reason=dict(shared_variables=[v.name for v in shared_vars])
                             )
                         ),
                     ),
                     "ehb",
                 )
 
     def _make_ehc(self):
@@ -790,17 +728,15 @@
                     Edge(
                         source=bi,
                         target=bj,
                         kind="coordination_dependency",
                         labels=lbs,
                         annotations=dict(
                             esl_info=dict(
-                                reason=dict(
-                                    shared_variables=[v.name for v in shared_vars]
-                                )
+                                reason=dict(shared_variables=[v.name for v in shared_vars])
                             )
                         ),
                     ),
                     "ehc",
                 )
 
     def _make_edc(self):
@@ -824,53 +760,44 @@
                     continue
 
                 self._add(
                     Edge(
                         source=di,
                         target=dj,
                         kind="coordination_dependency",
-                        labels=[
-                            v.annotations.esl_info["type_ref"] for v in shared_vars
-                        ],
+                        labels=[v.annotations.esl_info["type_ref"] for v in shared_vars],
                         annotations=dict(
                             esl_info=dict(
-                                reason=(
-                                    dict(shared_variables=[v.name for v in shared_vars])
-                                )
+                                reason=(dict(shared_variables=[v.name for v in shared_vars]))
                             )
                         ),
                     ),
                     "edc",
                 )
 
     def _make_enc(self):
         """Create coordination dependencies between needs."""
         nds = self.node_store.needs.values()
         for ni in nds:
             for nj in nds:
                 if ni == nj:
                     continue
 
-                if (
-                    not ni.annotations.esl_info["subject"]
-                    == nj.annotations.esl_info["subject"]
-                ):
+                if not ni.annotations.esl_info["subject"] == nj.annotations.esl_info["subject"]:
                     continue
 
                 self._add(
                     Edge(
                         source=ni,
                         target=nj,
                         kind="mapping_dependency",
                         labels=["shared subject"],
                         annotations=dict(
                             esl_info=dict(
-                                reason=dict(
-                                    shared_subject=ni.annotations.esl_info["subject"]
-                                )
+                                reason=dict(shared_subject=ni.annotations.esl_info["subject"])
                             )
                         ),
                     ),
                     "enc",
                 )
 
     def _make_erc(self):
@@ -898,21 +825,16 @@
                     continue
 
                 self._add(
                     Edge(
                         source=ri,
                         target=rj,
                         kind="coordination_dependency",
-                        labels=[
-                            nodes[v].annotations.esl_info["type_ref"]
-                            for v in shared_vars
-                        ],
-                        annotations=dict(
-                            esl_info=dict(reason=dict(shared_vars=list(shared_vars)))
-                        ),
+                        labels=[nodes[v].annotations.esl_info["type_ref"] for v in shared_vars],
+                        annotations=dict(esl_info=dict(reason=dict(shared_vars=list(shared_vars)))),
                     ),
                     "erc",
                 )
 
     def _make_mcf(self):
         """Compute mapping relations between components and functions."""
         nodes = self.node_store.nodes
@@ -941,63 +863,51 @@
 
         for g in gls:
             gvs = set([nodes[v] for v in g.annotations.esl_info["body"]["variables"]])
             lbs = [v.annotations.esl_info["type_ref"] for v in gvs]
             a = n2c[g.annotations.esl_info["body"]["active"]]
             p = n2c[g.annotations.esl_info["body"]["passive"]]
 
-            self._add(
-                Edge(source=a, target=g, labels=lbs, kind="mapping_dependency"), "mcf"
-            )
-            self._add(
-                Edge(source=p, target=g, labels=lbs, kind="mapping_dependency"), "mcf"
-            )
+            self._add(Edge(source=a, target=g, labels=lbs, kind="mapping_dependency"), "mcf")
+            self._add(Edge(source=p, target=g, labels=lbs, kind="mapping_dependency"), "mcf")
 
             for d in a.descendants:
                 if not ctd.get(d):
                     continue
 
                 for t in ctd[d]:
                     outvars = set(
-                        nodes[v]
-                        for v in t.annotations.esl_info["body"]["output_variables"]
+                        nodes[v] for v in t.annotations.esl_info["body"]["output_variables"]
                     )
                     shared_vars = outvars.intersection(gvs)
 
                     if shared_vars:
                         self._add(
                             Edge(
                                 source=d,
                                 target=g,
-                                labels=[
-                                    v.annotations.esl_info["type_ref"]
-                                    for v in shared_vars
-                                ],
+                                labels=[v.annotations.esl_info["type_ref"] for v in shared_vars],
                                 kind="mapping_dependency",
                             ),
                             "mcf",
                         )
 
             for d in p.descendants:
                 for t in ctd[d]:
                     invars = set(
-                        nodes[v]
-                        for v in t.annotations.esl_info["body"]["input_variables"]
+                        nodes[v] for v in t.annotations.esl_info["body"]["input_variables"]
                     )
                     shared_vars = invars.intersection(gvs)
 
                     if shared_vars:
                         self._add(
                             Edge(
                                 source=d,
                                 target=g,
-                                labels=[
-                                    v.annotations.esl_info["type_ref"]
-                                    for v in shared_vars
-                                ],
+                                labels=[v.annotations.esl_info["type_ref"] for v in shared_vars],
                                 kind="mapping_dependency",
                             ),
                             "mcf",
                         )
 
     def _make_mcv(self):
         """Create mapping relations between components and variables."""
@@ -1173,22 +1083,18 @@
                         continue
 
                     self._add(
                         Edge(
                             source=c,
                             target=d,
                             kind="mapping_dependency",
-                            labels=[
-                                v.annotations.esl_info["type_ref"] for v in shared_vars
-                            ],
+                            labels=[v.annotations.esl_info["type_ref"] for v in shared_vars],
                             annotations=dict(
                                 esl_info=dict(
-                                    reason=dict(
-                                        shared_variables=[v.name for v in shared_vars]
-                                    )
+                                    reason=dict(shared_variables=[v.name for v in shared_vars])
                                 )
                             ),
                         ),
                         "mcd",
                     )
 
     def _make_mcr(self):
@@ -1216,21 +1122,16 @@
                     continue
 
                 self._add(
                     Edge(
                         source=c,
                         target=r,
                         kind="mapping_dependency",
-                        labels=[
-                            nodes[v].annotations.esl_info["type_ref"]
-                            for v in shared_vars
-                        ],
-                        annotations=dict(
-                            esl_info=dict(reason=dict(shared_vars=list(shared_vars)))
-                        ),
+                        labels=[nodes[v].annotations.esl_info["type_ref"] for v in shared_vars],
+                        annotations=dict(esl_info=dict(reason=dict(shared_vars=list(shared_vars)))),
                     ),
                     "mcr",
                 )
 
     def _make_mfv(self):
         """Construct mapping dependencies between function specs and variables."""
         nodes = self.node_store.nodes
@@ -1295,21 +1196,16 @@
                     continue
 
                 self._add(
                     Edge(
                         source=f,
                         target=d,
                         kind="mapping_dependency",
-                        labels=[
-                            nodes[v].annotations.esl_info["type_ref"]
-                            for v in shared_vars
-                        ],
-                        annotations=dict(
-                            esl_info=dict(reason=dict(shared_vars=list(shared_vars)))
-                        ),
+                        labels=[nodes[v].annotations.esl_info["type_ref"] for v in shared_vars],
+                        annotations=dict(esl_info=dict(reason=dict(shared_vars=list(shared_vars)))),
                     ),
                     "mfd",
                 )
 
     def _make_mfr(self):
         """Create mapping dependencies between functions specs and relation specs."""
         nodes = self.node_store.nodes
@@ -1342,21 +1238,16 @@
                     continue
 
                 self._add(
                     Edge(
                         source=f,
                         target=r,
                         kind="mapping_dependency",
-                        labels=[
-                            nodes[v].annotations.esl_info["type_ref"]
-                            for v in shared_vars
-                        ],
-                        annotations=dict(
-                            esl_info=dict(reason=dict(shared_vars=list(shared_vars)))
-                        ),
+                        labels=[nodes[v].annotations.esl_info["type_ref"] for v in shared_vars],
+                        annotations=dict(esl_info=dict(reason=dict(shared_vars=list(shared_vars)))),
                     ),
                     "mfr",
                 )
 
     def _make_mbd(self):
         """Create mapping dependencies between behavior requirements and design
         specifications.
@@ -1381,22 +1272,17 @@
                 shared_vars = bvs.intersection(dvs)
                 if shared_vars:
                     self._add(
                         Edge(
                             source=b,
                             target=d,
                             kind="mapping_dependency",
-                            labels=[
-                                nodes[v].annotations.esl_info["type_ref"]
-                                for v in shared_vars
-                            ],
+                            labels=[nodes[v].annotations.esl_info["type_ref"] for v in shared_vars],
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(shared_vars=list(shared_vars))
-                                )
+                                esl_info=dict(reason=dict(shared_vars=list(shared_vars)))
                             ),
                         ),
                         "mbd",
                     )
 
     def _make_mbr(self):
         """Create mapping dependencies between behavior requirements and relation
@@ -1427,22 +1313,17 @@
                 shared_vars = bvs.intersection(rvs)
                 if shared_vars:
                     self._add(
                         Edge(
                             source=b,
                             target=r,
                             kind="mapping_dependency",
-                            labels=[
-                                nodes[v].annotations.esl_info["type_ref"]
-                                for v in shared_vars
-                            ],
+                            labels=[nodes[v].annotations.esl_info["type_ref"] for v in shared_vars],
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(shared_vars=list(shared_vars))
-                                )
+                                esl_info=dict(reason=dict(shared_vars=list(shared_vars)))
                             ),
                         ),
                         "mbr",
                     )
 
     def _make_mvd(self):
         """Create mapping dependencies between variables and design specifications."""
@@ -1528,22 +1409,17 @@
                 shared_vars = dvs.intersection(rvs)
                 if shared_vars:
                     self._add(
                         Edge(
                             source=d,
                             target=r,
                             kind="mapping_dependency",
-                            labels=[
-                                nodes[v].annotations.esl_info["type_ref"]
-                                for v in shared_vars
-                            ],
+                            labels=[nodes[v].annotations.esl_info["type_ref"] for v in shared_vars],
                             annotations=dict(
-                                esl_info=dict(
-                                    reason=dict(shared_vars=list(shared_vars))
-                                )
+                                esl_info=dict(reason=dict(shared_vars=list(shared_vars)))
                             ),
                         ),
                         "mdr",
                     )
 
     def _make_mnx(self):
         """Create mapping dependencies between needs and all other elements."""
@@ -1642,34 +1518,30 @@
 
     paths = _get_paths_between_all(srcs=vis, trgs=vjs, edges=edges)
     for path in paths:
         if len(path) == 2:
             vi, vj = path[0], path[1]
             edges = ev_dict.get((nodes[vi], nodes[vj]), [])
             for e in edges:
-                reasons.update(
-                    e.annotations.esl_info["reason"]["behavior_specifications"]
-                )
+                reasons.update(e.annotations.esl_info["reason"]["behavior_specifications"])
             vrs.extend([nodes[path[0]], nodes[path[-1]]])
         else:
             # Check id none of the intermediate path variables relate to a function
             # spec. If so proceed.
             transformation_check = True
             for v in path[1:-1]:
                 if v in vf_dict:
                     transformation_check = False
                     break
 
             if transformation_check:
                 for vi, vj in zip(path[:-1], path[1:]):
                     edges = ev_dict.get((nodes[vi], nodes[vj]))
                     for e in edges:
-                        reasons.update(
-                            e.annotations.esl_info["reason"]["behavior_specifications"]
-                        )
+                        reasons.update(e.annotations.esl_info["reason"]["behavior_specifications"])
 
             vrs.extend([nodes[path[0]], nodes[path[-1]]])
 
     if reasons:
         lbs = [v.annotations.esl_info["type_ref"] for v in vrs]
         return Edge(
             source=ci,
@@ -1685,17 +1557,15 @@
                 )
             ),
         )
     else:
         return None
 
 
-def _get_paths_between_all(
-    srcs=List[Node], trgs=List[Node], edges=List[Edge]
-) -> List[List[str]]:
+def _get_paths_between_all(srcs=List[Node], trgs=List[Node], edges=List[Edge]) -> List[List[str]]:
     """Compute paths between nodes. Based on depth first search.
 
     Arguments:
          srcs: List of starting nodes of paths.
          trgs: Set of ending nodes of path.
          edges: List of edges between nodes.
 
@@ -1745,17 +1615,15 @@
             continue
         elif n in trgs:
             # A target has been reached
             visited.append(n.name)
             paths.append(visited)
         else:
             new_path = deepcopy(visited)
-            paths.extend(
-                _get_paths(src=n, edge_dct=edge_dct, trgs=trgs, visited=new_path)
-            )
+            paths.extend(_get_paths(src=n, edge_dct=edge_dct, trgs=trgs, visited=new_path))
 
     return paths
 
 
 def _get_function_behavior_dependency(
     nodes: Dict[str, Node],
     src: Node,
@@ -1793,43 +1661,37 @@
 
     paths = _get_paths_between_all(srcs=vis, trgs=vjs, edges=edges)
     for path in paths:
         if len(path) == 2:
             vi, vj = path[0], path[1]
             edges = ev_dict.get((nodes[vi], nodes[vj]), [])
             for e in edges:
-                reasons.update(
-                    e.annotations.esl_info["reason"]["behavior_specifications"]
-                )
+                reasons.update(e.annotations.esl_info["reason"]["behavior_specifications"])
             vrs.extend([nodes[path[0]], nodes[path[-1]]])
         else:
             # Check id none of the intermediate path variables relate to a function
             # spec. If so proceed.
             transformation_check = True
             for v in path[1:-1]:
                 if v in vf_dict:
                     transformation_check = False
                     break
 
             if transformation_check:
                 for vi, vj in zip(path[:-1], path[1:]):
                     edges = ev_dict.get((nodes[vi], nodes[vj]))
                     for e in edges:
-                        reasons.update(
-                            e.annotations.esl_info["reason"]["behavior_specifications"]
-                        )
+                        reasons.update(e.annotations.esl_info["reason"]["behavior_specifications"])
 
             vrs.extend([nodes[path[0]], nodes[path[-1]]])
 
     if reasons:
         lbs = [v.annotations.esl_info["type_ref"] for v in vrs]
         return Edge(
             source=src,
             target=trg,
             kind="logical_dependency",
             labels=lbs,
-            annotations=dict(
-                esl_info=dict(reason=dict(behavior_specifications=sorted(reasons)))
-            ),
+            annotations=dict(esl_info=dict(reason=dict(behavior_specifications=sorted(reasons)))),
         )
     else:
         return None
```

### Comparing `raesl-0.12.1/raesl/compile/instantiating/graph_building.py` & `raesl-0.12.2/raesl/compile/instantiating/graph_building.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,15 @@
         self,
         diag_store: diagnostics.DiagnosticStore,
         spec: Optional[Specification] = None,
     ):
         self.diag_store = diag_store
         self.spec = spec
         self.node_factory = NodeFactory(self.diag_store, spec=spec)
-        self.edge_factory = EdgeFactory(
-            self.diag_store, node_store=self.node_factory.node_store
-        )
+        self.edge_factory = EdgeFactory(self.diag_store, node_store=self.node_factory.node_store)
 
     def make_graph(self, spec: Optional[Specification] = None) -> Optional[Graph]:
         """Instantiate the tree defined in the specification, and build a graph for it.
 
         Arguments:
             spec: Specification object holding parsed ESL data.
```

### Comparing `raesl-0.12.1/raesl/compile/instantiating/graph_data.py` & `raesl-0.12.2/raesl/compile/instantiating/graph_data.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/instantiating/instantation_graph_structure.yml` & `raesl-0.12.2/raesl/compile/instantiating/instantation_graph_structure.yml`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/instantiating/node_building.py` & `raesl-0.12.2/raesl/compile/instantiating/node_building.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,17 +101,15 @@
 
         # Create world node and instantiate it (recursively).
         self._add(
             Node(
                 name="world",
                 kind="component",
                 annotations=dict(
-                    esl_info=dict(
-                        definition_name="world", property_variables=[], comments=[]
-                    )
+                    esl_info=dict(definition_name="world", property_variables=[], comments=[])
                 ),
             ),
             "components",
         )
         self._instantiate_component(spec.world, {}, "world")
 
         post_process_comments(self.node_store.nodes.values())
@@ -153,37 +151,31 @@
         for comp_inst in comp_def.component_instances:
             assert comp_inst.compdef is not None
             assert len(comp_inst.arguments) == len(comp_inst.compdef.parameters)
 
             child_inst_map: Dict[ElementaryVarNode, InstNode] = {}
             for arg, param in zip(comp_inst.arguments, comp_inst.compdef.parameters):
                 assert arg.argnode is not None
-                result = make_parameter_instmap(
-                    param, param.node, arg.argnode, inst_map
-                )
+                result = make_parameter_instmap(param, param.node, arg.argnode, inst_map)
                 child_inst_map.update(result)
 
             # Full dotted name.
             child_inst_name = f"{inst_name}.{comp_inst.inst_name_tok.tok_text}"
 
             # Add component as a node.
             self._add(
-                make_component_node(
-                    c=comp_inst, inst_name=child_inst_name, params=child_inst_map
-                ),
+                make_component_node(c=comp_inst, inst_name=child_inst_name, params=child_inst_map),
                 "components",
             )
-            self._instantiate_component(
-                comp_inst.compdef, child_inst_map, child_inst_name
-            )
+            self._instantiate_component(comp_inst.compdef, child_inst_map, child_inst_name)
 
             # Set parent of child
-            self.node_store.components[
-                child_inst_name
-            ].parent = self.node_store.components[inst_name]
+            self.node_store.components[child_inst_name].parent = self.node_store.components[
+                inst_name
+            ]
 
         # Verify ownership of the variable InstNodes.
         for inst_node in local_varinst_list:
             inst_node.check_owner(self.diag_store)
 
         # Instantiate need, goal, transform, design, behavior and relation specs.
         for n in comp_def.needs:
@@ -278,32 +270,24 @@
                 instnode.add_comment(child.get_comment())
         return {param_node: instnode}
     else:
         child_map = {}
         assert isinstance(param_node, CompoundVarNode)
         if isinstance(arg_node, CompoundVarNode):
             assert len(param_node.child_nodes) == len(arg_node.child_nodes)
-            for param_child, arg_child in zip(
-                param_node.child_nodes, arg_node.child_nodes
-            ):
+            for param_child, arg_child in zip(param_node.child_nodes, arg_node.child_nodes):
                 child_map.update(
-                    make_parameter_instmap(
-                        param, param_child, arg_child, parent_inst_map
-                    )
+                    make_parameter_instmap(param, param_child, arg_child, parent_inst_map)
                 )
         else:
             assert isinstance(arg_node, GroupNode)
             assert len(param_node.child_nodes) == len(arg_node.child_nodes)
-            for param_child, arg_child in zip(
-                param_node.child_nodes, arg_node.child_nodes
-            ):
+            for param_child, arg_child in zip(param_node.child_nodes, arg_node.child_nodes):
                 child_map.update(
-                    make_parameter_instmap(
-                        param, param_child, arg_child, parent_inst_map
-                    )
+                    make_parameter_instmap(param, param_child, arg_child, parent_inst_map)
                 )
 
         return child_map
 
 
 def make_type_node(tdef: types.TypeDef) -> Node:
     """Node creation for a type definition.
@@ -355,17 +339,15 @@
             if interval[1].unit:
                 d["upperbound"]["unit"] = interval[1].unit.tok_text
         domain.append(d)
 
     return dict(esl_info=dict(units=units, domain=domain))
 
 
-def make_variable_node(
-    v: InstNode, type_inst_map: Dict[ElementaryType, TypeDef]
-) -> Node:
+def make_variable_node(v: InstNode, type_inst_map: Dict[ElementaryType, TypeDef]) -> Node:
     """Node creation for a variable.
 
     Arguments:
         v: The variable for which a nodes must be created.
 
     Returns:
         Node of kind "variable".
@@ -475,17 +457,15 @@
             subject=inst_prefix + "." + n.subject_tok.tok_text,
             text=n.description,
             comments=n.comments,
         )
     )
 
 
-def make_goal_node(
-    g: Goal, inst_name: str, inst_map: Dict[ElementaryVarNode, InstNode]
-) -> Node:
+def make_goal_node(g: Goal, inst_name: str, inst_map: Dict[ElementaryVarNode, InstNode]) -> Node:
     """Goal node creation.
 
     Arguments:
       g: The goal for which a node must be created.
       inst_name: The instantiation name of the component.
       inst_map: Dictionary containing the instantiated variables.
 
@@ -516,17 +496,15 @@
         verb=g.verb.tok_text,
         variables=_get_variable_inst_names(inst_map, g.flows),
         preposition=g.prepos.tok_text,
         passive=inst_name + "." + g.passive.tok_text,
         subclauses=_make_subclause_annotations(g, inst_map),
     )
 
-    return dict(
-        esl_info=dict(sub_kind="goal", form=g.goal_kind, body=body, comments=g.comments)
-    )
+    return dict(esl_info=dict(sub_kind="goal", form=g.goal_kind, body=body, comments=g.comments))
 
 
 def make_transform_node(
     t: Transformation, inst_name: str, inst_map: Dict[ElementaryVarNode, InstNode]
 ) -> Node:
     """Transformation node creation.
 
@@ -630,19 +608,15 @@
       inst_map: Dictionary containing the instantiated variables.
 
     Returns:
       See YAML output spec /components/schemas/DesignSpecAnotation.
     """
     body = _make_design_rule_annotation(expr=d.expr, inst_map=inst_map)
     subs = _make_subclause_annotations(d, inst_map)
-    return dict(
-        esl_info=dict(
-            form=d.design_kind, body=body, sub_clauses=subs, comments=d.comments
-        )
-    )
+    return dict(esl_info=dict(form=d.design_kind, body=body, sub_clauses=subs, comments=d.comments))
 
 
 def _make_subclause_annotations(
     e: Union[Goal, Transformation, Design], inst_map: Dict[ElementaryVarNode, InstNode]
 ) -> List[Dict[str, Any]]:
     """Subclause spec annotation creation.
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/__init__.py` & `raesl-0.12.2/raesl/compile/machine_files/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/machine_files/argument_list.py` & `raesl-0.12.2/raesl/compile/machine_files/argument_list.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/machine_files/behavior.py` & `raesl-0.12.2/raesl/compile/machine_files/behavior.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,15 @@
     start -> s1 [BEHAVIOR_CONSTRAINT_KW] tag=kind;
 
     end accept=behavior_header;
     s1 -> end [NL_TK];
 """
 
 
-def _process_behavior_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_behavior_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     behave_kind = tags["kind"][0]
     builder.notify_new_section(behave_kind, False)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.new_behavior_header(behave_kind)
 
@@ -64,17 +62,15 @@
     s2 -> s3 [COLON_TK];
 
     end accept=behavior_case;
     s3 -> end [NL_TK];
 """
 
 
-def _process_new_case(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_new_case(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     case_label = tags["case_name"][0]
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.behavior_case(case_label)
 
 
@@ -157,17 +153,15 @@
     Arguments:
         tags: Key pieces of text found in the input.
 
     Returns:
         The equivalent expression.
     """
     split_offsets = (
-        cast(List[Optional[int]], [None])
-        + [tok.offset for tok in tags.get("or", [])]
-        + [None]
+        cast(List[Optional[int]], [None]) + [tok.offset for tok in tags.get("or", [])] + [None]
     )
     equations = []
 
     unit_tags = tags.get("unit", [])
     for index in range(1, len(split_offsets)):
         start_offset = split_offsets[index - 1]
         end_offset = split_offsets[index]
@@ -190,17 +184,15 @@
 
     if len(equations) == 1:
         return equations[0]
     else:
         return exprs.Disjunction(equations)
 
 
-def _process_when_condition(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_when_condition(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     name_tok = tags["condition_name"][0]
     expr = _decode_when_comparisons(tags)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.behavior_when_condition(name_tok, expr)
 
@@ -212,17 +204,15 @@
     start -> s1 [THEN_KW] tag=then;
 
     end accept=behavior_then;
     s1 -> end [NL_TK];
 """
 
 
-def _process_then_start(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_then_start(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.behavior_normal_then(tags["then"][0])
 
 
 _BEHAVIOR_THEN_RESULT_SPEC = (
     """
@@ -283,22 +273,18 @@
         else:
             rhs = exprs.Value(varvalue, units[0])
 
         return exprs.RelationComparison(is_constraint, lhs, is_aux, compare_op[0], rhs)
 
     else:
         objective = tags["objective"][0]
-        return exprs.ObjectiveComparison(
-            lhs, is_aux, objective.tok_type == "MAXIMIZED_KW"
-        )
+        return exprs.ObjectiveComparison(lhs, is_aux, objective.tok_type == "MAXIMIZED_KW")
 
 
-def _process_then_result(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_then_result(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     name_tok = tags["result_name"][0]
     expr = _decode_result(tags)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.behavior_then_result(name_tok, expr)
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/builder.py` & `raesl-0.12.2/raesl/compile/machine_files/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,19 +100,15 @@
 class StateMachineParser(Parser):
     tokens = StateMachineLexer.tokens
 
     def error(self, t):
         if t is None:
             print("Unexpected EOF encountered.")
         else:
-            print(
-                "Syntax error at line {}, token {}, text={}".format(
-                    t.lineno, t.type, t.value
-                )
-            )
+            print("Syntax error at line {}, token {}, text={}".format(t.lineno, t.type, t.value))
 
     @_("NAME COLON_TK mlines")
     def machine(self, p):
         return (p[0], p[2])
 
     @_("")
     def mlines(self, p):
@@ -181,17 +177,15 @@
 
     Arguments:
         name: Name of the state machine, also the name of the matched sequence.
         processing_func: If not None, function that inserts relevant information from
             the matched line into the ast that is constructed.
     """
 
-    def __init__(
-        self, name: str, processing_func: Optional[typing.ProcessingFunc] = None
-    ):
+    def __init__(self, name: str, processing_func: Optional[typing.ProcessingFunc] = None):
         super().__init__(name)
         self.processing_func = processing_func
 
 
 class StateMachineBuilder:
     """Class for easily constructing a state machine from a textual description.
 
@@ -219,17 +213,15 @@
         """
         loc = self.locs.get(name)
         if loc is not None:
             return loc
 
         return self.create_loc(name, [])
 
-    def create_loc(
-        self, name: str, opts: List[Union[Tuple[str], Tuple[str, str]]]
-    ) -> Location:
+    def create_loc(self, name: str, opts: List[Union[Tuple[str], Tuple[str, str]]]) -> Location:
         """Create a new location.
 
         Arguments:
             name: Name of the location to create.
             opts: Location options, list of ('initial',) and/or ('accept', str) .
 
         Returns:
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/comments.py` & `raesl-0.12.2/raesl/compile/machine_files/comments.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,34 +13,30 @@
 
     end accept=comment_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_comment_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_comment_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["comment"][0], False)
 
 
 _COMMENT_LINE_SPEC = """
 comment_line:
     start initial;
     start -> s1 [DOTTEDNAME] tag=name;
 
     end accept=comment_name;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_comment_name(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_comment_name(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.add_comment(tags["name"][0])
 
 
 MACHINES: typing.MachineTripletList = [
     ("COMMENT_HEADER_MACHINE", _COMMENT_HEADER_SPEC, _process_comment_header),
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/component_definitions.py` & `raesl-0.12.2/raesl/compile/machine_files/component_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
     end accept=define_component;
     s3 -> end [NL_TK];
     s3 -> end [EOF_TK];
 """
 
 
-def _process_compdef(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_compdef(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     if "world" in tags:
         pos_tok = tags["world"][0]
         name_tok = None
     else:
         name_tok = tags["comp_name"][0]
         pos_tok = name_tok
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/component_instances.py` & `raesl-0.12.2/raesl/compile/machine_files/component_instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
     end accept=component_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_component_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_component_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["component"][0], False)
 
 
 _COMPONENT_INSTANCE_NO_ARGS_SPEC = """
 component_instance:
     start initial;
     start -> s1 [NAME] tag=component_instance;
@@ -34,17 +32,15 @@
 
     end accept=component_instance_no_arguments;
     s4 -> end [NL_TK];
     s4 -> end [EOF_TK];
 """
 
 
-def _process_instance_no_args(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_instance_no_args(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     instance_tok = tags["component_instance"][0]
     definition_tok = tags["component_def"][0]
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.add_compinst(instance_tok, definition_tok, False)
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/designs.py` & `raesl-0.12.2/raesl/compile/machine_files/designs.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
     end accept=design_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_design_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_design_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     kind = tags["design"][0]
     builder.notify_new_section(kind, False)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.new_design_header(kind)
 
@@ -48,17 +46,15 @@
     finish accept=design_with_subs;
     s6 -> finish [NL_TK];
     s6 -> finish [EOF_TK];
 """
 )
 
 
-def _process_design_line(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_design_line(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     label = tags["label"][0]
     condition = sub_clause.decode_disjunctive_comparisons(tags)
     design = components.Design(label, condition)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.design_line(design)
@@ -80,17 +76,15 @@
     s4 -> finish [EOF_TK];
 """
 )
 
 # _DESIGN_NO_SUBS_SPEC also uses _process_design_line.
 
 
-def _process_design_subclause(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_design_subclause(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     sub = sub_clause.decode_subclause(tags)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.add_design_subclause(sub)
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/goals.py` & `raesl-0.12.2/raesl/compile/machine_files/goals.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     start -> s1 [GOAL_CONSTRAINT_KW] tag=goal_kind;
 
     end accept=goal_header;
     s1 -> end [NL_TK];
 """
 
 
-def _process_goal_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_goal_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     goal_kind = tags["goal_kind"][0]
     builder.notify_new_section(goal_kind, False)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.new_goal_header(goal_kind)
 
@@ -57,17 +55,15 @@
     end accept=goal_main_with_subs;
     s11 -> end [NL_TK];
     s11 -> end [EOF_TK];
 """
 )
 
 
-def _process_goal_with_subs(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_goal_with_subs(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     label = tags["label"][0]
     active = tags["active_compname"][0]
     doesaux = tags["doesaux"][0]
     verb = tags["verb"][0]
     flows = [components.Flow(name_tok) for name_tok in tags["argument_name"]]
     prepos = tags["prepos"][0]
     passive = tags["passive_compname"][0]
@@ -98,34 +94,30 @@
     end accept=goal_main_no_subs;
     s9 -> end [NL_TK];
     s9 -> end [EOF_TK];
 """
 )
 
 
-def _process_goal_no_subs(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_goal_no_subs(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     label = tags["label"][0]
     active = tags["active_compname"][0]
     doesaux = tags["doesaux"][0]
     verb = tags["verb"][0]
     flows = [components.Flow(name_tok) for name_tok in tags["argument_name"]]
     prepos = tags["prepos"][0]
     passive = tags["passive_compname"][0]
     goal = components.Goal(label, active, doesaux, verb, flows, prepos, passive)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.add_goal(goal)
 
 
-def _process_goal_subclause(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_goal_subclause(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     sub = sub_clause.decode_subclause(tags)
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.add_goal_subclause(sub)
 
 
 MACHINES: typing.MachineTripletList = [
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/groups.py` & `raesl-0.12.2/raesl/compile/machine_files/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
     end accept=group_section_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_vargroup_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_vargroup_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["vargroup"][0], False)
 
 
 _GROUP_START_SPEC = """
 group_start:
     start initial;
     start -> s1 [NAME] tag=group_name;
@@ -35,25 +33,21 @@
 
     end accept=group_start;
     s5 -> end [NL_TK];
     s5 -> end [EOF_TK];
 """
 
 
-def _process_new_vargroup(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_new_vargroup(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.new_vargroup(tags["group_name"][0])
 
 
-def _process_arguments(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_arguments(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     names = argument_list.process_argument_list_line(tags)
     current_comp.vgroup_add_vars(names)
 
 
 MACHINES: typing.MachineTripletList = [
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/machine_parts.py` & `raesl-0.12.2/raesl/compile/machine_files/machine_parts.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,15 @@
         {start} -> {end} [SHOULD_KW] tag={tagname};
         {start} -> {end} [COULD_KW] tag={tagname};
         {start} -> {end} [WONT_KW] tag={tagname};
     """
     return text.format(start=start_loc, end=end_1locs[0], tagname=tagname)
 
 
-def get_does_auxiliary_verb_part(
-    start_loc: str, end_1locs: List[str], tagname: str
-) -> str:
+def get_does_auxiliary_verb_part(start_loc: str, end_1locs: List[str], tagname: str) -> str:
     """State machine part that implements:
 
     "does" | auxiliary-verb
     """
     assert len(end_1locs) == 1
 
     text = """\
@@ -123,17 +121,15 @@
             cmp5 -> {end} [MOST_KW] tag={tagname};
         {start} -> {end} [APPROXIMATELY_KW] tag={tagname};
     """
 
     return text.format(**locs)
 
 
-def get_disjunctive_comparison_part(
-    start_loc: str, end_2locs: List[str], prefix: str = ""
-) -> str:
+def get_disjunctive_comparison_part(start_loc: str, end_2locs: List[str], prefix: str = "") -> str:
     """State machine part implementing the 'comparison-rule-line' comparisons.
 
     comparison-rule-line ::=
         comparison { "or" comparison }
 
     comparison ::=
         argument-name ( constraint-rule-literal | requirement-rule-literal )
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/needs.py` & `raesl-0.12.2/raesl/compile/machine_files/needs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
     end accept=need_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_need_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_need_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["need"][0], False)
 
 
 _NEED_LINE_SPEC = """
 needs_line:
     start initial;
     start -> s1 [NAME] tag=label;
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/parameters.py` & `raesl-0.12.2/raesl/compile/machine_files/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
     end accept=parameter_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_paramheader(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_paramheader(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     token = tags["parameter"][0]
     builder.notify_new_section(token, False)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.notify_parameter_section(token)
 
@@ -46,17 +44,15 @@
 
     s4 -> s5 [PROPERTY_KW] tag=is_property;
     s5 -> end [NL_TK];
     s5 -> end [EOF_TK];
 """
 
 
-def _process_paramline(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_paramline(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     paramnames = tags["paramname"]
     typename = tags["typename"][0]
     is_property = "is_property" in tags
     parameters = [VarParam(False, vname, typename, is_property) for vname in paramnames]
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.add_parameters(parameters)
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/relation_definitions.py` & `raesl-0.12.2/raesl/compile/machine_files/relation_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
     end accept=define_relation;
     s2 -> end [NL_TK];
     s2 -> end [EOF_TK];
 """
 
 
-def _process_reldef_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_reldef_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["define"][0], True)
 
 
 _RELATION_NAME_LINE_SPEC = """
 relation_name:
     start initial;
     start -> s1 [NAME] tag=rel_name;
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/relation_instances.py` & `raesl-0.12.2/raesl/compile/machine_files/relation_instances.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
     end accept=relation_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_relinst_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_relinst_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["relation"][0], False)
 
 
 _RELATION_INSTANCE_SPEC = """
 relation_instance:
     start initial;
     start -> s1 [NAME] tag=relation_inst_name;
@@ -33,22 +31,18 @@
 
     end accept=instance_line;
     s3 -> end [NL_TK];
     s3 -> end [EOF_TK];
 """
 
 
-def _process_new_relinst(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_new_relinst(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
-    current_comp.new_relinst(
-        tags["relation_inst_name"][0], tags["relation_def_name"][0]
-    )
+    current_comp.new_relinst(tags["relation_inst_name"][0], tags["relation_def_name"][0])
 
 
 _RELATION_ARGUMENT_HEADER_SPEC = """
 relation_argument_header:
     start initial;
     start -> s1 [REQUIRING_KW] tag=argtype;
     start -> s1 [RETURNING_KW] tag=argtype;
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/sub_clause.py` & `raesl-0.12.2/raesl/compile/machine_files/sub_clause.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,17 +51,15 @@
         tags: Extracted data from a match of the machine defined in
             'machine_parts.get_disjunctive_comparison_part'.
 
     Returns:
         The expression equivalent to the matched text.
     """
     split_offsets = (
-        cast(List[Optional[int]], [None])
-        + [tok.offset for tok in tags.get("or", [])]
-        + [None]
+        cast(List[Optional[int]], [None]) + [tok.offset for tok in tags.get("or", [])] + [None]
     )
     equations: List[exprs.Expression] = []
 
     unit_tags = tags.get("unit", [])
     compare_tags = tags.get("compare_op", [])
     for index in range(1, len(split_offsets)):
         start_offset = split_offsets[index - 1]
@@ -87,17 +85,15 @@
 
             comp = exprs.RelationComparison(is_constraint, lhs, is_aux, compare_op, rhs)
             equations.append(comp)
 
         else:
             objective = get_one(tags["objective"], start_offset, end_offset)
 
-            comp = exprs.ObjectiveComparison(
-                lhs, is_aux, objective.tok_type == "MAXIMIZED_KW"
-            )
+            comp = exprs.ObjectiveComparison(lhs, is_aux, objective.tok_type == "MAXIMIZED_KW")
             equations.append(comp)
 
     if len(equations) == 1:
         return equations[0]
     else:
         return exprs.Disjunction(equations)
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/transforms.py` & `raesl-0.12.2/raesl/compile/machine_files/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
     end accept=transform_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_transform_header(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_transform_header(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     kind_tok = tags["transform_kind"][0]
     builder.notify_new_section(kind_tok, False)
 
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.notify_transform_section(kind_tok)
     current_comp.new_transform_header(kind_tok)
@@ -43,23 +41,19 @@
     start -> s1 [NAME] tag=label;
     s1 -> s2 [COLON_TK];
 """
     + get_does_auxiliary_verb_part("s2", ["s4"], tagname="doesaux")
     + """\
     s4 -> s5 [NAME] tag=verb;
 """
-    + get_argument_references_part(
-        "s5", ["s7"], tagname="from_argument_name", prefix="from"
-    )
+    + get_argument_references_part("s5", ["s7"], tagname="from_argument_name", prefix="from")
     + """\
     s7 -> s8 [NAME] tag=prepos;
 """
-    + get_argument_references_part(
-        "s8", ["s10"], tagname="to_argument_name", prefix="to"
-    )
+    + get_argument_references_part("s8", ["s10"], tagname="to_argument_name", prefix="to")
     + """\
     end accept=transform_main_no_subs;
     s10 -> end [NL_TK];
     s10 -> end [EOF_TK];
 """
 )
 
@@ -89,23 +83,19 @@
     start -> s1 [NAME] tag=label;
     s1 -> s2 [COLON_TK];
 """
     + get_does_auxiliary_verb_part("s2", ["s4"], tagname="doesaux")
     + """\
     s4 -> s5 [NAME] tag=verb;
 """
-    + get_argument_references_part(
-        "s5", ["s7"], tagname="from_argument_name", prefix="from"
-    )
+    + get_argument_references_part("s5", ["s7"], tagname="from_argument_name", prefix="from")
     + """\
     s7 -> s8 [NAME] tag=prepos;
 """
-    + get_argument_references_part(
-        "s8", ["s10"], tagname="to_argument_name", prefix="to"
-    )
+    + get_argument_references_part("s8", ["s10"], tagname="to_argument_name", prefix="to")
     + """\
     s10 -> s11 [WITH_KW];
     s11 -> s12 [SUB_CLAUSES_KW] tag=with_subclause;
 
     end accept=transform_main_with_subs;
     s12 -> end [NL_TK];
     s12 -> end [EOF_TK];
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/type_defs.py` & `raesl-0.12.2/raesl/compile/machine_files/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from raesl.compile.machine_files.utils import get_one, get_optional, make_loc_names
 
 if TYPE_CHECKING:
     from raesl.compile.scanner import Token
     from raesl.compile.typechecking.ast_builder import AstBuilder
 
 
-def get_unit_specification_part(
-    start_loc: str, end_1locs: List[str], prefix: str = ""
-) -> str:
+def get_unit_specification_part(start_loc: str, end_1locs: List[str], prefix: str = "") -> str:
     """State machine part implementing the 'unit-specification' rule.
 
     unit-specification ::=
         "with" ( "unit" | "units" ) UNIT-NAME { "," UNIT-NAME }
     """
     assert len(end_1locs) == 1
 
@@ -65,17 +63,15 @@
     text = """
         {lenum1}; {lenum2};
 
         {start} -> {lenum1} [IS_KW];
         {lenum1} -> {end} [A_KW];
     """
     text = text.format(**locs)
-    return text + get_short_enumeration_specification_part(
-        locs["end"], end_2locs, prefix
-    )
+    return text + get_short_enumeration_specification_part(locs["end"], end_2locs, prefix)
 
 
 def get_short_enumeration_specification_part(
     start_loc: str, end_2locs: List[str], prefix: str = ""
 ) -> str:
     """State machine part implementing the short 'enumeration-specification' rule.
 
@@ -114,29 +110,25 @@
 
     Returns:
         Values of the enumeration.
     """
     if "has_enum_spec" not in tags:
         return None
 
-    offsets = cast(List[Optional[int]], [tok.offset for tok in tags["enum_value"]]) + [
-        None
-    ]
+    offsets = cast(List[Optional[int]], [tok.offset for tok in tags["enum_value"]]) + [None]
 
     values = []
     unit_tags = tags.get("enum_unit", [])
     for i, val in enumerate(tags["enum_value"]):
         unit = get_optional(unit_tags, val.offset, offsets[i + 1])
         values.append(exprs.Value(val, unit))
     return values
 
 
-def get_interval_specification_part(
-    start_loc: str, end_4locs: List[str], prefix: str = ""
-) -> str:
+def get_interval_specification_part(start_loc: str, end_4locs: List[str], prefix: str = "") -> str:
     """State machine part implementing the 'interval-specification' rule.
 
     interval-specification ::=
         "of" interval { "or" interval }
     """
     assert len(end_4locs) == 4
 
@@ -216,17 +208,15 @@
             high_bound = None
 
         boundaries.append((low_bound, high_bound))
 
     return boundaries
 
 
-def get_constant_specification_part(
-    start_loc: str, end_2locs: List[str], prefix: str = ""
-) -> str:
+def get_constant_specification_part(start_loc: str, end_2locs: List[str], prefix: str = "") -> str:
     """State machine part implementing the 'constant-specification' rule.
 
     constant-specification ::=
         "equal" "to" VALUE [ UNIT ]
     """
     assert len(end_2locs) == 2
 
@@ -267,17 +257,15 @@
 
     end accept=define_type;
     s2 -> end [NL_TK];
     s2 -> end [EOF_TK];
 """
 
 
-def _process_define_type(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_define_type(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["define"][0], True)
 
 
 _NEW_TYPE_SPEC = (
     """
 new_type:
     start initial;
@@ -316,17 +304,15 @@
     s9 -> end [EOF_TK];
     s10 -> end [NL_TK];
     s10 -> end [EOF_TK];
 """
 )
 
 
-def _process_new_type_def(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_new_type_def(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     new_type = tags["new_type"][0]
     enum_spec = _convert_enum_spec(tags)
     unit_spec = _convert_unit_spec(tags)
     ival_spec = _convert_interval_spec(tags)
     cons_spec = _convert_constant_spec(tags)
     builder.add_typedef(new_type, None, enum_spec, unit_spec, ival_spec, cons_spec)
 
@@ -366,26 +352,22 @@
     s10 -> end [EOF_TK];
     s11 -> end [NL_TK];
     s11 -> end [EOF_TK];
 """
 )
 
 
-def _process_derived_type_def(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_derived_type_def(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     new_type = tags["new_type"][0]
     exist_type = tags["old_type"][0]
     enum_spec = _convert_enum_spec(tags)
     unit_spec = _convert_unit_spec(tags)
     ival_spec = _convert_interval_spec(tags)
     cons_spec = _convert_constant_spec(tags)
-    builder.add_typedef(
-        new_type, exist_type, enum_spec, unit_spec, ival_spec, cons_spec
-    )
+    builder.add_typedef(new_type, exist_type, enum_spec, unit_spec, ival_spec, cons_spec)
 
 
 _BUNDLE_TYPE_SPEC = """
 bundle_type:
     start initial;
     start -> s1 [NAME] tag=bundle_name;
     s1 -> s2 [IS_KW];
@@ -395,17 +377,15 @@
 
     end accept=bundle_type;
     s5 -> end [NL_TK];
     s5 -> end [EOF_TK];
 """
 
 
-def _process_bundle_type(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_bundle_type(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.new_bundle_type(tags["bundle_name"][0])
 
 
 _BUNDLE_FIELD_SPEC = """
 bundle_field:
     start initial;
     end accept=bundle_field;
@@ -418,17 +398,15 @@
     s4 -> s5 [NAME] tag=field_type;
 
     s5 -> end [NL_TK];
     s5 -> end [EOF_TK];
 """
 
 
-def _process_bundle_field(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_bundle_field(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     field_name = tags["field_name"][0]
     field_type = tags["field_type"][0]
     builder.add_bundle_field(field_name, field_type)
 
 
 MACHINES: typing.MachineTripletList = [
     ("DEFINE_TYPE_MACHINE", _DEFINE_TYPE_SPEC, _process_define_type),
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/typing.py` & `raesl-0.12.2/raesl/compile/machine_files/typing.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/machine_files/utils.py` & `raesl-0.12.2/raesl/compile/machine_files/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,39 +2,33 @@
 from typing import Dict, List, Optional
 
 from raesl.compile.scanner import Token
 
 
 def make_loc_names(prefix: str, name: str, count: int) -> Dict[str, str]:
     """Make a dict with 'count' names by combining the prefix, name, and a number."""
-    return dict(
-        (name + str(num), prefix + name + str(num)) for num in range(1, count + 1)
-    )
+    return dict((name + str(num), prefix + name + str(num)) for num in range(1, count + 1))
 
 
-def _in_range(
-    tok: Token, start_offset: Optional[int], end_offset: Optional[int]
-) -> bool:
+def _in_range(tok: Token, start_offset: Optional[int], end_offset: Optional[int]) -> bool:
     """Is the given token offset positioned between and not at 'start_offset' and
     'end_offset'? If start_offset or end_offset is None, use -1 and infinity as offsets,
     respectively.
 
     Returns:
         Whether the provided token is between (not at) the start_offset and end_offset.
     """
     if start_offset is not None and tok.offset <= start_offset:
         return False
     if end_offset is not None and tok.offset >= end_offset:
         return False
     return True
 
 
-def get_one(
-    tokens: List[Token], start_offset: Optional[int], end_offset: Optional[int]
-) -> Token:
+def get_one(tokens: List[Token], start_offset: Optional[int], end_offset: Optional[int]) -> Token:
     """Filter tokens on the provided start and end offsets, and return the only token
     between the positions.
     """
     matches = [tok for tok in tokens if _in_range(tok, start_offset, end_offset)]
     assert len(matches) == 1
     return matches[0]
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/variables.py` & `raesl-0.12.2/raesl/compile/machine_files/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
     end accept=variable_header;
     s1 -> end [NL_TK];
     s1 -> end [EOF_TK];
 """
 
 
-def _process_varheader(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_varheader(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["variable"][0], False)
 
 
 _VARIABLE_LINE_SPEC = """
 variable_line:
     start initial;
     start -> s1 [NAME] tag=varname;
@@ -37,17 +35,15 @@
 
     end accept=variable_line;
     s4 -> end [NL_TK];
     s4 -> end [EOF_TK];
 """
 
 
-def _process_varline(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_varline(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     varnames = tags["varname"]
     typename = tags["typename"][0]
     variables = [VarParam(True, vname, typename) for vname in varnames]
     current_comp = builder.compdef_builder.current_component
     assert current_comp is not None
     current_comp.add_variables(variables)
```

### Comparing `raesl-0.12.1/raesl/compile/machine_files/verb_defs.py` & `raesl-0.12.2/raesl/compile/machine_files/verb_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
     end accept=define_verb;
     s2 -> end [NL_TK];
     s2 -> end [EOF_TK];
 """
 
 
-def _process_define_verb(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_define_verb(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     builder.notify_new_section(tags["define"][0], True)
 
 
 _VERB_PREPOS_SPEC = """
 verb_prepos:
     start initial;
     start -> s1 [NAME] tag=verb;
@@ -33,17 +31,15 @@
 
     end accept=verb_is_verb;
     s2 -> end [NL_TK];
     s2 -> end [EOF_TK];
 """
 
 
-def _process_verb_def(
-    tags: typing.TokensDict, _accept: str, builder: "AstBuilder"
-) -> None:
+def _process_verb_def(tags: typing.TokensDict, _accept: str, builder: "AstBuilder") -> None:
     verb = tags["verb"][0]
     prepos = tags["prepos"][0]
     builder.add_verbdef(verb, prepos)
 
 
 MACHINES: typing.MachineTripletList = [
     ("DEFINE_VERB_MACHINE", _DEFINE_VERB_SPEC, _process_define_verb),
```

### Comparing `raesl-0.12.1/raesl/compile/parser.py` & `raesl-0.12.2/raesl/compile/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         lexer: Lexer to use in the matching process.
         current_loc: Current location in the line machine.
         tags: Relevant data extracted from the text line during the parsing process.
         matched_tokens: Tokens used for matching the line thus far.
         dest_loc: New specification location if a match was found.
     """
 
-    def __init__(
-        self, machine: "ProcessingStateMachine", lexer: "Lexer", dest_loc: "Location"
-    ):
+    def __init__(self, machine: "ProcessingStateMachine", lexer: "Lexer", dest_loc: "Location"):
         self.machine = machine
         self.lexer = lexer
         self.current_loc: Optional["Location"] = machine.initial_loc
         self.tags: Dict[str, List["Token"]] = {}
         self.matched_tokens: List["Token"] = []
 
         self.dest_loc = dest_loc
@@ -155,32 +153,28 @@
             # Life is simple, pick the one and only match.
             best_acceptor = acceptors[0]
         else:
             # Multiple lines match. Filter on the most specific match.
             best_match = None
             best_acceptor = None
             for acceptor in acceptors:
-                match_prio = [
-                    get_token_priority(tok.tok_type) for tok in acceptor.matched_tokens
-                ]
+                match_prio = [get_token_priority(tok.tok_type) for tok in acceptor.matched_tokens]
                 if best_match is None or match_prio < best_match:
                     best_match = match_prio
                     best_acceptor = acceptor
                 elif best_acceptor is not None and match_prio == best_match:
                     ambi_acceptors = (
                         best_acceptor.get_accept_name(),
                         acceptor.get_accept_name(),
                     )
                     best_acceptor = None  # Ambiguous best match (until now)
 
             # Sanity check and raise an Exception if it fails.
             if best_acceptor is None:
-                diag_store.add(
-                    diagnostics.E101(ambi_acceptors, location=lexer.get_location())
-                )
+                diag_store.add(diagnostics.E101(ambi_acceptors, location=lexer.get_location()))
 
         # Store information of the line into the ast builder instance.
         assert best_acceptor is not None
         processing_func = best_acceptor.machine.processing_func
         if processing_func:
             tags = best_acceptor.tags
             accept = best_acceptor.get_accept_name()
```

### Comparing `raesl-0.12.1/raesl/compile/scanner.py` & `raesl-0.12.2/raesl/compile/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,17 +354,15 @@
                 # 4, starting with matching ".*":
                 i = self.text.find("\n", self.offset + 1)
                 self._save_doc_comment(self.offset, i)
                 if i < 0:
                     self.offset = self.length
                     return
                 else:
-                    self.offset = (
-                        i  # A '\n' is needed to end the current line in the parser!
-                    )
+                    self.offset = i  # A '\n' is needed to end the current line in the parser!
                     return
 
             if self.text.startswith("...", self.offset):
                 # 5:
                 # Switch to using 'tmp_offset' as the offset, as we may have
                 # to revert skipping ... .
                 tmp_offset = self.offset + 3
```

### Comparing `raesl-0.12.1/raesl/compile/state_machine.py` & `raesl-0.12.2/raesl/compile/state_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,17 +99,15 @@
             processed_locs.add(loc)
             if loc.accept:
                 lines.append(f'    {loc.name} [shape="box"]')
             else:
                 lines.append(f"    {loc.name}")
 
             for edge in loc.out_edges:
-                lines.append(
-                    f'    {loc.name} -> {edge.dest.name} [label="{edge.tok_type}"]'
-                )
+                lines.append(f'    {loc.name} -> {edge.dest.name} [label="{edge.tok_type}"]')
                 notdone.append(edge.dest)
 
         lines.append("}")
 
         if fname is None:
             fname = self.name + ".dot"
         with open(fname, "w") as handle:
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/ast_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/ast_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,33 +125,29 @@
             # New section started, documentation after this point doesn't belong
             # to a previous element.
             self.doc_distributor.add_dummy_element(tok)
 
         for builder in self.section_notify_list:
             builder.notify_new_section(new_top_section)
 
-    def finish_parse(
-        self, doc_comments: List["Token"]
-    ) -> Optional[specification.Specification]:
+    def finish_parse(self, doc_comments: List["Token"]) -> Optional[specification.Specification]:
         """Finish processing the collected information, that is, perform type checking.
 
         Arguments:
             doc_comments: Raw documentation comments rescued from the scanner.
         """
         # Tell all builders current section is done.
         self.notify_new_section(None, True)
 
         # Convert collected information to AST.
         spec = specification.Specification()
         self.verb_builder.finish(spec)
         self.type_builder.finish(spec)
         self.reldef_builder.finish(spec)  # Requires types.
-        self.compdef_builder.finish(
-            spec, self.doc_distributor
-        )  # Requires types, verbs, reldefs.
+        self.compdef_builder.finish(spec, self.doc_distributor)  # Requires types, verbs, reldefs.
 
         # Add specification elements to the doc distributor.
         for elem in specification.get_doc_comment_spec_elements(spec):
             self.doc_distributor.add_element(elem)
 
         # Hand out all doc comments.
         self.doc_distributor.resolve(doc_comments)
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_behavior_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_behavior_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,15 @@
     def __init__(self, comp_child_builders: "CompDefChildBuilders"):
         self.diag_store = comp_child_builders.diag_store
         self.comp_child_builders = comp_child_builders
 
         self.behavior_kind: Optional[str] = None
         self.expect_conds = False
         self.expect_results = False
-        self.pbehaviors: List[
-            ParsedBehavior
-        ] = []  # Using List[ParsedCase] for its 'case's.
+        self.pbehaviors: List[ParsedBehavior] = []  # Using List[ParsedCase] for its 'case's.
 
     def new_behavior_header(self, kind_tok: "Token"):
         """A new 'behavior' section header was found."""
         if kind_tok.tok_type == "BEHAVIOR_REQUIREMENT_KW":
             self.behavior_kind = components.REQUIREMENT
         else:
             assert kind_tok.tok_type == "BEHAVIOR_CONSTRAINT_KW"
@@ -195,25 +193,21 @@
                 parameters. Checked designs should be added to it after checking.
             _spec: Specification being constructed, source for types and verbs.
         """
         vps = utils.construct_var_param_map(comp_def)
         expr_checker = ExprChecker(vps, self.diag_store)
 
         beh_funcs = []
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
         for pbeh in self.pbehaviors:
             # Store labels of functions for duplicate checking.
             elements_by_label[pbeh.name.tok_text].append(pbeh)
 
             beh_func = components.BehaviorFunction(pbeh.kind, pbeh.name)
-            default_cases: List[
-                "Token"
-            ] = []  # Positions of default cases in this function.
+            default_cases: List["Token"] = []  # Positions of default cases in this function.
             cases_ordered_by_label: Dict[str, List["Token"]] = defaultdict(list)
             for pcase in pbeh.cases:
                 cases_ordered_by_label[pcase.name.tok_text].append(pcase.name)
 
                 # Process conditions.
                 if pcase.whens is None:
                     # Default case.
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,15 @@
         """Forward call to variable group builder."""
         self.vargroup_builder.new_vargroup(name_tok)
 
     def vgroup_add_vars(self, varname_toks: List["Token"]):
         """Forward call to variable group builder."""
         self.vargroup_builder.vgroup_add_vars(varname_toks)
 
-    def add_compinst(
-        self, inst_name_tok: "Token", def_name_tok: "Token", has_arguments: bool
-    ):
+    def add_compinst(self, inst_name_tok: "Token", def_name_tok: "Token", has_arguments: bool):
         """Forward call to component instance builder."""
         self.compinst_builder.add_compinst(inst_name_tok, def_name_tok, has_arguments)
 
     def add_compinst_arguments(self, arguments: List["Token"]):
         """Forward call to component instance builder."""
         self.compinst_builder.add_compinst_arguments(arguments)
 
@@ -246,17 +244,15 @@
         self.compinst_builder.finish_comp(comp_def, spec)
         self.relinst_builder.finish_comp(comp_def, spec)
         self.goal_builder.finish_comp(comp_def, spec)
         self.transform_builder.finish_comp(comp_def, spec)
         self.behavior_builder.finish_comp(comp_def, spec)
         self.design_builder.finish_comp(comp_def, spec)
         self.need_builder.finish_comp(comp_def, spec)
-        self.comment_builder.finish_comp(
-            comp_def, doc_distributor
-        )  # Must be final build step.
+        self.comment_builder.finish_comp(comp_def, doc_distributor)  # Must be final build step.
 
         # Check for unique labels within the scope of each comp_def.
         for labeled_elements in self.elements_by_label.values():
             if len(labeled_elements) > 1:
                 locs = []
                 for elem in labeled_elements:
                     if isinstance(elem, (components.VarParam, CollectedVarGroup)):
@@ -302,25 +298,21 @@
         else:
             spec.comp_defs.append(comp_def)
 
     def notify_parameter_section(self, pos_tok: "Token"):
         """A parameter section was found, check if it is allowed."""
         if self.name_tok is None:  # We're processing 'world'
             # Parameter section not allowed in 'world'.
-            self.diag_store.add(
-                diagnostics.E201("parameter", "world", pos_tok.get_location())
-            )
+            self.diag_store.add(diagnostics.E201("parameter", "world", pos_tok.get_location()))
 
     def notify_transform_section(self, pos_tok: "Token"):
         """A transform section was found, check if it is allowed."""
         if self.name_tok is None:  # We're processing 'world'
             # Transformation section not allowed in 'world'.
-            self.diag_store.add(
-                diagnostics.E201("transformation", "world", pos_tok.get_location())
-            )
+            self.diag_store.add(diagnostics.E201("transformation", "world", pos_tok.get_location()))
 
 
 class ComponentDefBuilder:
     """Builder to construct component definitions of the entire specification. The
     builder keeps a list of component child builders, one for each component definition.
     The latter do all the work for each component definition.
     """
@@ -374,29 +366,25 @@
                 compdefs[name].append(ch_builder)
 
         if len(worlds) == 0:
             self.diag_store.add(diagnostics.E202("world definition"))
         elif len(worlds) > 1:
             locs = [world.pos_tok.get_location() for world in worlds]
             self.diag_store.add(
-                diagnostics.E200(
-                    "world", "component instance", location=locs[0], dupes=locs
-                )
+                diagnostics.E200("world", "component instance", location=locs[0], dupes=locs)
             )
 
         for cdefs in compdefs.values():
             if len(cdefs) > 1:
                 # Duplicate component definitions.
                 locs = [cdef.pos_tok.get_location() for cdef in cdefs]
                 assert cdefs[0].name_tok is not None
                 name = cdefs[0].name_tok.tok_text
                 self.diag_store.add(
-                    diagnostics.E200(
-                        name, "component definition", location=locs[0], dupes=locs
-                    )
+                    diagnostics.E200(name, "component definition", location=locs[0], dupes=locs)
                 )
 
         # Components to use.
         comp_builders = [cdef[0] for cdef in compdefs.values()]
         if len(worlds) > 0:
             comp_builders.append(worlds[0])
 
@@ -425,11 +413,9 @@
 
         if cycle:
             assert entry.data is not None
             locs = [entry.data.pos_tok.get_location() for entry in cycle]
             assert cycle[0].data is not None
             comp_name = cycle[0].data.name_tok.tok_text  # Cannot be world!
             self.diag_store.add(
-                diagnostics.E204(
-                    comp_name, "component definition", location=locs[0], cycle=locs
-                )
+                diagnostics.E204(comp_name, "component definition", location=locs[0], cycle=locs)
             )
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_comment_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_comment_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,15 @@
 
         Arguments:
             comp_def: Component definition to finish.
             doc_distributor: Object that distributes doc comments to interested elements
                 of the specification.
         """
         comp_def_doc_elements = get_doc_comment_comp_elements(comp_def)
-        available = (
-            {}
-        )  # Available elements in the specification, ordered by their name.
+        available = {}  # Available elements in the specification, ordered by their name.
         for elm in comp_def_doc_elements:
             assert elm.doc_tok is not None
             available[elm.doc_tok.tok_text] = elm
 
         for name_tok in self.name_toks:
             # Find language elements to point to by their main name only.
             i = name_tok.tok_text.find(".")
@@ -79,10 +77,8 @@
 
                 # Construct a dummy element so any comment after it is caught.
                 # No errors to report as the above already reported one.
                 doc_distributor.add_dummy_element(name_tok, False)
 
             else:
                 # Add a proxy, redirecting doc comments to the correct element.
-                doc_distributor.add_element(
-                    comment_storage.ProxyDocStore(name_tok, opt_elm)
-                )
+                doc_distributor.add_element(comment_storage.ProxyDocStore(name_tok, opt_elm))
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_compinst_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_compinst_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Builder to add child component instances to a component definition."""
-from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple
 
 from raesl.compile import diagnostics
 from raesl.compile.ast.components import ComponentInstance, InstanceArgument
 from raesl.compile.typechecking import utils
 from raesl.compile.typechecking.type_checker import check_type
 
@@ -30,17 +29,15 @@
 
     def __init__(self, comp_child_builders: "CompDefChildBuilders"):
         self.diag_store = comp_child_builders.diag_store
         self.instances: List[ComponentInstance] = []
         self.comp_child_builders = comp_child_builders
         self.last_instance: Optional[ComponentInstance] = None
 
-    def add_compinst(
-        self, inst_name_tok: "Token", def_name_tok: "Token", has_arguments: bool
-    ):
+    def add_compinst(self, inst_name_tok: "Token", def_name_tok: "Token", has_arguments: bool):
         """Store a new child component instance line."""
         compinst = ComponentInstance(inst_name_tok, def_name_tok)
         self.instances.append(compinst)
         if has_arguments:
             self.last_instance = compinst
         else:
             self.last_instance = None
@@ -72,22 +69,18 @@
         avail_vps = utils.construct_var_param_map(comp_def)
         avail_vgroups = utils.construct_vargroup_map(comp_def)
 
         # The 'other' component definition needed for checking the instance  is
         # already available, as ComponentDefBuilder ordered compdef checking on
         # instance use.
         avail_compdefs = dict(
-            (cdef.name_tok.tok_text, cdef)
-            for cdef in spec.comp_defs
-            if cdef.name_tok is not None
+            (cdef.name_tok.tok_text, cdef) for cdef in spec.comp_defs if cdef.name_tok is not None
         )
 
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
         for inst in self.instances:
             elements_by_label[inst.inst_name_tok.tok_text].append(inst)
 
         # Collection reported names to avoid double problem reports.
         reported_names: Set[str] = set()
 
         # Check 'my' instances.
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_design_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_design_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,32 +34,28 @@
         design.design_kind = self.design_kind
         self.designs.append(design)
 
     def add_design_subclause(self, sub: components.SubClause):
         """Subclause of the last design has been found, append it to the last design."""
         self.designs[-1].sub_clauses.append(sub)
 
-    def finish_comp(
-        self, comp_def: components.ComponentDefinition, _spec: "Specification"
-    ):
+    def finish_comp(self, comp_def: components.ComponentDefinition, _spec: "Specification"):
         """Check the found designs in the context of 'comp_def', and add them after
         verification.
 
         Arguments:
             comp_def: Surrounding component definition supplying variables and
                 parameters. Checked designs should be added to it after checking.
             _spec: Specification being constructed, source for types and verbs.
         """
         vps = utils.construct_var_param_map(comp_def)
         expr_checker = ExprChecker(vps, self.diag_store)
 
         good_designs = []  # Designs that can be added.
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
         for design in self.designs:
             is_good = True
 
             # Order by label for double use checking.
             elements_by_label[design.label_tok.tok_text].append(design)
 
             # Verify comparisons.
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_goal_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_goal_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Code for collecting and adding goals to component definitions."""
-from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
-from raesl.compile import diagnostics
 from raesl.compile.ast import components
 from raesl.compile.typechecking import utils
 from raesl.compile.typechecking.expr_checker import ExprChecker
 from raesl.compile.typechecking.goal_transform_base import GoalTransformBaseBuilder
 
 if TYPE_CHECKING:
     from raesl.compile.ast.specification import Specification
@@ -51,29 +49,25 @@
         goal.goal_kind = self.goal_kind
         self.goals.append(goal)
 
     def add_goal_subclause(self, sub_clause: components.SubClause):
         """Subclause of the last goal has been found, add it to the last goal."""
         self.goals[-1].sub_clauses.append(sub_clause)
 
-    def finish_comp(
-        self, comp_def: components.ComponentDefinition, spec: "Specification"
-    ):
+    def finish_comp(self, comp_def: components.ComponentDefinition, spec: "Specification"):
         """Check the found goals, and add them to the component."""
         vps = utils.construct_var_param_map(comp_def)
         cinsts = utils.construct_comp_instances_map(comp_def)
         vpps = utils.construct_verb_prepos_combis(spec)
 
         expr_checker = ExprChecker(vps, self.diag_store)
 
         # Verify all goals in the component.
         good_goals = []  # Goals without fatal error.
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
         for goal in self.goals:
             is_good = True
             assert goal.goal_kind is not None
             self.check_form("goal", goal.goal_kind, goal.doesaux, goal.sub_clauses)
 
             # Check existence of active and passive components.
             goal.active_comp = self.resolve_component(goal.active, cinsts)
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_need_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_need_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
         """Parser found another need, store it for future processing."""
         need = Need(label_tok, subject_tok, description)
         self.needs.append(need)
 
     def finish_comp(self, comp_def: "ComponentDefinition", _spec: "Specification"):
         """Check the collected needs, and store them in the component definition."""
         # Verify non-duplicated need labels.
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
         for need in self.needs:
             elements_by_label[need.label_tok.tok_text].append(need)
 
         # Construct link to the definition of the subject mentioned in the neEd.
         # If found, add the need to the component definition, else give an error.
         vps = utils.construct_var_param_map(comp_def)
         cinsts = utils.construct_comp_instances_map(comp_def)
@@ -61,17 +59,15 @@
             if rgtdb is not None:
                 # XXX Returned type of rgtdb looks like a subset of allowed subject
                 # types. Check!
                 need.subject = rgtdb
                 comp_def.needs.append(need)
                 continue
 
-            varparam = resolve_var_param_node(
-                need.subject_tok, vps, set(), self.diag_store
-            )
+            varparam = resolve_var_param_node(need.subject_tok, vps, set(), self.diag_store)
             if varparam is not None:
                 if isinstance(varparam, ElementaryVarNode):
                     need.subject = varparam
                     comp_def.needs.append(need)
                     continue
                 else:
                     loc = need.subject_tok.get_location()
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_relinst_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_relinst_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Relation instance type-checking in a component definition."""
-import collections
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union, cast
 
 from raesl.compile import diagnostics
 from raesl.compile.ast import relations
 from raesl.compile.ast.components import InstanceArgument, RelationInstance
 from raesl.compile.typechecking import utils
 from raesl.compile.typechecking.type_checker import check_type
@@ -25,17 +24,15 @@
     of argument lines.
 
     Arguments:
         argkind_tok: Token indicating the kind of arguments specified in the block.
         arg_name_toks: Arguments of the block.
     """
 
-    def __init__(
-        self, argkind_tok: "Token", arg_name_toks: Optional[List["Token"]] = None
-    ):
+    def __init__(self, argkind_tok: "Token", arg_name_toks: Optional[List["Token"]] = None):
         self.argkind_tok = argkind_tok
 
         self.arg_name_toks: List["Token"]
         if arg_name_toks is None:
             self.arg_name_toks = []
         else:
             self.arg_name_toks = arg_name_toks
@@ -134,17 +131,15 @@
         self._add_relation_instance_names()
 
         # Available names of variables, parameters, and variable-groups in the
         # component.
         avail_vps = utils.construct_var_param_map(comp_def)
         avail_vgroups = utils.construct_vargroup_map(comp_def)
 
-        reported_names: Set[
-            str
-        ] = set()  # Names already reported to avoid reporting them again.
+        reported_names: Set[str] = set()  # Names already reported to avoid reporting them again.
 
         # Make access to relation definitions in the specification easy.
         reldefs = dict((reldef.name.tok_text, reldef) for reldef in spec.rel_defs)
 
         # Check instances.
         for relinst in self.relinsts:
             # Look for a definition.
@@ -154,27 +149,23 @@
                 loc = relinst.def_name_tok.get_location()
                 name = relinst.def_name_tok.tok_text
                 self.diag_store.add(
                     diagnostics.E203("relation definition", name=name, location=loc)
                 )
                 continue
 
-            def_parameters = CompDefRelInstBuilder._split_definition_parameters_by_kind(
-                reldef
-            )
+            def_parameters = CompDefRelInstBuilder._split_definition_parameters_by_kind(reldef)
             instkind_groups: Optional[List[RelInstArgGroup]]
             instkind_groups = self._split_instance_arguments_by_kind(
                 relinst, reldef, def_parameters
             )
             if instkind_groups is None:
                 continue
 
-            reldef_param_indices = dict(
-                (rd_param, i) for i, rd_param in enumerate(reldef.params)
-            )
+            reldef_param_indices = dict((rd_param, i) for i, rd_param in enumerate(reldef.params))
             instance_arguments: List[Optional[List[InstanceArgument]]]
             instance_arguments = [None] * len(
                 reldef.params
             )  # Gets filled using 'reldef_param_indices'
 
             found_error = False
             for group in instkind_groups:
@@ -242,17 +233,15 @@
                 )
                 comp_def.relations.append(instance)
 
     def _add_relation_instance_names(self):
         """Check whether the relation instances all have unique instance names, else
         report an error.
         """
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
         for relinst in self.relinsts:
             elements_by_label[relinst.inst_name_tok.tok_text].append(relinst)
 
     @staticmethod
     def _split_definition_parameters_by_kind(
         reldef: relations.RelationDefinition,
     ) -> Dict[str, List[relations.RelationDefParameter]]:
@@ -305,17 +294,15 @@
         # Verify blocks for each kind, instance should have one block if definition has
         # one, else it should have no block.
         for argkind, arg_blocks in inst_blocks.items():
             if not def_parameters[argkind]:
                 # Definition has no arguments for the kind.
                 if arg_blocks:
                     rel_loc = reldef.name.get_location()
-                    block_locs = [
-                        arg_block.argkind_tok.get_location() for arg_block in arg_blocks
-                    ]
+                    block_locs = [arg_block.argkind_tok.get_location() for arg_block in arg_blocks]
                     self.diag_store.add(
                         diagnostics.E206(
                             reldef.name.tok_text,
                             argkind,
                             location=rel_loc,
                             blocks=block_locs,
                         )
@@ -325,27 +312,21 @@
             # Definition has arguments for the kind.
             if not arg_blocks:
                 # But the instance has not.
                 inst_loc = relinst.inst_name_tok.get_location()
                 def_loc = reldef.name.get_location()
                 name = relinst.inst_name_tok.tok_text
                 self.diag_store.add(
-                    diagnostics.E207(
-                        name, argkind, location=inst_loc, definition=def_loc
-                    )
+                    diagnostics.E207(name, argkind, location=inst_loc, definition=def_loc)
                 )
                 return None  # Fatal error.
 
             if len(arg_blocks) > 1:
-                locs = [
-                    arg_block.argkind_tok.get_location() for arg_block in arg_blocks
-                ]
-                diag = diagnostics.E200(
-                    argkind, "parameter block", location=locs[0], dupes=locs
-                )
+                locs = [arg_block.argkind_tok.get_location() for arg_block in arg_blocks]
+                diag = diagnostics.E200(argkind, "parameter block", location=locs[0], dupes=locs)
                 diag.severity = diagnostics.WARN
                 self.diag_store.add(diag)
                 # Not fatal, we merge the blocks below.
 
         groups = []
         for argkind, arg_blocks in inst_blocks.items():
             parameters = def_parameters[argkind]
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_transform_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_transform_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Code for collecting and type checking of transformations."""
-from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
-from raesl.compile import diagnostics
 from raesl.compile.ast import components
 from raesl.compile.typechecking import utils
 from raesl.compile.typechecking.expr_checker import ExprChecker
 from raesl.compile.typechecking.goal_transform_base import GoalTransformBaseBuilder
 
 if TYPE_CHECKING:
     from raesl.compile.ast.components import ComponentDefinition, SubClause
@@ -72,17 +70,15 @@
         vps = utils.construct_var_param_map(comp_def)
         vpps = utils.construct_verb_prepos_combis(spec)
 
         expr_checker = ExprChecker(vps, self.diag_store)
 
         # Verify all transformations in the component.
         good_transforms = []  # Transformations to add to the component.
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
         for trans in self.transforms:
             is_good = True
             assert trans.transform_kind is not None
             self.check_form(
                 "transformation",
                 trans.transform_kind,
                 trans.doesaux_tok,
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_vargroup_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_vargroup_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,44 +73,38 @@
                 definitions processed previously.
         """
         self.last_vgroup = None
 
         avail_varsparams = utils.construct_var_param_map(comp_def)
 
         # Check for duplicates and conflicts with variables and parameters.
-        elements_by_label: Dict[
-            str, List[Any]
-        ] = self.comp_child_builders.elements_by_label
+        elements_by_label: Dict[str, List[Any]] = self.comp_child_builders.elements_by_label
 
         groups_by_label: Dict[str, List[CollectedVarGroup]] = defaultdict(list)
 
         for cgroup in self.collected_var_groups:
             elements_by_label[cgroup.name_tok.tok_text].append(cgroup)
             groups_by_label[cgroup.name_tok.tok_text].append(cgroup)
         for name, vgrps in groups_by_label.items():
             varparam = avail_varsparams.get(name)
             if varparam is not None:
                 vp_loc = varparam.name_tok.get_location()
                 vg_locs = [vgrp.name_tok.get_location() for vgrp in vgrps]
                 kind = {True: "variable", False: "parameter"}[varparam.is_variable]
                 self.diag_store.add(
-                    diagnostics.E209(
-                        name, kind, "variable group", location=vp_loc, others=vg_locs
-                    )
+                    diagnostics.E209(name, kind, "variable group", location=vp_loc, others=vg_locs)
                 )
 
         # Build a dependency graph for the variable groups (as groups may include other
         # groups).
         orderer = Orderer()
         for cgroup in self.collected_var_groups:
             # Build a set required variables, parameters, and variable groups, using
             # non-dotted prefixes.
-            needs = set(
-                get_first_namepart(vtok.tok_text) for vtok in cgroup.child_name_toks
-            )
+            needs = set(get_first_namepart(vtok.tok_text) for vtok in cgroup.child_name_toks)
             orderer.add_dependency(cgroup.name_tok.tok_text, needs, cgroup)
 
         reported: Set[str] = set()  # Reported failures
         vargroups: Dict[str, VariableGroup] = {}  # Resolved variable groups.
 
         resolved, cycle = orderer.resolve()
         for entry in resolved:
@@ -119,17 +113,15 @@
                 # Need entry added by the orderer, ignore.
                 continue
 
             # Next collected group to deal with.
             #
             # Each of its variablepart_names either contains non-dotted previous
             # variable groups, or possibly dotted variables or parameters.
-            content_vgroup: List[
-                Node
-            ] = []  # Result content for the future variable group.
+            content_vgroup: List[Node] = []  # Result content for the future variable group.
             for partname_tok in cgroup.child_name_toks:
                 node = utils.resolve_var_param_group_node(
                     partname_tok,
                     avail_varsparams,
                     vargroups,
                     reported,
                     self.diag_store,
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/compdef_varparam_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/compdef_varparam_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,15 @@
             nodes.
 
     Attributes:
         variables: Variables of the component.
         parameters: Parameters of the component.
     """
 
-    def __init__(
-        self, comp_child_builders: "CompDefChildBuilders", varparam_counter: "Counter"
-    ):
+    def __init__(self, comp_child_builders: "CompDefChildBuilders", varparam_counter: "Counter"):
         self.diag_store: diagnostics.DiagnosticStore = comp_child_builders.diag_store
         self.varparam_counter = varparam_counter
         self.comp_child_builders = comp_child_builders
 
         self.variables: List[components.VarParam] = []
         self.parameters: List[components.VarParam] = []
 
@@ -37,17 +35,15 @@
         """Add variables of the component definition to the collection."""
         self.variables.extend(new_vars)
 
     def add_parameters(self, new_params: List[components.VarParam]):
         """Add parameters of the component definition to the collection."""
         self.parameters.extend(new_params)
 
-    def finish_comp(
-        self, comp_def: components.ComponentDefinition, spec: "Specification"
-    ):
+    def finish_comp(self, comp_def: components.ComponentDefinition, spec: "Specification"):
         """Check the collected variables and parameters, report errors, and add the
         instances to the given component.
 
         Arguments:
             comp_def: Component definition to extend with the found variables and
                 parameters.
             spec: Specification being constructed. Source for types, verbs and relation
@@ -65,36 +61,29 @@
         for name, varsparams in varsparams_by_name.items():
             # Verify properties of the variable or parameter.
             varparam = varsparams[0]
             typename = varparam.type_tok.tok_text
             vartypedef = spec.types.get(typename)
             if vartypedef is None:
                 loc = varparam.name_tok.get_location()
-                self.diag_store.add(
-                    diagnostics.E203("type", name=typename, location=loc)
-                )
+                self.diag_store.add(diagnostics.E203("type", name=typename, location=loc))
             else:
                 # Build node tree for the variable or parameter.
                 varparam.node = _make_varnodes(
                     varparam.name_tok, vartypedef.type, self.varparam_counter
                 )
 
                 # And store it at the right spot in the component definition.
                 if varparam.is_variable:
                     comp_def.variables.append(varparam)
                 else:
                     comp_def.parameters.append(varparam)
 
 
-def _make_varnodes(
-    name_tok: "Token", the_type: types.BaseType, varparam_counter: "Counter"
-):
+def _make_varnodes(name_tok: "Token", the_type: types.BaseType, varparam_counter: "Counter"):
     """Make a VarNode tree that matches the shape of the type."""
     if isinstance(the_type, types.ElementaryType):
         return nodes.ElementaryVarNode(name_tok, the_type, varparam_counter)
     else:
         assert isinstance(the_type, types.Compound)
-        childs = [
-            _make_varnodes(fld.name, fld.type, varparam_counter)
-            for fld in the_type.fields
-        ]
+        childs = [_make_varnodes(fld.name, fld.type, varparam_counter) for fld in the_type.fields]
         return nodes.CompoundVarNode(name_tok, the_type, childs)
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/expr_checker.py` & `raesl-0.12.2/raesl/compile/typechecking/expr_checker.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,20 +91,20 @@
 
         if left_side is None or right_side is None:
             return False
 
         lhs_pos, lhs_type, lhs_units = left_side
         rhs_pos, rhs_type, rhs_units = right_side
 
-        assert (
-            lhs_units is None or len(lhs_units) > 0
-        ), "lhs var {} has wrong units '{}'".format(expr.lhs_var, lhs_units)
-        assert (
-            rhs_units is None or len(rhs_units) > 0
-        ), "rhs varval {} has wrong units '{}'".format(expr.rhs_varval, rhs_units)
+        assert lhs_units is None or len(lhs_units) > 0, "lhs var {} has wrong units '{}'".format(
+            expr.lhs_var, lhs_units
+        )
+        assert rhs_units is None or len(rhs_units) > 0, "rhs varval {} has wrong units '{}'".format(
+            expr.rhs_varval, rhs_units
+        )
 
         # Check type compatibility.
         if lhs_type and rhs_type:
             # The lhs and rhs must be compatible in left -> right or in
             # right -> left direction. Additional subtype limits isn't a
             # problem, although it may result in a comparison that can
             # never hold.
@@ -153,30 +153,30 @@
         Returns:
             Information about the checked side. None means an error has been reported,
                 otherwise a triplet of token, type, and supported units is returned
                 for as far as the side supports each notion.
         """
         if isinstance(side, Value):
             units = side.get_units()
-            assert (
-                units is None or len(units) > 0
-            ), "Value {} has wrong units '{}'".format(side, units)
+            assert units is None or len(units) > 0, "Value {} has wrong units '{}'".format(
+                side, units
+            )
             return side.value, None, units
 
         else:
             assert isinstance(side, VariableValue)
             if not self._check_variable(side):
                 return None
 
             assert isinstance(side.var_node, VarNode)
             typ = side.var_node.the_type
             units = typ.get_units()
-            assert (
-                units is None or len(units) > 0
-            ), "Type {} has wrong units '{}'".format(typ, units)
+            assert units is None or len(units) > 0, "Type {} has wrong units '{}'".format(
+                typ, units
+            )
 
             return side.var_tok, typ, units
 
     def _check_variable(self, var: VariableValue) -> bool:
         """Check that the variable exists in the context.
 
         Arguments:
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/goal_transform_base.py` & `raesl-0.12.2/raesl/compile/typechecking/goal_transform_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,17 +52,15 @@
             vps: Available variables and parameters in the component.
 
         Returns:
             Whether all flows can be matched to a variable or parameter.
         """
         is_good = True
         for flow in flows:
-            node = resolve_var_param_node(
-                flow.name_tok, vps, self.reported_names, self.diag_store
-            )
+            node = resolve_var_param_node(flow.name_tok, vps, self.reported_names, self.diag_store)
             if node is None:
                 is_good = False
             else:
                 flow.flow_node = node
 
         return is_good
 
@@ -72,17 +70,15 @@
         """Find a component instance with the provided instance name. If it exists,
         return it, else report an error and return None, indicating failure.
         """
         compinst = cinsts.get(compinst_tok.tok_text)
         if compinst is None:
             loc = compinst_tok.get_location()
             self.diag_store.add(
-                diagnostics.E203(
-                    "component instance", name=compinst_tok.tok_text, location=loc
-                )
+                diagnostics.E203("component instance", name=compinst_tok.tok_text, location=loc)
             )
 
         return compinst
 
     def check_form(
         self,
         sect_name: str,
@@ -108,17 +104,15 @@
         for sub in sub_clauses:
             subclauses_by_label[sub.label_tok.tok_text].append(sub)
         for clauses in subclauses_by_label.values():
             if len(clauses) > 1:
                 locs = [sub.label_tok.get_location() for sub in clauses]
                 name = clauses[0].label_tok.tok_text
                 self.diag_store.add(
-                    diagnostics.E200(
-                        name, "subclause label", location=locs[0], dupes=locs
-                    )
+                    diagnostics.E200(name, "subclause label", location=locs[0], dupes=locs)
                 )
 
         # Check kind-specific requirements.
         if kind == components.CONSTRAINT:
             if doesaux.tok_type != "DOES_KW":
                 loc = doesaux.get_location()
                 self.diag_store.add(
@@ -149,40 +143,34 @@
                 )
 
             for sub in sub_clauses:
                 self._check_requirement_expr(sub.expr)
 
     def _check_constraint_expr(
         self,
-        expr: Union[
-            exprs.Disjunction, exprs.RelationComparison, exprs.ObjectiveComparison
-        ],
+        expr: Union[exprs.Disjunction, exprs.RelationComparison, exprs.ObjectiveComparison],
     ):
         """Check whether the subclauses have the proper form for a constraint section.
         Report an error if something wrong is found.
         """
         if isinstance(expr, exprs.Disjunction):
             for child in expr.childs:
                 self._check_constraint_expr(child)
 
         elif isinstance(expr, exprs.RelationComparison):
             if expr.isaux_tok.tok_type != "IS_KW":
                 loc = expr.isaux_tok.get_location()
                 self.diag_store.add(
-                    diagnostics.E212(
-                        "subclause", expr.isaux_tok.tok_text, "'is'", location=loc
-                    )
+                    diagnostics.E212("subclause", expr.isaux_tok.tok_text, "'is'", location=loc)
                 )
 
             if expr.math_compare == "~":
                 loc = expr.cmp_tok.get_location()
                 self.diag_store.add(
-                    diagnostics.E212(
-                        "subclause", "approximately", "hard limits", location=loc
-                    )
+                    diagnostics.E212("subclause", "approximately", "hard limits", location=loc)
                 )
 
         elif isinstance(expr, exprs.ObjectiveComparison):
             loc = expr.aux_tok.get_location()
             if expr.maximize:
                 obj_text = "maximize"
             else:
@@ -193,17 +181,15 @@
             )
 
         else:
             assert False, "Found unexpected expression node :" + repr(expr)
 
     def _check_requirement_expr(
         self,
-        expr: Union[
-            exprs.Disjunction, exprs.RelationComparison, exprs.ObjectiveComparison
-        ],
+        expr: Union[exprs.Disjunction, exprs.RelationComparison, exprs.ObjectiveComparison],
     ):
         """Check whether the subclauses have the proper form for a requirement section.
         Report an error if something wrong is found.
         """
         if isinstance(expr, exprs.Disjunction):
             for child in expr.childs:
                 self._check_requirement_expr(child)
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/orderer.py` & `raesl-0.12.2/raesl/compile/typechecking/orderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         _dependent_entries: Entries that depend on other entries.
     """
 
     def __init__(self) -> None:
         self._independent_entries: Dict[str, OrdererEntry] = {}
         self._dependent_entries: Dict[str, OrdererEntry] = {}
 
-    def add_dependency(
-        self, provide: str, needs: Iterable[str], data: TypeOfData = None
-    ):
+    def add_dependency(self, provide: str, needs: Iterable[str], data: TypeOfData = None):
         """Add a dependency where the 'provide' name depends on the 'needs' names.
 
         Arguments:
             provide: Name of the 'thing' that this dependency provides.
             needs: Names of 'things' that are required by the provide 'thing'.
             data: Optional data associated with 'provide'. At most one such data item
                 should exist, class cannot handle multiple data items.
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/reldef_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/reldef_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,31 +78,27 @@
             direction_text = {
                 INPUT: "require",
                 OUTPUT: "returning",
                 INPOUT: "relating",
             }[direction]
             locs = [header_tok.get_location(), last_occurrence.get_location()]
             self.diag_store.add(
-                diagnostics.E200(
-                    direction_text, "parameter section", location=locs[0], dupes=locs
-                )
+                diagnostics.E200(direction_text, "parameter section", location=locs[0], dupes=locs)
             )
             # Continue anyway
 
         self.last_occurrences[direction] = header_tok
         self.current_direction = direction
 
     def reldef_add_param(self, name: "Token", type_name: "Token", multi: bool):
         """Add a parameter to the current relation definition."""
         assert self.current_direction is not None
         assert self.current_reldef is not None
 
-        rel_param = relations.RelationDefParameter(
-            name, type_name, self.current_direction, multi
-        )
+        rel_param = relations.RelationDefParameter(name, type_name, self.current_direction, multi)
         self.current_reldef.params.append(rel_param)
 
     def finish(self, spec: "Specification"):
         """Check the relation definitions and add them to the result specification."""
         reldef_texts: Dict[
             str, "Token"
         ] = {}  # Map of defined names for relation definitions to their token.
@@ -121,22 +117,18 @@
                     )
                 )
                 continue
 
             reldef_texts[reldef_text] = rel_def.name
 
             # Verify parameters.
-            multi_value_params: Dict[
-                str, List[relations.RelationDefParameter]
-            ] = defaultdict(
+            multi_value_params: Dict[str, List[relations.RelationDefParameter]] = defaultdict(
                 list
             )  # Multi-value params in each direction.
-            param_texts: Dict[
-                str, "Token"
-            ] = {}  # Map of defined parameter names to their token.
+            param_texts: Dict[str, "Token"] = {}  # Map of defined parameter names to their token.
             for param in rel_def.params:
                 # Register multi-value params.
                 if param.multi:
                     multi_value_params[param.direction].append(param)
 
                 # Check unique name.
                 param_text = param.name.tok_text
@@ -158,17 +150,15 @@
                 param_texts[param_text] = param.name
 
                 # check type.
                 type_text = param.type_name.tok_text
                 typedef = spec.types.get(type_text)
                 if typedef is None:
                     loc = param.type_name.get_location()
-                    self.diag_store.add(
-                        diagnostics.E203("type", name=type_text, location=loc)
-                    )
+                    self.diag_store.add(diagnostics.E203("type", name=type_text, location=loc))
 
                     param.type = None
                 else:
                     param.type = typedef.type
 
             # Verify lack of more than one multi-value parameter in each direction.
             found_fatal = False
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/type_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/type_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,17 +287,15 @@
                 or (cons_spec is not None)
             )
 
             if not isinstance(parent_type, types.ElementaryType):
                 # Parent is a compound, type cannot be extended.
                 if is_extended:
                     self.diag_store.add(
-                        diagnostics.E215(
-                            parent_name.tok_text, location=parent_name.get_location()
-                        )
+                        diagnostics.E215(parent_name.tok_text, location=parent_name.get_location())
                     )
                     return None
 
                 return parent_type
 
             # Parent is an elementary type.
             if not is_extended and prefer_parent:
@@ -325,27 +323,23 @@
                     return None
                 if unit_text == "-":
                     self.diag_store.add(diagnostics.E217(location=unit.get_location()))
                     return None
 
                 if unit_text in available_units:
                     self.diag_store.add(
-                        diagnostics.W200(
-                            unit.tok_text, "unit", location=unit.get_location()
-                        )
+                        diagnostics.W200(unit.tok_text, "unit", location=unit.get_location())
                     )
                     continue  # Silently discard duplicates.
 
                 type_units.append(unit)
                 available_units[unit_text] = unit
 
         # Build intervals
-        type_intervals: Optional[
-            List[Tuple[Optional[exprs.Value], Optional[exprs.Value]]]
-        ]
+        type_intervals: Optional[List[Tuple[Optional[exprs.Value], Optional[exprs.Value]]]]
         type_intervals = None
 
         if ival_spec:
             type_intervals = ival_spec
 
         if enum_spec:
             assert not type_intervals
@@ -381,17 +375,15 @@
         if type_name.tok_text in STANDARD_TYPE_NAMES:
             self.diag_store.add(
                 diagnostics.E218(type_name.tok_text, location=type_name.get_location)
             )
             return True
         return False
 
-    def _make_typedef(
-        self, tdef: TempTypeDef, resolved_types: Dict[str, types.TypeDef]
-    ):
+    def _make_typedef(self, tdef: TempTypeDef, resolved_types: Dict[str, types.TypeDef]):
         """Add the type definition to the resolved collection. It is assumed the
         dependencies are already available (as ensured by the Orderer).
         """
         if self._check_override_standard_type(tdef.type_name):
             return  # Something failed and was reported.
 
         new_type = self._construct_type(
@@ -408,17 +400,15 @@
             self.types_with_error[tdef.type_name.tok_text] = tdef.type_name
             return  # Something failed and was reported.
 
         typedef = types.TypeDef(tdef.type_name, new_type)
         assert typedef.name.tok_text not in resolved_types
         resolved_types[typedef.name.tok_text] = typedef
 
-    def _make_bundledef(
-        self, bdef: TempBundleDef, resolved_types: Dict[str, types.TypeDef]
-    ):
+    def _make_bundledef(self, bdef: TempBundleDef, resolved_types: Dict[str, types.TypeDef]):
         """Add the bundle definition to the resolved collection. It is assumed the
         dependencies are already available (as ensured by the Orderer).
         """
         if self._check_override_standard_type(bdef.bundle_name):
             return
 
         fields = []
@@ -462,17 +452,15 @@
         parent_name: Optional["Token"],
         enum_spec: Optional[List[exprs.Value]],
         unit_spec: Optional[List["Token"]],
         ival_spec: Optional[List[Tuple[Optional[exprs.Value], Optional[exprs.Value]]]],
         cons_spec: Optional[exprs.Value],
     ):
         """The parser found a new type definition entry, store it."""
-        temp_tdef = TempTypeDef(
-            type_name, parent_name, enum_spec, unit_spec, ival_spec, cons_spec
-        )
+        temp_tdef = TempTypeDef(type_name, parent_name, enum_spec, unit_spec, ival_spec, cons_spec)
         self.type_defs.append(temp_tdef)
         self.current_bundle = None
 
     def new_bundle_type(self, bundle_name: "Token"):
         """The parser found a new bundle in the source code, create it."""
         temp_bdef = TempBundleDef(bundle_name)
         self.bundle_defs.append(temp_bdef)
@@ -481,22 +469,18 @@
     def add_bundle_field(
         self,
         field_name: "Token",
         type_name: Optional["Token"],
     ):
         """A new field in the current bundle has been found by the parser, add it."""
         temp_fdef = TempFieldDef(field_name, type_name)
-        assert (
-            self.current_bundle
-        ), "Trying to add a bundle field outside a type section."
+        assert self.current_bundle, "Trying to add a bundle field outside a type section."
         self.current_bundle.bundle_fields.append(temp_fdef)
 
-    def check_unit(
-        self, value: Optional[exprs.Value], available_units: Dict[str, "Token"]
-    ) -> None:
+    def check_unit(self, value: Optional[exprs.Value], available_units: Dict[str, "Token"]) -> None:
         """Check whether the unit possibly specified in 'value' is available for use.
         Report an error if it is not available.
         """
         if value is None or value.unit is None:
             return
 
         units = value.get_units()
@@ -505,10 +489,8 @@
 
         if units.intersection(available_units):
             return  # Value uses a known unit.
 
         unit_text = value.unit.tok_text
         if unit_text.startswith("[") and unit_text.endswith("]"):
             unit_text = unit_text[1:-1]
-        self.diag_store.add(
-            diagnostics.E219(unit_text, location=value.unit.get_location())
-        )
+        self.diag_store.add(diagnostics.E219(unit_text, location=value.unit.get_location()))
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/type_checker.py` & `raesl-0.12.2/raesl/compile/typechecking/type_checker.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/compile/typechecking/utils.py` & `raesl-0.12.2/raesl/compile/typechecking/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,32 +106,27 @@
     Construct a set with all defined verb/prepos combinations.
     """
     return set((vpp.verb.tok_text, vpp.prepos.tok_text) for vpp in spec.verb_prepos)
 
 
 def construct_relinst_goal_transform_design_behavior_map(
     comp_def: "ComponentDefinition",
-) -> Dict[
-    str,
-    Union["RelationInstance", "Goal", "Transformation", "Design", "BehaviorFunction"],
-]:
+) -> Dict[str, Union["RelationInstance", "Goal", "Transformation", "Design", "BehaviorFunction"],]:
     """Construct a dict to quickly find goals, transformations, designs, and behaviors
     by their label name.
 
     Arguments:
         comp_def: Definition to search.
 
     Returns:
         Dictionary of labels to their goals, transformations, designs, and behaviors.
     """
     label_map: Dict[
         str,
-        Union[
-            "RelationInstance", "Goal", "Transformation", "Design", "BehaviorFunction"
-        ],
+        Union["RelationInstance", "Goal", "Transformation", "Design", "BehaviorFunction"],
     ]
     label_map = {}
     for relinst in comp_def.relations:
         label_map[relinst.inst_name_tok.tok_text] = relinst
     for goal in comp_def.goals:
         label_map[goal.label_tok.tok_text] = goal
     for trans in comp_def.transforms:
@@ -158,17 +153,15 @@
         reported_names: Non-existing names and prefixes that are reported already.
         diag_store: Storage for found diagnostics.
 
     Returns:
         The node represented by the name, or None if it could not be found.
             In the latter case, an problem exists indicating failure to find the node.
     """
-    node = resolve_var_param_group_node(
-        name_tok, avail_vps, None, reported_names, diag_store
-    )
+    node = resolve_var_param_group_node(name_tok, avail_vps, None, reported_names, diag_store)
     if node is None:
         return None
     assert isinstance(node, VarNode)
     return node
 
 
 def resolve_var_param_group_node(
@@ -250,12 +243,10 @@
             if avail_vgroups is not None:
                 kind = "variable, parameter, or variable group instance"
             else:
                 kind = "variable or parameter instance"
         else:
             assert avail_vgroups is not None, "Must have at least one set of names."
             kind = "variable group instance"
-        diag_store.add(
-            diagnostics.E203(kind, name=first_part, location=name_tok.get_location())
-        )
+        diag_store.add(diagnostics.E203(kind, name=first_part, location=name_tok.get_location()))
 
     return None
```

### Comparing `raesl-0.12.1/raesl/compile/typechecking/verb_builder.py` & `raesl-0.12.2/raesl/compile/typechecking/verb_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/datasets/__init__.py` & `raesl-0.12.2/raesl/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/doc/__init__.py` & `raesl-0.12.2/raesl/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/doc/cli.py` & `raesl-0.12.2/raesl/doc/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import raesl.doc
 from raesl import logger
 
 run = raesl.doc.convert
 
 
 @click.command("doc")
-@click.argument(
-    "paths", nargs=-1, type=click.Path(exists=True, file_okay=True, dir_okay=True)
-)
+@click.argument("paths", nargs=-1, type=click.Path(exists=True, file_okay=True, dir_okay=True))
 @click.option(
     "--output",
     "-o",
     default=raesl.doc.OUTPUT,
     type=click.Path(file_okay=True, dir_okay=False, writable=True),
     help="Output file to write to.",
 )
@@ -78,17 +76,15 @@
     epilogue: Optional[str],
     rich: Optional[str],
     force: bool,
     dry: bool,
 ):
     """Convert ESL files and/or directories to a formatted document."""
     logger.info("This is the Ratio ESL Doc command line utility.")
-    logger.info(
-        f"Populating '{output}', titled as '{title}' in language '{language}'..."
-    )
+    logger.info(f"Populating '{output}', titled as '{title}' in language '{language}'...")
     try:
         run(
             *paths,
             output=output,
             language=language,
             title=title,
             prologue=prologue,
```

### Comparing `raesl-0.12.1/raesl/doc/doc.py` & `raesl-0.12.2/raesl/doc/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         Document metadata. See pandoc documentation.
     """
 
     # Format used when exporting to a Markdown file.
     markdown_file_format = "markdown+table_captions+multiline_tables+pipe_tables"
 
     # Format used in Doc generation.
-    markdown_generated = (
-        "markdown+table_captions+multiline_tables+pipe_tables+grid_tables"
-    )
+    markdown_generated = "markdown+table_captions+multiline_tables+pipe_tables+grid_tables"
 
     def __init__(
         self,
         *paths: Union[str, Path],
         language: str = "en",
         prologue: Optional[Path] = None,
         epilogue: Optional[Path] = None,
@@ -171,20 +169,16 @@
                 self.pars.append(Par(lns.lines(comp, h=h + 1)))
                 self.pars.append(Par(secs.comp_node_props(comp, g, h + 2)))
                 if self.goal_section:
                     self.pars.append(Par(secs.comp_node_goal_reqs(comp, g, h + 2)))
                     self.pars.append(Par(secs.comp_node_goal_cons(comp, g, h + 2)))
 
                 if self.transformation_section:
-                    self.pars.append(
-                        Par(secs.comp_node_transformation_reqs(comp, g, h + 2))
-                    )
-                    self.pars.append(
-                        Par(secs.comp_node_transformation_cons(comp, g, h + 2))
-                    )
+                    self.pars.append(Par(secs.comp_node_transformation_reqs(comp, g, h + 2)))
+                    self.pars.append(Par(secs.comp_node_transformation_cons(comp, g, h + 2)))
 
                 if self.behavior_section:
                     self.pars.append(Par(secs.comp_node_behavior_reqs(comp, g, h + 2)))
                     self.pars.append(Par(secs.comp_node_behavior_cons(comp, g, h + 2)))
 
                 if self.design_section:
                     self.pars.append(Par(secs.comp_node_design_reqs(comp, g, h + 2)))
@@ -203,20 +197,16 @@
                 children.extend(comp.children)
             comps = children
             depth += 1
 
         # Check for any miscellaneous needs and design specifications that haven't
         # been printed yet.
         gn = [line for line in secs.global_needs(g, h + 1) if self.need_section]
-        gdr = [
-            line for line in secs.global_design_reqs(g, h + 1) if self.design_section
-        ]
-        gdc = [
-            line for line in secs.global_design_cons(g, h + 1) if self.design_section
-        ]
+        gdr = [line for line in secs.global_design_reqs(g, h + 1) if self.design_section]
+        gdc = [line for line in secs.global_design_cons(g, h + 1) if self.design_section]
         if len(gn) > 0 or len(gdr) > 0 or len(gdc) > 0:
             self.pars.append(Par(secs.global_needs_and_designs(h)))
             self.pars.append(Par(gn))
             self.pars.append(Par(gdr))
             self.pars.append(Par(gdc))
 
         if self.epilogue:
@@ -286,15 +276,14 @@
         if (to == "tex" or to == "pdf") and self.rich == "md":
             self.rich = "tex"
             self.parse_esl()
 
         if logger.level <= logging.DEBUG and to != "md":
             logger.debug("Saving Markdown file for debugging purposes...")
             try:
-
                 pypandoc.convert_text(
                     self.as_markdown,
                     self.markdown_file_format,
                     format=self.markdown_generated,
                     outputfile=str(path.with_suffix(".md")),
                     encoding="utf-8",
                     extra_args=pandoc_args,
```

### Comparing `raesl-0.12.1/raesl/doc/lines.py` & `raesl-0.12.2/raesl/doc/lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,15 @@
     if sizing:
         attrs += " {}".format(sizing)
     if attrs:
         line += "{" + attrs + "}"
     return line + "\n\n"
 
 
-def node_path(
-    path: str, italic: bool = False, arrows: bool = True, skip: str = "world"
-):
+def node_path(path: str, italic: bool = False, arrows: bool = True, skip: str = "world"):
     """Get a friendly representation of a node path."""
     skips = skip.split(".")
     for skip in skips:
         if path.startswith(skip):
             idx = len(skip) + 1
             path = path[idx:]
         else:
@@ -230,19 +228,15 @@
 
 def component_node(node: Node, h: int) -> LineGen:
     """Yield component section"""
     nameparts = node.name.split(".")
     yield header(h, "{}".format(nameparts[-1]))
     yield snt(_("this section describes **{}**".format(nameparts[-1])))
     if node.parent.name != "world":
-        yield snt(
-            _("this component is a sub-component of {}").format(
-                node_path(node.parent.name)
-            )
-        )
+        yield snt(_("this component is a sub-component of {}").format(node_path(node.parent.name)))
 
     comments = node.annotations.esl_info.get("comments", [])
     if comments:
         yield "\n"
         yield boldhead(_("comments")).replace("\n", "")
         yield "\n"
         yield from comments
```

### Comparing `raesl-0.12.1/raesl/doc/locales/__init__.py` & `raesl-0.12.2/raesl/doc/locales/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
 def list_locales():
     """List available locales."""
     from pathlib import Path
 
     here = Path(__file__).parent
     return list(
-        p.stem
-        for p in here.glob("*")
-        if p.suffix == ".py" and p.name not in {"__init__.py"}
+        p.stem for p in here.glob("*") if p.suffix == ".py" and p.name not in {"__init__.py"}
     )
 
 
 def register_locale(locale: str = "en"):
     """Register a locale. Existing locales are re-registered."""
     if pm.has_plugin(locale):
         pm.unregister(name=locale)
```

### Comparing `raesl-0.12.1/raesl/doc/locales/en.py` & `raesl-0.12.2/raesl/doc/locales/en.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,34 +80,30 @@
             items=sorted(
                 list(
                     set(
                         [
                             graph[flow].annotations.esl_info["bundle_root_name"]
                             if graph[flow].annotations.esl_info["bundle_root_name"]
                             else flow.split(".")[-1]
-                            for flow in node.annotations.esl_info["body"][
-                                "input_variables"
-                            ]
+                            for flow in node.annotations.esl_info["body"]["input_variables"]
                         ]
                     )
                 )
             )
         )
         prep = node.annotations.esl_info["body"]["preposition"]
         out_flows = pm.hook.linguistic_enumeration(
             items=sorted(
                 list(
                     set(
                         [
                             graph[flow].annotations.esl_info["bundle_root_name"]
                             if graph[flow].annotations.esl_info["bundle_root_name"]
                             else flow.split(".")[-1]
-                            for flow in node.annotations.esl_info["body"][
-                                "output_variables"
-                            ]
+                            for flow in node.annotations.esl_info["body"]["output_variables"]
                         ]
                     )
                 )
             )
         )
         line = "{} {} {} {} {} {}".format(comp, aux, verb, in_flows, prep, out_flows)
 
@@ -167,48 +163,39 @@
 
 @hookimpl
 def design_spec_node(node: Node, graph: Graph) -> LineGen:
     line = " or ".join([design_rule_line(r) for r in node.annotations.esl_info["body"]])
     if node.annotations.esl_info.get("sub_clauses", "node"):
         yield lns.cap(line) + ", with subclauses:\n"
         yield from lns.unordered(
-            [
-                "\n".join(subclause_line(s=sc))
-                for sc in node.annotations.esl_info["sub_clauses"]
-            ]
+            ["\n".join(subclause_line(s=sc)) for sc in node.annotations.esl_info["sub_clauses"]]
         )
     else:
         yield lns.snt(line)
 
     bvars = [
         v
-        for v in lns.get_design_rule_line_vars(
-            rules=node.annotations.esl_info["body"], g=graph
-        )
+        for v in lns.get_design_rule_line_vars(rules=node.annotations.esl_info["body"], g=graph)
         if v.annotations.esl_info["bundle_root_name"]
     ]
 
     if bvars:
         yield from lns.var_clarification(bvars=bvars)
 
 
 @hookimpl
 def behavior_spec_node(node: Node, graph: Graph) -> LineGen:
     clauses = []
     for case in node.annotations.esl_info["cases"]:
         yield lns.cap("case {}:\n".format(lns.emph(case["name"])))
         yield ""
         yield "when:\n"
-        yield from lns.unordered(
-            ["\n".join(subclause_line(s=sc)) for sc in case["when_clauses"]]
-        )
+        yield from lns.unordered(["\n".join(subclause_line(s=sc)) for sc in case["when_clauses"]])
         yield "then:\n"
-        yield from lns.unordered(
-            ["\n".join(subclause_line(s=sc)) for sc in case["then_clauses"]]
-        )
+        yield from lns.unordered(["\n".join(subclause_line(s=sc)) for sc in case["then_clauses"]])
         clauses += case["when_clauses"] + case["then_clauses"]
 
     default = node.annotations.esl_info.get("default")
     if default:
         yield lns.cap("case {}:\n".format(lns.emph("default")))
         yield ""
         yield "when no other case applies, then:\n"
```

### Comparing `raesl-0.12.1/raesl/doc/locales/nl.py` & `raesl-0.12.2/raesl/doc/locales/nl.py`

 * *Files 12% similar despite different names*

```diff
@@ -190,17 +190,15 @@
     else:
         value = r["bound"]["value"].split(".")[-1]
     unit = ""
     if r["bound"]["unit"]:
         unit = r["bound"]["unit"]
 
     if r["auxiliary"] == "won't":
-        return "{} {} nimmer {} {} {} {}".format(
-            s, aux[0], comparison, value, unit, aux[1]
-        )
+        return "{} {} nimmer {} {} {} {}".format(s, aux[0], comparison, value, unit, aux[1])
     else:
         return "{} {} {} {} {} {}".format(s, aux[0], comparison, value, unit, aux[1])
 
 
 def then_clause_line(s: Dict[str, Any]):
     """Yield subclause line."""
 
@@ -219,17 +217,15 @@
     else:
         value = r["bound"]["value"].split(".")[-1]
     unit = ""
     if r["bound"]["unit"]:
         unit = r["bound"]["unit"]
 
     if r["auxiliary"] == "won't":
-        return "{} {} nimmer {} {} {} {}".format(
-            s, aux[0], comparison, value, unit, aux[1]
-        )
+        return "{} {} nimmer {} {} {} {}".format(s, aux[0], comparison, value, unit, aux[1])
     else:
         return "{} {} {} {} {} {}".format(aux[0], s, comparison, value, unit, aux[1])
 
 
 srule_auxmap = {
     "must be": "dient te zijn",
     "shall be": "zal zijn",
@@ -271,65 +267,53 @@
             items=sorted(
                 list(
                     set(
                         [
                             graph[flow].annotations.esl_info["bundle_root_name"]
                             if graph[flow].annotations.esl_info["bundle_root_name"]
                             else flow.split(".")[-1]
-                            for flow in node.annotations.esl_info["body"][
-                                "input_variables"
-                            ]
+                            for flow in node.annotations.esl_info["body"]["input_variables"]
                         ]
                     )
                 )
             )
         )
         prep = node.annotations.esl_info["body"]["preposition"]
         out_flows = pm.hook.linguistic_enumeration(
             items=sorted(
                 list(
                     set(
                         [
                             graph[flow].annotations.esl_info["bundle_root_name"]
                             if graph[flow].annotations.esl_info["bundle_root_name"]
                             else flow.split(".")[-1]
-                            for flow in node.annotations.esl_info["body"][
-                                "output_variables"
-                            ]
+                            for flow in node.annotations.esl_info["body"]["output_variables"]
                         ]
                     )
                 )
             )
         )
         if aux == "must":
             line = "{} dient {} {} {} {}".format(
                 comp, in_flows, prep, out_flows, make_predicate(verb)
             )
         elif aux == "should":
             line = "{} behoort {} {} {} {}".format(
                 comp, in_flows, prep, out_flows, make_predicate(verb)
             )
         elif aux == "could":
-            line = "{} zou {} {} {} kunnen {}".format(
-                comp, in_flows, prep, out_flows, verb
-            )
+            line = "{} zou {} {} {} kunnen {}".format(comp, in_flows, prep, out_flows, verb)
         elif aux == "won't":
-            line = "{} zal nimmer {} {} {} {}".format(
-                comp, in_flows, prep, out_flows, verb
-            )
+            line = "{} zal nimmer {} {} {} {}".format(comp, in_flows, prep, out_flows, verb)
         elif aux == "shall":
             line = "{} zal {} {} {} {}".format(comp, in_flows, prep, out_flows, verb)
         elif aux == "is":
-            line = "{} vervult het {} van {} {} {}".format(
-                comp, verb, in_flows, prep, out_flows
-            )
+            line = "{} vervult het {} van {} {} {}".format(comp, verb, in_flows, prep, out_flows)
         else:
-            line = "{} {} {} {} {} {}".format(
-                comp, aux, verb, in_flows, prep, out_flows
-            )
+            line = "{} {} {} {} {} {}".format(comp, aux, verb, in_flows, prep, out_flows)
 
         # Bundle root varaible dict
         brvdict = defaultdict(list)
         for flow in (
             node.annotations.esl_info["body"]["input_variables"]
             + node.annotations.esl_info["body"]["output_variables"]
         ):
@@ -355,33 +339,25 @@
                 )
             )
         )
         prep = node.annotations.esl_info["body"]["preposition"]
         passive = node.annotations.esl_info["body"]["passive"].split(".")[-1]
 
         if aux == "must":
-            line = "{} dient {} {} {} {}".format(
-                active, flows, prep, passive, make_predicate(verb)
-            )
+            line = "{} dient {} {} {} {}".format(active, flows, prep, passive, make_predicate(verb))
         elif aux == "should":
             line = "{} behoort {} {} {} {}".format(
                 active, flows, prep, passive, make_predicate(verb)
             )
         elif aux == "could":
-            line = "{} zou {} {} {} kunnen {}".format(
-                active, flows, prep, passive, verb
-            )
+            line = "{} zou {} {} {} kunnen {}".format(active, flows, prep, passive, verb)
         elif aux == "won't":
-            line = "{} zal nimmer {} {} {} {}".format(
-                active, flows, prep, passive, verb
-            )
+            line = "{} zal nimmer {} {} {} {}".format(active, flows, prep, passive, verb)
         elif aux == "does":
-            line = "{} vervult het {} van {} {} {}".format(
-                active, verb, flows, prep, passive
-            )
+            line = "{} vervult het {} van {} {} {}".format(active, verb, flows, prep, passive)
         elif aux == "shall":
             line = "{} zal {} {} {} {}".format(active, flows, prep, passive, verb)
         else:
             line = "{} {} {} {} {} {}".format(
                 active, aux, make_predicate(verb), flows, prep, passive
             )
 
@@ -409,48 +385,39 @@
 
 @hookimpl
 def design_spec_node(node: Node, graph: Graph) -> LineGen:
     line = " of ".join([design_rule_line(r) for r in node.annotations.esl_info["body"]])
     if node.annotations.esl_info.get("sub_clauses"):
         yield lns.cap(line) + ", waarbij:\n"
         yield from lns.unordered(
-            [
-                "\n".join(subclause_line(s=sc))
-                for sc in node.annotations.esl_info["sub_clauses"]
-            ]
+            ["\n".join(subclause_line(s=sc)) for sc in node.annotations.esl_info["sub_clauses"]]
         )
     else:
         yield lns.snt(line)
 
     bvars = [
         v
-        for v in lns.get_design_rule_line_vars(
-            rules=node.annotations.esl_info["body"], g=graph
-        )
+        for v in lns.get_design_rule_line_vars(rules=node.annotations.esl_info["body"], g=graph)
         if v.annotations.esl_info["bundle_root_name"]
     ]
 
     if bvars:
         yield from lns.var_clarification(bvars=bvars)
 
 
 @hookimpl
 def behavior_spec_node(node: Node, graph: Graph) -> LineGen:
     clauses = []
     for case in node.annotations.esl_info["cases"]:
         yield lns.cap("situatie {}:\n".format(lns.emph(case["name"])))
         yield ""
         yield "als:\n"
-        yield from lns.unordered(
-            ["\n".join(subclause_line(s=sc)) for sc in case["when_clauses"]]
-        )
+        yield from lns.unordered(["\n".join(subclause_line(s=sc)) for sc in case["when_clauses"]])
         yield "dan:\n"
-        yield from lns.unordered(
-            ["\n".join(then_clause_line(s=sc)) for sc in case["then_clauses"]]
-        )
+        yield from lns.unordered(["\n".join(then_clause_line(s=sc)) for sc in case["then_clauses"]])
         clauses += case["when_clauses"] + case["then_clauses"]
 
     default = node.annotations.esl_info.get("default")
     if default:
         yield lns.cap("situatie {}:\n".format(lns.emph("default")))
         yield ""
         yield "als geen andere situatie van toepassing is, dan:\n"
```

### Comparing `raesl-0.12.1/raesl/doc/rich.py` & `raesl-0.12.2/raesl/doc/rich.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
 
     Yields:
         Rich output lines.
     """
     logger.debug("Generating MDM for depth {}...".format(depth))
 
-    img_dir = Path(
-        img_dir if img_dir is not None else rich_opts.get("img_dir", IMG_DIR)
-    )
+    img_dir = Path(img_dir if img_dir is not None else rich_opts.get("img_dir", IMG_DIR))
     img_dir.mkdir(parents=True, exist_ok=True)
 
     level = depth + 1
 
     style = raesl.plot.Style(
         ragraph=dict(
             piemap={
@@ -55,17 +53,15 @@
 
     # Width of a pixel in mm on A4 paper with 96 dpi print quality.
     pix_in_mm = 0.26458
     # Width of a line on A4 paper with 20 mm side margins
     line_width = 170
 
     if fig.layout.width * pix_in_mm < line_width:
-        fig_size = "width={:.3f}\\linewidth".format(
-            fig.layout.width * pix_in_mm / line_width
-        )
+        fig_size = "width={:.3f}\\linewidth".format(fig.layout.width * pix_in_mm / line_width)
         angle = 0
     else:
         fig_size = "height={:.3f}\\linewidth".format(
             min(1.0, fig.layout.height * pix_in_mm / line_width)
         )
         angle = 90
 
@@ -90,20 +86,16 @@
 
         if rich == "tex":
             img_path = f"{img_path}.pdf"
             fig.write_image(img_path)
             latex_path = img_path.replace("\\", "/").replace("_", "-underscore-")
             yield "\\begin{figure}[!htbp]"
             yield "\\centering"
-            yield "\\includegraphics[{}, angle={}]{{{}}}".format(
-                fig_size, angle, latex_path
-            )
-            yield "\\caption{{{}}}\\label{{{}}}".format(
-                caption, "fig:mdmlevel" + str(level)
-            )
+            yield "\\includegraphics[{}, angle={}]{{{}}}".format(fig_size, angle, latex_path)
+            yield "\\caption{{{}}}\\label{{{}}}".format(caption, "fig:mdmlevel" + str(level))
             yield "\\end{figure}"
             logger.debug("Included image as {}.".format(rich))
 
         elif rich == "md":
             img_path = f"{img_path}.svg"
             fig.write_image(img_path)
             yield "![{}\\label{{{}}}]({})".format(
```

### Comparing `raesl-0.12.1/raesl/doc/sections.py` & `raesl-0.12.2/raesl/doc/sections.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,31 +54,28 @@
             ).format(depth + 1, len(comps))
         )
     yield leader
 
     if rich == "tex" or rich == "md":
         yield lns.snt(
             _(
-                "in Figure \\ref{{{}}} the associated design-structure-matrix (DSM) is "
-                "shown"
+                "in Figure \\ref{{{}}} the associated design-structure-matrix (DSM) is " "shown"
             ).format("fig:mdmlevel" + str(depth + 1))
         )
         yield lns.snt(
             _(
                 "the DSM shows the dependencies between the elements that are relevant "
                 "to this decomposition level"
             )
         )
 
 
 def global_needs_and_designs(h: int = 1):
     """Yield a global need and design specification intro section."""
-    yield lns.header(
-        h, "{}".format(_("system-wide qualitative and quantitative specifications"))
-    )
+    yield lns.header(h, "{}".format(_("system-wide qualitative and quantitative specifications")))
 
     yield lns.snt(
         _(
             "this chapter lists all qualitative and quantitative design specifications "
             "that cannot be linked to a component"
         )
     )
@@ -119,15 +116,14 @@
         if node.annotations.esl_info.get("comments", [])
         else []
     )
 
     for key, comments in plain_comments + list(
         node.annotations.esl_info["tagged_comments"].items()
     ):
-
         table.append("| {} |".format(lns.boldhead(_(key)).replace("\n", "")))
         table.append(TABLE_SINGLE)
         for comment in comments:
             table.append("| {} |".format(comment.replace("\n", "")))
         table.append(TABLE_SINGLE)
 
     table.append("")
@@ -150,17 +146,17 @@
         table = get_node_table(node=gl, graph=g)
         yield from table
 
     for gl in glsa:
         temp = deepcopy(gl)
         temp.annotations.esl_info["comments"].append(
             lns.snt(
-                _(
-                    "this goal function requirement automatically migrated from {}"
-                ).format(lns.node_path(temp.annotations.esl_info["body"]["active"]))
+                _("this goal function requirement automatically migrated from {}").format(
+                    lns.node_path(temp.annotations.esl_info["body"]["active"])
+                )
             )
         )
         temp.annotations.esl_info["body"]["active"] = node.name
         table = get_node_table(node=temp, graph=g)
         yield from table
 
 
@@ -177,17 +173,17 @@
         table = get_node_table(node=gl, graph=g)
         yield from table
 
     for gl in glsa:
         temp = deepcopy(gl)
         temp.annotations.esl_info["comments"].append(
             lns.snt(
-                _(
-                    "this goal function constraint automatically migrated from {}"
-                ).format(lns.node_path(temp.annotations.esl_info["body"]["active"]))
+                _("this goal function constraint automatically migrated from {}").format(
+                    lns.node_path(temp.annotations.esl_info["body"]["active"])
+                )
             )
         )
         temp.annotations.esl_info["body"]["active"] = node.name
         table = get_node_table(node=temp, graph=g)
         yield from table
 
 
@@ -222,17 +218,15 @@
 
     trs = sorted(trs, key=lambda x: lns.node_path(x.name))
 
     yield lns.header(h, _("transformation function constraints"))
 
     for tr in trs:
         subs = [
-            e.target.name
-            for e in g.edges
-            if e.source == tr and e.kind == "traceability_dependency"
+            e.target.name for e in g.edges if e.source == tr and e.kind == "traceability_dependency"
         ]
         table = get_node_table(tr, graph=g, sub_nodes=subs)
         yield from table
 
 
 # Behavior specs
 def comp_node_behavior_reqs(node: Node, g: Graph, h: int = 1) -> LineGen:
@@ -381,17 +375,15 @@
         table.append(TABLE_SINGLE)
         for v in ri.get("related_variables"):
             table.append("|    |")
             table.append("| {} |".format(lns.var_path(g[v]).replace("\n", "")))
             table.append("|    |")
         table.append(TABLE_SINGLE)
 
-    plain_comments = (
-        [("comments", ri.get("comments", []))] if ri.get("comments", []) else []
-    )
+    plain_comments = [("comments", ri.get("comments", []))] if ri.get("comments", []) else []
 
     for key, comments in plain_comments + list(ri["tagged_comments"].items()):
         table.append("| {} |".format(lns.boldhead(_(key)).replace("\n", "")))
         table.append(TABLE_SINGLE)
         for comment in comments:
             table.append("| {} |".format(comment.replace("\n", "")))
         table.append(TABLE_SINGLE)
@@ -548,17 +540,15 @@
                 value = ival["lowerbound"]["value"]
                 if ival["lowerbound"]["unit"]:
                     value += " " + ival["lowerbound"]["unit"]
                 intervals.append(value)
         if not is_enum:
             domain = ", ".join(intervals)
         else:
-            domain = _("enumeration of ") + pm.hook.linguistic_enumeration(
-                items=intervals
-            )
+            domain = _("enumeration of ") + pm.hook.linguistic_enumeration(items=intervals)
     else:
         domain = ""
     if t.annotations.esl_info.get("units"):
         units = ",".join(t.annotations.esl_info.get("units"))
     else:
         units = ""
```

### Comparing `raesl-0.12.1/raesl/doc/templates/background.pdf` & `raesl-0.12.2/raesl/doc/templates/background.pdf`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/doc/templates/eisvogel.latex` & `raesl-0.12.2/raesl/doc/templates/eisvogel.latex`

 * *Files 0% similar despite different names*

```diff
@@ -335,14 +335,20 @@
 % pandoc includes fvextra in the default template.
 \usepackage{fvextra}
 \DefineVerbatimEnvironment{Highlighting}{Verbatim}{breaklines,fontsize=$if(code-block-font-size)$$code-block-font-size$$else$\small$endif$,commandchars=\\\{\}}
 
 $endif$
 $if(tables)$
 \usepackage{longtable,booktabs,array}
+\usepackage{csvsimple}
+\usepackage{siunitx}
+\usepackage{makecell}
+\usepackage{collcell}
+\usepackage{ifmtarg}
+\newcommand*{\mythead}[1]{{\thead{\textbf{#1}}}}
 $if(multirow)$
 \usepackage{multirow}
 $endif$
 \usepackage{calc} % for calculating minipage widths
 $if(beamer)$
 \usepackage{caption}
 % Make caption package work with longtable
```

### Comparing `raesl-0.12.1/raesl/doc/utils.py` & `raesl-0.12.2/raesl/doc/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,15 @@
         and n.annotations.esl_info.get("sub_kind") == "goal"
         and n.annotations.esl_info.get("form") == form
         and (
             n.annotations.esl_info["body"].get("active") in ancestors
             if inherited
             else n.annotations.esl_info["body"].get("active") == component.name
         )
-        and [
-            e
-            for e in graph.edges_between(component, n)
-            if e.kind == "mapping_dependency"
-        ]
+        and [e for e in graph.edges_between(component, n) if e.kind == "mapping_dependency"]
     ]
     return goals
 
 
 def get_component_transformations(
     component: Node, graph: Graph, constraint: bool = True
 ) -> List[Node]:
@@ -44,31 +40,27 @@
         and n.annotations.esl_info.get("sub_kind") == "transformation"
         and n.annotations.esl_info.get("form") == form
         and n.annotations.esl_info["body"].get("active") == component.name
     ]
     return transformations
 
 
-def get_component_behaviors(
-    component: Node, graph: Graph, constraint: bool = True
-) -> List[Node]:
+def get_component_behaviors(component: Node, graph: Graph, constraint: bool = True) -> List[Node]:
     """Get relevant behavior requirements or constraints for a component."""
     form = "constraint" if constraint else "requirement"
     return [
         b
         for b in graph.nodes
         if b.kind == "behavior_spec"
         and b.annotations.esl_info.get("form") == form
         and graph[component.name, b.name]
     ]
 
 
-def get_component_designs(
-    component: Node, graph: Graph, constraint: bool = True
-) -> List[Node]:
+def get_component_designs(component: Node, graph: Graph, constraint: bool = True) -> List[Node]:
     """Get relevant design requirements or constraints for a component."""
     form = "constraint" if constraint else "requirement"
     return [
         d
         for d in graph.nodes
         if d.kind == "design_spec"
         and d.annotations.esl_info.get("form") == form
@@ -94,22 +86,18 @@
     ]
 
     return drs
 
 
 def get_component_needs(component: Node, graph: Graph) -> List[Node]:
     """Get relevant needs for a component."""
-    subjects = set(
-        [n.name for n in graph.targets_of(component) if n.kind != "component"]
-    )
+    subjects = set([n.name for n in graph.targets_of(component) if n.kind != "component"])
     subjects.add(component.name)
     return [
-        n
-        for n in graph.nodes
-        if n.kind == "need" and n.annotations.esl_info["subject"] in subjects
+        n for n in graph.nodes if n.kind == "need" and n.annotations.esl_info["subject"] in subjects
     ]
 
 
 def get_global_needs(graph: Graph) -> List[Node]:
     """Get globally relevant needs."""
     sc_dict = {}
     for e in graph.edges:
@@ -121,27 +109,19 @@
 
     def get_subject(need):
         return need.annotations.esl_info["subject"]
 
     return [
         need
         for need in all_needs
-        if get_subject(need) not in sc_dict
-        and graph[get_subject(need)].kind != "component"
+        if get_subject(need) not in sc_dict and graph[get_subject(need)].kind != "component"
     ]
 
 
 def get_component_relations(component: Node, graph: Graph) -> List[Node]:
     """Get relevant relations for a component."""
-    return [
-        n
-        for n in graph.nodes
-        if n.kind == "relation_spec" and graph[component.name, n.name]
-    ]
+    return [n for n in graph.nodes if n.kind == "relation_spec" and graph[component.name, n.name]]
 
 
 def get_component_properties(component: Node, graph: Graph) -> List[Node]:
     """Get relevant properties for a component."""
-    return [
-        graph[prop]
-        for prop in component.annotations.esl_info.get("property_variables", [])
-    ]
+    return [graph[prop] for prop in component.annotations.esl_info.get("property_variables", [])]
```

### Comparing `raesl-0.12.1/raesl/excel/__init__.py` & `raesl-0.12.2/raesl/excel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,21 +32,17 @@
     graph = to_graph(*paths)
 
     # Create workbook, but delete default sheet.
     wb = Workbook()
     wb.remove(wb["Sheet"])
 
     # Derive components from scopes.
-    components = [
-        node for node in get_scoped_nodes(graph, scopes) if node.kind == "component"
-    ]
+    components = [node for node in get_scoped_nodes(graph, scopes) if node.kind == "component"]
     if not components:
-        raise ValueError(
-            f"No components found in selected scopes ('{scopes}'). Please reconsider."
-        )
+        raise ValueError(f"No components found in selected scopes ('{scopes}'). Please reconsider.")
 
     # Add sheets.
     _, components = sheets.add_components_sheet(wb, components)
     _, goals = sheets.add_goals_sheet(wb, graph, components)
     _, transformations = sheets.add_transformations_sheet(wb, graph, components)
     _, designs = sheets.add_designs_sheet(wb, graph, components)
     _, behaviors = sheets.add_behaviors_sheet(wb, graph, components)
```

### Comparing `raesl-0.12.1/raesl/excel/cli.py` & `raesl-0.12.2/raesl/excel/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import click
 import raesl.excel
 import raesl.excel.defaults
 from raesl import logger
 
 
 @click.command("excel")
-@click.argument(
-    "paths", nargs=-1, type=click.Path(exists=True, file_okay=True, dir_okay=True)
-)
+@click.argument("paths", nargs=-1, type=click.Path(exists=True, file_okay=True, dir_okay=True))
 @click.option(
     "--output",
     "-o",
     default=raesl.excel.defaults.OUTPUT,
     type=click.Path(file_okay=True, dir_okay=False, writable=True),
     help="Output file to write to.",
     show_default=True,
```

### Comparing `raesl-0.12.1/raesl/excel/defaults.py` & `raesl-0.12.2/raesl/excel/defaults.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,118 +12,82 @@
     sort=False,
     autoFilter=False,
 )
 
 OPTIONS = {
     # General
     "instance path": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)),
         width=30,
     ),
     "component path": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)),
         width=40,
     ),
     "instance name": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)),
         width=20,
     ),
     "parent component": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="right", vertical="top", wrap_text=False)
-        ),
+        styles=dict(alignment=Alignment(horizontal="right", vertical="top", wrap_text=False)),
         width=30,
     ),
     "component definition": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)),
         width=30,
     ),
-    "kind": dict(
-        styles=dict(alignment=Alignment(horizontal="center", vertical="top")), width=20
-    ),
-    "form": dict(
-        styles=dict(alignment=Alignment(horizontal="center", vertical="top")), width=15
-    ),
+    "kind": dict(styles=dict(alignment=Alignment(horizontal="center", vertical="top")), width=20),
+    "form": dict(styles=dict(alignment=Alignment(horizontal="center", vertical="top")), width=15),
     # Helper words
     "auxiliary": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)),
         width=12,
     ),
     "comparison": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)),
         width=20,
     ),
     "comments": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)),
         width=60,
     ),
     # Overview
     "specification text": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)),
         width=60,
     ),
     # Need
     "subject": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)),
         width=30,
     ),
     # Goal/transform specific
     "source component": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)),
         width=40,
     ),
     "target component": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)),
         width=40,
     ),
     "verb": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)),
         width=15,
     ),
     "preposition": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="center", vertical="top", wrap_text=True)),
         width=10,
     ),
     "variables": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="left", vertical="top", wrap_text=True)),
         width=30,
     ),
     # Design requirements
     "bound": dict(
-        styles=dict(
-            alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)
-        ),
+        styles=dict(alignment=Alignment(horizontal="right", vertical="top", wrap_text=True)),
         width=20,
     ),
     "subclauses": dict(
         styles=dict(alignment=Alignment(horizontal="left", vertical="top")), width=60
     ),
 }
```

### Comparing `raesl-0.12.1/raesl/excel/sheets.py` & `raesl-0.12.2/raesl/excel/sheets.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from raesl.doc.sections import get_var_table_row_elements
 from raesl.excel import text, utils
 from raesl.excel.defaults import OPTIONS
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 
-def add_components_sheet(
-    wb: Workbook, components: List[Node]
-) -> Tuple[Worksheet, List[Node]]:
+def add_components_sheet(wb: Workbook, components: List[Node]) -> Tuple[Worksheet, List[Node]]:
     """Add a components overview sheet to an Excel workbook.
 
     Arguments:
         wb: Excel workbook to add the components sheet to.
         components: List of component nodes.
 
     Returns:
@@ -86,38 +84,30 @@
     ws = wb.create_sheet("Goals")
 
     # Get requirements.
     requirements = utils.dedupe(
         [
             r
             for c in components
-            for r in doc_utils.get_component_goals(
-                c, graph, constraint=False, inherited=False
-            )
+            for r in doc_utils.get_component_goals(c, graph, constraint=False, inherited=False)
         ]
         + [
             r
             for c in components
-            for r in doc_utils.get_component_goals(
-                c, graph, constraint=False, inherited=True
-            )
+            for r in doc_utils.get_component_goals(c, graph, constraint=False, inherited=True)
         ]
         + [
             r
             for c in components
-            for r in doc_utils.get_component_goals(
-                c, graph, constraint=True, inherited=False
-            )
+            for r in doc_utils.get_component_goals(c, graph, constraint=True, inherited=False)
         ]
         + [
             r
             for c in components
-            for r in doc_utils.get_component_goals(
-                c, graph, constraint=True, inherited=True
-            )
+            for r in doc_utils.get_component_goals(c, graph, constraint=True, inherited=True)
         ]
     )
 
     # Handle headers.
     default_headers = [
         "instance path",
         "component definition",
@@ -279,19 +269,15 @@
     Returns:
         Design requirements worksheet instance.
     """
     ws = wb.create_sheet("Design requirements")
 
     # Select requirements.
     requirements = utils.dedupe(
-        [
-            r
-            for c in components
-            for r in doc_utils.get_component_designs(c, graph, constraint=False)
-        ]
+        [r for c in components for r in doc_utils.get_component_designs(c, graph, constraint=False)]
         + [
             r
             for c in components
             for r in doc_utils.get_component_designs(c, graph, constraint=True)
         ]
     )
 
@@ -316,28 +302,23 @@
     for requirement in requirements:
         info = requirement.annotations.esl_info
         for body in info["body"]:
             default_content = [
                 node_path(requirement.name, italic=False, arrows=False, skip="world"),
                 utils.parent_def(graph, requirement),
                 info["form"],
-                var_path(
-                    graph[body["subject"]], italic=False, arrows=False, skip="world"
-                ),
-                "{}{}".format(
-                    "EITHER " if len(info["body"]) > 1 else "", body["auxiliary"]
-                ),
+                var_path(graph[body["subject"]], italic=False, arrows=False, skip="world"),
+                "{}{}".format("EITHER " if len(info["body"]) > 1 else "", body["auxiliary"]),
                 body["comparison"],
                 "{} {}".format(body["bound"]["value"], body["bound"]["unit"]),
                 text.subclauses_text(requirement, graph, skip="world", spaces=0),
                 utils.format_multiline(info["comments"]),
             ]
             tagged_content = [
-                utils.format_multiline(info["tagged_comments"].get(tag, []))
-                for tag in tags
+                utils.format_multiline(info["tagged_comments"].get(tag, [])) for tag in tags
             ]
             ws.append(default_content + tagged_content)
             rows += 1
 
     # Handle styling.
     utils.make_table(
         ws,
```

### Comparing `raesl-0.12.1/raesl/excel/text.py` & `raesl-0.12.2/raesl/excel/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from typing import Any, Dict, List, Optional
 
 from raesl.doc import lines
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 
-def requirement_text(
-    requirement: Node, graph: Graph, skip: Optional[str] = "world"
-) -> str:
+def requirement_text(requirement: Node, graph: Graph, skip: Optional[str] = "world") -> str:
     """Re-format the requirement as text."""
     info = requirement.annotations.esl_info
     if requirement.kind == "function_spec":
         if info["sub_kind"] == "goal":
             func = goal_text
         elif info["sub_kind"] == "transformation":
             func = transformation_text
@@ -56,22 +54,18 @@
         ),
         preposition=body["preposition"],
         passive=lines.node_path(body["passive"], italic=False, arrows=False, skip=skip),
     )
     return text
 
 
-def transformation_text(
-    requirement: Node, graph: Graph, skip: Optional[str] = "world"
-) -> str:
+def transformation_text(requirement: Node, graph: Graph, skip: Optional[str] = "world") -> str:
     """Re-format transformation requirement as text."""
     body = requirement.annotations.esl_info["body"]
-    text = (
-        "{auxiliary} {verb} {input_variables} {preposition} {output_variables}"
-    ).format(
+    text = ("{auxiliary} {verb} {input_variables} {preposition} {output_variables}").format(
         auxiliary=body["auxiliary"],
         verb=body["verb"],
         input_variables=", ".join(
             lines.var_path(graph[var], italic=False, arrows=False, skip=skip)
             for var in body["input_variables"]
         ),
         preposition=body["preposition"],
@@ -86,17 +80,15 @@
 def designrule_text(
     body: Dict[str, Any],
     graph: Graph,
     skip: Optional[str] = "world",
 ) -> str:
     """Re-format design rule as text."""
     return "{subject} {auxiliary} {comparison} {value} {unit}".format(
-        subject=lines.var_path(
-            graph[body["subject"]], italic=False, arrows=False, skip=skip
-        ),
+        subject=lines.var_path(graph[body["subject"]], italic=False, arrows=False, skip=skip),
         auxiliary=body["auxiliary"],
         comparison=body["comparison"],
         value=body["bound"]["value"],
         unit=body["bound"]["unit"],
     )
 
 
@@ -137,58 +129,48 @@
 
 def case_text(case: Dict[str, Any], graph: Graph, skip: str = "world") -> str:
     """Re-format behavior requirement case as text."""
     return "{name}:\n  when:\n{whens}\n  then:\n{thens}".format(
         name=case["name"],
         whens=indent(
             "\n".join(
-                designclause_text(
-                    clause["body"], graph, label=clause["name"], skip=skip
-                )
+                designclause_text(clause["body"], graph, label=clause["name"], skip=skip)
                 for clause in case["when_clauses"]
             ),
             prefix=4 * " ",
         ),
         thens=indent(
             "\n".join(
-                designclause_text(
-                    clause["body"], graph, label=clause["name"], skip=skip
-                )
+                designclause_text(clause["body"], graph, label=clause["name"], skip=skip)
                 for clause in case["then_clauses"]
             ),
             prefix=4 * " ",
         ),
     )
 
 
-def behavior_text(
-    requirement: Node, graph: Graph, skip: Optional[str] = "world"
-) -> str:
+def behavior_text(requirement: Node, graph: Graph, skip: Optional[str] = "world") -> str:
     """Re-format behavior requirement as text."""
     info = requirement.annotations.esl_info
 
     text = "\n\n".join(case_text(case, graph, skip=skip) for case in info["cases"])
     if info["default"]:
         text += "\n\nwhen no other case applies:\n{}".format(
             indent(
                 "\n".join(
-                    designclause_text(
-                        clause["body"], graph, label=clause["name"], skip=skip
-                    )
+                    designclause_text(clause["body"], graph, label=clause["name"], skip=skip)
                     for clause in info["default"]
                 ),
                 prefix=4 * " ",
             ),
         )
     return text
 
 
 def need_text(requirement: Node, graph: Graph, skip: Optional[str] = "world") -> str:
     """Re-format need as text."""
     info = requirement.annotations.esl_info
     text = ("{subject} {text}").format(
-        subject=lines.var_path(
-            graph[info["subject"]], italic=False, arrows=False, skip=skip
-        ),
+        subject=lines.var_path(graph[info["subject"]], italic=False, arrows=False, skip=skip),
         text=info["text"],
     )
     return text
```

### Comparing `raesl-0.12.1/raesl/excel/utils.py` & `raesl-0.12.2/raesl/excel/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,29 @@
 
 def get_all_tags(nodes: List[Node]) -> List[str]:
     """Get all tagged comment keys from a list of nodes."""
     tags: List[str] = []
     seen: Set[str] = set()
     for node in nodes:
         node_tags = [
-            tag
-            for tag in node.annotations.esl_info["tagged_comments"].keys()
-            if tag not in seen
+            tag for tag in node.annotations.esl_info["tagged_comments"].keys() if tag not in seen
         ]
         tags.extend(node_tags)
         seen.update(node_tags)
     return tags
 
 
 def make_table(
     ws: Worksheet,
     name: str = "Table",
     min_row: int = 1,
     max_row: int = 1,
     min_col: int = 1,
     max_col: int = 1,
-    style: TableStyleInfo = TableStyleInfo(
-        name="TableStyleMedium9", showRowStripes=True
-    ),
+    style: TableStyleInfo = TableStyleInfo(name="TableStyleMedium9", showRowStripes=True),
 ) -> Table:
     """Make a table of a cell range in a worksheet."""
     ref = CellRange(min_row=min_row, max_row=max_row, min_col=min_col, max_col=max_col)
     table = Table(name=name, displayName=name, ref=ref.coord)
     table.tableStyleInfo = style
     ws.add_table(table)
     return table
```

### Comparing `raesl-0.12.1/raesl/jupyter/cli.py` & `raesl-0.12.2/raesl/jupyter/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/jupyter/kernel.py` & `raesl-0.12.2/raesl/jupyter/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,14 @@
         kernel_id = connection_file.split("-", 1)[1].split(".")[0]
 
         for srv in notebookapp.list_running_servers():
             try:
                 if srv["token"] == "" and not srv["password"]:
                     req = urllib.request.urlopen(srv["url"] + "api/sessions")
                 else:
-                    req = urllib.request.urlopen(
-                        srv["url"] + "api/sessions?token=" + srv["token"]
-                    )
+                    req = urllib.request.urlopen(srv["url"] + "api/sessions?token=" + srv["token"])
                 sessions = json.load(req)
                 for sess in sessions:
                     if sess["kernel"]["id"] == kernel_id:
-                        return pathlib.Path(
-                            srv["notebook_dir"], sess["notebook"]["path"]
-                        )
+                        return pathlib.Path(srv["notebook_dir"], sess["notebook"]["path"])
             except Exception:
                 return None
```

### Comparing `raesl-0.12.1/raesl/plot/diagrams.py` & `raesl-0.12.2/raesl/plot/diagrams.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,15 @@
         style: RaESL style options.
 
     Returns:
         Graphviz Digraph object of the functional dependency diagram.
     """
     if root.kind != "component":
         raise ValueError(
-            "Root node is of kind '{}' while it must be of kind 'component'.".format(
-                root.kind
-            )
+            "Root node is of kind '{}' while it must be of kind 'component'.".format(root.kind)
         )
 
     view = GraphView(
         graph,
         view_func=view_funcs.functional_dependency,
         view_kwargs={"root": root, "levels": levels},
     )
@@ -83,17 +81,15 @@
         style: RaESL style options.
 
     Returns:
         Graphviz Digraph object of the functional context diagram.
     """
     if root.kind != "component":
         raise ValueError(
-            "Root node is of kind '{}' while it must be of kind 'component'.".format(
-                root.kind
-            )
+            "Root node is of kind '{}' while it must be of kind 'component'.".format(root.kind)
         )
 
     view = GraphView(
         graph,
         view_func=view_funcs.functional_context,
         view_kwargs={"root": root, "degree": degree, "style": style},
     )
@@ -169,17 +165,15 @@
     Returns
         Graphviz Digraph object of the functional traceability diagram.
     """
 
     # Input checks.
     if root.kind != "function_spec":
         raise ValueError(
-            "Root node must be of kind 'function_spec' not of kind '{}'".format(
-                root.kind
-            )
+            "Root node must be of kind 'function_spec' not of kind '{}'".format(root.kind)
         )
 
     if root.annotations.esl_info["sub_kind"] != "transformation":
         raise ValueError(
             """Root node must be of sub-kind 'transformation'
             not of sub-kind '{}'""".format(
                 root.annotations.esl_info["sub_kind"]
@@ -211,19 +205,15 @@
         style: RaESL style options.
     """
     digraph = Digraph("G", comment=view.name, **style.diagram.digraph)
     digraph.graph_attr["rankdir"] = style.diagram["orientation"]
 
     trans, goals = utils.get_component_function_dicts(view)
     cmps = set([n for n in view.nodes if n.kind == "component"])
-    leafs = {
-        c.name: c
-        for c in cmps
-        if not c.children or not set(c.children).intersection(cmps)
-    }
+    leafs = {c.name: c for c in cmps if not c.children or not set(c.children).intersection(cmps)}
 
     for r in roots:
         if r.name in leafs:
             _add_component(digraph, r, trans, goals, style)
         else:
             migrated_goals = []
             for a in r.ancestors:
@@ -315,16 +305,15 @@
     Arguments:
         digraph: Digraph object to add the goal specification to.
         node: The Node corresponding to the goal specification to be added.
         style: RaESL style options.
     """
     if style.diagram.list_variables:
         label = "\n - ".join(
-            [node.name + "\n Variables:"]
-            + node.annotations.esl_info["body"]["variables"]
+            [node.name + "\n Variables:"] + node.annotations.esl_info["body"]["variables"]
         )
         digraph.node(
             name=node.name,
             label=label,
             shape=style.diagram.node_shapes["goal"],
         )
     else:
@@ -340,30 +329,27 @@
         style: RaESL style options.
     """
     if style.diagram.list_variables:
         inputs = "\n -".join(
             ["Input variables:"] + trans.annotations.esl_info["body"]["input_variables"]
         )
         outputs = "\n -".join(
-            ["Output variables:"]
-            + trans.annotations.esl_info["body"]["output_variables"]
+            ["Output variables:"] + trans.annotations.esl_info["body"]["output_variables"]
         )
         label = "\n".join([trans.name, inputs, outputs])
         digraph.node(
             name=trans.name,
             label=label,
             shape=style.diagram.node_shapes["transformation"],
         )
     else:
         digraph.node(trans.name, shape=style.diagram.node_shapes["transformation"])
 
 
-def _get_display_name(
-    node: Node, trans: Dict[str, List[str]], leafs: Dict[str, Node]
-) -> str:
+def _get_display_name(node: Node, trans: Dict[str, List[str]], leafs: Dict[str, Node]) -> str:
     """Get the display name for a Node in the diagram.
 
     Arguments:
         node: Node to get the display name for.
         trans: Dictionary of component node names to a list of transformation specs.
         leafs: Dictionary of leaf node names to leaf nodes.
```

### Comparing `raesl-0.12.1/raesl/plot/generic.py` & `raesl-0.12.2/raesl/plot/generic.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/plot/matrix.py` & `raesl-0.12.2/raesl/plot/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,10 +67,8 @@
     elif style.piemap.display == "kinds":
         if not style.piemap.fields:
             style.piemap.fields = edge_kinds
     elif style.piemap.display in ["weights", "weight labels"]:
         if not style.piemap.fields:
             style.piemap.fields = edge_weights
 
-    return ragraph.plot.mdm(
-        leafs=view.nodes, edges=view.edges, show=False, style=style, sort=False
-    )
+    return ragraph.plot.mdm(leafs=view.nodes, edges=view.edges, show=False, style=style, sort=False)
```

### Comparing `raesl-0.12.1/raesl/plot/utils.py` & `raesl-0.12.2/raesl/plot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,29 +243,27 @@
     """
     components = sliced.get_nodes_by_kind(kind="component")
     depth = max([graph[c.name].depth for c in components]) if components else 0
     parents = set(
         [
             graph[c.name].parent
             for c in components
-            if graph[c.name].parent is not None
-            and graph[c.name].parent.depth == depth - 1
+            if graph[c.name].parent is not None and graph[c.name].parent.depth == depth - 1
         ]
     )
 
     while parents:
         add_level(graph, sliced, parents=parents)
         depth -= 1
         comps = sliced.get_nodes_by_kind(kind="component")
         parents = set(
             [
                 graph[c.name].parent
                 for c in comps
-                if graph[c.name].parent is not None
-                and graph[c.name].parent.depth == depth - 1
+                if graph[c.name].parent is not None and graph[c.name].parent.depth == depth - 1
             ]
         )
 
 
 def get_all_descendants(nodes: List[Node]) -> Set[Node]:
     """Get all descendants from a list of provided nodes.
 
@@ -293,31 +291,27 @@
     """
     for point in points:
         comp = point[0]
         functions = point[1]
         for f in functions:
             if comp.name != f.annotations.esl_info["body"]["active"]:
                 msg = "Active component of '{}' is not equal to start component '{}'."
-                raise ValueError(
-                    msg.format(comp.name, f.annotations.esl_info["body"]["active"])
-                )
+                raise ValueError(msg.format(comp.name, f.annotations.esl_info["body"]["active"]))
 
 
 def check_tree_disjunction(nodes: List[Node]):
     """Check if list of nodes are not part of each others descendants.
 
     Raises:
         ValueError: If node is in the descendants of another node that was provided.
     """
     decendants = get_all_descendants(nodes)
     for n in nodes:
         if n in decendants:
-            raise ValueError(
-                "Node {} is a descendant of another provided node.".format(n.name)
-            )
+            raise ValueError("Node {} is a descendant of another provided node.".format(n.name))
 
 
 def check_start_and_end_points(
     start_points: List[Tuple[Node, List[Node]]],
     end_points: List[Tuple[Node, List[Node]]],
 ):
     """Check start and end points for consistency.
@@ -334,17 +328,15 @@
         ValueError: If any of the components are a descendant of another component.
     """
     points = start_points + end_points
     check_comp_func_pairs(points)
     check_tree_disjunction([p[0] for p in points])
 
 
-def get_function_tree(
-    graph: Graph, node: Node, levels: int
-) -> Tuple[Set[Node], Set[Edge]]:
+def get_function_tree(graph: Graph, node: Node, levels: int) -> Tuple[Set[Node], Set[Edge]]:
     """Walk down the traceability tree of a node.
 
     Arguments:
         graph: Instantiated ESL graph.
         node: Node to start the walk from.
         levels: Number of levels to continue walking.
 
@@ -355,21 +347,15 @@
     """
     edges = set()
     functions = set()
     functions.add(node)
 
     if levels > 1:
         edges.update(
-            set(
-                [
-                    e
-                    for e in graph.edges_from(node)
-                    if e.kind == "traceability_dependency"
-                ]
-            )
+            set([e for e in graph.edges_from(node) if e.kind == "traceability_dependency"])
         )
 
         function_targets = set([e.target for e in edges])
         functions.update(function_targets)
         for f in function_targets:
             if f.annotations.esl_info["sub_kind"] == "goal":
                 continue
@@ -378,17 +364,15 @@
 
             edges.update(es)
             functions.update(fs)
 
     return functions, edges
 
 
-def migrate_edges_between_variables(
-    graph: Graph, lead_components: List[Node]
-) -> List[Edge]:
+def migrate_edges_between_variables(graph: Graph, lead_components: List[Node]) -> List[Edge]:
     """Migrate edges between variables up into the decomposition tree.
 
     Arguments:
         graph: Instantiated ESL graph.
         lead_components: The components that are displayed.
 
     Returns:
@@ -406,29 +390,26 @@
         if not c.children:
             continue
         # Component is a collapsed component so get transformation specs and add
         # dependencies between in and output variables.
         tfs = [
             n
             for n in graph.targets_of(c)
-            if n.kind == "function_spec"
-            and n.annotations.esl_info["sub_kind"] == "transformation"
+            if n.kind == "function_spec" and n.annotations.esl_info["sub_kind"] == "transformation"
         ]
         for t in tfs:
             for vi in t.annotations.esl_info["body"]["input_variables"]:
                 for vj in t.annotations.esl_info["body"]["output_variables"]:
                     edges.append(
                         Edge(
                             source=graph[vi],
                             target=graph[vj],
                             labels=[graph[vi].annotations.esl_info["type_ref"]],
                             kind="functional_dependency",
-                            annotations=dict(
-                                esl_info=dict(reason=dict(transformations=[t.name]))
-                            ),
+                            annotations=dict(esl_info=dict(reason=dict(transformations=[t.name]))),
                         )
                     )
     return edges
 
 
 def has_mapping_dependency(graph: Graph, node: Node, nodes: List[Node]) -> bool:
     """Check if a node is mapped to any node in a list of nodes.
@@ -439,27 +420,19 @@
         nodes: List of nodes which are to be considered for checking the existence
             of a mapping dependency.
 
     Returns:
         Bool that indicates if a mapping dependency exists.
     """
     return any(
-        True
-        for e in graph.edges_between_all(nodes, [node])
-        if e.kind == "mapping_dependency"
-    ) or any(
-        True
-        for e in graph.edges_between_all([node], nodes)
-        if e.kind == "mapping_dependency"
-    )
+        True for e in graph.edges_between_all(nodes, [node]) if e.kind == "mapping_dependency"
+    ) or any(True for e in graph.edges_between_all([node], nodes) if e.kind == "mapping_dependency")
 
 
-def filter_nodes(
-    graph: Graph, lead_components: List[Node], node_kinds: List[str]
-) -> List[Node]:
+def filter_nodes(graph: Graph, lead_components: List[Node], node_kinds: List[str]) -> List[Node]:
     """Filter nodes for displaying a multi-domain-matrix.
 
     Arguments:
         graph: Instantiated ESL graph.
         lead_components: List of nodes of kind 'component' that are leading in
            filter the other nodes.
         node_kinds: List of node kinds to be included.
```

### Comparing `raesl-0.12.1/raesl/plot/view_funcs.py` & `raesl-0.12.2/raesl/plot/view_funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,22 +49,18 @@
         )
 
     node_kinds = graph.node_kinds if node_kinds is None else node_kinds
     edge_kinds = graph.edge_kinds if edge_kinds is None else edge_kinds
     edge_labels = graph.edge_labels if edge_labels is None else edge_labels
     edge_weights = graph.edge_weight_labels if edge_weights is None else edge_weights
 
-    nodes = utils.filter_nodes(
-        graph, lead_components=lead_components, node_kinds=node_kinds
-    )
+    nodes = utils.filter_nodes(graph, lead_components=lead_components, node_kinds=node_kinds)
 
     edges = [
-        e
-        for e in graph.edges_between_all(sources=nodes, targets=nodes)
-        if e.kind in edge_kinds
+        e for e in graph.edges_between_all(sources=nodes, targets=nodes) if e.kind in edge_kinds
     ]
 
     # Ensure that mapping dependencies appear below the diagonal.
     n2n = {kind: idx for idx, kind in enumerate(node_kinds)}
     modified_edges = []
     added_edges = []
     for e in edges:
@@ -79,24 +75,20 @@
 
     for e in modified_edges:
         edges.remove(e)
 
     edges += added_edges
 
     if "variable" in node_kinds and "functional_dependency" in edge_kinds:
-        edges += utils.migrate_edges_between_variables(
-            graph, lead_components=lead_components
-        )
+        edges += utils.migrate_edges_between_variables(graph, lead_components=lead_components)
 
     return nodes, edges
 
 
-def hierarchy(
-    graph: Graph, roots: List[Node], levels: int
-) -> Tuple[List[Node], List[Edge]]:
+def hierarchy(graph: Graph, roots: List[Node], levels: int) -> Tuple[List[Node], List[Edge]]:
     """Filter nodes and create edges for drawing a hierarchical decomposition diagram.
 
     Arguments:
        graph: Source data graph.
        roots: Roots of the hierarchical diagram.
        levels: Number of levels to include in the diagram.
 
@@ -126,17 +118,15 @@
     for e in edges:
         e.source = node_dict[e.source.name]
         e.target = node_dict[e.target.name]
 
     return stripped_nodes, edges
 
 
-def functional_dependency(
-    graph: Graph, root: Node, levels: int
-) -> Tuple[List[Node], List[Node]]:
+def functional_dependency(graph: Graph, root: Node, levels: int) -> Tuple[List[Node], List[Node]]:
     """Filter method for drawing a nested functional dependency structure.
 
     Arguments
         graph: Instantiated ESL graph.
         root: Root node for which the dependency structure must be drawn.
         levels: Number of levels to include in the tree.
 
@@ -183,17 +173,15 @@
     Returns:
         List of selected nodes and list of selected edges.
     """
     # Get functions in tree and traceability edges.
     g = deepcopy(graph)
     functions, edges = utils.get_function_tree(g, root, levels)
 
-    components = [
-        c for c in set([g[f.annotations.esl_info["body"]["active"]] for f in functions])
-    ]
+    components = [c for c in set([g[f.annotations.esl_info["body"]["active"]] for f in functions])]
 
     # Remove component hierarchy to make traceability hierarchy leading.
     for c in components:
         c.parent = None
         c.children = []
 
     if style.diagram.show_function_dependencies:
@@ -291,17 +279,15 @@
             drawn.
         degree: Degree up to which neighbors of neighbors must be sought.
         style: RaESL style options.
 
     Returns:
         List of selected nodes and list of selected edges.
     """
-    neighbors = utils.get_neighbors(
-        graph, root, root, node_kinds={"component"}, degree=degree
-    )
+    neighbors = utils.get_neighbors(graph, root, root, node_kinds={"component"}, degree=degree)
 
     components = []
     tree = set()
     tree.add(root.name)
     if style.diagram.show_root_children and root.children:
         components.extend(root.children)
         tree.update(set([c.name for c in root.children]))
@@ -327,17 +313,15 @@
     )
 
     edges += _add_component_goal_edges(graph, sorted(tree), functions)
 
     return components + functions, edges
 
 
-def _add_component_goal_edges(
-    graph: Graph, tree: List[Node], functions: List[Node]
-) -> List[Edge]:
+def _add_component_goal_edges(graph: Graph, tree: List[Node], functions: List[Node]) -> List[Edge]:
     """Create edges between component or cluster nodes if a goal cannot be related
     to a transformation:
 
     Arguments:
         graph: Instantiated ESL graph.
         tree: List of components that are within the (sub)tree that is plotted.
         functions: List of function specs that is plotted.
@@ -353,17 +337,15 @@
     for goal in goals:
         if (
             not list(graph.edges_between_all(sources=[goal], targets=transformations))
             and goal.annotations.esl_info["body"]["passive"] in tree
         ):
             # No destination transformation is found. Add edge to destination component
             # if the destination component is part of the selected components.
-            for e in graph.directed_edges[goal.annotations.esl_info["body"]["passive"]][
-                goal.name
-            ]:
+            for e in graph.directed_edges[goal.annotations.esl_info["body"]["passive"]][goal.name]:
                 edges.append(
                     Edge(
                         source=e.target,
                         target=e.source,
                         kind=e.kind,
                         labels=e.labels,
                         weights=e.weights,
@@ -373,13 +355,11 @@
 
         if (
             not list(graph.edges_between_all(sources=transformations, targets=[goal]))
             and goal.annotations.esl_info["body"]["active"] in tree
         ):
             # No source transformation is found. Add edge from to source component.
             edges.extend(
-                graph.directed_edges[goal.annotations.esl_info["body"]["active"]][
-                    goal.name
-                ]
+                graph.directed_edges[goal.annotations.esl_info["body"]["active"]][goal.name]
             )
 
     return edges
```

### Comparing `raesl-0.12.1/raesl/pygments.py` & `raesl-0.12.2/raesl/pygments.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/server/cli.py` & `raesl-0.12.2/raesl/server/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     help="An optional TCP port to run on, useful for debugging.",
 )
 def serve(port: Optional[int] = None):
     """Start the ESL Language Server."""
     try:
         from raesl.server.server import ls
     except ImportError:
-        logger.error(
-            "Missing dependencies. Make sure the 'server' extras are installed."
-        )
+        logger.error("Missing dependencies. Make sure the 'server' extras are installed.")
         return
 
     if port is None:
         logger.info("Starting ESL Language Server on STDIO...")
         ls.start_io()
     else:
         logger.info(f"Starting ESL Language Server on port {port}...")
```

### Comparing `raesl-0.12.1/raesl/server/config.py` & `raesl-0.12.2/raesl/server/config.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.1/raesl/server/server.py` & `raesl-0.12.2/raesl/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,17 +106,15 @@
         )
         if diag_store.has_severe() or spec is None:
             _publish(ls, paths, diag_store)
             logger.error("Parsing failed validation.")
             return False
 
         # Derive dependency graph.
-        graph = graph_building.GraphFactory(
-            diag_store=diag_store, spec=spec
-        ).make_graph()
+        graph = graph_building.GraphFactory(diag_store=diag_store, spec=spec).make_graph()
         if diag_store.has_severe() or graph is None:
             _publish(ls, paths, diag_store)
             logger.error("Graph building failed validation.")
             return False
         elif ls.config.output is not None:
             ls.show_message_log(f"Dumping output graph to '{ls.config.output}'...")
             from ragraph.io.json import to_json
```

### Comparing `raesl-0.12.1/raesl/types.py` & `raesl-0.12.2/raesl/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,19 +107,15 @@
     """
 
     def __init__(self, start: Position, end: Position):
         self.start = start
         self.end = end
 
     def __eq__(self, other):
-        return (
-            isinstance(other, Range)
-            and self.start == other.start
-            and self.end == other.end
-        )
+        return isinstance(other, Range) and self.start == other.start and self.end == other.end
 
     def __hash__(self):
         return hash((self.start, self.end))
 
     def __iter__(self):
         return iter((self.start, self.end))
 
@@ -145,19 +141,15 @@
         self.range = range
 
     def get_key(self) -> Tuple[str, int, int]:
         """Get a tuple with identification for this position."""
         return self.uri, self.range.start.line, self.range.start.character
 
     def __eq__(self, other):
-        return (
-            isinstance(other, Location)
-            and self.uri == other.uri
-            and self.range == other.range
-        )
+        return isinstance(other, Location) and self.uri == other.uri and self.range == other.range
 
     def __lt__(self, other: "Location"):
         return self.get_key() < other.get_key()
 
     def __le__(self, other: "Location"):
         return self.get_key() <= other.get_key()
```

### Comparing `raesl-0.12.1/raesl/utils.py` & `raesl-0.12.2/raesl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 
         if not p.exists():
             logger.info(f"Skipped '{p}' as it does not exist.")
             continue
 
         if p.is_dir():
             result.update(
-                p
-                for p in p.glob("**/*.esl")
-                if not any(part.startswith(".") for part in p.parts)
+                p for p in p.glob("**/*.esl") if not any(part.startswith(".") for part in p.parts)
             )
 
         if p.is_file():
             result.add(p)
 
     if not result:
         raise ValueError("No ESL files found.")
```

### Comparing `raesl-0.12.1/PKG-INFO` & `raesl-0.12.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: raesl
-Version: 0.12.1
+Version: 0.12.2
 Summary: Ratio ESL support in Python.
-Home-page: https://gitlab.com/ratio-case/python/raesl
+Home-page: https://raesl.ratio-case.nl
 License: GPL-3.0-or-later
 Author: Ratio Innovations B.V.
 Author-email: info@ratio-case.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,34 +14,34 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: jupyter
 Provides-Extra: pygments
 Provides-Extra: rich
 Provides-Extra: server
-Requires-Dist: IPython (>=7.13.0,<8.0.0) ; extra == "jupyter" or extra == "all"
-Requires-Dist: click (>=8.0.0,<9.0.0)
-Requires-Dist: click-log (>=0.3.2,<0.4.0)
+Requires-Dist: IPython (>=7,<8) ; extra == "jupyter" or extra == "all"
+Requires-Dist: click (>=8,<9)
+Requires-Dist: click-log (>=0.3,<0.4)
 Requires-Dist: graphviz (>=0.17,<0.18)
-Requires-Dist: ipykernel (>=6.4.1,<7.0.0) ; extra == "jupyter" or extra == "all"
-Requires-Dist: ipywidgets (>=7.5,<8.0) ; extra == "jupyter" or extra == "all"
-Requires-Dist: jupyter_client (>=7.0.6,<8.0.0) ; extra == "jupyter" or extra == "all"
+Requires-Dist: ipykernel (>=6,<7) ; extra == "jupyter" or extra == "all"
+Requires-Dist: ipywidgets (>=7,<8) ; extra == "jupyter" or extra == "all"
+Requires-Dist: jupyter_client (>=7,<8) ; extra == "jupyter" or extra == "all"
 Requires-Dist: kaleido (==0.2.1) ; extra == "rich" or extra == "all"
-Requires-Dist: notebook (>=6.0.0,<7.0.0) ; extra == "jupyter" or extra == "all"
-Requires-Dist: numpy (>=1.21.1,<2.0.0)
-Requires-Dist: openpyxl (>=3.0.8,<4.0.0)
-Requires-Dist: pandoc_fignos (>=2.4.0,<3.0.0) ; extra == "doc" or extra == "all"
-Requires-Dist: plotly (>=5.0.0,<6.0.0) ; extra == "rich" or extra == "all"
-Requires-Dist: pluggy (>=1.0.0,<2.0.0) ; extra == "doc" or extra == "all"
-Requires-Dist: pygls (>=0.11.0,<0.12.0) ; extra == "server" or extra == "all"
-Requires-Dist: pypandoc (>=1.4.0,<2.0.0) ; extra == "doc" or extra == "all"
-Requires-Dist: ragraph (>=1.15.1,<2.0.0)
-Requires-Dist: sly (>=0.4.0,<0.5.0)
+Requires-Dist: notebook (>=6,<7) ; extra == "jupyter" or extra == "all"
+Requires-Dist: numpy (>=1,<2)
+Requires-Dist: openpyxl (>=3,<4)
+Requires-Dist: pandoc_fignos (>=2,<3) ; extra == "doc" or extra == "all"
+Requires-Dist: plotly (>=5,<6) ; extra == "rich" or extra == "all"
+Requires-Dist: pluggy (>=1,<2) ; extra == "doc" or extra == "all"
+Requires-Dist: pygls (>=0.11,<0.12) ; extra == "server" or extra == "all"
+Requires-Dist: pypandoc (>=1,<2) ; extra == "doc" or extra == "all"
+Requires-Dist: ragraph (>=1,<2)
+Requires-Dist: sly (>=0.4,<0.5)
 Project-URL: Documentation, https://raesl.ratio-case.nl
-Project-URL: Repository, https://gitlab.com/ratio-case/python/raesl
+Project-URL: Repository, https://gitlab.com/ratio-case-os/python/raesl
 Description-Content-Type: text/x-rst
 
 #########
 Ratio ESL
 #########
 
 Ratio support for the  Elephant Specification Language (ESL) in Python.
@@ -50,59 +50,59 @@
 **********
 Quickstart
 **********
 
 Installation
 ============
 
-RaESL can be installed using ``pip install raesl`` for any Python version >=3.9. Or,
-for Poetry managed projects, use ``poetry add raesl`` to add it as a dependency.
+RaESL can be installed using ``pip install raesl[all]`` for any Python version >=3.9. Or,
+for Poetry managed projects, use ``poetry add raesl -E all`` to add it as a dependency.
 
-For RaESL's different subcommands and functionality, the wheel provides extras:
+For RaESL's different subcommands and functionality, the wheel provides extras which you could
+provide instead of the ``all`` used above:
 
-* doc: documentation generation using pandoc, Markdown and optionally LaTeX.
-* jupyter: a Jupyter ESL kernel.
-* pygments: an ESL syntax highlighter for pygments.
-* rich: Rich doc output in the form of Plotly images.
-* server: A language server to parse documents.
+* ``doc``: documentation generation using pandoc, Markdown and optionally LaTeX.
+* ``jupyter``: a Jupyter ESL kernel.
+* ``pygments``: an ESL syntax highlighter for pygments.
+* ``rich``: Rich doc output in the form of Plotly images.
+* ``server``: A language server to parse documents.
 
 
 The default ``compile`` command is always available.
 
 Please refer to the `usage documentation <https://raesl.ratio-case.nl>`_ for more info
 on how to use RaESL.
 
-
 ***************
 Developer guide
 ***************
 
 Python packaging information
 ============================
 
 This project is packaged using `poetry <https://python-poetry.org/>`_. Packaging
 information as well as dependencies are stored in `pyproject.toml <./pyproject.toml>`_.
 
-Installing the project and its development dependencies can be done using ``poetry install``.
-
-
-Invoke tasks
-============
-
-Most elemental maintenance tasks can be accomplished using
-[Invoke](https://www.pyinvoke.org/). After installing using ``poetry install`` and
-enabling the environment using ``poetry shell``, you can run all tasks using ``inv
-[taskname]`` or ``invoke [taskname]``. E.g. ``inv docs`` builds the documentation.
-
+Installing the project and its development dependencies can be done using ``poetry install -E all``.
 
 Versioning
 ==========
 
 This project uses `semantic versioning <https://semver.org>`_. Version increments are
 checked using `Raver <https://raver.ratio-case.nl>`_.
 
-
 Changelog
 =========
 
-Changelog format as described by https://keepachangelog.com/ has been adopted.
+Changelog format as described by https://keepachangelog.com/ has been adopted and can be reviewed
+`on this page <https://raesl.ratio-case.nl/changelog.html>`.
+
+Tests
+=====
+
+Tests can be run using ``poetry run pytest``.
+
+Linting
+=======
+
+Linting config is included in `pyproject.toml <./pyproject.toml>`_ for both Black and Ruff.
```

