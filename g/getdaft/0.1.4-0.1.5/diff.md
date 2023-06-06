# Comparing `tmp/getdaft-0.1.4.tar.gz` & `tmp/getdaft-0.1.5.tar.gz`

## Comparing `getdaft-0.1.4.tar` & `getdaft-0.1.5.tar`

### file list

```diff
@@ -1,462 +1,469 @@
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 getdaft-0.1.4/Cargo.toml
--rw-r--r--   0      501       20      834 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      595 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0      501       20      428 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/dependabot.yml
--rw-r--r--   0      501       20     1333 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/broken-link-checker.yml
--rw-r--r--   0      501       20     3378 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/daft-profiling.yml
--rw-r--r--   0      501       20     1627 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/notebook-checker.yml
--rw-r--r--   0      501       20     2194 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/property-based-tests.yml
--rw-r--r--   0      501       20    12886 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/python-package.yml
--rw-r--r--   0      501       20     6182 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     2638 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/ray-compatibility.yml
--rw-r--r--   0      501       20      300 2023-06-03 10:38:04.000000 getdaft-0.1.4/.gitignore
--rw-r--r--   0      501       20     2126 2023-06-03 10:38:04.000000 getdaft-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0      501       20      205 2023-06-03 10:38:04.000000 getdaft-0.1.4/.readthedocs.yaml
--rw-r--r--   0      501       20     1550 2023-06-03 10:38:04.000000 getdaft-0.1.4/CONTRIBUTING.md
--rw-r--r--   0      501       20    11357 2023-06-03 10:38:04.000000 getdaft-0.1.4/LICENSE
--rw-r--r--   0      501       20     1295 2023-06-03 10:38:04.000000 getdaft-0.1.4/Makefile
--rw-r--r--   0      501       20     6126 2023-06-03 10:38:04.000000 getdaft-0.1.4/README.rst
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/__init__.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/__init__.py
--rw-r--r--   0      501       20     9495 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/__main__.py
--rw-r--r--   0      501       20    12428 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/answers.py
--rw-r--r--   0      501       20    12140 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/data_generation.py
--rw-r--r--   0      501       20     4573 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/pipelined_data_generation.py
--rw-r--r--   0      501       20     1436 2023-06-03 10:38:04.000000 getdaft-0.1.4/ci/upload_wheels.sh
--rw-r--r--   0      501       20      440 2023-06-03 10:38:04.000000 getdaft-0.1.4/codecov.yml
--rw-r--r--   0      501       20     2092 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/__init__.py
--rw-r--r--   0      501       20     6724 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/analytics.py
--rw-r--r--   0      501       20     3935 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/api_annotations.py
--rw-r--r--   0      501       20    10591 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/arrow_utils.py
--rw-r--r--   0      501       20     5395 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/context.py
--rw-r--r--   0      501       20     3403 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/convert.py
--rw-r--r--   0      501       20      724 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/daft.pyi
--rw-r--r--   0      501       20       94 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/dataframe/__init__.py
--rw-r--r--   0      501       20    49646 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/dataframe/dataframe.py
--rw-r--r--   0      501       20      306 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/dataframe/preview.py
--rw-r--r--   0      501       20      850 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/datasources.py
--rw-r--r--   0      501       20    13221 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/datatype.py
--rw-r--r--   0      501       20       84 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/errors.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/__init__.py
--rw-r--r--   0      501       20    24774 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/execution_step.py
--rw-r--r--   0      501       20     4231 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/logical_op_runners.py
--rw-r--r--   0      501       20    28173 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/physical_plan.py
--rw-r--r--   0      501       20     6110 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/physical_plan_factory.py
--rw-r--r--   0      501       20      170 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/expressions/__init__.py
--rw-r--r--   0      501       20    25203 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/expressions/expressions.py
--rw-r--r--   0      501       20      572 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/expressions/testing.py
--rw-r--r--   0      501       20    12728 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/filesystem.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/__init__.py
--rw-r--r--   0      501       20      509 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/gpu.py
--rw-r--r--   0      501       20     1804 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/rule.py
--rw-r--r--   0      501       20     2030 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/rule_runner.py
--rw-r--r--   0      501       20     3490 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/treenode.py
--rw-r--r--   0      501       20      263 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/__init__.py
--rw-r--r--   0      501       20     1682 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/_csv.py
--rw-r--r--   0      501       20     1223 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/_json.py
--rw-r--r--   0      501       20     2032 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/common.py
--rw-r--r--   0      501       20     2034 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/file_path.py
--rw-r--r--   0      501       20     1243 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/parquet.py
--rw-r--r--   0      501       20      264 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logging.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/__init__.py
--rw-r--r--   0      501       20     8601 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/aggregation_plan_builder.py
--rw-r--r--   0      501       20    37496 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/logical_plan.py
--rw-r--r--   0      501       20     1492 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/map_partition_ops.py
--rw-r--r--   0      501       20    19183 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/optimizer.py
--rw-r--r--   0      501       20     3625 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/schema.py
--rw-r--r--   0      501       20       99 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/__init__.py
--rw-r--r--   0      501       20    34760 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/cloudpickle.py
--rw-r--r--   0      501       20    34262 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/cloudpickle_fast.py
--rw-r--r--   0      501       20      639 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/compat.py
--rw-r--r--   0      501       20      312 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/pickle.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/py.typed
--rw-r--r--   0      501       20     2036 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/resource_request.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/__init__.py
--rw-r--r--   0      501       20     5708 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/partitioning.py
--rw-r--r--   0      501       20     1488 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/profiler.py
--rw-r--r--   0      501       20    13059 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/pyrunner.py
--rw-r--r--   0      501       20    25296 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/ray_runner.py
--rw-r--r--   0      501       20      918 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/runner.py
--rw-r--r--   0      501       20     4324 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/runner_io.py
--rw-r--r--   0      501       20    19568 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/series.py
--rw-r--r--   0      501       20       82 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/table/__init__.py
--rw-r--r--   0      501       20    13765 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/table/table.py
--rw-r--r--   0      501       20     9457 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/table/table_io.py
--rw-r--r--   0      501       20     7263 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/udf.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/udf_library/__init__.py
--rw-r--r--   0      501       20     3486 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/udf_library/url_udfs.py
--rw-r--r--   0      501       20     2796 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/utils.py
--rw-r--r--   0      501       20      183 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/__init__.py
--rw-r--r--   0      501       20     1699 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/dataframe_display.py
--rw-r--r--   0      501       20     1517 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/html_viz_hooks.py
--rw-r--r--   0      501       20     6592 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/repr.py
--rw-r--r--   0      501       20      148 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/CONTRIBUTING.md
--rw-r--r--   0      501       20      638 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/Makefile
--rw-r--r--   0      501       20    71692 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/10-min.ipynb
--rw-r--r--   0      501       20      389 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/custom-function-signatures.css
--rw-r--r--   0      501       20      565 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/daft-favicon.png
--rw-r--r--   0      501       20     7804 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/daft-logo.png
--rw-r--r--   0      501       20    42148 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/daft_illustration.png
--rw-r--r--   0      501       20    25200 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/execution_model.png
--rw-r--r--   0      501       20     1901 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/header.css
--rw-r--r--   0      501       20    32864 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/high_level_architecture.png
--rw-r--r--   0      501       20      343 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/icon-menu-close.svg
--rw-r--r--   0      501       20      333 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/icon-menu-dots.svg
--rw-r--r--   0      501       20    18177 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/in_memory_data_representation.png
--rw-r--r--   0      501       20      786 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/mobile-menu.js
--rw-r--r--   0      501       20     9142 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/tpch-1000sf.html
--rw-r--r--   0      501       20     9647 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/tpch-100sf.html
--rw-r--r--   0      501       20     8757 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
--rw-r--r--   0      501       20      856 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_templates/layout.html
--rw-r--r--   0      501       20      994 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_templates/sections/header.html
--rw-r--r--   0      501       20      957 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_templates/sections/mobile-menu.html
--rw-r--r--   0      501       20      325 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/context.rst
--rw-r--r--   0      501       20     2564 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/dataframe.rst
--rw-r--r--   0      501       20     1881 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/datatype.rst
--rw-r--r--   0      501       20     3474 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/expressions.rst
--rw-r--r--   0      501       20      784 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/groupby.rst
--rw-r--r--   0      501       20      136 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/index.rst
--rw-r--r--   0      501       20     1457 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/input_output.rst
--rw-r--r--   0      501       20       88 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/udf.rst
--rw-r--r--   0      501       20    14528 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/benchmarks/index.rst
--rw-r--r--   0      501       20     3547 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/conf.py
--rw-r--r--   0      501       20     4964 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/dataframe_comparison.rst
--rw-r--r--   0      501       20     1666 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/index.rst
--rw-r--r--   0      501       20     1089 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/install.rst
--rw-r--r--   0      501       20      743 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/index.rst
--rw-r--r--   0      501       20     7586 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/key_concepts.rst
--rw-r--r--   0      501       20     1398 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/tutorials.rst
--rw-r--r--   0      501       20     1388 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/aggregations.rst
--rw-r--r--   0      501       20     6686 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/dataframe-operations.rst
--rw-r--r--   0      501       20     4695 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/datatypes.rst
--rw-r--r--   0      501       20     9131 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/expressions.rst
--rw-r--r--   0      501       20     7829 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/intro-dataframes.rst
--rw-r--r--   0      501       20      206 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/partitioning.rst
--rw-r--r--   0      501       20     3190 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/read-write.rst
--rw-r--r--   0      501       20     1257 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/scaling-up.rst
--rw-r--r--   0      501       20     8691 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/udf.rst
--rw-r--r--   0      501       20     1577 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides.rst
--rw-r--r--   0      501       20     3575 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.13.rst
--rw-r--r--   0      501       20     2241 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.14.rst
--rw-r--r--   0      501       20     1913 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.16.rst
--rw-r--r--   0      501       20     1750 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.17.rst
--rw-r--r--   0      501       20     2100 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.18.rst
--rw-r--r--   0      501       20     3647 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.19.rst
--rw-r--r--   0      501       20     4240 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.20.rst
--rw-r--r--   0      501       20     4633 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.21.rst
--rw-r--r--   0      501       20     8016 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.22.rst
--rw-r--r--   0      501       20     5385 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.23.rst
--rw-r--r--   0      501       20    11759 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.24.rst
--rw-r--r--   0      501       20     4750 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.0.rst
--rw-r--r--   0      501       20     2411 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.1.rst
--rw-r--r--   0      501       20     2557 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.2.rst
--rw-r--r--   0      501       20      839 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.3.rst
--rw-r--r--   0      501       20     3065 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.4.rst
--rw-r--r--   0      501       20      935 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/_template.rst
--rw-r--r--   0      501       20      350 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/index.rst
--rw-r--r--   0      501       20     6574 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/technical_architecture.rst
--rw-r--r--   0      501       20     1316 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/telemetry.rst
--rw-r--r--   0      501       20     1873 2023-06-03 10:38:04.000000 getdaft-0.1.4/pyproject.toml
--rw-r--r--   0      501       20      843 2023-06-03 10:38:04.000000 getdaft-0.1.4/requirements-dev.txt
--rw-r--r--   0      501       20       98 2023-06-03 10:38:04.000000 getdaft-0.1.4/rust-toolchain.toml
--rw-r--r--   0      501       20     4732 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/from.rs
--rw-r--r--   0      501       20      734 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/iterator.rs
--rw-r--r--   0      501       20     2945 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/mod.rs
--rw-r--r--   0      501       20      257 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/abs.rs
--rw-r--r--   0      501       20      726 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/apply.rs
--rw-r--r--   0      501       20      841 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arange.rs
--rw-r--r--   0      501       20     6964 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arithmetic.rs
--rw-r--r--   0      501       20     3048 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/comparison.rs
--rw-r--r--   0      501       20       34 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/mod.rs
--rw-r--r--   0      501       20       19 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/mod.rs
--rw-r--r--   0      501       20     3482 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/common.rs
--rw-r--r--   0      501       20      723 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/indices.rs
--rw-r--r--   0      501       20       47 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/mod.rs
--rw-r--r--   0      501       20     8075 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/sort.rs
--rw-r--r--   0      501       20     3407 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/as_arrow.rs
--rw-r--r--   0      501       20    11304 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/broadcast.rs
--rw-r--r--   0      501       20    26977 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/cast.rs
--rw-r--r--   0      501       20    11017 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/compare_agg.rs
--rw-r--r--   0      501       20    47218 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/comparison.rs
--rw-r--r--   0      501       20     1634 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/concat.rs
--rw-r--r--   0      501       20     5982 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/concat_agg.rs
--rw-r--r--   0      501       20     1433 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/count.rs
--rw-r--r--   0      501       20     1550 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/date.rs
--rw-r--r--   0      501       20     3335 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/filter.rs
--rw-r--r--   0      501       20     1264 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/float.rs
--rw-r--r--   0      501       20     1936 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/full.rs
--rw-r--r--   0      501       20     4112 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/groups.rs
--rw-r--r--   0      501       20     1515 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/hash.rs
--rw-r--r--   0      501       20    12551 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/if_else.rs
--rw-r--r--   0      501       20    16405 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/image.rs
--rw-r--r--   0      501       20     1058 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/len.rs
--rw-r--r--   0      501       20     3446 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/list.rs
--rw-r--r--   0      501       20     3360 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/list_agg.rs
--rw-r--r--   0      501       20     1622 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/mean.rs
--rw-r--r--   0      501       20     2617 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/mod.rs
--rw-r--r--   0      501       20     1314 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/null.rs
--rw-r--r--   0      501       20     3819 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/pairwise.rs
--rw-r--r--   0      501       20      484 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/search_sorted.rs
--rw-r--r--   0      501       20    19387 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/sort.rs
--rw-r--r--   0      501       20     2383 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/sum.rs
--rw-r--r--   0      501       20    17241 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/take.rs
--rw-r--r--   0      501       20     5279 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/utf8.rs
--rw-r--r--   0      501       20      995 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/pseudo_arrow/compute.rs
--rw-r--r--   0      501       20    13611 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/pseudo_arrow/mod.rs
--rw-r--r--   0      501       20     2502 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/pseudo_arrow/python.rs
--rw-r--r--   0      501       20    14860 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/dtype.rs
--rw-r--r--   0      501       20     2012 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/field.rs
--rw-r--r--   0      501       20     4549 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/image_mode.rs
--rw-r--r--   0      501       20     2889 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/logical.rs
--rw-r--r--   0      501       20     9088 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/matching.rs
--rw-r--r--   0      501       20     6836 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/mod.rs
--rw-r--r--   0      501       20     1083 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/time_unit.rs
--rw-r--r--   0      501       20      273 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/README.md
--rw-r--r--   0      501       20     1474 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/arithmetic.rs
--rw-r--r--   0      501       20    21828 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/expr.rs
--rw-r--r--   0      501       20     1431 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/float/is_nan.rs
--rw-r--r--   0      501       20      587 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/float/mod.rs
--rw-r--r--   0      501       20      496 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/image/decode.rs
--rw-r--r--   0      501       20      914 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/image/mod.rs
--rw-r--r--   0      501       20     1071 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/image/resize.rs
--rw-r--r--   0      501       20     1122 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/list/explode.rs
--rw-r--r--   0      501       20      597 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/list/mod.rs
--rw-r--r--   0      501       20     1944 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/mod.rs
--rw-r--r--   0      501       20     1188 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/numeric/abs.rs
--rw-r--r--   0      501       20      580 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/numeric/mod.rs
--rw-r--r--   0      501       20      676 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/python/mod.rs
--rw-r--r--   0      501       20     2050 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/python/partial_udf.rs
--rw-r--r--   0      501       20     2779 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/python/udf.rs
--rw-r--r--   0      501       20     1320 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/day.rs
--rw-r--r--   0      501       20     1348 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/day_of_week.rs
--rw-r--r--   0      501       20     1425 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/mod.rs
--rw-r--r--   0      501       20     1330 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/month.rs
--rw-r--r--   0      501       20     1324 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/year.rs
--rw-r--r--   0      501       20     1627 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/contains.rs
--rw-r--r--   0      501       20     1627 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/endswith.rs
--rw-r--r--   0      501       20     1346 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/length.rs
--rw-r--r--   0      501       20     1524 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/mod.rs
--rw-r--r--   0      501       20     1637 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/startswith.rs
--rw-r--r--   0      501       20     4961 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/lit.rs
--rw-r--r--   0      501       20      233 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/mod.rs
--rw-r--r--   0      501       20     5298 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/optimization.rs
--rw-r--r--   0      501       20     1982 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/pyobject.rs
--rw-r--r--   0      501       20     1681 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/error.rs
--rw-r--r--   0      501       20     7867 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/ffi.rs
--rw-r--r--   0      501       20     6022 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/hashing.rs
--rw-r--r--   0      501       20       54 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/mod.rs
--rw-r--r--   0      501       20    12159 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/search_sorted.rs
--rw-r--r--   0      501       20     3917 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/utf8.rs
--rw-r--r--   0      501       20     1117 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/lib.rs
--rw-r--r--   0      501       20     6900 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/datatype.rs
--rw-r--r--   0      501       20      307 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/error.rs
--rw-r--r--   0      501       20    10801 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/expr.rs
--rw-r--r--   0      501       20     1644 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/field.rs
--rw-r--r--   0      501       20      802 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/mod.rs
--rw-r--r--   0      501       20     2425 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/schema.rs
--rw-r--r--   0      501       20     9789 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/series.rs
--rw-r--r--   0      501       20    10760 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/table.rs
--rw-r--r--   0      501       20     3016 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/schema.rs
--rw-r--r--   0      501       20    10158 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/array_impl/data_array.rs
--rw-r--r--   0      501       20     5459 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/array_impl/logical_array.rs
--rw-r--r--   0      501       20      161 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/array_impl/mod.rs
--rw-r--r--   0      501       20     2099 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/from.rs
--rw-r--r--   0      501       20     2190 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/mod.rs
--rw-r--r--   0      501       20      902 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/abs.rs
--rw-r--r--   0      501       20     5207 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/agg.rs
--rw-r--r--   0      501       20     6298 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/arithmetic.rs
--rw-r--r--   0      501       20     1925 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/broadcast.rs
--rw-r--r--   0      501       20      194 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/cast.rs
--rw-r--r--   0      501       20     2609 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/comparison.rs
--rw-r--r--   0      501       20     1558 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/concat.rs
--rw-r--r--   0      501       20     1822 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/date.rs
--rw-r--r--   0      501       20     3612 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/downcast.rs
--rw-r--r--   0      501       20      697 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/filter.rs
--rw-r--r--   0      501       20      399 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/float.rs
--rw-r--r--   0      501       20      432 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/groups.rs
--rw-r--r--   0      501       20      412 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/hash.rs
--rw-r--r--   0      501       20      314 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/if_else.rs
--rw-r--r--   0      501       20     1024 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/image.rs
--rw-r--r--   0      501       20      229 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/len.rs
--rw-r--r--   0      501       20     1925 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/list.rs
--rw-r--r--   0      501       20     2367 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/mod.rs
--rw-r--r--   0      501       20      475 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/not.rs
--rw-r--r--   0      501       20      150 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/null.rs
--rw-r--r--   0      501       20      638 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/search_sorted.rs
--rw-r--r--   0      501       20     1492 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/sort.rs
--rw-r--r--   0      501       20      557 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/take.rs
--rw-r--r--   0      501       20     1528 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/utf8.rs
--rw-r--r--   0      501       20     1351 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/series_like.rs
--rw-r--r--   0      501       20    16798 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/mod.rs
--rw-r--r--   0      501       20     2165 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/agg.rs
--rw-r--r--   0      501       20     3729 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/explode.rs
--rw-r--r--   0      501       20     4403 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/groups.rs
--rw-r--r--   0      501       20     2886 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/hash.rs
--rw-r--r--   0      501       20     2483 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/joins/hash_join.rs
--rw-r--r--   0      501       20     3712 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/joins/mod.rs
--rw-r--r--   0      501       20       99 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/mod.rs
--rw-r--r--   0      501       20     3468 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/partition.rs
--rw-r--r--   0      501       20     1804 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/search_sorted.rs
--rw-r--r--   0      501       20      999 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/sort.rs
--rw-r--r--   0      501       20     5371 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/utils/arrow.rs
--rw-r--r--   0      501       20       34 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/utils/mod.rs
--rw-r--r--   0      501       20    10065 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/utils/supertype.rs
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/__init__.py
--rw-r--r--   0      501       20      299 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/__init__.py
--rw-r--r--   0      501       20      544 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/1.sql
--rw-r--r--   0      501       20      542 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/10.sql
--rw-r--r--   0      501       20      703 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/2.sql
--rw-r--r--   0      501       20      444 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/3.sql
--rw-r--r--   0      501       20      371 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/4.sql
--rw-r--r--   0      501       20      504 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/5.sql
--rw-r--r--   0      501       20      259 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/6.sql
--rw-r--r--   0      501       20      834 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/7.sql
--rw-r--r--   0      501       20      815 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/8.sql
--rw-r--r--   0      501       20      627 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/9.sql
--rw-r--r--   0      501       20       48 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/README.md
--rw-r--r--   0      501       20      604 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/conftest.py
--rw-r--r--   0      501       20     1227 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_df_arithmetic.py
--rw-r--r--   0      501       20     2706 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_file_read.py
--rw-r--r--   0      501       20     5604 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_groups_and_aggs.py
--rw-r--r--   0      501       20     7292 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_join.py
--rw-r--r--   0      501       20     2603 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_repartition.py
--rw-r--r--   0      501       20     4005 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_sort.py
--rw-r--r--   0      501       20     2911 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/conftest.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/__init__.py
--rw-r--r--   0      501       20    13229 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/assets/311-service-requests.24.csv
--rw-r--r--   0      501       20      255 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/assets/__init__.py
--rw-r--r--   0      501       20      882 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/conftest.py
--rw-r--r--   0      501       20     9268 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_aggregations.py
--rw-r--r--   0      501       20     2979 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_computations.py
--rw-r--r--   0      501       20     1798 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_count_rows.py
--rw-r--r--   0      501       20     7099 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_dataloading.py
--rw-r--r--   0      501       20      800 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_distinct.py
--rw-r--r--   0      501       20     6049 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_filter.py
--rw-r--r--   0      501       20     3810 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_joins.py
--rw-r--r--   0      501       20     2878 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_literals.py
--rw-r--r--   0      501       20    10311 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_pandas_cookbook.py
--rw-r--r--   0      501       20     4148 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_sorting.py
--rw-r--r--   0      501       20     1497 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_write.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/__init__.py
--rw-r--r--   0      501       20      751 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/conftest.py
--rw-r--r--   0      501       20      805 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_accessors.py
--rw-r--r--   0      501       20    10308 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_aggregations.py
--rw-r--r--   0      501       20    21893 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_creation.py
--rw-r--r--   0      501       20     1824 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_distinct.py
--rw-r--r--   0      501       20     1428 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_explode.py
--rw-r--r--   0      501       20     1097 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_filter.py
--rw-r--r--   0      501       20     2435 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_getitem.py
--rw-r--r--   0      501       20     4091 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_joins.py
--rw-r--r--   0      501       20     1940 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_logical_type.py
--rw-r--r--   0      501       20      223 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_repartition.py
--rw-r--r--   0      501       20     4858 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_repr.py
--rw-r--r--   0      501       20      815 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_select.py
--rw-r--r--   0      501       20      656 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_show.py
--rw-r--r--   0      501       20     6364 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_sort.py
--rw-r--r--   0      501       20     3596 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_temporals.py
--rw-r--r--   0      501       20     2385 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_to_integrations.py
--rw-r--r--   0      501       20      850 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_with_column.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/__init__.py
--rw-r--r--   0      501       20     1417 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_apply.py
--rw-r--r--   0      501       20     3533 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_expressions.py
--rw-r--r--   0      501       20     4259 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_expressions_projection.py
--rw-r--r--   0      501       20     5019 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_udf.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/__init__.py
--rw-r--r--   0      501       20     6290 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/conftest.py
--rw-r--r--   0      501       20     1363 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_aggs.py
--rw-r--r--   0      501       20     2335 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_arithmetic.py
--rw-r--r--   0      501       20      853 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_compare.py
--rw-r--r--   0      501       20      792 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_dt.py
--rw-r--r--   0      501       20      531 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_float.py
--rw-r--r--   0      501       20      684 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_if_else.py
--rw-r--r--   0      501       20      422 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_is_null.py
--rw-r--r--   0      501       20     1176 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_logical.py
--rw-r--r--   0      501       20     1544 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_str.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/integration/__init__.py
--rw-r--r--   0      501       20     4193 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/integration/test_tpch.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/__init__.py
--rw-r--r--   0      501       20     1116 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/conftest.py
--rw-r--r--   0      501       20     1666 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_drop_projections.py
--rw-r--r--   0      501       20     1847 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_drop_repartition.py
--rw-r--r--   0      501       20     2463 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_fold_projections.py
--rw-r--r--   0      501       20     7624 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_prune_columns.py
--rw-r--r--   0      501       20     3597 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_pushdown_clauses_into_scan.py
--rw-r--r--   0      501       20     1170 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_pushdown_limit.py
--rw-r--r--   0      501       20     8453 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_pushdown_predicates.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/property_based_testing/__init__.py
--rw-r--r--   0      501       20     4575 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/property_based_testing/strategies.py
--rw-r--r--   0      501       20     8895 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/property_based_testing/test_sort.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/ray/__init__.py
--rw-r--r--   0      501       20     5375 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/ray/test_dask.py
--rw-r--r--   0      501       20     8461 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/ray/test_datasets.py
--rw-r--r--   0      501       20      278 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/__init__.py
--rw-r--r--   0      501       20     9299 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_arithmetic.py
--rw-r--r--   0      501       20     8932 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_cast.py
--rw-r--r--   0      501       20    17207 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_comparisons.py
--rw-r--r--   0      501       20     7188 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_concat.py
--rw-r--r--   0      501       20      864 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_embedding.py
--rw-r--r--   0      501       20     6151 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_filter.py
--rw-r--r--   0      501       20      874 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_float.py
--rw-r--r--   0      501       20     3344 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_hash.py
--rw-r--r--   0      501       20    21522 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_if_else.py
--rw-r--r--   0      501       20     9303 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_image.py
--rw-r--r--   0      501       20      889 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_numeric_ops.py
--rw-r--r--   0      501       20     3418 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_series.py
--rw-r--r--   0      501       20     9173 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_size_bytes.py
--rw-r--r--   0      501       20     2188 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_slice.py
--rw-r--r--   0      501       20     5495 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_sort.py
--rw-r--r--   0      501       20     6111 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_take.py
--rw-r--r--   0      501       20     1934 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_temporal_ops.py
--rw-r--r--   0      501       20     4413 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_utf8_ops.py
--rw-r--r--   0      501       20      694 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/__init__.py
--rw-r--r--   0      501       20     1070 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_blackbox_kernels.py
--rw-r--r--   0      501       20      426 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_broadcasts.py
--rw-r--r--   0      501       20     2123 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_concat.py
--rw-r--r--   0      501       20     4900 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_eval.py
--rw-r--r--   0      501       20     3930 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_explodes.py
--rw-r--r--   0      501       20     7413 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_filter.py
--rw-r--r--   0      501       20    23374 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_from_py.py
--rw-r--r--   0      501       20      842 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_head.py
--rw-r--r--   0      501       20    10974 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_joins.py
--rw-r--r--   0      501       20     7811 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_partitioning.py
--rw-r--r--   0      501       20      654 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_size_bytes.py
--rw-r--r--   0      501       20    10955 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_sorting.py
--rw-r--r--   0      501       20    20923 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_table_aggs.py
--rw-r--r--   0      501       20    10064 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_table_io.py
--rw-r--r--   0      501       20     5061 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_take.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/utf8/__init__.py
--rw-r--r--   0      501       20     1165 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/utf8/test_compares.py
--rw-r--r--   0      501       20      321 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/utf8/test_length.py
--rw-r--r--   0      501       20     3533 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/test_analytics.py
--rw-r--r--   0      501       20      703 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/test_datatypes.py
--rw-r--r--   0      501       20     3542 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/test_schema.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/udf_library/__init__.py
--rw-r--r--   0      501       20     3777 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/udf_library/test_url_udfs.py
--rw-r--r--   0      501       20      338 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/utils.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests_legacy/__init__.py
--rw-r--r--   0      501       20     6988 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests_legacy/test_resource_requests.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/__init__.py
--rw-r--r--   0      501       20     1633 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/patch_package_version.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/__init__.py
--rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/__init__.py
--rw-r--r--   0      501       20     1125 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/LICENSE.txt
--rw-r--r--   0      501       20       59 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/__init__.py
--rw-r--r--   0      501       20     2499 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/__init__.py
--rw-r--r--   0      501       20     9514 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/convert.py
--rw-r--r--   0      501       20     3113 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/pack.py
--rw-r--r--   0      501       20      662 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/unpack.py
--rw-r--r--   0      501       20     1246 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/pkginfo.py
--rw-r--r--   0      501       20      974 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/util.py
--rw-r--r--   0      501       20     7125 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/wheelfile.py
--rw-r--r--   0      501       20      878 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/fix-and-copy-wheel.py
--rw-r--r--   0      501       20     2981 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/tmpdirs.py
--rw-r--r--   0      501       20     4469 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/tools.py
--rw-r--r--   0      501       20     9484 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/wheeltools.py
--rw-r--r--   0      501       20       19 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/.gitignore
--rw-r--r--   0      501       20    19576 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
--rw-r--r--   0      501       20    12068 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/image_querying/top_n_red_color.ipynb
--rw-r--r--   0      501       20    98730 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/mnist.ipynb
--rw-r--r--   0      501       20    11847 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/text_to_image/text_to_image_generation.ipynb
--rw-r--r--   0      501       20     9134 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/text_to_image/using_cloud_with_ray.ipynb
--rw-r--r--   0      501       20    34807 2023-06-03 10:38:04.000000 getdaft-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 getdaft-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 getdaft-0.1.5/Cargo.toml
+-rw-r--r--   0      501       20      834 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20      428 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/dependabot.yml
+-rw-r--r--   0      501       20     1333 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3378 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     1627 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     2194 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    12886 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     6182 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2638 2023-06-06 06:00:19.000000 getdaft-0.1.5/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20      300 2023-06-06 06:00:19.000000 getdaft-0.1.5/.gitignore
+-rw-r--r--   0      501       20     2126 2023-06-06 06:00:19.000000 getdaft-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2023-06-06 06:00:19.000000 getdaft-0.1.5/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2023-06-06 06:00:19.000000 getdaft-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2023-06-06 06:00:19.000000 getdaft-0.1.5/LICENSE
+-rw-r--r--   0      501       20     1295 2023-06-06 06:00:19.000000 getdaft-0.1.5/Makefile
+-rw-r--r--   0      501       20     9185 2023-06-06 06:00:19.000000 getdaft-0.1.5/README.rst
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20     9495 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12140 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4573 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     2654 2023-06-06 06:00:19.000000 getdaft-0.1.5/benchmarking/tpch/subprefix_s3_files.py
+-rw-r--r--   0      501       20     1436 2023-06-06 06:00:19.000000 getdaft-0.1.5/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      440 2023-06-06 06:00:19.000000 getdaft-0.1.5/codecov.yml
+-rw-r--r--   0      501       20     2092 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/__init__.py
+-rw-r--r--   0      501       20     6724 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/analytics.py
+-rw-r--r--   0      501       20     3935 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/api_annotations.py
+-rw-r--r--   0      501       20    10591 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/arrow_utils.py
+-rw-r--r--   0      501       20     5395 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/context.py
+-rw-r--r--   0      501       20     3403 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/convert.py
+-rw-r--r--   0      501       20      724 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/daft.pyi
+-rw-r--r--   0      501       20       94 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    49646 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      306 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/dataframe/preview.py
+-rw-r--r--   0      501       20      850 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/datasources.py
+-rw-r--r--   0      501       20    13221 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/datatype.py
+-rw-r--r--   0      501       20       84 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/errors.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/__init__.py
+-rw-r--r--   0      501       20    24774 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/execution_step.py
+-rw-r--r--   0      501       20     4231 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/logical_op_runners.py
+-rw-r--r--   0      501       20    28173 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     6110 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/execution/physical_plan_factory.py
+-rw-r--r--   0      501       20      170 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    25203 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/expressions/testing.py
+-rw-r--r--   0      501       20    12728 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/gpu.py
+-rw-r--r--   0      501       20     1804 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/rule.py
+-rw-r--r--   0      501       20     2030 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/rule_runner.py
+-rw-r--r--   0      501       20     3490 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/internal/treenode.py
+-rw-r--r--   0      501       20      263 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/__init__.py
+-rw-r--r--   0      501       20     1682 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/_csv.py
+-rw-r--r--   0      501       20     1223 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/_json.py
+-rw-r--r--   0      501       20     2032 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/common.py
+-rw-r--r--   0      501       20     2034 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/file_path.py
+-rw-r--r--   0      501       20     1243 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/io/parquet.py
+-rw-r--r--   0      501       20      264 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logging.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8601 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/aggregation_plan_builder.py
+-rw-r--r--   0      501       20    37496 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/logical_plan.py
+-rw-r--r--   0      501       20     1492 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20    19183 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/optimizer.py
+-rw-r--r--   0      501       20     3625 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/pickle/pickle.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/py.typed
+-rw-r--r--   0      501       20     2036 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/resource_request.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/__init__.py
+-rw-r--r--   0      501       20     5708 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1488 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/profiler.py
+-rw-r--r--   0      501       20    13059 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    25296 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20      918 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/runner.py
+-rw-r--r--   0      501       20     4324 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    19568 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/series.py
+-rw-r--r--   0      501       20       82 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/table/__init__.py
+-rw-r--r--   0      501       20    13765 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/table/table.py
+-rw-r--r--   0      501       20     9457 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/table/table_io.py
+-rw-r--r--   0      501       20     7263 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/udf.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     3486 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     2796 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/utils.py
+-rw-r--r--   0      501       20      183 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1699 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1517 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20     6592 2023-06-06 06:00:19.000000 getdaft-0.1.5/daft/viz/repr.py
+-rw-r--r--   0      501       20      148 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/Makefile
+-rw-r--r--   0      501       20    71692 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20      583 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/dataframe-comp-table.csv
+-rw-r--r--   0      501       20    25200 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/execution_model.png
+-rw-r--r--   0      501       20     1901 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/header.css
+-rw-r--r--   0      501       20    32864 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/high_level_architecture.png
+-rw-r--r--   0      501       20      343 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20    18177 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/in_memory_data_representation.png
+-rw-r--r--   0      501       20      786 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20     9142 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/tpch-1000sf.html
+-rw-r--r--   0      501       20     9647 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/tpch-100sf.html
+-rw-r--r--   0      501       20     8757 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
+-rw-r--r--   0      501       20      856 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20     1179 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20     1129 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      325 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2564 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     1997 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/datatype.rst
+-rw-r--r--   0      501       20     3898 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      784 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      136 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     1457 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20       88 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20    14528 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/benchmarks/index.rst
+-rw-r--r--   0      501       20     3868 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/conf.py
+-rw-r--r--   0      501       20     5078 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1665 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/index.rst
+-rw-r--r--   0      501       20     1089 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/install.rst
+-rw-r--r--   0      501       20      743 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7586 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1783 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     6686 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     4801 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/datatypes.rst
+-rw-r--r--   0      501       20     9131 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     7829 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20      206 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3190 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8691 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1577 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     3575 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.13.rst
+-rw-r--r--   0      501       20     2241 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.14.rst
+-rw-r--r--   0      501       20     1913 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.16.rst
+-rw-r--r--   0      501       20     1750 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.17.rst
+-rw-r--r--   0      501       20     2100 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.18.rst
+-rw-r--r--   0      501       20     3647 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.19.rst
+-rw-r--r--   0      501       20     4240 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.20.rst
+-rw-r--r--   0      501       20     4633 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.21.rst
+-rw-r--r--   0      501       20     8016 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.22.rst
+-rw-r--r--   0      501       20     5385 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.23.rst
+-rw-r--r--   0      501       20    11759 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.0.24.rst
+-rw-r--r--   0      501       20     4750 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.0.rst
+-rw-r--r--   0      501       20     2411 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.1.rst
+-rw-r--r--   0      501       20     2557 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.2.rst
+-rw-r--r--   0      501       20      839 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.3.rst
+-rw-r--r--   0      501       20     3065 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/0.1.4.rst
+-rw-r--r--   0      501       20      935 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/_template.rst
+-rw-r--r--   0      501       20      369 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/release_notes/index.rst
+-rw-r--r--   0      501       20     6574 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/technical_architecture.rst
+-rw-r--r--   0      501       20     1316 2023-06-06 06:00:19.000000 getdaft-0.1.5/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1873 2023-06-06 06:00:19.000000 getdaft-0.1.5/pyproject.toml
+-rw-r--r--   0      501       20      843 2023-06-06 06:00:19.000000 getdaft-0.1.5/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2023-06-06 06:00:19.000000 getdaft-0.1.5/rust-toolchain.toml
+-rw-r--r--   0      501       20     4732 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/from.rs
+-rw-r--r--   0      501       20      734 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/iterator.rs
+-rw-r--r--   0      501       20     2945 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/mod.rs
+-rw-r--r--   0      501       20      257 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      726 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      841 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     6964 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3048 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     8075 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20     3501 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/as_arrow.rs
+-rw-r--r--   0      501       20    11387 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20    30767 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/cast.rs
+-rw-r--r--   0      501       20    11017 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    47218 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     1634 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/concat.rs
+-rw-r--r--   0      501       20     5982 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     1433 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/count.rs
+-rw-r--r--   0      501       20     1550 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/date.rs
+-rw-r--r--   0      501       20     3335 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1264 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/float.rs
+-rw-r--r--   0      501       20     1936 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/full.rs
+-rw-r--r--   0      501       20     4112 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1515 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/hash.rs
+-rw-r--r--   0      501       20    12551 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20    16433 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/image.rs
+-rw-r--r--   0      501       20     1058 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/len.rs
+-rw-r--r--   0      501       20     3446 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/list.rs
+-rw-r--r--   0      501       20     3360 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1622 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2617 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     1314 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3819 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20      484 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    19387 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2383 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/sum.rs
+-rw-r--r--   0      501       20    17241 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/take.rs
+-rw-r--r--   0      501       20     5279 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13611 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2502 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20    14860 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     2012 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/field.rs
+-rw-r--r--   0      501       20     4549 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/image_mode.rs
+-rw-r--r--   0      501       20     2889 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/logical.rs
+-rw-r--r--   0      501       20     9088 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     6836 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1083 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20      273 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/README.md
+-rw-r--r--   0      501       20     1474 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/arithmetic.rs
+-rw-r--r--   0      501       20    21828 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/expr.rs
+-rw-r--r--   0      501       20     1431 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      587 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/float/mod.rs
+-rw-r--r--   0      501       20     1414 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/image/decode.rs
+-rw-r--r--   0      501       20      914 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/image/mod.rs
+-rw-r--r--   0      501       20     1663 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/image/resize.rs
+-rw-r--r--   0      501       20     1122 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/list/explode.rs
+-rw-r--r--   0      501       20      597 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/list/mod.rs
+-rw-r--r--   0      501       20     1944 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/mod.rs
+-rw-r--r--   0      501       20     1188 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      580 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/numeric/mod.rs
+-rw-r--r--   0      501       20      676 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/python/mod.rs
+-rw-r--r--   0      501       20     2050 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2779 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/python/udf.rs
+-rw-r--r--   0      501       20     1320 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1348 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1425 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1330 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1324 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/temporal/year.rs
+-rw-r--r--   0      501       20     1627 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1627 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1346 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1524 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1637 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20     4961 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/lit.rs
+-rw-r--r--   0      501       20      233 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/mod.rs
+-rw-r--r--   0      501       20     5298 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/optimization.rs
+-rw-r--r--   0      501       20     1982 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/dsl/pyobject.rs
+-rw-r--r--   0      501       20     1681 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/error.rs
+-rw-r--r--   0      501       20     7867 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/mod.rs
+-rw-r--r--   0      501       20    12159 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3917 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/kernels/utf8.rs
+-rw-r--r--   0      501       20     1117 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/lib.rs
+-rw-r--r--   0      501       20     6900 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/datatype.rs
+-rw-r--r--   0      501       20      307 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/error.rs
+-rw-r--r--   0      501       20    10801 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/expr.rs
+-rw-r--r--   0      501       20     1644 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/field.rs
+-rw-r--r--   0      501       20      802 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/mod.rs
+-rw-r--r--   0      501       20     2425 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/schema.rs
+-rw-r--r--   0      501       20     9789 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/series.rs
+-rw-r--r--   0      501       20    10760 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/python/table.rs
+-rw-r--r--   0      501       20     3016 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/schema.rs
+-rw-r--r--   0      501       20    10158 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/array_impl/data_array.rs
+-rw-r--r--   0      501       20     5459 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/array_impl/logical_array.rs
+-rw-r--r--   0      501       20      161 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/array_impl/mod.rs
+-rw-r--r--   0      501       20     2099 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/from.rs
+-rw-r--r--   0      501       20     2190 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/mod.rs
+-rw-r--r--   0      501       20      902 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     5207 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     6298 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     1925 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20      194 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/cast.rs
+-rw-r--r--   0      501       20     2609 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1558 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     1822 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/date.rs
+-rw-r--r--   0      501       20     3612 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20      697 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      399 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/float.rs
+-rw-r--r--   0      501       20      432 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      412 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/hash.rs
+-rw-r--r--   0      501       20      314 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20     1024 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/image.rs
+-rw-r--r--   0      501       20      229 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/len.rs
+-rw-r--r--   0      501       20     1925 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2367 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      475 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/not.rs
+-rw-r--r--   0      501       20      150 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/null.rs
+-rw-r--r--   0      501       20      638 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1492 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/sort.rs
+-rw-r--r--   0      501       20      557 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1528 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20     1351 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/series/series_like.rs
+-rw-r--r--   0      501       20    16798 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/mod.rs
+-rw-r--r--   0      501       20     2165 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/agg.rs
+-rw-r--r--   0      501       20     3729 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/explode.rs
+-rw-r--r--   0      501       20     4403 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/groups.rs
+-rw-r--r--   0      501       20     2886 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/hash.rs
+-rw-r--r--   0      501       20     2483 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     3712 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/joins/mod.rs
+-rw-r--r--   0      501       20       99 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/mod.rs
+-rw-r--r--   0      501       20     3468 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/partition.rs
+-rw-r--r--   0      501       20     1804 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/search_sorted.rs
+-rw-r--r--   0      501       20      999 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/table/ops/sort.rs
+-rw-r--r--   0      501       20     5371 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/utils/arrow.rs
+-rw-r--r--   0      501       20       34 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/utils/mod.rs
+-rw-r--r--   0      501       20    10065 2023-06-06 06:00:19.000000 getdaft-0.1.5/src/utils/supertype.rs
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/__init__.py
+-rw-r--r--   0      501       20      299 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/__init__.py
+-rw-r--r--   0      501       20      544 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20     1227 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     2706 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     5604 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     7292 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2603 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     4005 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     2911 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      924 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0000.jpg
+-rw-r--r--   0      501       20      941 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0007.jpg
+-rw-r--r--   0      501       20     2740 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0018.png
+-rw-r--r--   0      501       20     7462 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/assets/images/0025.tiff
+-rw-r--r--   0      501       20      882 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1798 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     7099 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     2301 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_image.py
+-rw-r--r--   0      501       20     3810 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4148 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      805 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10308 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20    21893 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1824 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1428 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1097 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     4091 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20     1940 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_logical_type.py
+-rw-r--r--   0      501       20      223 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_repartition.py
+-rw-r--r--   0      501       20     4858 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      815 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20      656 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6364 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     3596 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_temporals.py
+-rw-r--r--   0      501       20     2385 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      850 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     3533 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4259 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5019 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     6290 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      792 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1544 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/integration/__init__.py
+-rw-r--r--   0      501       20     4193 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/__init__.py
+-rw-r--r--   0      501       20     1116 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/conftest.py
+-rw-r--r--   0      501       20     1666 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_drop_projections.py
+-rw-r--r--   0      501       20     1847 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_drop_repartition.py
+-rw-r--r--   0      501       20     2463 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_fold_projections.py
+-rw-r--r--   0      501       20     7624 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_prune_columns.py
+-rw-r--r--   0      501       20     3597 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_pushdown_clauses_into_scan.py
+-rw-r--r--   0      501       20     1170 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_pushdown_limit.py
+-rw-r--r--   0      501       20     8453 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/optimizer/test_pushdown_predicates.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/ray/__init__.py
+-rw-r--r--   0      501       20     5375 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     8461 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20     8932 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_cast.py
+-rw-r--r--   0      501       20    17207 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     7188 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_concat.py
+-rw-r--r--   0      501       20      864 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_embedding.py
+-rw-r--r--   0      501       20     6151 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_float.py
+-rw-r--r--   0      501       20     3344 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_hash.py
+-rw-r--r--   0      501       20    21522 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_if_else.py
+-rw-r--r--   0      501       20     8674 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_image.py
+-rw-r--r--   0      501       20      889 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     3418 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_series.py
+-rw-r--r--   0      501       20     9173 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2188 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_sort.py
+-rw-r--r--   0      501       20     6111 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_take.py
+-rw-r--r--   0      501       20     1934 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     4413 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/__init__.py
+-rw-r--r--   0      501       20     1070 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      426 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2123 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4900 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_eval.py
+-rw-r--r--   0      501       20     3930 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7413 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_filter.py
+-rw-r--r--   0      501       20    23374 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      842 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_head.py
+-rw-r--r--   0      501       20    10974 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_joins.py
+-rw-r--r--   0      501       20     7811 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20      654 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    10955 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    20923 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20    10064 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_table_io.py
+-rw-r--r--   0      501       20     5061 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1165 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      321 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20     3533 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/test_datatypes.py
+-rw-r--r--   0      501       20     3542 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     3777 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      338 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests/utils.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests_legacy/__init__.py
+-rw-r--r--   0      501       20     6988 2023-06-06 06:00:19.000000 getdaft-0.1.5/tests_legacy/test_resource_requests.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/__init__.py
+-rw-r--r--   0      501       20     1633 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/patch_package_version.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/__init__.py
+-rw-r--r--   0      501       20     1125 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0      501       20       59 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/__init__.py
+-rw-r--r--   0      501       20     2499 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0      501       20     9514 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/convert.py
+-rw-r--r--   0      501       20     3113 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/pack.py
+-rw-r--r--   0      501       20      662 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0      501       20     1246 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/pkginfo.py
+-rw-r--r--   0      501       20      974 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/util.py
+-rw-r--r--   0      501       20     7125 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/_vendor/wheel/wheelfile.py
+-rw-r--r--   0      501       20      878 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/fix-and-copy-wheel.py
+-rw-r--r--   0      501       20     2981 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/tmpdirs.py
+-rw-r--r--   0      501       20     4469 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/tools.py
+-rw-r--r--   0      501       20     9484 2023-06-06 06:00:19.000000 getdaft-0.1.5/tools/wheels/wheeltools.py
+-rw-r--r--   0      501       20       19 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/.gitignore
+-rw-r--r--   0      501       20    19576 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
+-rw-r--r--   0      501       20    12068 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20    98730 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20    11847 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9134 2023-06-06 06:00:19.000000 getdaft-0.1.5/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20    34807 2023-06-06 06:00:59.000000 getdaft-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0    10384 1970-01-01 00:00:00.000000 getdaft-0.1.5/PKG-INFO
```

### Comparing `getdaft-0.1.4/Cargo.toml` & `getdaft-0.1.5/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [dependencies]
 dyn-clone = "1.0.11"
 fnv = "1.0.7"
 ndarray = "0.15.6"
 num-derive = "0.3.3"
 prettytable-rs = "^0.10"
-pyo3-log = "0.8.1"
+pyo3-log = "0.8.2"
 rand = "^0.8"
 serde_json = "1.0.96"
 
 [features]
 default = [ "python",]
 python = [ "dep:pyo3", "dep:numpy",]
 
@@ -18,15 +18,15 @@
 
 [net]
 git-fetch-with-cli = true
 
 [package]
 edition = "2021"
 name = "daft"
-version = "0.1.4"
+version = "0.1.5"
 
 [dependencies.arrow2]
 branch = "clark/expand-casting-support"
 features = [ "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc",]
 git = "https://github.com/Eventual-Inc/arrow2"
 package = "arrow2"
 version = "0.17.1"
```

### Comparing `getdaft-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `getdaft-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `getdaft-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/workflows/broken-link-checker.yml` & `getdaft-0.1.5/.github/workflows/broken-link-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/workflows/daft-profiling.yml` & `getdaft-0.1.5/.github/workflows/daft-profiling.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/workflows/notebook-checker.yml` & `getdaft-0.1.5/.github/workflows/notebook-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/workflows/property-based-tests.yml` & `getdaft-0.1.5/.github/workflows/property-based-tests.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/workflows/python-package.yml` & `getdaft-0.1.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/workflows/python-publish.yml` & `getdaft-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.github/workflows/ray-compatibility.yml` & `getdaft-0.1.5/.github/workflows/ray-compatibility.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/.pre-commit-config.yaml` & `getdaft-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/CONTRIBUTING.md` & `getdaft-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/LICENSE` & `getdaft-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/Makefile` & `getdaft-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/benchmarking/tpch/__main__.py` & `getdaft-0.1.5/benchmarking/tpch/__main__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/benchmarking/tpch/answers.py` & `getdaft-0.1.5/benchmarking/tpch/answers.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/benchmarking/tpch/data_generation.py` & `getdaft-0.1.5/benchmarking/tpch/data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/benchmarking/tpch/pipelined_data_generation.py` & `getdaft-0.1.5/benchmarking/tpch/pipelined_data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/ci/upload_wheels.sh` & `getdaft-0.1.5/ci/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/__init__.py` & `getdaft-0.1.5/daft/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/analytics.py` & `getdaft-0.1.5/daft/analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/api_annotations.py` & `getdaft-0.1.5/daft/api_annotations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/arrow_utils.py` & `getdaft-0.1.5/daft/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/context.py` & `getdaft-0.1.5/daft/context.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/convert.py` & `getdaft-0.1.5/daft/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/daft.pyi` & `getdaft-0.1.5/daft/daft.pyi`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/dataframe/dataframe.py` & `getdaft-0.1.5/daft/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/datasources.py` & `getdaft-0.1.5/daft/datasources.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/datatype.py` & `getdaft-0.1.5/daft/datatype.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/execution/execution_step.py` & `getdaft-0.1.5/daft/execution/execution_step.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/execution/logical_op_runners.py` & `getdaft-0.1.5/daft/execution/logical_op_runners.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/execution/physical_plan.py` & `getdaft-0.1.5/daft/execution/physical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/execution/physical_plan_factory.py` & `getdaft-0.1.5/daft/execution/physical_plan_factory.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/expressions/expressions.py` & `getdaft-0.1.5/daft/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/expressions/testing.py` & `getdaft-0.1.5/daft/expressions/testing.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/filesystem.py` & `getdaft-0.1.5/daft/filesystem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/internal/rule.py` & `getdaft-0.1.5/daft/internal/rule.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/internal/rule_runner.py` & `getdaft-0.1.5/daft/internal/rule_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/internal/treenode.py` & `getdaft-0.1.5/daft/internal/treenode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/io/_csv.py` & `getdaft-0.1.5/daft/io/_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/io/_json.py` & `getdaft-0.1.5/daft/io/_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/io/common.py` & `getdaft-0.1.5/daft/io/common.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/io/file_path.py` & `getdaft-0.1.5/daft/io/file_path.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/io/parquet.py` & `getdaft-0.1.5/daft/io/parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/logical/aggregation_plan_builder.py` & `getdaft-0.1.5/daft/logical/aggregation_plan_builder.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/logical/logical_plan.py` & `getdaft-0.1.5/daft/logical/logical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/logical/map_partition_ops.py` & `getdaft-0.1.5/daft/logical/map_partition_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/logical/optimizer.py` & `getdaft-0.1.5/daft/logical/optimizer.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/logical/schema.py` & `getdaft-0.1.5/daft/logical/schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/pickle/cloudpickle.py` & `getdaft-0.1.5/daft/pickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/pickle/cloudpickle_fast.py` & `getdaft-0.1.5/daft/pickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/pickle/compat.py` & `getdaft-0.1.5/daft/pickle/compat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/resource_request.py` & `getdaft-0.1.5/daft/resource_request.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/runners/partitioning.py` & `getdaft-0.1.5/daft/runners/partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/runners/profiler.py` & `getdaft-0.1.5/daft/runners/profiler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/runners/pyrunner.py` & `getdaft-0.1.5/daft/runners/pyrunner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/runners/ray_runner.py` & `getdaft-0.1.5/daft/runners/ray_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/runners/runner.py` & `getdaft-0.1.5/daft/runners/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/runners/runner_io.py` & `getdaft-0.1.5/daft/runners/runner_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/series.py` & `getdaft-0.1.5/daft/series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/table/table.py` & `getdaft-0.1.5/daft/table/table.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/table/table_io.py` & `getdaft-0.1.5/daft/table/table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/udf.py` & `getdaft-0.1.5/daft/udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/udf_library/url_udfs.py` & `getdaft-0.1.5/daft/udf_library/url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/utils.py` & `getdaft-0.1.5/daft/utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/viz/dataframe_display.py` & `getdaft-0.1.5/daft/viz/dataframe_display.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/viz/html_viz_hooks.py` & `getdaft-0.1.5/daft/viz/html_viz_hooks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/daft/viz/repr.py` & `getdaft-0.1.5/daft/viz/repr.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/Makefile` & `getdaft-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/10-min.ipynb` & `getdaft-0.1.5/docs/source/10-min.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/daft-favicon.png` & `getdaft-0.1.5/docs/source/_static/daft-favicon.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/daft-logo.png` & `getdaft-0.1.5/docs/source/_static/daft-logo.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/daft_illustration.png` & `getdaft-0.1.5/docs/source/_static/daft_illustration.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/execution_model.png` & `getdaft-0.1.5/docs/source/_static/execution_model.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/header.css` & `getdaft-0.1.5/docs/source/_static/header.css`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/high_level_architecture.png` & `getdaft-0.1.5/docs/source/_static/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/in_memory_data_representation.png` & `getdaft-0.1.5/docs/source/_static/in_memory_data_representation.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/mobile-menu.js` & `getdaft-0.1.5/docs/source/_static/mobile-menu.js`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/tpch-1000sf.html` & `getdaft-0.1.5/docs/source/_static/tpch-1000sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/tpch-100sf.html` & `getdaft-0.1.5/docs/source/_static/tpch-100sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_static/tpch-nodes-count-daft-1000-sf.html` & `getdaft-0.1.5/docs/source/_static/tpch-nodes-count-daft-1000-sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_templates/layout.html` & `getdaft-0.1.5/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/_templates/sections/header.html` & `getdaft-0.1.5/docs/source/_templates/sections/header.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 <div class="header-container">
     <a href="/"><img class="header-logo" src="{{ pathto('_static/daft-logo.png', 1) }}" alt="Daft logo" /></a>
     <nav class="header-nav">
         <ul class="header-nav-list">
             <li class="header-nav-listitem">
-                <a href="/index.html#get-started">
+                <a href="https://www.getdaft.io/#get-started">
                     Get Started
                 </a>
             </li>
             <li class="header-nav-listitem">
                 <a href="/projects/docs/">
                     Documentation
                 </a>
             </li>
             <li class="header-nav-listitem">
                 <a href="https://www.github.com/Eventual-Inc/Daft">
                     Github
                 </a>
             </li>
             <li class="header-nav-listitem">
-                <a href="/index.html#community">
+                <a href="https://blog.getdaft.io/">
+                    Blog
+                </a>
+            </li>
+            <li class="header-nav-listitem">
+                <a href="https://www.getdaft.io/#community">
                     Community
                 </a>
             </li>
         </ul>
     </nav>
     <a class="main-menu-open-button" href="#" data-behavior="open-mobile-menu"></a>
 </div>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
 [Daft_logo]
     * Get_Started
     * Documentation
     * Github
+    * Blog
     * Community
```

### Comparing `getdaft-0.1.4/docs/source/_templates/sections/mobile-menu.html` & `getdaft-0.1.5/docs/source/_templates/sections/mobile-menu.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 <div class="mobile-main-menu">
     <div class="header-container">
         <a href="/"><img class="header-logo" src="{{ pathto('_static/daft-logo.png', 1) }}" alt="Daft logo" /></a>
         <a href="#" class="main-menu-close-button" data-behavior="close-mobile-menu"></a>
     </div>
     <ul class="header-nav-list mobile">
         <li class="header-nav-listitem mobile">
-            <a href="/index.html#get-started">
+            <a href="https://www.getdaft.io/#get-started">
                 Get Started
             </a>
         </li>
         <li class="header-nav-listitem mobile">
             <a href="/projects/docs/">
                 Documentation
             </a>
         </li>
         <li class="header-nav-listitem mobile">
             <a href="https://www.github.com/Eventual-Inc/Daft">
                 Github
             </a>
         </li>
         <li class="header-nav-listitem mobile">
-            <a href="/index.html#community">
+            <a href="https://blog.getdaft.io/">
+                Blog
+            </a>
+        </li>
+        <li class="header-nav-listitem mobile">
+            <a href="https://www.getdaft.io/#community">
                 Community
             </a>
         </li>
     </ul>
 </div>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 [Daft_logo]
     * Get_Started
     * Documentation
     * Github
+    * Blog
     * Community
```

### Comparing `getdaft-0.1.4/docs/source/api_docs/dataframe.rst` & `getdaft-0.1.5/docs/source/api_docs/dataframe.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/api_docs/datatype.rst` & `getdaft-0.1.5/docs/source/api_docs/datatype.rst`

 * *Files 8% similar despite different names*

```diff
@@ -103,26 +103,35 @@
     :toctree: datatype_methods
 
     daft.DataType.python
 
 
 .. _api-datatypes-complex:
 
-More Complex Types
-------------------
+Complex Types
+-------------
 
 Machine Learning
 ^^^^^^^^^^^^^^^^
 
 .. autosummary::
     :nosignatures:
     :toctree: datatype_methods
 
     daft.DataType.embedding
 
+Computer Vision
+^^^^^^^^^^^^^^^
+
+.. autosummary::
+    :nosignatures:
+    :toctree: datatype_methods
+
+    daft.DataType.image
+
 
 Miscellaneous
 ^^^^^^^^^^^^^
 .. autosummary::
     :nosignatures:
     :toctree: datatype_methods
```

### Comparing `getdaft-0.1.4/docs/source/api_docs/expressions.rst` & `getdaft-0.1.5/docs/source/api_docs/expressions.rst`

 * *Files 10% similar despite different names*

```diff
@@ -69,28 +69,30 @@
     daft.expressions.Expression.__ne__
     daft.expressions.Expression.__gt__
     daft.expressions.Expression.__ge__
     daft.expressions.Expression.is_null
 
 .. _expression-accessor-properties:
 
-.. _api-string-expression-operations:
+.. _api-float-expression-operations:
 
 Floats
 ******
 
 Operations on strings, accessible through the ``Expression.float`` method accessor.
 
 Example: ``e1.float.is_nan()``
 
 .. autosummary::
     :toctree: expression_methods
 
     daft.expressions.expressions.ExpressionFloatNamespace.is_nan
 
+.. _api-string-expression-operations:
+
 Strings
 *******
 
 Operations on strings, accessible through the ``Expression.str`` method accessor.
 
 Example: ``e1.str.concat(e2)``
 
@@ -117,28 +119,45 @@
     :toctree: expression_methods
 
     daft.expressions.expressions.ExpressionDatetimeNamespace.day
     daft.expressions.expressions.ExpressionDatetimeNamespace.month
     daft.expressions.expressions.ExpressionDatetimeNamespace.year
     daft.expressions.expressions.ExpressionDatetimeNamespace.day_of_week
 
+.. _api-expressions-urls:
 
 URLs
 ****
 
 Operations on URLs, accessible through the ``Expression.url`` method accessor:
 
 Example: ``e.url.download()``
 
 .. autosummary::
     :nosignatures:
     :toctree: expression_methods
 
     daft.expressions.expressions.ExpressionUrlNamespace.download
 
+.. _api-expressions-images:
+
+Images
+******
+
+Operations on images, accessible through the ``Expression.image`` method accessor:
+
+Example: ``e.image.resize()``
+
+.. autosummary::
+    :nosignatures:
+    :toctree: expression_methods
+
+    daft.expressions.expressions.ExpressionImageNamespace.resize
+    daft.expressions.expressions.ExpressionImageNamespace.decode
+
 
 Changing Column Names/Types
 ###########################
 
 .. autosummary::
     :nosignatures:
     :toctree: expression_methods
```

### Comparing `getdaft-0.1.4/docs/source/api_docs/groupby.rst` & `getdaft-0.1.5/docs/source/api_docs/groupby.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/api_docs/input_output.rst` & `getdaft-0.1.5/docs/source/api_docs/input_output.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/benchmarks/index.rst` & `getdaft-0.1.5/docs/source/benchmarks/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/conf.py` & `getdaft-0.1.5/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 author = "Eventual"
 # html_logo = "_static/daft-logo.png"
 html_favicon = "_static/daft-favicon.png"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
+# The name of a reST role (builtin or Sphinx extension) to use as the default role, that
+# is, for text marked up `like this`. This can be set to 'py:obj' to make `filter` a
+# cross-reference to the Python function “filter”. The default is None, which doesn’t
+# reassign the default role.
+
+default_role = "py:obj"
+
 extensions = [
     "sphinx_reredirects",
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.autosummary",
     "sphinx.ext.linkcode",
     "IPython.sphinxext.ipython_console_highlighting",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `getdaft-0.1.4/docs/source/dataframe_comparison.rst` & `getdaft-0.1.5/docs/source/dataframe_comparison.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 * Extract/Transform/Load (ETL): Defining data pipelines that clean and process data for consumption by other users
 * Data Analytics: Analyzing data by producing summaries and reports
 
 Daft Dataframe focuses on Machine Learning/Deep Learning workloads that often involve Complex media data (images, video, audio, text documents and more).
 
 Below we discuss some other Dataframe libraries and compare them to Daft.
 
+
+.. csv-table::
+ :file: _static/dataframe-comp-table.csv
+ :widths: 30, 30, 50, 30, 50, 30, 30
+ :header-rows: 1
+
+
+
 Pandas/Modin
 ------------
 
 The main drawback of using Pandas is scalability. Pandas is single-threaded and not built for distributed computing. While this is not as much of a problem for purely tabular datasets, when dealing with data such as images/video your data can get very large and expensive to compute very quickly.
 
 Modin is a project that provides "distributed Pandas". If the use-case is tabular, has code that is already written in Pandas but just needs to be scaled up to larger data, Modin may be a good choice. Modin aims to be 100% Pandas API compatible which means that certain operations that are important for performance in the world of complex data such as requesting for certain amount of resources (e.g. GPUs) is not yet possible.
```

### Comparing `getdaft-0.1.4/docs/source/index.rst` & `getdaft-0.1.5/docs/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Daft Documentation
 ==================
 
 Daft is a **fast and scalable Python dataframe** for Complex Data and Machine Learning workloads.
 
 .. NOTE::
 
-   *Daft is currently in its Alpha release phase - please expect bugs and rapid improvements to the project. We welcome user feedback/feature requests in our* `Discussions forums <https://github.com/Eventual-Inc/Daft/discussions>`_.
+   *Daft is currently in its Beta release phase - please expect bugs and rapid improvements to the project. We welcome user feedback/feature requests in our* `Discussions forums <https://github.com/Eventual-Inc/Daft/discussions>`_.
 
 Installing Daft
 ---------------
 
 To install Daft, run this from your terminal:
 
 ``pip install getdaft``
```

### Comparing `getdaft-0.1.4/docs/source/install.rst` & `getdaft-0.1.5/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/index.rst` & `getdaft-0.1.5/docs/source/learn/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/key_concepts.rst` & `getdaft-0.1.5/docs/source/learn/key_concepts.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/tutorials.rst` & `getdaft-0.1.5/docs/source/learn/tutorials.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,35 @@
 MNIST Digit Classification
 --------------------------
 
 Load the MNIST image dataset and use a simple deep learning model to run classification on each image. Evaluate the model's performance with simple aggregations.
 
 `Run this tutorial on Google Colab <https://colab.research.google.com/github/Eventual-Inc/Daft/blob/main/tutorials/mnist.ipynb>`__
 
+
+Running LLMs on the Red Pajamas Dataset
+---------------------------------------
+
+Load the Red Pajamas dataset and perform similarity search on Stack Exchange questions using language models and embeddings.
+
+`Run this tutorial on Google Colab <https://colab.research.google.com/github/Eventual-Inc/Daft/blob/main/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb>`__
+
 Querying Images with UDFs
 -------------------------
 
 Query the Open Images dataset to retrieve the top N "reddest" images. This tutorial uses common open-source tools such as numpy and Pillow inside Daft UDFs to execute this query.
 
 `Run this tutorial on Google Colab <https://colab.research.google.com/github/Eventual-Inc/Daft/blob/main/tutorials/image_querying/top_n_red_color.ipynb>`__
 
 Image generation on GPUs
 ------------------------
 
 Generate images from text prompts using a deep learning model (Mini DALL-E) and Daft UDFs. Run Daft UDFs on GPUs for more efficient resource allocation.
 
 `Run this tutorial on Google Colab <https://colab.research.google.com/github/Eventual-Inc/Daft/blob/main/tutorials/text_to_image/text_to_image_generation.ipynb>`__
 
+
 .. Other ideas:
 .. Scaling up in the cloud with Ray **[Coming Soon]**
 .. Building a HTTP service **[Coming Soon]**
 .. Interacting with external services to build a data annotation pipeline **[Coming Soon]**
 .. Data preparation for ML model training **[Coming Soon]**
```

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/aggregations.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/aggregations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/dataframe-operations.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/dataframe-operations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/datatypes.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/datatypes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -99,26 +99,26 @@
 Python is AWESOME because it's so flexible, but it's also slow and memory inefficient! Thus we recommend:
 
 1. **Cast early!**: Casting your Python data into native Daft DataTypes if possible - this results in much more efficient downstream data serialization and computation.
 2. **Use Python UDFs**: If there is no suitable Daft representation for your Python objects, use Python UDFs to process your Python data and extract the relevant data to be returned as native Daft DataTypes!
 
 .. NOTE::
 
-    If you work with Python class for a generalizable use-case (e.g. images, documents, protobufs), it may be that these types are good candidates for "promotion" into a native Daft type!
+    If you work with Python classes for a generalizable use-case (e.g. images, documents, protobufs), it may be that these types are good candidates for "promotion" into a native Daft type!
     Please get in touch with the Daft team and we would love to work together on building your type into canonical Daft types.
 
-Other Complex Types
--------------------
+Complex Types
+-------------
 
 Daft supports many more interesting complex DataTypes, for example:
 
-* ``DataType.embedding()``: Embeddings used in Machine Learning
-* ``DataType.image()``: 2D Images!
+* :meth:`~daft.DataType.embedding()`: Lower-dimensional vector representation of data (e.g. words)
+* :meth:`~daft.DataType.image()`: NHWC images
 
-Daft abstracts away the in-memory representation of your data, as well as provides kernels for many common operations on top of this type of data (e.g. resizing an image).
+Daft abstracts away the in-memory representation of your data and provides kernels for many common operations on top of these data types. For supported image operations see the :ref:`image expressions API reference <api-expressions-images>`.
 
 For more complex algorithms, you can also drop into a Python UDF to process this data using your custom Python libraries.
 
 Please add suggestions for new DataTypes to our Github Discussions page!
 
 See also:
```

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/expressions.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/intro-dataframes.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/intro-dataframes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/read-write.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/read-write.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/scaling-up.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/scaling-up.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides/udf.rst` & `getdaft-0.1.5/docs/source/learn/user_guides/udf.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/learn/user_guides.rst` & `getdaft-0.1.5/docs/source/learn/user_guides.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.13.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.13.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.14.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.14.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.16.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.16.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.17.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.17.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.18.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.18.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.19.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.19.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.20.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.20.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.21.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.21.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.22.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.22.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.23.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.23.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.0.24.rst` & `getdaft-0.1.5/docs/source/release_notes/0.0.24.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.1.0.rst` & `getdaft-0.1.5/docs/source/release_notes/0.1.0.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.1.1.rst` & `getdaft-0.1.5/docs/source/release_notes/0.1.1.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.1.2.rst` & `getdaft-0.1.5/docs/source/release_notes/0.1.2.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.1.3.rst` & `getdaft-0.1.5/docs/source/release_notes/0.1.3.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/0.1.4.rst` & `getdaft-0.1.5/docs/source/release_notes/0.1.4.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/release_notes/_template.rst` & `getdaft-0.1.5/docs/source/release_notes/_template.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/technical_architecture.rst` & `getdaft-0.1.5/docs/source/technical_architecture.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/docs/source/telemetry.rst` & `getdaft-0.1.5/docs/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/pyproject.toml` & `getdaft-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/requirements-dev.txt` & `getdaft-0.1.5/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Tracing
 orjson==3.9.0  # orjson recommended for viztracer
 py-spy==0.3.14
 viztracer==0.15.6
 
 # Testing frameworks
-hypothesis==6.75.9
+hypothesis==6.76.0
 pytest==7.3.1
 pytest-benchmark==4.0.0
 pytest-cov==4.1.0
 
 # Testing dependencies
 lxml==4.9.2
 dask==2022.2.0; python_version < '3.8'
```

### Comparing `getdaft-0.1.4/src/array/from.rs` & `getdaft-0.1.5/src/array/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/iterator.rs` & `getdaft-0.1.5/src/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/mod.rs` & `getdaft-0.1.5/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/apply.rs` & `getdaft-0.1.5/src/array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/arange.rs` & `getdaft-0.1.5/src/array/ops/arange.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/arithmetic.rs` & `getdaft-0.1.5/src/array/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/arrow2/comparison.rs` & `getdaft-0.1.5/src/array/ops/arrow2/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/common.rs` & `getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/common.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/indices.rs` & `getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/indices.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/sort.rs` & `getdaft-0.1.5/src/array/ops/arrow2/sort/primitive/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/as_arrow.rs` & `getdaft-0.1.5/src/array/ops/as_arrow.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,19 @@
     datatypes::{
         logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
         BinaryArray, BooleanArray, DaftNumericType, FixedSizeListArray, ListArray, StructArray,
         Utf8Array,
     },
 };
 
+#[cfg(feature = "python")]
+use crate::array::pseudo_arrow::PseudoArrowArray;
+#[cfg(feature = "python")]
+use crate::datatypes::PythonArray;
+
 pub trait AsArrow {
     type Output;
 
     fn as_arrow(&self) -> &Self::Output;
 }
 
 impl<T> AsArrow for DataArray<T>
@@ -88,16 +93,16 @@
     // downcasts a DataArray<T> to an Arrow StructArray.
     fn as_arrow(&self) -> &Self::Output {
         self.data().as_any().downcast_ref().unwrap()
     }
 }
 
 #[cfg(feature = "python")]
-impl AsArrow for crate::datatypes::PythonArray {
-    type Output = crate::array::pseudo_arrow::PseudoArrowArray<pyo3::PyObject>;
+impl AsArrow for PythonArray {
+    type Output = PseudoArrowArray<pyo3::PyObject>;
 
     // downcasts a DataArray<T> to a PseudoArrowArray of PyObject.
     fn as_arrow(&self) -> &Self::Output {
         self.data().as_any().downcast_ref().unwrap()
     }
 }
```

### Comparing `getdaft-0.1.4/src/array/ops/broadcast.rs` & `getdaft-0.1.5/src/array/ops/broadcast.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,19 @@
         ListArray, NullArray, StructArray, Utf8Array,
     },
     error::{DaftError, DaftResult},
 };
 
 use super::as_arrow::AsArrow;
 
+#[cfg(feature = "python")]
+use crate::array::pseudo_arrow::PseudoArrowArray;
+#[cfg(feature = "python")]
+use crate::datatypes::PythonArray;
+
 pub trait Broadcastable {
     fn broadcast(&self, num: usize) -> DaftResult<Self>
     where
         Self: Sized;
 }
 
 impl<T> Broadcastable for DataArray<T>
@@ -288,13 +293,12 @@
             let is_none = Python::with_gil(|py| val.is_none(py));
             match is_none {
                 true => Some(arrow2::bitmap::Bitmap::new_zeroed(num)),
                 false => None,
             }
         };
 
-        let repeated_values_array: Box<dyn arrow2::array::Array> = Box::new(
-            crate::array::pseudo_arrow::PseudoArrowArray::new(repeated_values.into(), validity),
-        );
-        crate::datatypes::PythonArray::new(self.field.clone(), repeated_values_array)
+        let repeated_values_array: Box<dyn arrow2::array::Array> =
+            Box::new(PseudoArrowArray::new(repeated_values.into(), validity));
+        PythonArray::new(self.field.clone(), repeated_values_array)
     }
 }
```

### Comparing `getdaft-0.1.4/src/array/ops/cast.rs` & `getdaft-0.1.5/src/array/ops/cast.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 use arrow2::compute::{
     self,
     cast::{can_cast_types, cast, CastOptions},
 };
 
 use crate::series::IntoSeries;
 use crate::{
-    array::{ops::image::ImageArrayVecs, DataArray},
+    array::DataArray,
     datatypes::logical::{
         DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, LogicalArray,
     },
     datatypes::{DaftArrowBackedType, DataType, Field, Utf8Array},
     error::{DaftError, DaftResult},
     series::Series,
-    with_match_arrow_daft_types, with_match_daft_logical_types, with_match_numeric_daft_types,
+    with_match_arrow_daft_types, with_match_daft_logical_types,
 };
-use arrow2::array::Array;
-use num_traits::NumCast;
 
 #[cfg(feature = "python")]
-use crate::datatypes::{FixedSizeListArray, ListArray};
+use crate::array::{ops::image::ImageArrayVecs, pseudo_arrow::PseudoArrowArray};
+#[cfg(feature = "python")]
+use crate::datatypes::{FixedSizeListArray, ImageMode, ListArray, PythonArray};
+#[cfg(feature = "python")]
+use crate::ffi;
 #[cfg(feature = "python")]
-use crate::datatypes::{ImageMode, PythonArray};
+use crate::with_match_numeric_daft_types;
+#[cfg(feature = "python")]
+use arrow2::array::Array;
 #[cfg(feature = "python")]
 use log;
 #[cfg(feature = "python")]
-use num_traits::ToPrimitive;
+use ndarray::IntoDimension;
+#[cfg(feature = "python")]
+use num_traits::{NumCast, ToPrimitive};
 #[cfg(feature = "python")]
-use numpy::PyReadonlyArrayDyn;
+use numpy::{PyArray3, PyReadonlyArrayDyn};
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
 #[cfg(feature = "python")]
 use std::iter;
+#[cfg(feature = "python")]
+use std::ops::Deref;
 
 use super::as_arrow::AsArrow;
 use std::sync::Arc;
 fn arrow_cast<T>(to_cast: &DataArray<T>, dtype: &DataType) -> DaftResult<Series>
 where
     T: DaftArrowBackedType,
 {
@@ -697,16 +705,91 @@
     pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
         self.physical.cast(dtype)
     }
 }
 
 impl ImageArray {
     pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
-        self.physical.cast(dtype)
+        match dtype {
+            #[cfg(feature = "python")]
+            DataType::Python => Python::with_gil(|py| {
+                let mut ndarrays = Vec::with_capacity(self.len());
+                let da = self.data_array();
+                let ca = self.channel_array();
+                let ha = self.height_array();
+                let wa = self.width_array();
+                let pyarrow = py.import("pyarrow")?;
+                for (i, arrow_array) in da.iter().enumerate() {
+                    let shape = (
+                        ha.value(i) as usize,
+                        wa.value(i) as usize,
+                        ca.value(i) as usize,
+                    );
+                    let py_array = match arrow_array {
+                        Some(arrow_array) => ffi::to_py_array(arrow_array, py, pyarrow)?
+                            .call_method1(py, pyo3::intern!(py, "to_numpy"), (false,))?
+                            .call_method1(py, pyo3::intern!(py, "reshape"), (shape,))?,
+                        None => PyArray3::<u8>::zeros(py, shape.into_dimension(), false)
+                            .deref()
+                            .to_object(py),
+                    };
+                    ndarrays.push(py_array);
+                }
+                let values_array =
+                    PseudoArrowArray::new(ndarrays.into(), self.as_arrow().validity().cloned());
+                Ok(PythonArray::new(
+                    Field::new(self.name(), dtype.clone()).into(),
+                    values_array.to_boxed(),
+                )?
+                .into_series())
+            }),
+            _ => self.physical.cast(dtype),
+        }
     }
 }
 
 impl FixedShapeImageArray {
     pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
-        self.physical.cast(dtype)
+        match (dtype, self.logical_type()) {
+            #[cfg(feature = "python")]
+            (DataType::Python, DataType::FixedShapeImage(_, mode, height, width)) => {
+                pyo3::Python::with_gil(|py| {
+                    let shape = (
+                        self.len(),
+                        *height as usize,
+                        *width as usize,
+                        mode.num_channels() as usize,
+                    );
+                    let pyarrow = py.import("pyarrow")?;
+                    // Only go through FFI layer once instead of for every image.
+                    // We create an (N, H, W, C) ndarray view on the entire image array
+                    // buffer sans the validity mask, and then create a subndarray view
+                    // for each image ndarray in the PythonArray.
+                    let py_array = ffi::to_py_array(
+                        self.as_arrow().values().with_validity(None),
+                        py,
+                        pyarrow,
+                    )?
+                    .call_method1(py, pyo3::intern!(py, "to_numpy"), (false,))?
+                    .call_method1(
+                        py,
+                        pyo3::intern!(py, "reshape"),
+                        (shape,),
+                    )?;
+                    let ndarrays = py_array
+                        .as_ref(py)
+                        .iter()?
+                        .map(|a| a.unwrap().to_object(py))
+                        .collect::<Vec<PyObject>>();
+                    let values_array =
+                        PseudoArrowArray::new(ndarrays.into(), self.as_arrow().validity().cloned());
+                    Ok(PythonArray::new(
+                        Field::new(self.name(), dtype.clone()).into(),
+                        values_array.to_boxed(),
+                    )?
+                    .into_series())
+                })
+            }
+            (_, _) => self.physical.cast(dtype),
+        }
     }
 }
```

### Comparing `getdaft-0.1.4/src/array/ops/compare_agg.rs` & `getdaft-0.1.5/src/array/ops/compare_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/comparison.rs` & `getdaft-0.1.5/src/array/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/concat.rs` & `getdaft-0.1.5/src/array/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/concat_agg.rs` & `getdaft-0.1.5/src/array/ops/concat_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/count.rs` & `getdaft-0.1.5/src/array/ops/count.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/date.rs` & `getdaft-0.1.5/src/array/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/filter.rs` & `getdaft-0.1.5/src/array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/float.rs` & `getdaft-0.1.5/src/array/ops/float.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/full.rs` & `getdaft-0.1.5/src/array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/groups.rs` & `getdaft-0.1.5/src/array/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/hash.rs` & `getdaft-0.1.5/src/array/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/if_else.rs` & `getdaft-0.1.5/src/array/ops/if_else.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/image.rs` & `getdaft-0.1.5/src/array/ops/image.rs`

 * *Files 0% similar despite different names*

```diff
@@ -180,50 +180,50 @@
     pub widths: Vec<u32>,
     pub modes: Vec<u8>,
     pub offsets: Vec<i64>,
     pub validity: Option<arrow2::bitmap::Bitmap>,
 }
 
 impl ImageArray {
-    fn image_mode(&self) -> &Option<ImageMode> {
+    pub fn image_mode(&self) -> &Option<ImageMode> {
         match self.logical_type() {
             DataType::Image(_, mode) => mode,
             _ => panic!("Expected dtype to be Image"),
         }
     }
 
-    fn data_array(&self) -> &arrow2::array::ListArray<i64> {
+    pub fn data_array(&self) -> &arrow2::array::ListArray<i64> {
         let p = self.physical.as_arrow();
         const IMAGE_DATA_IDX: usize = 0;
         let array = p.values().get(IMAGE_DATA_IDX).unwrap();
         array.as_ref().as_any().downcast_ref().unwrap()
     }
 
-    fn channel_array(&self) -> &arrow2::array::UInt16Array {
+    pub fn channel_array(&self) -> &arrow2::array::UInt16Array {
         let p = self.physical.as_arrow();
         const IMAGE_CHANNEL_IDX: usize = 1;
         let array = p.values().get(IMAGE_CHANNEL_IDX).unwrap();
         array.as_ref().as_any().downcast_ref().unwrap()
     }
 
-    fn height_array(&self) -> &arrow2::array::UInt32Array {
+    pub fn height_array(&self) -> &arrow2::array::UInt32Array {
         let p = self.physical.as_arrow();
         const IMAGE_HEIGHT_IDX: usize = 2;
         let array = p.values().get(IMAGE_HEIGHT_IDX).unwrap();
         array.as_ref().as_any().downcast_ref().unwrap()
     }
 
-    fn width_array(&self) -> &arrow2::array::UInt32Array {
+    pub fn width_array(&self) -> &arrow2::array::UInt32Array {
         let p = self.physical.as_arrow();
         const IMAGE_WIDTH_IDX: usize = 3;
         let array = p.values().get(IMAGE_WIDTH_IDX).unwrap();
         array.as_ref().as_any().downcast_ref().unwrap()
     }
 
-    fn mode_array(&self) -> &arrow2::array::UInt8Array {
+    pub fn mode_array(&self) -> &arrow2::array::UInt8Array {
         let p = self.physical.as_arrow();
         const IMAGE_MODE_IDX: usize = 4;
         let array = p.values().get(IMAGE_MODE_IDX).unwrap();
         array.as_ref().as_any().downcast_ref().unwrap()
     }
 
     pub fn from_vecs<T: arrow2::types::NativeType>(
@@ -293,15 +293,15 @@
         )?;
         Ok(ImageArray::new(
             Field::new(name, data_type),
             daft_struct_array,
         ))
     }
 
-    fn as_image_obj<'a>(&'a self, idx: usize) -> Option<DaftImageBuffer<'a>> {
+    pub fn as_image_obj<'a>(&'a self, idx: usize) -> Option<DaftImageBuffer<'a>> {
         assert!(idx < self.len());
         if !self.physical.is_valid(idx) {
             return None;
         }
 
         let da = self.data_array();
         let ca = self.channel_array();
```

### Comparing `getdaft-0.1.4/src/array/ops/len.rs` & `getdaft-0.1.5/src/array/ops/len.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/list.rs` & `getdaft-0.1.5/src/array/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/list_agg.rs` & `getdaft-0.1.5/src/array/ops/list_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/mean.rs` & `getdaft-0.1.5/src/array/ops/mean.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/mod.rs` & `getdaft-0.1.5/src/array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/null.rs` & `getdaft-0.1.5/src/array/ops/null.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/pairwise.rs` & `getdaft-0.1.5/src/array/ops/pairwise.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/sort.rs` & `getdaft-0.1.5/src/array/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/sum.rs` & `getdaft-0.1.5/src/array/ops/sum.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/take.rs` & `getdaft-0.1.5/src/array/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/ops/utf8.rs` & `getdaft-0.1.5/src/array/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/pseudo_arrow/compute.rs` & `getdaft-0.1.5/src/array/pseudo_arrow/compute.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/pseudo_arrow/mod.rs` & `getdaft-0.1.5/src/array/pseudo_arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/array/pseudo_arrow/python.rs` & `getdaft-0.1.5/src/array/pseudo_arrow/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/datatypes/dtype.rs` & `getdaft-0.1.5/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/datatypes/field.rs` & `getdaft-0.1.5/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/datatypes/image_mode.rs` & `getdaft-0.1.5/src/datatypes/image_mode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/datatypes/logical.rs` & `getdaft-0.1.5/src/datatypes/logical.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/datatypes/matching.rs` & `getdaft-0.1.5/src/datatypes/matching.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/datatypes/mod.rs` & `getdaft-0.1.5/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/datatypes/time_unit.rs` & `getdaft-0.1.5/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/arithmetic.rs` & `getdaft-0.1.5/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/expr.rs` & `getdaft-0.1.5/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/float/is_nan.rs` & `getdaft-0.1.5/src/dsl/functions/float/is_nan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/float/mod.rs` & `getdaft-0.1.5/src/dsl/functions/float/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/image/mod.rs` & `getdaft-0.1.5/src/dsl/functions/image/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/image/resize.rs` & `getdaft-0.1.5/src/dsl/functions/temporal/day_of_week.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-use crate::dsl::functions::image::ImageExpr;
-use crate::error::DaftError;
-use crate::{datatypes::Field, dsl::Expr, error::DaftResult, schema::Schema, series::Series};
+use crate::{
+    datatypes::{DataType, Field},
+    dsl::Expr,
+    error::{DaftError, DaftResult},
+    schema::Schema,
+    series::Series,
+};
 
 use super::super::FunctionEvaluator;
 
-use super::super::FunctionExpr;
+pub(super) struct DayOfWeekEvaluator {}
 
-pub struct ResizeEvaluator {}
-
-impl FunctionEvaluator for ResizeEvaluator {
+impl FunctionEvaluator for DayOfWeekEvaluator {
     fn fn_name(&self) -> &'static str {
-        "resize"
+        "day_of_week"
     }
 
-    fn to_field(&self, _: &[Expr], _: &Schema) -> DaftResult<Field> {
-        todo!("not implemented");
+    fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field> {
+        match inputs {
+            [input] => match input.to_field(schema) {
+                Ok(field) if field.dtype.is_temporal() => {
+                    Ok(Field::new(field.name, DataType::UInt32))
+                }
+                Ok(field) => Err(DaftError::TypeError(format!(
+                    "Expected input to day to be temporal, got {}",
+                    field.dtype
+                ))),
+                Err(e) => Err(e),
+            },
+            _ => Err(DaftError::SchemaMismatch(format!(
+                "Expected 1 input arg, got {}",
+                inputs.len()
+            ))),
+        }
     }
 
-    fn evaluate(&self, inputs: &[Series], expr: &Expr) -> DaftResult<Series> {
-        let (w, h) = match expr {
-            Expr::Function {
-                func: FunctionExpr::Image(ImageExpr::Resize { w, h }),
-                inputs: _,
-            } => (w, h),
-            _ => panic!("Expected ImageResize Expr, got {expr}"),
-        };
-
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
-            [input] => input.image_resize(*w, *h),
+            [input] => input.dt_day_of_week(),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 }
```

### Comparing `getdaft-0.1.4/src/dsl/functions/list/explode.rs` & `getdaft-0.1.5/src/dsl/functions/list/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/list/mod.rs` & `getdaft-0.1.5/src/dsl/functions/list/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/mod.rs` & `getdaft-0.1.5/src/dsl/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/numeric/abs.rs` & `getdaft-0.1.5/src/dsl/functions/numeric/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/numeric/mod.rs` & `getdaft-0.1.5/src/dsl/functions/numeric/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/python/mod.rs` & `getdaft-0.1.5/src/dsl/functions/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/python/partial_udf.rs` & `getdaft-0.1.5/src/dsl/functions/python/partial_udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/python/udf.rs` & `getdaft-0.1.5/src/dsl/functions/python/udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/temporal/day.rs` & `getdaft-0.1.5/src/dsl/functions/temporal/day.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/temporal/day_of_week.rs` & `getdaft-0.1.5/src/dsl/functions/temporal/year.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,43 +4,43 @@
     error::{DaftError, DaftResult},
     schema::Schema,
     series::Series,
 };
 
 use super::super::FunctionEvaluator;
 
-pub(super) struct DayOfWeekEvaluator {}
+pub(super) struct YearEvaluator {}
 
-impl FunctionEvaluator for DayOfWeekEvaluator {
+impl FunctionEvaluator for YearEvaluator {
     fn fn_name(&self) -> &'static str {
-        "day_of_week"
+        "year"
     }
 
     fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field> {
         match inputs {
             [input] => match input.to_field(schema) {
                 Ok(field) if field.dtype.is_temporal() => {
-                    Ok(Field::new(field.name, DataType::UInt32))
+                    Ok(Field::new(field.name, DataType::Int32))
                 }
                 Ok(field) => Err(DaftError::TypeError(format!(
-                    "Expected input to day to be temporal, got {}",
+                    "Expected input to year to be temporal, got {}",
                     field.dtype
                 ))),
                 Err(e) => Err(e),
             },
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 
     fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
-            [input] => input.dt_day_of_week(),
+            [input] => input.dt_year(),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 }
```

### Comparing `getdaft-0.1.4/src/dsl/functions/temporal/mod.rs` & `getdaft-0.1.5/src/dsl/functions/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/temporal/month.rs` & `getdaft-0.1.5/src/dsl/functions/temporal/month.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/temporal/year.rs` & `getdaft-0.1.5/src/dsl/functions/utf8/length.rs`

 * *Files 26% similar despite different names*

```diff
@@ -4,43 +4,42 @@
     error::{DaftError, DaftResult},
     schema::Schema,
     series::Series,
 };
 
 use super::super::FunctionEvaluator;
 
-pub(super) struct YearEvaluator {}
+pub(super) struct LengthEvaluator {}
 
-impl FunctionEvaluator for YearEvaluator {
+impl FunctionEvaluator for LengthEvaluator {
     fn fn_name(&self) -> &'static str {
-        "year"
+        "length"
     }
 
     fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field> {
         match inputs {
-            [input] => match input.to_field(schema) {
-                Ok(field) if field.dtype.is_temporal() => {
-                    Ok(Field::new(field.name, DataType::Int32))
-                }
-                Ok(field) => Err(DaftError::TypeError(format!(
-                    "Expected input to year to be temporal, got {}",
-                    field.dtype
-                ))),
+            [data] => match data.to_field(schema) {
+                Ok(data_field) => match &data_field.dtype {
+                    DataType::Utf8 => Ok(Field::new(data_field.name, DataType::UInt64)),
+                    _ => Err(DaftError::TypeError(format!(
+                        "Expects input to length to be utf8, but received {data_field}",
+                    ))),
+                },
                 Err(e) => Err(e),
             },
             _ => Err(DaftError::SchemaMismatch(format!(
-                "Expected 1 input arg, got {}",
+                "Expected 1 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 
     fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
-            [input] => input.dt_year(),
+            [data] => data.utf8_length(),
             _ => Err(DaftError::ValueError(format!(
-                "Expected 1 input arg, got {}",
+                "Expected 1 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 }
```

### Comparing `getdaft-0.1.4/src/dsl/functions/utf8/contains.rs` & `getdaft-0.1.5/src/dsl/functions/utf8/contains.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/utf8/endswith.rs` & `getdaft-0.1.5/src/dsl/functions/utf8/endswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/utf8/length.rs` & `getdaft-0.1.5/src/dsl/functions/image/decode.rs`

 * *Files 12% similar despite different names*

```diff
@@ -4,42 +4,46 @@
     error::{DaftError, DaftResult},
     schema::Schema,
     series::Series,
 };
 
 use super::super::FunctionEvaluator;
 
-pub(super) struct LengthEvaluator {}
+pub struct DecodeEvaluator {}
 
-impl FunctionEvaluator for LengthEvaluator {
+impl FunctionEvaluator for DecodeEvaluator {
     fn fn_name(&self) -> &'static str {
-        "length"
+        "decode"
     }
 
     fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field> {
         match inputs {
-            [data] => match data.to_field(schema) {
-                Ok(data_field) => match &data_field.dtype {
-                    DataType::Utf8 => Ok(Field::new(data_field.name, DataType::UInt64)),
-                    _ => Err(DaftError::TypeError(format!(
-                        "Expects input to length to be utf8, but received {data_field}",
-                    ))),
-                },
-                Err(e) => Err(e),
-            },
+            [input] => {
+                let field = input.to_field(schema)?;
+                if !matches!(field.dtype, DataType::Binary) {
+                    return Err(DaftError::TypeError(format!(
+                        "ImageDecode can only decode BinaryArrays, got {}",
+                        field
+                    )));
+                }
+                Ok(Field::new(
+                    field.name,
+                    DataType::Image(Box::new(DataType::UInt8), None),
+                ))
+            }
             _ => Err(DaftError::SchemaMismatch(format!(
-                "Expected 1 input args, got {}",
+                "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 
     fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
-            [data] => data.utf8_length(),
+            [input] => input.image_decode(),
             _ => Err(DaftError::ValueError(format!(
-                "Expected 1 input args, got {}",
+                "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 }
```

### Comparing `getdaft-0.1.4/src/dsl/functions/utf8/mod.rs` & `getdaft-0.1.5/src/dsl/functions/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/functions/utf8/startswith.rs` & `getdaft-0.1.5/src/dsl/functions/utf8/startswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/lit.rs` & `getdaft-0.1.5/src/dsl/lit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/optimization.rs` & `getdaft-0.1.5/src/dsl/optimization.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/dsl/pyobject.rs` & `getdaft-0.1.5/src/dsl/pyobject.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/error.rs` & `getdaft-0.1.5/src/error.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/ffi.rs` & `getdaft-0.1.5/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/kernels/hashing.rs` & `getdaft-0.1.5/src/kernels/hashing.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/kernels/search_sorted.rs` & `getdaft-0.1.5/src/kernels/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/kernels/utf8.rs` & `getdaft-0.1.5/src/kernels/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/lib.rs` & `getdaft-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/python/datatype.rs` & `getdaft-0.1.5/src/python/datatype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/python/expr.rs` & `getdaft-0.1.5/src/python/expr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/python/field.rs` & `getdaft-0.1.5/src/python/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/python/mod.rs` & `getdaft-0.1.5/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/python/schema.rs` & `getdaft-0.1.5/src/python/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/python/series.rs` & `getdaft-0.1.5/src/python/series.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/python/table.rs` & `getdaft-0.1.5/src/python/table.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/schema.rs` & `getdaft-0.1.5/src/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/array_impl/data_array.rs` & `getdaft-0.1.5/src/series/array_impl/data_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/array_impl/logical_array.rs` & `getdaft-0.1.5/src/series/array_impl/logical_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/from.rs` & `getdaft-0.1.5/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/mod.rs` & `getdaft-0.1.5/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/abs.rs` & `getdaft-0.1.5/src/series/ops/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/agg.rs` & `getdaft-0.1.5/src/series/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/arithmetic.rs` & `getdaft-0.1.5/src/series/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/broadcast.rs` & `getdaft-0.1.5/src/series/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/comparison.rs` & `getdaft-0.1.5/src/series/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/concat.rs` & `getdaft-0.1.5/src/series/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/date.rs` & `getdaft-0.1.5/src/series/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/downcast.rs` & `getdaft-0.1.5/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/filter.rs` & `getdaft-0.1.5/src/series/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/image.rs` & `getdaft-0.1.5/src/series/ops/image.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/list.rs` & `getdaft-0.1.5/src/series/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/mod.rs` & `getdaft-0.1.5/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/search_sorted.rs` & `getdaft-0.1.5/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/sort.rs` & `getdaft-0.1.5/src/series/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/take.rs` & `getdaft-0.1.5/src/series/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/ops/utf8.rs` & `getdaft-0.1.5/src/series/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/series/series_like.rs` & `getdaft-0.1.5/src/series/series_like.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/mod.rs` & `getdaft-0.1.5/src/table/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/agg.rs` & `getdaft-0.1.5/src/table/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/explode.rs` & `getdaft-0.1.5/src/table/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/groups.rs` & `getdaft-0.1.5/src/table/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/hash.rs` & `getdaft-0.1.5/src/table/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/joins/hash_join.rs` & `getdaft-0.1.5/src/table/ops/joins/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/joins/mod.rs` & `getdaft-0.1.5/src/table/ops/joins/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/partition.rs` & `getdaft-0.1.5/src/table/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/search_sorted.rs` & `getdaft-0.1.5/src/table/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/table/ops/sort.rs` & `getdaft-0.1.5/src/table/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/utils/arrow.rs` & `getdaft-0.1.5/src/utils/arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/src/utils/supertype.rs` & `getdaft-0.1.5/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/1.sql` & `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/1.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/10.sql` & `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/10.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/2.sql` & `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/2.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/7.sql` & `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/7.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/8.sql` & `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/8.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/9.sql` & `getdaft-0.1.5/tests/assets/tpch-sqlite-queries/9.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/benchmarks/conftest.py` & `getdaft-0.1.5/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/benchmarks/test_df_arithmetic.py` & `getdaft-0.1.5/tests/benchmarks/test_df_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/benchmarks/test_file_read.py` & `getdaft-0.1.5/tests/benchmarks/test_file_read.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/benchmarks/test_groups_and_aggs.py` & `getdaft-0.1.5/tests/benchmarks/test_groups_and_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/benchmarks/test_join.py` & `getdaft-0.1.5/tests/benchmarks/test_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/benchmarks/test_repartition.py` & `getdaft-0.1.5/tests/benchmarks/test_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/benchmarks/test_sort.py` & `getdaft-0.1.5/tests/benchmarks/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/conftest.py` & `getdaft-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/assets/311-service-requests.24.csv` & `getdaft-0.1.5/tests/cookbook/assets/311-service-requests.24.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/conftest.py` & `getdaft-0.1.5/tests/cookbook/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_aggregations.py` & `getdaft-0.1.5/tests/cookbook/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_computations.py` & `getdaft-0.1.5/tests/cookbook/test_computations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_count_rows.py` & `getdaft-0.1.5/tests/cookbook/test_count_rows.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_dataloading.py` & `getdaft-0.1.5/tests/cookbook/test_dataloading.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_distinct.py` & `getdaft-0.1.5/tests/cookbook/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_filter.py` & `getdaft-0.1.5/tests/cookbook/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_joins.py` & `getdaft-0.1.5/tests/cookbook/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_literals.py` & `getdaft-0.1.5/tests/cookbook/test_literals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_pandas_cookbook.py` & `getdaft-0.1.5/tests/cookbook/test_pandas_cookbook.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_sorting.py` & `getdaft-0.1.5/tests/cookbook/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/cookbook/test_write.py` & `getdaft-0.1.5/tests/cookbook/test_write.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/conftest.py` & `getdaft-0.1.5/tests/dataframe/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_accessors.py` & `getdaft-0.1.5/tests/dataframe/test_accessors.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_aggregations.py` & `getdaft-0.1.5/tests/dataframe/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_creation.py` & `getdaft-0.1.5/tests/dataframe/test_creation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_distinct.py` & `getdaft-0.1.5/tests/dataframe/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_explode.py` & `getdaft-0.1.5/tests/dataframe/test_explode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_filter.py` & `getdaft-0.1.5/tests/dataframe/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_getitem.py` & `getdaft-0.1.5/tests/dataframe/test_getitem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_joins.py` & `getdaft-0.1.5/tests/dataframe/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_logical_type.py` & `getdaft-0.1.5/tests/dataframe/test_logical_type.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_repr.py` & `getdaft-0.1.5/tests/dataframe/test_repr.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_select.py` & `getdaft-0.1.5/tests/dataframe/test_select.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_show.py` & `getdaft-0.1.5/tests/dataframe/test_show.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_sort.py` & `getdaft-0.1.5/tests/dataframe/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_temporals.py` & `getdaft-0.1.5/tests/dataframe/test_temporals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_to_integrations.py` & `getdaft-0.1.5/tests/dataframe/test_to_integrations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/dataframe/test_with_column.py` & `getdaft-0.1.5/tests/dataframe/test_with_column.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/test_apply.py` & `getdaft-0.1.5/tests/expressions/test_apply.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/test_expressions.py` & `getdaft-0.1.5/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/test_expressions_projection.py` & `getdaft-0.1.5/tests/expressions/test_expressions_projection.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/test_udf.py` & `getdaft-0.1.5/tests/expressions/test_udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/conftest.py` & `getdaft-0.1.5/tests/expressions/typing/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_aggs.py` & `getdaft-0.1.5/tests/expressions/typing/test_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_arithmetic.py` & `getdaft-0.1.5/tests/expressions/typing/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_compare.py` & `getdaft-0.1.5/tests/expressions/typing/test_compare.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_dt.py` & `getdaft-0.1.5/tests/expressions/typing/test_dt.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_float.py` & `getdaft-0.1.5/tests/expressions/typing/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_if_else.py` & `getdaft-0.1.5/tests/expressions/typing/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_logical.py` & `getdaft-0.1.5/tests/expressions/typing/test_logical.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/expressions/typing/test_str.py` & `getdaft-0.1.5/tests/expressions/typing/test_str.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/integration/test_tpch.py` & `getdaft-0.1.5/tests/integration/test_tpch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/conftest.py` & `getdaft-0.1.5/tests/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/test_drop_projections.py` & `getdaft-0.1.5/tests/optimizer/test_drop_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/test_drop_repartition.py` & `getdaft-0.1.5/tests/optimizer/test_drop_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/test_fold_projections.py` & `getdaft-0.1.5/tests/optimizer/test_fold_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/test_prune_columns.py` & `getdaft-0.1.5/tests/optimizer/test_prune_columns.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/test_pushdown_clauses_into_scan.py` & `getdaft-0.1.5/tests/optimizer/test_pushdown_clauses_into_scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/test_pushdown_limit.py` & `getdaft-0.1.5/tests/optimizer/test_pushdown_limit.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/optimizer/test_pushdown_predicates.py` & `getdaft-0.1.5/tests/optimizer/test_pushdown_predicates.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/property_based_testing/strategies.py` & `getdaft-0.1.5/tests/property_based_testing/strategies.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/property_based_testing/test_sort.py` & `getdaft-0.1.5/tests/property_based_testing/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/ray/test_dask.py` & `getdaft-0.1.5/tests/ray/test_dask.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/ray/test_datasets.py` & `getdaft-0.1.5/tests/ray/test_datasets.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_arithmetic.py` & `getdaft-0.1.5/tests/series/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_cast.py` & `getdaft-0.1.5/tests/series/test_cast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_comparisons.py` & `getdaft-0.1.5/tests/series/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_concat.py` & `getdaft-0.1.5/tests/series/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_embedding.py` & `getdaft-0.1.5/tests/series/test_embedding.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_filter.py` & `getdaft-0.1.5/tests/series/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_float.py` & `getdaft-0.1.5/tests/series/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_hash.py` & `getdaft-0.1.5/tests/series/test_hash.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_if_else.py` & `getdaft-0.1.5/tests/series/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_image.py` & `getdaft-0.1.5/tests/series/test_image.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,28 +44,38 @@
     "RGB16": cv2.COLOR_RGB2BGR,
     "RGBA16": cv2.COLOR_RGBA2BGRA,
     "RGB32F": cv2.COLOR_RGB2BGR,
     "RGBA32F": cv2.COLOR_RGBA2BGRA,
 }
 
 
-def test_image_arrow_round_trip():
+def test_image_round_trip():
     data = [
         np.arange(12, dtype=np.uint8).reshape((2, 2, 3)),
         np.arange(12, 39, dtype=np.uint8).reshape((3, 3, 3)),
         None,
     ]
     s = Series.from_pylist(data, pyobj="force")
 
     target_dtype = DataType.image("RGB")
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
 
+    # Test pylist roundtrip.
+    back_dtype = DataType.python()
+    back = t.cast(back_dtype)
+
+    assert back.datatype() == back_dtype
+
+    out = back.to_pylist()
+    np.testing.assert_equal(out, data)
+
+    # Test Arrow roundtrip.
     arrow_arr = t.to_arrow()
 
     assert isinstance(arrow_arr.type, DaftExtension)
     from_arrow = Series.from_arrow(t.to_arrow())
 
     assert from_arrow.datatype() == t.datatype()
     assert from_arrow.to_pylist() == t.to_pylist()
@@ -90,35 +100,34 @@
         ("RGBA", "tiff"),
         # Not supported by Daft or PIL.
         # "L16", "LA16", "RGB16", "RGBA16", "RGB32F", "RGBA32F"
     ],
 )
 def test_image_decode_pil(mode, file_format):
     np_dtype = MODE_TO_NP_DTYPE[mode]
-    img_mode = ImageMode.from_mode_string(mode)
+    ImageMode.from_mode_string(mode)
     num_channels = MODE_TO_NUM_CHANNELS[mode]
     shape = (4, 4)
     if num_channels > 1:
         shape += (num_channels,)
     arr = np.arange(np.prod(shape)).reshape(shape).astype(np_dtype)
     img = Image.fromarray(arr, mode=mode)
     img_bytes = io.BytesIO()
     img.save(img_bytes, file_format)
     img_bytes = img_bytes.getvalue()
     arrow_arr = pa.array([img_bytes, img_bytes, img_bytes], type=pa.binary())
     s = Series.from_arrow(arrow_arr)
     t = s.image.decode()
     # TODO(Clark): Infer type-leve mode if all images are the same mode.
     assert t.datatype() == DataType.image()
-    for py_img in t.to_pylist():
-        assert py_img["channel"] == num_channels
-        assert py_img["height"] == shape[0]
-        assert py_img["width"] == shape[1]
-        assert py_img["mode"] == img_mode
-        np.testing.assert_equal(np.array(py_img["data"]).reshape(shape).astype(np_dtype), arr)
+    out = t.cast(DataType.python()).to_pylist()
+    expected_arrs = [arr, arr, arr]
+    if num_channels == 1:
+        expected_arrs = [np.expand_dims(arr, -1) for arr in expected_arrs]
+    np.testing.assert_equal(out, expected_arrs)
 
 
 @pytest.mark.parametrize(
     ["mode", "file_format"],
     [
         ("L", "png"),
         ("L", "tiff"),
@@ -142,15 +151,15 @@
         # Image crate doesn't support LogLuv HDR encoding.
         # ("RGB32F", "tiff"),
         # ("RGBA32F", "tiff"),
     ],
 )
 def test_image_decode_opencv(mode, file_format):
     np_dtype = MODE_TO_NP_DTYPE[mode]
-    img_mode = ImageMode.from_mode_string(mode)
+    ImageMode.from_mode_string(mode)
     num_channels = MODE_TO_NUM_CHANNELS[mode]
     shape = (4, 4, num_channels)
     arr = np.arange(np.prod(shape)).reshape(shape).astype(np_dtype)
     cv2_arr = arr
     color_conv = MODE_TO_OPENCV_COLOR_CONVERSION.get(mode)
     if color_conv is not None:
         cv2_arr = cv2.cvtColor(arr, color_conv)
@@ -159,20 +168,17 @@
     arrow_arr = pa.array([img_bytes, img_bytes, img_bytes], type=pa.binary())
     s = Series.from_arrow(arrow_arr)
     t = s.image.decode()
     # TODO(Clark): Support constructing an Image type with an unknown mode by known dtype.
     if np_dtype == np.uint8:
         # TODO(Clark): Infer type-leve mode if all images are the same mode.
         assert t.datatype() == DataType.image()
-    for py_img in t.to_pylist():
-        assert py_img["channel"] == num_channels
-        assert py_img["height"] == shape[0]
-        assert py_img["width"] == shape[1]
-        assert py_img["mode"] == img_mode
-        np.testing.assert_equal(np.array(py_img["data"]).reshape(shape).astype(np_dtype), arr)
+    out = t.cast(DataType.python()).to_pylist()
+    expected_arrs = [arr, arr, arr]
+    np.testing.assert_equal(out, expected_arrs)
 
 
 def test_image_resize():
     first = np.ones((2, 2, 3), dtype=np.uint8)
     first[..., 1] = 2
     first[..., 2] = 3
 
@@ -184,28 +190,23 @@
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
 
     resized = t.image.resize(5, 5)
 
-    as_py = resized.to_pylist()
-
     assert resized.datatype() == target_dtype
 
-    first_resized = np.array(as_py[0]["data"]).reshape(5, 5, 3)
-    assert np.all(first_resized[..., 0] == 1)
-    assert np.all(first_resized[..., 1] == 2)
-    assert np.all(first_resized[..., 2] == 3)
-
-    sec_resized = np.array(as_py[1]["data"]).reshape(5, 5, 3)
-    sec_resized_gt = np.asarray(Image.fromarray(second).resize((5, 5), resample=Image.BILINEAR))
-    assert np.all(sec_resized == sec_resized_gt)
+    out = resized.cast(DataType.python()).to_pylist()
+
+    def resize(arr):
+        # Use opencv as a resizing baseline.
+        return cv2.resize(arr, dsize=(5, 5), interpolation=cv2.INTER_LINEAR_EXACT)
 
-    assert as_py[2] == None
+    np.testing.assert_equal(out, [resize(first), resize(second), None])
 
 
 def test_image_resize_mixed_modes():
     rgba = np.ones((2, 2, 4), dtype=np.uint8)
     rgba[..., 1] = 2
     rgba[..., 2] = 3
     rgba[..., 3] = 4
@@ -225,54 +226,49 @@
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
 
     resized = t.image.resize(5, 5)
 
-    as_py = resized.to_pylist()
+    out = resized.cast(DataType.python()).to_pylist()
 
-    assert resized.datatype() == target_dtype
-
-    first_resized = np.array(as_py[0]["data"]).reshape(5, 5, 3)
-    assert np.all(first_resized[..., 0] == 1)
-    assert np.all(first_resized[..., 1] == 2)
-    assert np.all(first_resized[..., 2] == 3)
-
-    second_resized = np.array(as_py[1]["data"]).reshape(5, 5, 4)
-    assert np.all(second_resized[..., 0] == 1)
-    assert np.all(second_resized[..., 1] == 2)
-    assert np.all(second_resized[..., 2] == 3)
-    assert np.all(second_resized[..., 3] == 4)
-
-    for i in range(2, 4):
-        resized_i = np.array(as_py[i]["data"]).reshape(5, 5, -1)
-        resized_i_gt = np.asarray(Image.fromarray(data[i]).resize((5, 5), resample=Image.BILINEAR)).reshape(5, 5, -1)
-        assert np.all(resized_i == resized_i_gt), f"{i} does not match"
-
-    # LA sampling doesn't work for some reason in PIL
-    resized_i = np.array(as_py[4]["data"]).reshape(5, 5, -1)
-    assert np.all(resized_i == 10)
+    def resize(arr):
+        # Use opencv as a resizing baseline.
+        arr = cv2.resize(arr, dsize=(5, 5), interpolation=cv2.INTER_LINEAR_EXACT)
+        if arr.ndim == 2:
+            arr = np.expand_dims(arr, -1)
+        return arr
 
-    assert as_py[-1] == None
+    np.testing.assert_equal(out, [resize(arr) if arr is not None else None for arr in data])
 
 
-def test_fixed_shape_image_arrow_round_trip():
+def test_fixed_shape_image_roundtrip():
     height = 2
     width = 2
     shape = (height, width, 3)
     data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
     s = Series.from_pylist(data, pyobj="force")
 
     target_dtype = DataType.image("RGB", height, width)
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
 
+    # Test pylist roundtrip.
+    back_dtype = DataType.python()
+    back = t.cast(back_dtype)
+
+    assert back.datatype() == back_dtype
+
+    out = back.to_pylist()
+    np.testing.assert_equal(out, data)
+
+    # Test Arrow roundtrip.
     arrow_arr = t.to_arrow()
 
     assert isinstance(arrow_arr.type, DaftExtension)
     from_arrow = Series.from_arrow(t.to_arrow())
 
     assert from_arrow.datatype() == t.datatype()
     assert from_arrow.to_pylist() == t.to_pylist()
```

### Comparing `getdaft-0.1.4/tests/series/test_numeric_ops.py` & `getdaft-0.1.5/tests/series/test_numeric_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_series.py` & `getdaft-0.1.5/tests/series/test_series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_size_bytes.py` & `getdaft-0.1.5/tests/series/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_slice.py` & `getdaft-0.1.5/tests/series/test_slice.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_sort.py` & `getdaft-0.1.5/tests/series/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_take.py` & `getdaft-0.1.5/tests/series/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_temporal_ops.py` & `getdaft-0.1.5/tests/series/test_temporal_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/series/test_utf8_ops.py` & `getdaft-0.1.5/tests/series/test_utf8_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/__init__.py` & `getdaft-0.1.5/tests/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_blackbox_kernels.py` & `getdaft-0.1.5/tests/table/test_blackbox_kernels.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_concat.py` & `getdaft-0.1.5/tests/table/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_eval.py` & `getdaft-0.1.5/tests/table/test_eval.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_explodes.py` & `getdaft-0.1.5/tests/table/test_explodes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_filter.py` & `getdaft-0.1.5/tests/table/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_from_py.py` & `getdaft-0.1.5/tests/table/test_from_py.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_head.py` & `getdaft-0.1.5/tests/table/test_head.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_joins.py` & `getdaft-0.1.5/tests/table/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_partitioning.py` & `getdaft-0.1.5/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_size_bytes.py` & `getdaft-0.1.5/tests/table/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_sorting.py` & `getdaft-0.1.5/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_table_aggs.py` & `getdaft-0.1.5/tests/table/test_table_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_table_io.py` & `getdaft-0.1.5/tests/table/test_table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/test_take.py` & `getdaft-0.1.5/tests/table/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/table/utf8/test_compares.py` & `getdaft-0.1.5/tests/table/utf8/test_compares.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/test_analytics.py` & `getdaft-0.1.5/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/test_datatypes.py` & `getdaft-0.1.5/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/test_schema.py` & `getdaft-0.1.5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests/udf_library/test_url_udfs.py` & `getdaft-0.1.5/tests/udf_library/test_url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tests_legacy/test_resource_requests.py` & `getdaft-0.1.5/tests_legacy/test_resource_requests.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/patch_package_version.py` & `getdaft-0.1.5/tools/patch_package_version.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/LICENSE.txt` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/__init__.py` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/convert.py` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/pack.py` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/unpack.py` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/pkginfo.py` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/util.py` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/_vendor/wheel/wheelfile.py` & `getdaft-0.1.5/tools/wheels/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/fix-and-copy-wheel.py` & `getdaft-0.1.5/tools/wheels/fix-and-copy-wheel.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/tmpdirs.py` & `getdaft-0.1.5/tools/wheels/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/tools.py` & `getdaft-0.1.5/tools/wheels/tools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tools/wheels/wheeltools.py` & `getdaft-0.1.5/tools/wheels/wheeltools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb` & `getdaft-0.1.5/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tutorials/image_querying/top_n_red_color.ipynb` & `getdaft-0.1.5/tutorials/image_querying/top_n_red_color.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tutorials/mnist.ipynb` & `getdaft-0.1.5/tutorials/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tutorials/text_to_image/text_to_image_generation.ipynb` & `getdaft-0.1.5/tutorials/text_to_image/text_to_image_generation.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/tutorials/text_to_image/using_cloud_with_ray.ipynb` & `getdaft-0.1.5/tutorials/text_to_image/using_cloud_with_ray.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.4/Cargo.lock` & `getdaft-0.1.5/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "daft"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "arrow2",
  "bincode",
  "dyn-clone",
  "fnv",
  "image",
  "indexmap",
@@ -778,17 +778,17 @@
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9c8b57fe71fb5dcf38970ebedc2b1531cf1c14b1b9b4c560a182a57e115575c"
+checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
```

