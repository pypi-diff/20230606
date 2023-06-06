# Comparing `tmp/orquestra-opt-0.7.0.tar.gz` & `tmp/orquestra-opt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquestra-opt-0.7.0.tar", last modified: Fri Jan 13 15:53:19 2023, max compression
+gzip compressed data, was "orquestra-opt-0.8.0.tar", last modified: Tue Jun  6 20:42:38 2023, max compression
```

## Comparing `orquestra-opt-0.7.0.tar` & `orquestra-opt-0.8.0.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.287612 orquestra-opt-0.7.0/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.243770 orquestra-opt-0.7.0/.github/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.244583 orquestra-opt-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/.github/pull_request_template.md
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.245728 orquestra-opt-0.7.0/.github/workflows/
--rw-r--r--   0 maxradin   (501) staff       (20)      930 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/.github/workflows/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      876 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/.github/workflows/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      945 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/.github/workflows/style.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1833 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/.gitignore
--rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/LICENSE
--rw-r--r--   0 maxradin   (501) staff       (20)      482 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     2173 2023-01-13 15:53:19.287854 orquestra-opt-0.7.0/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     1425 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/README.md
--rw-r--r--   0 maxradin   (501) staff       (20)     1334 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)     1164 2023-01-13 15:53:19.291057 orquestra-opt-0.7.0/setup.cfg
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.224977 orquestra-opt-0.7.0/src/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.221883 orquestra-opt-0.7.0/src/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.248190 orquestra-opt-0.7.0/src/orquestra/opt/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.252671 orquestra-opt-0.7.0/src/orquestra/opt/api/
--rw-r--r--   0 maxradin   (501) staff       (20)      692 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4881 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/_problem_evaluation.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1242 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/bqm_solver.py
--rw-r--r--   0 maxradin   (501) staff       (20)      265 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/bqm_solver_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1182 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/cost_function.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4788 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/example_functions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3828 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/functions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7184 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/optimizer.py
--rw-r--r--   0 maxradin   (501) staff       (20)    10395 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/optimizer_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1608 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/problem.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2015 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/api/save_conditions.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.254301 orquestra-opt-0.7.0/src/orquestra/opt/bqm/
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/bqm/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6768 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/bqm/conversions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3066 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/bqm/io.py
--rw-r--r--   0 maxradin   (501) staff       (20)      788 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/bqm/utils.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4459 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/convex.py
--rw-r--r--   0 maxradin   (501) staff       (20)    10390 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/cost_function_augmentations.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1257 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/gradients.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.255429 orquestra-opt-0.7.0/src/orquestra/opt/history/
--rw-r--r--   0 maxradin   (501) staff       (20)      352 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/history/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)    12025 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/history/recorder.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3364 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/mock_objects.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.259296 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/
--rw-r--r--   0 maxradin   (501) staff       (20)      789 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3971 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/basin_hopping.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2803 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/cma_es_optimizer.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.260491 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/pso/
--rw-r--r--   0 maxradin   (501) staff       (20)       88 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/pso/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)    13139 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/pso/continuous_pso_optimizer.py
--rw-r--r--   0 maxradin   (501) staff       (20)      704 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/pso/topologies.py
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/py.typed
--rw-r--r--   0 maxradin   (501) staff       (20)     3140 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/qiskit_optimizer.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4553 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/scikit_quant_optimizer.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3218 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/scipy_optimizer.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2547 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/search_points_optimizer.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3068 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/optimizers/simple_gradient_descent.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.263223 orquestra-opt-0.7.0/src/orquestra/opt/problems/
--rw-r--r--   0 maxradin   (501) staff       (20)      498 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/problems/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1434 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/problems/generators.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4956 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/problems/graph.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1738 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/problems/graph_partition.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1604 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/problems/max_independent_set.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2194 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/problems/maxcut.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2043 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/problems/vertex_cover.py
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/src/orquestra/opt/py.typed
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.265887 orquestra-opt-0.7.0/src/orquestra_opt.egg-info/
--rw-r--r--   0 maxradin   (501) staff       (20)     2173 2023-01-13 15:53:19.000000 orquestra-opt-0.7.0/src/orquestra_opt.egg-info/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     4561 2023-01-13 15:53:19.000000 orquestra-opt-0.7.0/src/orquestra_opt.egg-info/SOURCES.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:53:19.000000 orquestra-opt-0.7.0/src/orquestra_opt.egg-info/dependency_links.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:53:18.000000 orquestra-opt-0.7.0/src/orquestra_opt.egg-info/not-zip-safe
--rw-r--r--   0 maxradin   (501) staff       (20)      317 2023-01-13 15:53:19.000000 orquestra-opt-0.7.0/src/orquestra_opt.egg-info/requires.txt
--rw-r--r--   0 maxradin   (501) staff       (20)       10 2023-01-13 15:53:19.000000 orquestra-opt-0.7.0/src/orquestra_opt.egg-info/top_level.txt
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.225755 orquestra-opt-0.7.0/subtrees/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.269125 orquestra-opt-0.7.0/subtrees/z_quantum_actions/
--rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/MANIFEST.in
--rw-r--r--   0 maxradin   (501) staff       (20)     3835 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/README.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.227181 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.269902 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/coverage/
--rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/coverage/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.270355 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/publish-release/
--rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.270709 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/ssh_setup/
--rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.271140 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/style/
--rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/style/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.271537 orquestra-opt-0.7.0/subtrees/z_quantum_actions/bin/
--rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/bin/get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/pytest.ini
--rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/sample_setup.py
--rw-r--r--   0 maxradin   (501) staff       (20)      585 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/setup_extras.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.272070 orquestra-opt-0.7.0/subtrees/z_quantum_actions/tests/
--rw-r--r--   0 maxradin   (501) staff       (20)     1131 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/variables.mk
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.274257 orquestra-opt-0.7.0/subtrees/z_quantum_actions/workflow-templates/
--rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/subtrees/z_quantum_actions/workflow-templates/style.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.229467 orquestra-opt-0.7.0/tests/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.229715 orquestra-opt-0.7.0/tests/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.274793 orquestra-opt-0.7.0/tests/orquestra/opt/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.278428 orquestra-opt-0.7.0/tests/orquestra/opt/api/
--rw-r--r--   0 maxradin   (501) staff       (20)     2220 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/artifact_storage_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1558 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/attribute_forwarding_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1072 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/copying_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1242 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/functions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1392 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/gradients_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4077 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/optimizer_contract_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)      761 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/optimizer_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2519 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/optimizer_utils_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1153 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/api/save_conditions_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.279372 orquestra-opt-0.7.0/tests/orquestra/opt/bqm/
--rw-r--r--   0 maxradin   (501) staff       (20)     8774 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/bqm/test_conversion.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5195 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/bqm/test_io.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.280142 orquestra-opt-0.7.0/tests/orquestra/opt/history/
--rw-r--r--   0 maxradin   (501) staff       (20)     4996 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/history/recording_functions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1653 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/history/recording_functions_with_gradient_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.284186 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/
--rw-r--r--   0 maxradin   (501) staff       (20)     1682 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/basin_hopping_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1069 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/cma_es_optimizer_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)      760 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/pso_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6198 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/qiskit_optimizer_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3214 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/scikit_quant_optimizer_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3613 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/scipy_optimizer_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1510 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/search_points_optimizer_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3261 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/simple_gradient_descent_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:19.287341 orquestra-opt-0.7.0/tests/orquestra/opt/problems/
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)      597 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/_helpers.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1916 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/generators_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7487 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/graph_partition_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7410 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/max_independent_set_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5665 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/maxcut_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1159 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/solve_problem_by_exhaustive_search_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7174 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/problems/vertex_cover_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5705 2023-01-13 15:53:11.000000 orquestra-opt-0.7.0/tests/orquestra/opt/test_cost_function_augmentations.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.278358 orquestra-opt-0.8.0/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.218419 orquestra-opt-0.8.0/.github/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.219145 orquestra-opt-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      605 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      600 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      533 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/.github/pull_request_template.md
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.220265 orquestra-opt-0.8.0/.github/workflows/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      930 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/.github/workflows/coverage.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      876 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      945 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/.github/workflows/style.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1833 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/.gitignore
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    11357 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/LICENSE
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      482 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/Makefile
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2195 2023-06-06 20:42:38.278754 orquestra-opt-0.8.0/PKG-INFO
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1425 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/README.md
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1349 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/pyproject.toml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1217 2023-06-06 20:42:38.280169 orquestra-opt-0.8.0/setup.cfg
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.212068 orquestra-opt-0.8.0/src/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.210715 orquestra-opt-0.8.0/src/orquestra/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.222157 orquestra-opt-0.8.0/src/orquestra/opt/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.226191 orquestra-opt-0.8.0/src/orquestra/opt/api/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      866 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4881 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/_problem_evaluation.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1242 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/bqm_solver.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      265 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/bqm_solver_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1182 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/cost_function.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4788 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/example_functions.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3828 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/functions.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     7184 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/optimizer.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    10395 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/optimizer_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1608 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/problem.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2015 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/api/save_conditions.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.228129 orquestra-opt-0.8.0/src/orquestra/opt/bqm/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/bqm/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     6768 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/bqm/conversions.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3066 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/bqm/io.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      788 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/bqm/utils.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4459 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/convex.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    10390 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/cost_function_augmentations.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1257 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/gradients.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.229105 orquestra-opt-0.8.0/src/orquestra/opt/history/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      352 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/history/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    12025 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/history/recorder.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3364 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/mock_objects.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.233928 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      892 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3971 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/basin_hopping.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2803 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/cma_es_optimizer.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.235333 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/pso/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       88 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/pso/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    13041 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/pso/continuous_pso_optimizer.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      704 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/pso/topologies.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/py.typed
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3140 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/qiskit_optimizer.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4553 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/scikit_quant_optimizer.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     6987 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/scipy_optimizer.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2547 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/search_points_optimizer.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4715 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/simple_gradient_descent.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    12118 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/optimizers/tensor_train_optimizer.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.238644 orquestra-opt-0.8.0/src/orquestra/opt/problems/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      498 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/problems/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1434 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/problems/generators.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4956 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/problems/graph.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1738 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/problems/graph_partition.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1604 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/problems/max_independent_set.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2194 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/problems/maxcut.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2043 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/problems/vertex_cover.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/src/orquestra/opt/py.typed
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.241551 orquestra-opt-0.8.0/src/orquestra_opt.egg-info/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2195 2023-06-06 20:42:38.000000 orquestra-opt-0.8.0/src/orquestra_opt.egg-info/PKG-INFO
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4678 2023-06-06 20:42:38.000000 orquestra-opt-0.8.0/src/orquestra_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        1 2023-06-06 20:42:38.000000 orquestra-opt-0.8.0/src/orquestra_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        1 2023-06-06 20:42:37.000000 orquestra-opt-0.8.0/src/orquestra_opt.egg-info/not-zip-safe
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      367 2023-06-06 20:42:38.000000 orquestra-opt-0.8.0/src/orquestra_opt.egg-info/requires.txt
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       10 2023-06-06 20:42:38.000000 orquestra-opt-0.8.0/src/orquestra_opt.egg-info/top_level.txt
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.212439 orquestra-opt-0.8.0/subtrees/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.245640 orquestra-opt-0.8.0/subtrees/z_quantum_actions/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        9 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/MANIFEST.in
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3835 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/Makefile
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     5600 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/README.rst
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.213443 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.246127 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/coverage/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      790 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.246569 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/publish-release/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3132 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.247008 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      458 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.247449 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/style/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      467 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/style/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.247959 orquestra-opt-0.8.0/subtrees/z_quantum_actions/bin/
+-rwxr-xr-x   0 athenacaesura   (501) staff       (20)     2756 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1253 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/pyproject.toml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       24 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/pytest.ini
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1526 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/sample_setup.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      585 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/setup_extras.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.248424 orquestra-opt-0.8.0/subtrees/z_quantum_actions/tests/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1131 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       19 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/variables.mk
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.249990 orquestra-opt-0.8.0/subtrees/z_quantum_actions/workflow-templates/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1233 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      696 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1248 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.214606 orquestra-opt-0.8.0/tests/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.214723 orquestra-opt-0.8.0/tests/orquestra/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.250537 orquestra-opt-0.8.0/tests/orquestra/opt/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.255393 orquestra-opt-0.8.0/tests/orquestra/opt/api/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2220 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/artifact_storage_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1558 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/attribute_forwarding_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1072 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/copying_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1242 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/functions_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1392 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/gradients_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4077 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/optimizer_contract_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      761 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/optimizer_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2519 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/optimizer_utils_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1153 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/api/save_conditions_test.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.256493 orquestra-opt-0.8.0/tests/orquestra/opt/bqm/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     8774 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/bqm/test_conversion.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     5195 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/bqm/test_io.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.257495 orquestra-opt-0.8.0/tests/orquestra/opt/history/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     4996 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/history/recording_functions_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1653 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/history/recording_functions_with_gradient_test.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.262625 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1682 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/basin_hopping_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1069 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/cma_es_optimizer_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      760 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/pso_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     6198 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/qiskit_optimizer_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3214 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/scikit_quant_optimizer_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     5050 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/scipy_optimizer_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1510 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/search_points_optimizer_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3389 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/simple_gradient_descent_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      748 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/tensor_train_optimizer_test.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:38.274680 orquestra-opt-0.8.0/tests/orquestra/opt/problems/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      597 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/_helpers.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1916 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/generators_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     7487 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/graph_partition_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     7410 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/max_independent_set_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     5665 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/maxcut_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1159 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/solve_problem_by_exhaustive_search_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     7174 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/problems/vertex_cover_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     5705 2023-06-06 20:42:33.000000 orquestra-opt-0.8.0/tests/orquestra/opt/test_cost_function_augmentations.py
```

### Comparing `orquestra-opt-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `orquestra-opt-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `orquestra-opt-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/.github/pull_request_template.md` & `orquestra-opt-0.8.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/.github/workflows/coverage.yml` & `orquestra-opt-0.8.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/.github/workflows/publish_release.yml` & `orquestra-opt-0.8.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/.github/workflows/style.yml` & `orquestra-opt-0.8.0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/.gitignore` & `orquestra-opt-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/LICENSE` & `orquestra-opt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/PKG-INFO` & `orquestra-opt-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-opt
-Version: 0.7.0
+Version: 0.8.0
 Summary: "Orquestra's library with optimization routines and interfaces"
 Home-page: https://github.com/zapatacomputing/orquestra-opt
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: !=3.9.7,<3.11,>=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: scikit-quant
 Provides-Extra: cma
 Provides-Extra: qiskit
 Provides-Extra: qubo
+Provides-Extra: ttopt
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 # orquestra-opt
 
 ## What is it?
```

### Comparing `orquestra-opt-0.7.0/README.md` & `orquestra-opt-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/pyproject.toml` & `orquestra-opt-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 module = [
     'qiskit.*',
     'scipy.*',
     'symengine.*',
     'cma.*',
     'networkx.*',
     'skquant.*',
+    'ttopt.*',
 ]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 omit = ["*/__init__.py"]
 
 [tool.coverage.report]
```

### Comparing `orquestra-opt-0.7.0/setup.cfg` & `orquestra-opt-0.8.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -36,19 +36,23 @@
 cma = 
 	cma>=3.0.0
 qiskit = 
 	orquestra-qiskit
 qubo = 
 	dimod>=0.9.11
 	cvxpy~=1.1.11
+ttopt = 
+	ttopt~=0.5.0
+	teneva
 all = 
 	orquestra-opt[cma]
 	orquestra-opt[qiskit]
 	orquestra-opt[qubo]
 	orquestra-opt[scikit-quant]
+	orquestra-opt[ttopt]
 dev = 
 	orquestra-python-dev
 	orquestra-opt[all]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/__init__.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
+from typing import Sequence, Tuple, Union
+
+from scipy.optimize import Bounds as ScipyBounds
+
 from .cost_function import CostFunction
 from .functions import (
     CallableStoringArtifacts,
     CallableWithGradient,
     CallableWithGradientStoringArtifacts,
     FunctionWithGradient,
     FunctionWithGradientStoringArtifacts,
@@ -15,7 +19,9 @@
 from .optimizer import (
     NestedOptimizer,
     Optimizer,
     construct_history_info,
     optimization_result,
 )
 from .save_conditions import SaveCondition, always, every_nth
+
+Bounds = Union[ScipyBounds, Sequence[Tuple[float, float]], Tuple[float, float]]
```

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/_problem_evaluation.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/_problem_evaluation.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/bqm_solver.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/bqm_solver.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/cost_function.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/cost_function.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/example_functions.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/example_functions.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/functions.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/functions.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/optimizer.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/optimizer.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/optimizer_test.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/optimizer_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/problem.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/problem.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/api/save_conditions.py` & `orquestra-opt-0.8.0/src/orquestra/opt/api/save_conditions.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/bqm/conversions.py` & `orquestra-opt-0.8.0/src/orquestra/opt/bqm/conversions.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/bqm/io.py` & `orquestra-opt-0.8.0/src/orquestra/opt/bqm/io.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/bqm/utils.py` & `orquestra-opt-0.8.0/src/orquestra/opt/bqm/utils.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/convex.py` & `orquestra-opt-0.8.0/src/orquestra/opt/convex.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/cost_function_augmentations.py` & `orquestra-opt-0.8.0/src/orquestra/opt/cost_function_augmentations.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/gradients.py` & `orquestra-opt-0.8.0/src/orquestra/opt/gradients.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/history/recorder.py` & `orquestra-opt-0.8.0/src/orquestra/opt/history/recorder.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/mock_objects.py` & `orquestra-opt-0.8.0/src/orquestra/opt/mock_objects.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/__init__.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,10 +12,14 @@
     from .qiskit_optimizer import QiskitOptimizer
 except ModuleNotFoundError:
     pass
 try:
     from .scikit_quant_optimizer import ScikitQuantOptimizer
 except ModuleNotFoundError:
     pass
+try:
+    from .tensor_train_optimizer import TensorTrainOptimizer
+except ModuleNotFoundError:
+    pass
 from .scipy_optimizer import ScipyOptimizer
 from .search_points_optimizer import SearchPointsOptimizer
 from .simple_gradient_descent import SimpleGradientDescent
```

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/basin_hopping.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/basin_hopping.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/cma_es_optimizer.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/cma_es_optimizer.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/pso/continuous_pso_optimizer.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/pso/continuous_pso_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from typing import Callable, Optional, Sequence, Tuple, Union
+from typing import Callable, Optional, Tuple, Union
 
 import numpy as np
-from scipy.optimize import Bounds as ScipyBounds
 from scipy.optimize import OptimizeResult
 
 from orquestra.opt.api import (
+    Bounds,
     CallableWithGradient,
     Optimizer,
+    ScipyBounds,
     construct_history_info,
     optimization_result,
 )
 from orquestra.opt.history.recorder import RecorderFactory
 from orquestra.opt.history.recorder import recorder as _recorder
 from orquestra.opt.optimizers.pso.topologies import StarTopology, SwarmTopology
 
-Bounds = Union[ScipyBounds, Sequence[Tuple[float, float]], Tuple[float, float]]
-
 
 def _get_bounds_like_array(
     bounds: Bounds,
 ) -> Union[Tuple[np.ndarray, np.ndarray], Tuple[float, float]]:
     """
     Casts a Bounds object to an object with two entries: the first being the lower
     bounds and the second being the upper bounds.
@@ -32,15 +31,15 @@
     Returns:
         Union[Tuple[np.ndarray, np.ndarray], Tuple[float, float]]: Lower and
             upper bounds.
     """
     if isinstance(bounds, ScipyBounds):
         return bounds.lb, bounds.ub
     else:
-        _bounds = np.array(bounds).T
+        _bounds = np.array(bounds, dtype=float).T
         return _bounds[0], _bounds[1]
 
 
 class PSOOptimizer(Optimizer):
     def __init__(
         self,
         swarm_size: int,
```

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/pso/topologies.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/pso/topologies.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/qiskit_optimizer.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/qiskit_optimizer.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/scikit_quant_optimizer.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/scikit_quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/optimizers/search_points_optimizer.py` & `orquestra-opt-0.8.0/src/orquestra/opt/optimizers/search_points_optimizer.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/problems/generators.py` & `orquestra-opt-0.8.0/src/orquestra/opt/problems/generators.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/problems/graph.py` & `orquestra-opt-0.8.0/src/orquestra/opt/problems/graph.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/problems/graph_partition.py` & `orquestra-opt-0.8.0/src/orquestra/opt/problems/graph_partition.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/problems/max_independent_set.py` & `orquestra-opt-0.8.0/src/orquestra/opt/problems/max_independent_set.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/problems/maxcut.py` & `orquestra-opt-0.8.0/src/orquestra/opt/problems/maxcut.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra/opt/problems/vertex_cover.py` & `orquestra-opt-0.8.0/src/orquestra/opt/problems/vertex_cover.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/src/orquestra_opt.egg-info/PKG-INFO` & `orquestra-opt-0.8.0/src/orquestra_opt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-opt
-Version: 0.7.0
+Version: 0.8.0
 Summary: "Orquestra's library with optimization routines and interfaces"
 Home-page: https://github.com/zapatacomputing/orquestra-opt
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: !=3.9.7,<3.11,>=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: scikit-quant
 Provides-Extra: cma
 Provides-Extra: qiskit
 Provides-Extra: qubo
+Provides-Extra: ttopt
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 # orquestra-opt
 
 ## What is it?
```

### Comparing `orquestra-opt-0.7.0/src/orquestra_opt.egg-info/SOURCES.txt` & `orquestra-opt-0.8.0/src/orquestra_opt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 src/orquestra/opt/optimizers/cma_es_optimizer.py
 src/orquestra/opt/optimizers/py.typed
 src/orquestra/opt/optimizers/qiskit_optimizer.py
 src/orquestra/opt/optimizers/scikit_quant_optimizer.py
 src/orquestra/opt/optimizers/scipy_optimizer.py
 src/orquestra/opt/optimizers/search_points_optimizer.py
 src/orquestra/opt/optimizers/simple_gradient_descent.py
+src/orquestra/opt/optimizers/tensor_train_optimizer.py
 src/orquestra/opt/optimizers/pso/__init__.py
 src/orquestra/opt/optimizers/pso/continuous_pso_optimizer.py
 src/orquestra/opt/optimizers/pso/topologies.py
 src/orquestra/opt/problems/__init__.py
 src/orquestra/opt/problems/generators.py
 src/orquestra/opt/problems/graph.py
 src/orquestra/opt/problems/graph_partition.py
@@ -92,14 +93,15 @@
 tests/orquestra/opt/optimizers/cma_es_optimizer_test.py
 tests/orquestra/opt/optimizers/pso_test.py
 tests/orquestra/opt/optimizers/qiskit_optimizer_test.py
 tests/orquestra/opt/optimizers/scikit_quant_optimizer_test.py
 tests/orquestra/opt/optimizers/scipy_optimizer_test.py
 tests/orquestra/opt/optimizers/search_points_optimizer_test.py
 tests/orquestra/opt/optimizers/simple_gradient_descent_test.py
+tests/orquestra/opt/optimizers/tensor_train_optimizer_test.py
 tests/orquestra/opt/problems/__init__.py
 tests/orquestra/opt/problems/_helpers.py
 tests/orquestra/opt/problems/generators_test.py
 tests/orquestra/opt/problems/graph_partition_test.py
 tests/orquestra/opt/problems/max_independent_set_test.py
 tests/orquestra/opt/problems/maxcut_test.py
 tests/orquestra/opt/problems/solve_problem_by_exhaustive_search_test.py
```

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/Makefile` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/README.rst` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/README.rst`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/coverage/action.yml` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/actions/publish-release/action.yml` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/bin/get_next_version.py` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/pyproject.toml` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/sample_setup.py` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/sample_setup.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/setup_extras.py` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/setup_extras.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/tests/test_get_next_version.py` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/subtrees/z_quantum_actions/workflow-templates/style.yml` & `orquestra-opt-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/artifact_storage_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/artifact_storage_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/attribute_forwarding_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/attribute_forwarding_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/copying_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/copying_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/functions_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/functions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/gradients_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/gradients_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/optimizer_contract_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/optimizer_contract_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/optimizer_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/optimizer_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/optimizer_utils_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/optimizer_utils_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/api/save_conditions_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/api/save_conditions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/bqm/test_conversion.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/bqm/test_conversion.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/bqm/test_io.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/bqm/test_io.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/history/recording_functions_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/history/recording_functions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/history/recording_functions_with_gradient_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/history/recording_functions_with_gradient_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/basin_hopping_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/basin_hopping_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/cma_es_optimizer_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/cma_es_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/pso_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/pso_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/qiskit_optimizer_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/qiskit_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/scikit_quant_optimizer_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/scikit_quant_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/search_points_optimizer_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/search_points_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/optimizers/simple_gradient_descent_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/optimizers/simple_gradient_descent_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,20 +58,21 @@
             _sum_x_squared, finite_differences_gradient(_sum_x_squared)
         )
 
     def test_fails_to_initialize_when_number_of_iterations_is_negative(self):
         with pytest.raises(AssertionError):
             SimpleGradientDescent(0.1, -1)
 
-    def test_fails_to_minimize_when_cost_function_does_not_have_gradient_method(
+    def test_minimize_succeeds_when_cost_function_does_not_have_gradient_method(
         self, optimizer
     ):
-        def cost_function(x):
-            return sum(x)
+        def sum_x_squared_no_gradient(x):
+            return sum(x**2)
 
-        with pytest.raises(AssertionError):
-            optimizer.minimize(cost_function, np.array([0, 0]))
+        result = optimizer.minimize(sum_x_squared_no_gradient, np.array([1.0, 1.0]))
+        np.testing.assert_almost_equal(result.opt_value, 0)
+        np.testing.assert_almost_equal(result.opt_params, np.array([0, 0]))
 
     def test_history_contains_function_evaluations(self, optimizer, sum_x_squared):
         results = optimizer.minimize(sum_x_squared, np.array([1, 0]), keep_history=True)
 
         assert len(results.history) == optimizer.number_of_iterations
```

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/problems/_helpers.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/problems/_helpers.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/problems/generators_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/problems/generators_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/problems/graph_partition_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/problems/graph_partition_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/problems/max_independent_set_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/problems/max_independent_set_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/problems/maxcut_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/problems/maxcut_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/problems/solve_problem_by_exhaustive_search_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/problems/solve_problem_by_exhaustive_search_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/problems/vertex_cover_test.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/problems/vertex_cover_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-opt-0.7.0/tests/orquestra/opt/test_cost_function_augmentations.py` & `orquestra-opt-0.8.0/tests/orquestra/opt/test_cost_function_augmentations.py`

 * *Files identical despite different names*

