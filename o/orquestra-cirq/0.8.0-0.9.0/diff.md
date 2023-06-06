# Comparing `tmp/orquestra-cirq-0.8.0.tar.gz` & `tmp/orquestra-cirq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquestra-cirq-0.8.0.tar", last modified: Fri Jan 13 15:54:47 2023, max compression
+gzip compressed data, was "orquestra-cirq-0.9.0.tar", last modified: Tue Jun  6 20:43:08 2023, max compression
```

## Comparing `orquestra-cirq-0.8.0.tar` & `orquestra-cirq-0.9.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.950988 orquestra-cirq-0.8.0/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.923019 orquestra-cirq-0.8.0/.github/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.923850 orquestra-cirq-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/.github/pull_request_template.md
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.926129 orquestra-cirq-0.8.0/.github/workflows/
--rw-r--r--   0 maxradin   (501) staff       (20)      930 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/.github/workflows/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      876 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/.github/workflows/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      945 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/.github/workflows/style.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1683 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/.gitignore
--rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/LICENSE
--rw-r--r--   0 maxradin   (501) staff       (20)      619 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     3223 2023-01-13 15:54:47.951186 orquestra-cirq-0.8.0/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     2605 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/README.md
--rw-r--r--   0 maxradin   (501) staff       (20)      161 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/codecov.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1278 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)      960 2023-01-13 15:54:47.951943 orquestra-cirq-0.8.0/setup.cfg
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.894447 orquestra-cirq-0.8.0/src/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.891130 orquestra-cirq-0.8.0/src/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.893686 orquestra-cirq-0.8.0/src/orquestra/integrations/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.927057 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/__init__.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.931229 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/
--rw-r--r--   0 maxradin   (501) staff       (20)      409 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)    12646 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/_circuit_conversions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1354 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/_cirq_pauli_conversions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1189 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/_openfermion_conversions.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.932614 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/decompositions/
--rw-r--r--   0 maxradin   (501) staff       (20)      295 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/decompositions/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2846 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/decompositions/_cirq_decompositions.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.934492 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/noise/
--rw-r--r--   0 maxradin   (501) staff       (20)      375 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/noise/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3662 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/noise/basic.py
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/py.typed
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.936283 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/
--rw-r--r--   0 maxradin   (501) staff       (20)      342 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6649 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/_base.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1456 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/_cirq_simulator.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3040 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/_qsim_simulator.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.936679 orquestra-cirq-0.8.0/src/orquestra/integrations/custatevec/
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/custatevec/py.typed
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.937391 orquestra-cirq-0.8.0/src/orquestra/integrations/custatevec/simulator/
--rw-r--r--   0 maxradin   (501) staff       (20)       45 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/custatevec/simulator/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2318 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/src/orquestra/integrations/custatevec/simulator/_custatevec.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.941238 orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/
--rw-r--r--   0 maxradin   (501) staff       (20)     3223 2023-01-13 15:54:47.000000 orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     2764 2023-01-13 15:54:47.000000 orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/SOURCES.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:54:47.000000 orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/dependency_links.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:54:47.000000 orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/not-zip-safe
--rw-r--r--   0 maxradin   (501) staff       (20)      156 2023-01-13 15:54:47.000000 orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/requires.txt
--rw-r--r--   0 maxradin   (501) staff       (20)       10 2023-01-13 15:54:47.000000 orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/top_level.txt
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.896517 orquestra-cirq-0.8.0/subtrees/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.944142 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/
--rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/MANIFEST.in
--rw-r--r--   0 maxradin   (501) staff       (20)     3835 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/README.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.899145 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.944419 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/coverage/
--rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.944779 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/publish-release/
--rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.945143 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/
--rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.945533 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/style/
--rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/style/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.945959 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/bin/
--rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/pytest.ini
--rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/sample_setup.py
--rw-r--r--   0 maxradin   (501) staff       (20)      585 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/setup_extras.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.946279 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/tests/
--rw-r--r--   0 maxradin   (501) staff       (20)     1131 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/variables.mk
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.947839 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/workflow-templates/
--rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.902509 orquestra-cirq-0.8.0/tests/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.902894 orquestra-cirq-0.8.0/tests/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.903368 orquestra-cirq-0.8.0/tests/orquestra/integrations/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.905092 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.949080 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/conversions/
--rw-r--r--   0 maxradin   (501) staff       (20)    11092 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/conversions/circuit_conversions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2923 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/conversions/cirq_pauli_conversions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3296 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/conversions/openfermion_conversions_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.949657 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/decompositions/
--rw-r--r--   0 maxradin   (501) staff       (20)     5601 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/decompositions/cirq_decomposition_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.950186 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/noise/
--rw-r--r--   0 maxradin   (501) staff       (20)     3766 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/noise/basic_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:54:47.950729 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/simulator/
--rw-r--r--   0 maxradin   (501) staff       (20)     6862 2023-01-13 15:54:40.000000 orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/simulator/simulator_test.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.794996 orquestra-cirq-0.9.0/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.770173 orquestra-cirq-0.9.0/.github/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.770935 orquestra-cirq-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      605 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      600 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      533 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.771976 orquestra-cirq-0.9.0/.github/workflows/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      930 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/.github/workflows/coverage.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      876 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      945 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/.github/workflows/style.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1683 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/.gitignore
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    11357 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/LICENSE
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      619 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/Makefile
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3223 2023-06-06 20:43:08.795321 orquestra-cirq-0.9.0/PKG-INFO
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2605 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/README.md
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      161 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/codecov.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1278 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/pyproject.toml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      960 2023-06-06 20:43:08.796606 orquestra-cirq-0.9.0/setup.cfg
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.763562 orquestra-cirq-0.9.0/src/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.762094 orquestra-cirq-0.9.0/src/orquestra/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.763178 orquestra-cirq-0.9.0/src/orquestra/integrations/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.772738 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/__init__.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.774253 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      409 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    13696 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/_circuit_conversions.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1354 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/_cirq_pauli_conversions.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1189 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/_openfermion_conversions.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.775159 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/decompositions/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      295 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/decompositions/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2846 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/decompositions/_cirq_decompositions.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.776091 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/noise/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      375 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/noise/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3662 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/noise/basic.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/py.typed
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.777699 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      342 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     6649 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/_base.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1456 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/_cirq_simulator.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3040 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/_qsim_simulator.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.778276 orquestra-cirq-0.9.0/src/orquestra/integrations/custatevec/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/custatevec/py.typed
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.779009 orquestra-cirq-0.9.0/src/orquestra/integrations/custatevec/simulator/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       45 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/custatevec/simulator/__init__.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2318 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/src/orquestra/integrations/custatevec/simulator/_custatevec.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.781603 orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3223 2023-06-06 20:43:08.000000 orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/PKG-INFO
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2764 2023-06-06 20:43:08.000000 orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/SOURCES.txt
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        1 2023-06-06 20:43:08.000000 orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/dependency_links.txt
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        1 2023-06-06 20:43:08.000000 orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/not-zip-safe
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      156 2023-06-06 20:43:08.000000 orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/requires.txt
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       10 2023-06-06 20:43:08.000000 orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/top_level.txt
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.763893 orquestra-cirq-0.9.0/subtrees/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.785874 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)        9 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/MANIFEST.in
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3835 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/Makefile
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     5600 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/README.rst
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.764791 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.786408 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/coverage/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      790 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.786910 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/publish-release/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3132 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.787418 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      458 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.787952 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/style/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      467 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/style/action.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.788505 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/bin/
+-rwxr-xr-x   0 athenacaesura   (501) staff       (20)     2756 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1253 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/pyproject.toml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       24 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/pytest.ini
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1526 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/sample_setup.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      585 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/setup_extras.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.789094 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/tests/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1131 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)       19 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/variables.mk
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.790881 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/workflow-templates/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1233 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)      696 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     1248 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.765762 orquestra-cirq-0.9.0/tests/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.765888 orquestra-cirq-0.9.0/tests/orquestra/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.766015 orquestra-cirq-0.9.0/tests/orquestra/integrations/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.766739 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.792630 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/conversions/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)    13161 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/conversions/circuit_conversions_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     2923 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/conversions/cirq_pauli_conversions_test.py
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3296 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/conversions/openfermion_conversions_test.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.793364 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/decompositions/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     5601 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/decompositions/cirq_decomposition_test.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.793947 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/noise/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     3766 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/noise/basic_test.py
+drwxr-xr-x   0 athenacaesura   (501) staff       (20)        0 2023-06-06 20:43:08.794500 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/simulator/
+-rw-r--r--   0 athenacaesura   (501) staff       (20)     6862 2023-06-06 20:43:04.000000 orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/simulator/simulator_test.py
```

### Comparing `orquestra-cirq-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `orquestra-cirq-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `orquestra-cirq-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/.github/pull_request_template.md` & `orquestra-cirq-0.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/.github/workflows/coverage.yml` & `orquestra-cirq-0.9.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/.github/workflows/publish_release.yml` & `orquestra-cirq-0.9.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/.github/workflows/style.yml` & `orquestra-cirq-0.9.0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/.gitignore` & `orquestra-cirq-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/LICENSE` & `orquestra-cirq-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/Makefile` & `orquestra-cirq-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/PKG-INFO` & `orquestra-cirq-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-cirq
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra Cirq package"
 Home-page: https://github.com/zapatacomputing/orquestra-cirq
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-cirq-0.8.0/README.md` & `orquestra-cirq-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/pyproject.toml` & `orquestra-cirq-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/setup.cfg` & `orquestra-cirq-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 include_package_data = True
 package_dir = 
 	= src
 packages = find_namespace:
 python_requires = >=3.8,!=3.9.7,<3.11
 install_requires = 
 	protobuf<4
-	cirq-core~=1.0.0
-	cirq-google~=1.0.0
+	cirq-core~=1.1.0
+	cirq-google~=1.1.0
 	orquestra-quantum
 	openfermion~=1.4
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
```

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/_circuit_conversions.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/_circuit_conversions.py`

 * *Files 4% similar despite different names*

```diff
@@ -279,16 +279,16 @@
     circuits composed of such gates will use the native definitions, e.g. `cirq.X` will
     become `circuits.X`.
 
     Importing gates from Cirq that don't have built-in counterparts in Orquestra will
     result in custom gates. See `help(orquestra.quantum.circuits)` for examples of
     custom gates.
 
-    Also note that only objects using only LineQubits are supported, as currently there
-    is no notion of GridQubit in Orquestra circuits.
+    Also note that objects using GridQubits are never supported. NamedQubits are only
+    supported inside circuits, not as standalone Operations.
     """
     return _import_from_cirq(obj)
 
 
 @dataclass
 class NonNativeGate:
     matrix: np.ndarray
@@ -366,15 +366,16 @@
 
 
 @_import_from_cirq.register(cirq.GateOperation)
 @_import_from_cirq.register(cirq.ControlledOperation)
 def _convert_gate_operation_to_orquestra(operation) -> _gates.GateOperation:
     if not all(isinstance(qubit, cirq.LineQubit) for qubit in operation.qubits):
         raise NotImplementedError(
-            f"Failed to import {operation}. Only LineQubits are supported."
+            f"Failed to import {operation}. Only GateOperations on LineQubits are"
+            "supported. Try converting the underlying Gate and adding qubits after."
         )
 
     imported_gate = _import_from_cirq(operation.gate)
     qubit_indices = map(qubit_index, operation.qubits)
 
     if isinstance(imported_gate, NonNativeGate):
         custom_gate = _gates.CustomGateDefinition(
@@ -387,10 +388,35 @@
         return custom_gate(*custom_gate.matrix.free_symbols)(*qubit_indices)
     else:
         return imported_gate(*qubit_indices)
 
 
 @_import_from_cirq.register
 def _import_circuit_from_cirq(circuit: cirq.Circuit) -> _circuit.Circuit:
+    all_qubits = sorted(circuit.all_qubits())
+    max_line_id = 0
+    contains_line_qubit = False
+    for qubit in all_qubits:
+        if isinstance(qubit, cirq.GridQubit):
+            raise NotImplementedError(
+                "Failed to import circuit. GridQubits are not supported."
+            )
+        if isinstance(qubit, cirq.LineQubit):
+            contains_line_qubit = True
+            if qubit.x < 0:
+                raise ValueError(
+                    f"LineQubit with negative index {qubit.x} is not supported."
+                )
+            if qubit.x > max_line_id:
+                max_line_id = qubit.x
+
+    qubit_map = {}
+    current_qubit_id = max_line_id + 1 if contains_line_qubit else 0
+    for qubit in all_qubits:
+        if isinstance(qubit, cirq.NamedQubit):
+            qubit_map[qubit] = cirq.LineQubit(current_qubit_id)
+            current_qubit_id += 1
+    circuit = circuit.transform_qubits(qubit_map)  # type: ignore
+
     return _circuit.Circuit(
         [_import_from_cirq(op) for op in chain.from_iterable(circuit.moments)]
     )
```

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/_cirq_pauli_conversions.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/_cirq_pauli_conversions.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/conversions/_openfermion_conversions.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/conversions/_openfermion_conversions.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/decompositions/_cirq_decompositions.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/decompositions/_cirq_decompositions.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/noise/basic.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/noise/basic.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/_base.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/_base.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/_cirq_simulator.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/_cirq_simulator.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/cirq/simulator/_qsim_simulator.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/cirq/simulator/_qsim_simulator.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra/integrations/custatevec/simulator/_custatevec.py` & `orquestra-cirq-0.9.0/src/orquestra/integrations/custatevec/simulator/_custatevec.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/PKG-INFO` & `orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-cirq
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra Cirq package"
 Home-page: https://github.com/zapatacomputing/orquestra-cirq
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-cirq-0.8.0/src/orquestra_cirq.egg-info/SOURCES.txt` & `orquestra-cirq-0.9.0/src/orquestra_cirq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/Makefile` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/README.rst` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/README.rst`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/pyproject.toml` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/sample_setup.py` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/sample_setup.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/setup_extras.py` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/setup_extras.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml` & `orquestra-cirq-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/conversions/circuit_conversions_test.py` & `orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/conversions/circuit_conversions_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -333,7 +333,71 @@
 
         assert len(circuit.free_symbols) != 0
 
     @pytest.mark.parametrize("cirq_circuit", UNSUPPORTED_CIRQ_CIRCUITS)
     def test_with_unsupported_gates_raises_not_implemented_error(self, cirq_circuit):
         with pytest.raises(NotImplementedError):
             import_from_cirq(cirq_circuit)
+
+    @pytest.mark.parametrize(
+        "cirq_circuit, num_qubits, target_labels",
+        [
+            (
+                cirq.Circuit(
+                    [
+                        cirq.X(cirq.NamedQubit("a")),
+                        cirq.CNOT(cirq.NamedQubit("a"), cirq.NamedQubit("b")),
+                    ]
+                ),
+                2,
+                [(0,), (0, 1)],
+            ),
+            (
+                cirq.Circuit(
+                    [
+                        cirq.X(cirq.LineQubit(0)),
+                        cirq.CNOT(cirq.NamedQubit("a"), cirq.NamedQubit("b")),
+                    ]
+                ),
+                3,
+                [(0,), (1, 2)],
+            ),
+            (
+                cirq.Circuit(
+                    [
+                        cirq.X(cirq.LineQubit(20)),
+                        cirq.X(cirq.NamedQubit("b")),
+                    ]
+                ),
+                22,
+                [(20,), (21,)],
+            ),
+            (
+                cirq.Circuit(
+                    [
+                        cirq.X(cirq.NamedQubit("a")),
+                        cirq.X(cirq.LineQubit(0)),
+                        cirq.X(cirq.NamedQubit("b")),
+                    ]
+                ),
+                3,
+                [(1,), (0,), (2,)],
+            ),
+        ],
+    )
+    def test_named_qubits_are_converted_to_labeled_qubit(
+        self, cirq_circuit, num_qubits, target_labels
+    ):
+        circuit = import_from_cirq(cirq_circuit)
+        assert circuit.n_qubits == num_qubits
+        assert all(
+            target_label == operation.qubit_indices
+            for target_label, operation in zip(target_labels, circuit.operations)
+        )
+
+    def test_named_qubit_in_gate_operation_throws_error(self):
+        with pytest.raises(NotImplementedError):
+            import_from_cirq(cirq.X(cirq.NamedQubit("a")))
+
+    def test_negative_line_qubit_in_gate_operation_throws_error(self):
+        with pytest.raises(ValueError):
+            import_from_cirq(cirq.Circuit([cirq.X(cirq.LineQubit(-1))]))
```

### Comparing `orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/conversions/cirq_pauli_conversions_test.py` & `orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/conversions/cirq_pauli_conversions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/conversions/openfermion_conversions_test.py` & `orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/conversions/openfermion_conversions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/decompositions/cirq_decomposition_test.py` & `orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/decompositions/cirq_decomposition_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/noise/basic_test.py` & `orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/noise/basic_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-cirq-0.8.0/tests/orquestra/integrations/cirq/simulator/simulator_test.py` & `orquestra-cirq-0.9.0/tests/orquestra/integrations/cirq/simulator/simulator_test.py`

 * *Files identical despite different names*

