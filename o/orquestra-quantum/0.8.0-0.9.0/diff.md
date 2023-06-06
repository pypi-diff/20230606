# Comparing `tmp/orquestra-quantum-0.8.0.tar.gz` & `tmp/orquestra-quantum-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquestra-quantum-0.8.0.tar", last modified: Fri Jan 13 15:51:59 2023, max compression
+gzip compressed data, was "orquestra-quantum-0.9.0.tar", last modified: Tue Feb  7 21:00:59 2023, max compression
```

## Comparing `orquestra-quantum-0.8.0.tar` & `orquestra-quantum-0.9.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.850500 orquestra-quantum-0.8.0/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.790109 orquestra-quantum-0.8.0/.github/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.790888 orquestra-quantum-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/.github/pull_request_template.md
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.792768 orquestra-quantum-0.8.0/.github/workflows/
--rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/.github/workflows/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/.github/workflows/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/.github/workflows/style.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1733 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/.gitignore
--rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/LICENSE
--rw-r--r--   0 maxradin   (501) staff       (20)      247 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     3011 2023-01-13 15:51:59.850720 orquestra-quantum-0.8.0/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     2380 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/README.md
--rw-r--r--   0 maxradin   (501) staff       (20)       46 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/list.json
--rw-r--r--   0 maxradin   (501) staff       (20)     1318 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)      955 2023-01-13 15:51:59.851527 orquestra-quantum-0.8.0/setup.cfg
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.781183 orquestra-quantum-0.8.0/src/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.777755 orquestra-quantum-0.8.0/src/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.794700 orquestra-quantum-0.8.0/src/orquestra/quantum/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.798120 orquestra-quantum-0.8.0/src/orquestra/quantum/api/
--rw-r--r--   0 maxradin   (501) staff       (20)      389 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/api/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     9695 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/api/circuit_runner.py
--rw-r--r--   0 maxradin   (501) staff       (20)    15408 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/api/circuit_runner_contracts.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2558 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/api/estimation.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3869 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/api/estimator_contract.py
--rw-r--r--   0 maxradin   (501) staff       (20)     8816 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/api/wavefunction_simulator.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7035 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/api/wavefunction_simulator_contracts.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.804049 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/
--rw-r--r--   0 maxradin   (501) staff       (20)     4742 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3110 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_builtin_gates.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7562 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_circuit.py
--rw-r--r--   0 maxradin   (501) staff       (20)    20082 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_gates.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2892 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_generators.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7016 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_itertools.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5350 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_matrices.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3033 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_operations.py
--rw-r--r--   0 maxradin   (501) staff       (20)     8939 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_serde.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2395 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_testing.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6234 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_unitary_tools.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3089 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_wavefunction_operations.py
--rw-r--r--   0 maxradin   (501) staff       (20)     8805 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/layouts.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.807340 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/
--rw-r--r--   0 maxradin   (501) staff       (20)      294 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2527 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/_sorting.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1301 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/expressions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4646 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/sympy_expressions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1442 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/translations.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.809147 orquestra-quantum-0.8.0/src/orquestra/quantum/decompositions/
--rw-r--r--   0 maxradin   (501) staff       (20)      343 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/decompositions/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1720 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/decompositions/_decomposition.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1751 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/decompositions/_orquestra_decompositions.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.812507 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/
--rw-r--r--   0 maxradin   (501) staff       (20)     3019 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/BAS_dataset.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1093 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)    15855 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/_measurement_outcome_distribution.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1814 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/clipped_negative_log_likelihood.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1607 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/jensen_shannon_divergence.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5139 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/mmd.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7607 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/target_thermal_states.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.813553 orquestra-quantum-0.8.0/src/orquestra/quantum/estimation/
--rw-r--r--   0 maxradin   (501) staff       (20)      441 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/estimation/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7496 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/estimation/_estimation.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6811 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/evolution.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.815711 orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/
--rw-r--r--   0 maxradin   (501) staff       (20)      779 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     8100 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/expectation_values.py
--rw-r--r--   0 maxradin   (501) staff       (20)    13616 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/measurements.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7006 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/parities.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.817456 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/
--rw-r--r--   0 maxradin   (501) staff       (20)      748 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4149 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_io.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.819476 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/
--rw-r--r--   0 maxradin   (501) staff       (20)     1178 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)      751 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/config.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2700 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/operator_utils.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5986 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/sparse_tools.py
--rw-r--r--   0 maxradin   (501) staff       (20)    18888 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_pauli_operators.py
--rw-r--r--   0 maxradin   (501) staff       (20)    10283 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_utils.py
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/py.typed
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.820662 orquestra-quantum-0.8.0/src/orquestra/quantum/runners/
--rw-r--r--   0 maxradin   (501) staff       (20)       99 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/runners/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1090 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/runners/symbolic_simulator.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4789 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/runners/trackers.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.825247 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/
--rw-r--r--   0 maxradin   (501) staff       (20)      287 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)      714 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/_initialize.py
--rw-r--r--   0 maxradin   (501) staff       (20)    13975 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/generate_cases_for_backend_tests.py
--rw-r--r--   0 maxradin   (501) staff       (20)    12112 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/hamiltonian_H2_minimal_basis.json
--rw-r--r--   0 maxradin   (501) staff       (20)    12120 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/hamiltonian_H2_minus_ROHF_minimal_basis.json
--rw-r--r--   0 maxradin   (501) staff       (20)     3869 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/hamiltonian_HeH_plus_STO-3G.json
--rw-r--r--   0 maxradin   (501) staff       (20)     1087 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/mocks.py
--rw-r--r--   0 maxradin   (501) staff       (20)    56539 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/testing/test_cases_for_backend_tests.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1153 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/typing.py
--rw-r--r--   0 maxradin   (501) staff       (20)    15787 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/utils.py
--rw-r--r--   0 maxradin   (501) staff       (20)     9958 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/src/orquestra/quantum/wavefunction.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.827619 orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/
--rw-r--r--   0 maxradin   (501) staff       (20)     3011 2023-01-13 15:51:59.000000 orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     6586 2023-01-13 15:51:59.000000 orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:51:59.000000 orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:51:59.000000 orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/not-zip-safe
--rw-r--r--   0 maxradin   (501) staff       (20)      120 2023-01-13 15:51:59.000000 orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/requires.txt
--rw-r--r--   0 maxradin   (501) staff       (20)       10 2023-01-13 15:51:59.000000 orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/top_level.txt
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.781583 orquestra-quantum-0.8.0/subtrees/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.831565 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/
--rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/MANIFEST.in
--rw-r--r--   0 maxradin   (501) staff       (20)     3835 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/README.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.782585 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.832034 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/coverage/
--rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.832434 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/publish-release/
--rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.832769 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/
--rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.833106 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/style/
--rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/style/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.833667 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/bin/
--rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/pytest.ini
--rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/sample_setup.py
--rw-r--r--   0 maxradin   (501) staff       (20)      585 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/setup_extras.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.834284 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/tests/
--rw-r--r--   0 maxradin   (501) staff       (20)     1130 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/variables.mk
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.835458 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/workflow-templates/
--rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.783460 orquestra-quantum-0.8.0/tests/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.783630 orquestra-quantum-0.8.0/tests/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.836394 orquestra-quantum-0.8.0/tests/orquestra/quantum/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.836865 orquestra-quantum-0.8.0/tests/orquestra/quantum/api/
--rw-r--r--   0 maxradin   (501) staff       (20)     3053 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/api/estimator_contract_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.841526 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1339 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_builtin_gates_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7943 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_circuit_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    18738 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_gates_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3735 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_generators_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4891 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_itertools_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6023 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_serde_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2657 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_unitary_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5187 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_wavefunction_operations_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    98961 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/hardcoded_cirq_unitaries.npy
--rw-r--r--   0 maxradin   (501) staff       (20)     3912 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/layouts_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.842590 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/symbolic/
--rw-r--r--   0 maxradin   (501) staff       (20)     2502 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/symbolic/sorting_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     8040 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/symbolic/sympy_expressions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1551 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/symbolic/translations_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.843055 orquestra-quantum-0.8.0/tests/orquestra/quantum/decompositions/
--rw-r--r--   0 maxradin   (501) staff       (20)     4700 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/decompositions/_zquantum_decomposition_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.844860 orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/
--rw-r--r--   0 maxradin   (501) staff       (20)     2981 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/BAS_dataset_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    16983 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/_measurement_outcome_distribution_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6477 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/distance_measures_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     6821 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/target_thermal_states_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.845229 orquestra-quantum-0.8.0/tests/orquestra/quantum/estimation/
--rw-r--r--   0 maxradin   (501) staff       (20)    23556 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/estimation/estimation_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7921 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/evolution_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.846475 orquestra-quantum-0.8.0/tests/orquestra/quantum/measurements/
--rw-r--r--   0 maxradin   (501) staff       (20)     5462 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/measurements/expectation_values_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    19053 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/measurements/measurements_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2170 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/measurements/parities_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.848668 orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/
--rw-r--r--   0 maxradin   (501) staff       (20)     2218 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_io_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.849559 orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_openfermion_utils/
--rw-r--r--   0 maxradin   (501) staff       (20)     3571 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_openfermion_utils/operator_utils_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2848 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_openfermion_utils/sparse_tools_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    22844 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_operators_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     4541 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_utils_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:51:59.850283 orquestra-quantum-0.8.0/tests/orquestra/quantum/runners/
--rw-r--r--   0 maxradin   (501) staff       (20)     2532 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/runners/symbolic_simulator_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    10180 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/runners/trackers_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    10098 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/utils_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)    13086 2023-01-13 15:51:51.000000 orquestra-quantum-0.8.0/tests/orquestra/quantum/wavefunction_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.805857 orquestra-quantum-0.9.0/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.749080 orquestra-quantum-0.9.0/.github/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.750018 orquestra-quantum-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.751417 orquestra-quantum-0.9.0/.github/workflows/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/.github/workflows/coverage.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/.github/workflows/style.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1733 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/.gitignore
+-rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/LICENSE
+-rw-r--r--   0 maxradin   (501) staff       (20)      247 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/Makefile
+-rw-r--r--   0 maxradin   (501) staff       (20)     3011 2023-02-07 21:00:59.806053 orquestra-quantum-0.9.0/PKG-INFO
+-rw-r--r--   0 maxradin   (501) staff       (20)     2380 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/README.md
+-rw-r--r--   0 maxradin   (501) staff       (20)       46 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/list.json
+-rw-r--r--   0 maxradin   (501) staff       (20)     1318 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/pyproject.toml
+-rw-r--r--   0 maxradin   (501) staff       (20)      955 2023-02-07 21:00:59.814070 orquestra-quantum-0.9.0/setup.cfg
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.689796 orquestra-quantum-0.9.0/src/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.679083 orquestra-quantum-0.9.0/src/orquestra/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.753737 orquestra-quantum-0.9.0/src/orquestra/quantum/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.756824 orquestra-quantum-0.9.0/src/orquestra/quantum/api/
+-rw-r--r--   0 maxradin   (501) staff       (20)      389 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/api/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     9695 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/api/circuit_runner.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    15408 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/api/circuit_runner_contracts.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2558 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/api/estimation.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3869 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/api/estimator_contract.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     8816 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/api/wavefunction_simulator.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7035 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/api/wavefunction_simulator_contracts.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.763570 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/
+-rw-r--r--   0 maxradin   (501) staff       (20)     4793 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3336 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_builtin_gates.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7562 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_circuit.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    20082 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_gates.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2892 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_generators.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     9015 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_itertools.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     6266 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_matrices.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3033 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_operations.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     8939 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_serde.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2395 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_testing.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     6234 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_unitary_tools.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3089 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_wavefunction_operations.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     8805 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/layouts.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.765646 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/
+-rw-r--r--   0 maxradin   (501) staff       (20)      294 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2527 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/_sorting.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1301 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/expressions.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     4646 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/sympy_expressions.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1442 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/translations.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.766936 orquestra-quantum-0.9.0/src/orquestra/quantum/decompositions/
+-rw-r--r--   0 maxradin   (501) staff       (20)      343 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/decompositions/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1720 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/decompositions/_decomposition.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1751 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/decompositions/_orquestra_decompositions.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.770652 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3019 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/BAS_dataset.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1093 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    15855 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/_measurement_outcome_distribution.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1814 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/clipped_negative_log_likelihood.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1607 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/jensen_shannon_divergence.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     5139 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/mmd.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7607 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/target_thermal_states.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.771640 orquestra-quantum-0.9.0/src/orquestra/quantum/estimation/
+-rw-r--r--   0 maxradin   (501) staff       (20)      441 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/estimation/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7496 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/estimation/_estimation.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     6811 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/evolution.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.773040 orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/
+-rw-r--r--   0 maxradin   (501) staff       (20)      779 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     8100 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/expectation_values.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    13616 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/measurements.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7006 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/parities.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.775018 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/
+-rw-r--r--   0 maxradin   (501) staff       (20)      748 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     4149 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_io.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.776433 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1178 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      751 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/config.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2700 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/operator_utils.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     5986 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/sparse_tools.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    18888 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_pauli_operators.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    10283 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_utils.py
+-rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/py.typed
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.777547 orquestra-quantum-0.9.0/src/orquestra/quantum/runners/
+-rw-r--r--   0 maxradin   (501) staff       (20)       99 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/runners/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1090 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/runners/symbolic_simulator.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     4789 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/runners/trackers.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.780839 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/
+-rw-r--r--   0 maxradin   (501) staff       (20)      287 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      714 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/_initialize.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    13975 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/generate_cases_for_backend_tests.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    12112 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/hamiltonian_H2_minimal_basis.json
+-rw-r--r--   0 maxradin   (501) staff       (20)    12120 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/hamiltonian_H2_minus_ROHF_minimal_basis.json
+-rw-r--r--   0 maxradin   (501) staff       (20)     3869 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/hamiltonian_HeH_plus_STO-3G.json
+-rw-r--r--   0 maxradin   (501) staff       (20)     1087 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/mocks.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    56539 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/testing/test_cases_for_backend_tests.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1153 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/typing.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    15787 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/utils.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     9958 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/src/orquestra/quantum/wavefunction.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.783314 orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3011 2023-02-07 21:00:59.000000 orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 maxradin   (501) staff       (20)     6586 2023-02-07 21:00:59.000000 orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-02-07 21:00:59.000000 orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-02-07 21:00:58.000000 orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/not-zip-safe
+-rw-r--r--   0 maxradin   (501) staff       (20)      120 2023-02-07 21:00:59.000000 orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/requires.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)       10 2023-02-07 21:00:59.000000 orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/top_level.txt
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.712331 orquestra-quantum-0.9.0/subtrees/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.786943 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/
+-rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/MANIFEST.in
+-rw-r--r--   0 maxradin   (501) staff       (20)     3835 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/Makefile
+-rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/README.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.714045 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.787328 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/coverage/
+-rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.787743 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/publish-release/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.788122 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/
+-rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.788492 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/style/
+-rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/style/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.788838 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/bin/
+-rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/pyproject.toml
+-rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/pytest.ini
+-rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/sample_setup.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      585 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/setup_extras.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.789316 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/tests/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1130 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
+-rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/variables.mk
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.790434 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/workflow-templates/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.715816 orquestra-quantum-0.9.0/tests/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.716049 orquestra-quantum-0.9.0/tests/orquestra/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.791745 orquestra-quantum-0.9.0/tests/orquestra/quantum/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.792214 orquestra-quantum-0.9.0/tests/orquestra/quantum/api/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3053 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/api/estimator_contract_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.797028 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/
+-rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1455 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_builtin_gates_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7943 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_circuit_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    18890 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_gates_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3735 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_generators_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     6443 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_itertools_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     6023 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_serde_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2657 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_unitary_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     5187 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_wavefunction_operations_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    98961 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/hardcoded_cirq_unitaries.npy
+-rw-r--r--   0 maxradin   (501) staff       (20)     3912 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/layouts_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.798332 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/symbolic/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2502 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/symbolic/sorting_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     8040 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/symbolic/sympy_expressions_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1551 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/symbolic/translations_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.798760 orquestra-quantum-0.9.0/tests/orquestra/quantum/decompositions/
+-rw-r--r--   0 maxradin   (501) staff       (20)     4700 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/decompositions/_zquantum_decomposition_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.801031 orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2981 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/BAS_dataset_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    16983 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/_measurement_outcome_distribution_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     6477 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/distance_measures_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     6821 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/target_thermal_states_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.801388 orquestra-quantum-0.9.0/tests/orquestra/quantum/estimation/
+-rw-r--r--   0 maxradin   (501) staff       (20)    23556 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/estimation/estimation_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7921 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/evolution_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.802630 orquestra-quantum-0.9.0/tests/orquestra/quantum/measurements/
+-rw-r--r--   0 maxradin   (501) staff       (20)     5462 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/measurements/expectation_values_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    19053 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/measurements/measurements_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2170 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/measurements/parities_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.804080 orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2218 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_io_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.804885 orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_openfermion_utils/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3571 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_openfermion_utils/operator_utils_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2848 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_openfermion_utils/sparse_tools_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    22844 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_operators_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     4541 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_utils_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:00:59.805581 orquestra-quantum-0.9.0/tests/orquestra/quantum/runners/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2532 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/runners/symbolic_simulator_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    10180 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/runners/trackers_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    10098 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/utils_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    13086 2023-02-07 21:00:43.000000 orquestra-quantum-0.9.0/tests/orquestra/quantum/wavefunction_test.py
```

### Comparing `orquestra-quantum-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `orquestra-quantum-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `orquestra-quantum-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/.github/pull_request_template.md` & `orquestra-quantum-0.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/.github/workflows/coverage.yml` & `orquestra-quantum-0.9.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/.github/workflows/publish_release.yml` & `orquestra-quantum-0.9.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/.github/workflows/style.yml` & `orquestra-quantum-0.9.0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/.gitignore` & `orquestra-quantum-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/LICENSE` & `orquestra-quantum-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/PKG-INFO` & `orquestra-quantum-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-quantum
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra's library with basic quantum operations"
 Home-page: https://github.com/zapatacomputing/orquestra-quantum
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-quantum-0.8.0/README.md` & `orquestra-quantum-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/pyproject.toml` & `orquestra-quantum-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/setup.cfg` & `orquestra-quantum-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/api/circuit_runner.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/api/circuit_runner.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/api/circuit_runner_contracts.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/api/circuit_runner_contracts.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/api/estimation.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/api/estimation.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/api/estimator_contract.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/api/estimator_contract.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/api/wavefunction_simulator.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/api/wavefunction_simulator.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/api/wavefunction_simulator_contracts.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/api/wavefunction_simulator_contracts.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/__init__.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,27 +143,30 @@
 """
 
 from ._builtin_gates import (
     CNOT,
     CPHASE,
     CZ,
     ISWAP,
+    MS,
     PHASE,
     RH,
     RX,
     RY,
     RZ,
     SWAP,
     U3,
     XX,
     XY,
     YY,
     ZZ,
     Delay,
     GatePrototype,
+    GPi,
+    GPi2,
     H,
     I,
     S,
     T,
     X,
     Y,
     Z,
@@ -181,14 +184,15 @@
 )
 from ._generators import (
     add_ancilla_register,
     apply_gate_to_qubits,
     create_layer_of_gates,
 )
 from ._itertools import (
+    combine_bitstrings,
     combine_measurement_counts,
     expand_sample_sizes,
     split_into_batches,
 )
 from ._operations import Operation
 from ._serde import (
     circuit_from_dict,
```

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_builtin_gates.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_builtin_gates.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
 RX = make_parametric_gate_prototype("RX", _matrices.rx_matrix, 1)
 RY = make_parametric_gate_prototype("RY", _matrices.ry_matrix, 1)
 RZ = make_parametric_gate_prototype("RZ", _matrices.rz_matrix, 1)
 RH = make_parametric_gate_prototype("RH", _matrices.rh_matrix, 1)
 PHASE = make_parametric_gate_prototype("PHASE", _matrices.phase_matrix, 1)
 U3 = make_parametric_gate_prototype("U3", _matrices.u3_matrix, 1)
+GPi = make_parametric_gate_prototype("GPi", _matrices.gpi_matrix, 1, is_hermitian=True)
+GPi2 = make_parametric_gate_prototype("GPi2", _matrices.gpi2_matrix, 1)
 
 
 # --- non-parametric, two qubit gates ---
 
 CNOT = _gates.MatrixFactoryGate("CNOT", _matrices.cnot_matrix, (), 2, is_hermitian=True)
 CZ = _gates.MatrixFactoryGate("CZ", _matrices.cz_matrix, (), 2, is_hermitian=True)
 SWAP = _gates.MatrixFactoryGate("SWAP", _matrices.swap_matrix, (), 2, is_hermitian=True)
@@ -67,14 +69,15 @@
 # --- parametric, two qubit gates ---
 
 CPHASE = make_parametric_gate_prototype("CPHASE", _matrices.cphase_matrix, 2)
 XX = make_parametric_gate_prototype("XX", _matrices.xx_matrix, 2)
 YY = make_parametric_gate_prototype("YY", _matrices.yy_matrix, 2)
 ZZ = make_parametric_gate_prototype("ZZ", _matrices.zz_matrix, 2)
 XY = make_parametric_gate_prototype("XY", _matrices.xy_matrix, 2)
+MS = make_parametric_gate_prototype("MS", _matrices.ms_matrix, 2)
 
 
 # --- misc ----
 # The Delay gate acts as an identity, however delays further circuit execution
 # on the given qubit by n-units of time.
 Delay = make_parametric_gate_prototype(
     "Delay", _matrices.delay_matrix, 1, is_hermitian=True
```

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_circuit.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_circuit.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_gates.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_gates.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_generators.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_generators.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_itertools.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_itertools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import Counter
 from functools import reduce
 from itertools import islice
 from math import ceil
-from typing import Dict, Iterable, Sequence, Tuple, TypeVar
+from typing import Dict, Iterable, List, Sequence, Tuple, TypeVar
 
 T = TypeVar("T")
 
 
 def _iterate_in_batches(items: Iterable[T], batch_size: int) -> Iterable[Tuple[T, ...]]:
     it = iter(items)
     while chunk := tuple(islice(it, batch_size)):
@@ -136,15 +136,15 @@
     for bitstring, count in second.items():
         result[bitstring] += count
     return dict(result)
 
 
 def combine_measurement_counts(
     all_measurements: Sequence[Dict[str, int]], multiplicities: Sequence[int]
-) -> Sequence[Dict[str, int]]:
+) -> List[Dict[str, int]]:
     """Combine (aggregate) measurements of the same circuits run several times.
 
     Suppose multiplicities is a list [1, 2 ,3]. Then, the all_measurements should
     be a sequence of 1+2+3=6 elements m0,m1,m2,m3,m4,m5, and the results will
     contain three dictionaries M0, M1, M2 s.t.
 
     - M0 contains counts from m0 only
@@ -161,20 +161,65 @@
           instance, multiplicities [1, 2, 3] mean that first group of
           measurements comprises 1 Measurement, second group comprises 2
           consecutive Measurements, third group contains 3 consecutive
           Measurements and so on.
     Returns:
         Sequence of combined measurements of length equal len(multiplicities)
     Raises:
-        ValueError: if len(all_measurements != sum(multiplicities)
+        ValueError: if len(all_measurements) != sum(multiplicities)
     """
     if len(all_measurements) != (sum_multiplicities := sum(multiplicities)):
         raise ValueError(
             "Mismatch between multiplicities and number of measurements to combine. "
             f"Got {len(all_measurements)} Measurements objects to combine "
             f"but multiplicities sum to {sum_multiplicities}"
         )
     measurements_it = iter(all_measurements)
     return [
         reduce(_combine_measurements, islice(measurements_it, multiplicity))
         for multiplicity in multiplicities
     ]
+
+
+def combine_bitstrings(
+    all_bitstrings: Sequence[List[str]], multiplicities: Sequence[int]
+) -> List[List[str]]:
+    """Combine (aggregate) bitstrings of the same circuits run several times.
+
+    Suppose multiplicities is a list [1, 2 ,3]. Then, the all_bitstrings should
+    be a sequence of 1+2+3=6 elements, each of them being a sequence of bitstrings.
+    For instance, all_bitstrings could be equal to:
+    [["00", "01"], ["1", "0"], ["0"], ["001", "001"], ["111", "000"], ["000"]]
+    and then the result would be:
+    [
+        ["00", "01"],
+        ["1", "0", "0],
+        ["001", "001", "111", "000", "000"]
+    ]
+
+    Args:
+        all_bitstrings: sequence of lists containing bitstrings
+          gathered from some, possibly duplicated, circuits. The bitstrings
+          lists objects corresponding to the same circuit should be placed next
+          to each other. Should have the same length as sum(multiplicities).
+        multiplicities: sequence of positive integers marking groups of
+          consecutive measurements corresponding to the same circuit. For
+          instance, multiplicities [1, 2, 3] mean that first group of
+          bitstrings comprises 1 sequence, second group comprises 2
+          consecutive sequences, third group contains 3 consecutive
+          sequences and so on.
+    Returns:
+        Sequence of combined measurements of length equal len(multiplicities)
+    Raises:
+        ValueError: if len(all_bitstrings) != sum(multiplicities)
+    """
+    if len(all_bitstrings) != (sum_multiplicities := sum(multiplicities)):
+        raise ValueError(
+            "Mismatch between multiplicities and number of measurements to combine. "
+            f"Got {len(all_bitstrings)} bitstrings lists objects to combine "
+            f"but multiplicities sum to {sum_multiplicities}"
+        )
+    bitstrings_it = iter(all_bitstrings)
+    return [
+        sum(islice(bitstrings_it, multiplicity), start=[])
+        for multiplicity in multiplicities
+    ]
```

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_matrices.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_matrices.py`

 * *Files 10% similar despite different names*

```diff
@@ -126,14 +126,34 @@
     """
     return sympy.simplify(
         (rz_matrix(phi) * ry_matrix(theta) * rz_matrix(lambda_))
         / sympy.exp(-0.5j * (phi + lambda_))
     )
 
 
+def gpi_matrix(theta):
+    """Based on https://ionq.com/docs/getting-started-with-native-gates"""
+    return sympy.Matrix(
+        [
+            [0, sympy.exp(-1j * theta)],
+            [sympy.exp(1j * theta), 0],
+        ]
+    )
+
+
+def gpi2_matrix(theta):
+    """Based on https://ionq.com/docs/getting-started-with-native-gates"""
+    return (2 ** (-0.5)) * sympy.Matrix(
+        [
+            [1, -1j * sympy.exp(-1j * theta)],
+            [-1j * sympy.exp(1j * theta), 1],
+        ]
+    )
+
+
 # --- non-parametric two qubit gates ---
 
 
 def cnot_matrix():
     return sympy.Matrix(
         [
             [1, 0, 0, 0],
@@ -217,13 +237,25 @@
             [0, sympy.cos(angle / 2), 1j * sympy.sin(angle / 2), 0],
             [0, 1j * sympy.sin(angle / 2), sympy.cos(angle / 2), 0],
             [0, 0, 0, 1],
         ]
     )
 
 
+def ms_matrix(phi_0, phi_1):
+    """Based on https://ionq.com/docs/getting-started-with-native-gates"""
+    return (2 ** (-0.5)) * sympy.Matrix(
+        [
+            [1, 0, 0, -1j * sympy.exp(-1j * (phi_0 + phi_1))],
+            [0, 1, -1j * sympy.exp(-1j * (phi_0 - phi_1)), 0],
+            [0, -1j * sympy.exp(1j * (phi_0 - phi_1)), 1, 0],
+            [-1j * sympy.exp(1j * (phi_0 + phi_1)), 0, 0, 1],
+        ]
+    )
+
+
 def delay_matrix(_duration):
     # Note that _duration parameter is not used when constructing the
     # matrix, because Delay always acts as identity.
     # Therefore, the Delay gate will always evaluate to identity on simulator,
     # but it will have an effect if used on an actual hardware.
     return i_matrix()
```

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_operations.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_operations.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_serde.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_serde.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_testing.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_testing.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_unitary_tools.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_unitary_tools.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/_wavefunction_operations.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/_wavefunction_operations.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/layouts.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/layouts.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/_sorting.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/_sorting.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/expressions.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/expressions.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/sympy_expressions.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/sympy_expressions.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/circuits/symbolic/translations.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/circuits/symbolic/translations.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/decompositions/_decomposition.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/decompositions/_decomposition.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/decompositions/_orquestra_decompositions.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/decompositions/_orquestra_decompositions.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/BAS_dataset.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/BAS_dataset.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/__init__.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/_measurement_outcome_distribution.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/_measurement_outcome_distribution.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/clipped_negative_log_likelihood.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/clipped_negative_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/jensen_shannon_divergence.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/jensen_shannon_divergence.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/mmd.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/mmd.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/distributions/target_thermal_states.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/distributions/target_thermal_states.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/estimation/_estimation.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/estimation/_estimation.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/evolution.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/evolution.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/__init__.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/expectation_values.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/expectation_values.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/measurements.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/measurements.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/measurements/parities.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/measurements/parities.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/__init__.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_io.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_io.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/__init__.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/config.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/config.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/operator_utils.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/operator_utils.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_openfermion_utils/sparse_tools.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_openfermion_utils/sparse_tools.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_pauli_operators.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_pauli_operators.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/operators/_utils.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/operators/_utils.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/runners/symbolic_simulator.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/runners/symbolic_simulator.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/runners/trackers.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/runners/trackers.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/testing/_initialize.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/testing/_initialize.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/testing/generate_cases_for_backend_tests.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/testing/generate_cases_for_backend_tests.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/testing/hamiltonian_H2_minimal_basis.json` & `orquestra-quantum-0.9.0/src/orquestra/quantum/testing/hamiltonian_H2_minimal_basis.json`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/testing/hamiltonian_H2_minus_ROHF_minimal_basis.json` & `orquestra-quantum-0.9.0/src/orquestra/quantum/testing/hamiltonian_H2_minus_ROHF_minimal_basis.json`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/testing/hamiltonian_HeH_plus_STO-3G.json` & `orquestra-quantum-0.9.0/src/orquestra/quantum/testing/hamiltonian_HeH_plus_STO-3G.json`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/testing/mocks.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/testing/test_cases_for_backend_tests.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/testing/test_cases_for_backend_tests.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/typing.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/typing.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/utils.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/utils.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra/quantum/wavefunction.py` & `orquestra-quantum-0.9.0/src/orquestra/quantum/wavefunction.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/PKG-INFO` & `orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-quantum
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra's library with basic quantum operations"
 Home-page: https://github.com/zapatacomputing/orquestra-quantum
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-quantum-0.8.0/src/orquestra_quantum.egg-info/SOURCES.txt` & `orquestra-quantum-0.9.0/src/orquestra_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/Makefile` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/README.rst` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/README.rst`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/pyproject.toml` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/sample_setup.py` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/sample_setup.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/setup_extras.py` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/setup_extras.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml` & `orquestra-quantum-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/api/estimator_contract_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/api/estimator_contract_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_builtin_gates_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_builtin_gates_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,12 +28,15 @@
             _builtin_gates.RH(1.5),
             _builtin_gates.U3(0.5, -3.14, 0),
             _builtin_gates.XX(0.1),
             _builtin_gates.YY(0.2),
             _builtin_gates.ZZ(0.3),
             _builtin_gates.PHASE(1),
             _builtin_gates.CPHASE(0.1),
+            _builtin_gates.GPi(0.1),
+            _builtin_gates.GPi2(0.1),
+            _builtin_gates.MS(0.1, 0.2),
             _builtin_gates.Delay(0.5),
         ],
     )
     def test_gates_matrix_equals_its_adjoint_iff_gate_is_hermitian(self, gate):
         assert (gate.matrix == gate.matrix.adjoint()) == gate.is_hermitian
```

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_circuit_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_circuit_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_gates_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_gates_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,22 +24,25 @@
     _builtin_gates.H,
     _builtin_gates.I,
     _builtin_gates.RX(sympy.Symbol("theta")),
     _builtin_gates.RY(0.5),
     _builtin_gates.RZ(0),
     _builtin_gates.PHASE(sympy.pi / 5),
     _builtin_gates.U3(np.pi, sympy.pi / 2, sympy.Symbol("x")),
+    _builtin_gates.GPi(sympy.Symbol("theta")),
+    _builtin_gates.GPi2(sympy.Symbol("theta")),
     _builtin_gates.CZ,
     _builtin_gates.CNOT,
     _builtin_gates.SWAP,
     _builtin_gates.ISWAP,
     _builtin_gates.XX(sympy.cos(sympy.Symbol("phi"))),
     _builtin_gates.YY(sympy.pi),
     _builtin_gates.ZZ(sympy.Symbol("x") + sympy.Symbol("y")),
     _builtin_gates.CPHASE(1.5),
+    _builtin_gates.MS(sympy.Symbol("theta"), np.pi / 2),
 ]
 
 POWER_GATE_EXPONENTS = [-2.0, 0, 0.5, 1.0]
 
 
 def example_one_qubit_matrix_factory(a, b):
     return sympy.Matrix([[a, b], [b, a]])
```

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_generators_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_generators_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_itertools_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_itertools_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from orquestra.quantum.circuits import CNOT, H, X
 from orquestra.quantum.circuits._circuit import Circuit
 from orquestra.quantum.circuits._itertools import (
+    combine_bitstrings,
     combine_measurement_counts,
     expand_sample_sizes,
     split_into_batches,
 )
 from orquestra.quantum.measurements import Measurements
 
 
@@ -135,7 +136,54 @@
         assert all(
             actual == expected
             for actual, expected in zip(
                 combine_measurement_counts(all_counts, multiplicities),
                 combined_counts,
             )
         )
+
+
+class TestCombiningBitstrings:
+    def test_raises_error_when_multiplicities_dont_match_measurements(self):
+        multiplicities = [1, 2, 3, 2, 2]
+        # Clearly a mismatch, we should have 10 bitstring sequences
+        measurements = [["00", "11"] for _ in range(5)]
+
+        with pytest.raises(ValueError):
+            combine_measurement_counts(measurements, multiplicities)
+
+    @pytest.mark.parametrize(
+        "all_bitstrings, multiplicities, combined_bitstrings",
+        [
+            ([["00", "11"]], [1], [["00", "11"]]),
+            (
+                [
+                    ["00", "11"],
+                    ["01", "00"],
+                    ["00", "00"],
+                    ["000"],
+                    ["111", "001"],
+                    ["00000"],
+                    ["0", "0", "0"],
+                    ["1", "0"],
+                    ["0", "0"],
+                ],
+                [3, 2, 1, 3],
+                [
+                    ["00", "11", "01", "00", "00", "00"],
+                    ["000", "111", "001"],
+                    ["00000"],
+                    ["0", "0", "0", "1", "0", "0", "0"],
+                ],
+            ),
+        ],
+    )
+    def test_counts_of_combined_bitstrings_are_correct(
+        self, all_bitstrings, multiplicities, combined_bitstrings
+    ):
+        assert all(
+            actual == expected
+            for actual, expected in zip(
+                combine_bitstrings(all_bitstrings, multiplicities),
+                combined_bitstrings,
+            )
+        )
```

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_serde_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_serde_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_unitary_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_unitary_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/_wavefunction_operations_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/_wavefunction_operations_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/hardcoded_cirq_unitaries.npy` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/hardcoded_cirq_unitaries.npy`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/layouts_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/layouts_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/symbolic/sorting_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/symbolic/sorting_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/symbolic/sympy_expressions_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/symbolic/sympy_expressions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/circuits/symbolic/translations_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/circuits/symbolic/translations_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/decompositions/_zquantum_decomposition_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/decompositions/_zquantum_decomposition_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/BAS_dataset_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/BAS_dataset_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/_measurement_outcome_distribution_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/_measurement_outcome_distribution_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/distance_measures_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/distance_measures_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/distributions/target_thermal_states_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/distributions/target_thermal_states_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/estimation/estimation_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/estimation/estimation_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/evolution_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/evolution_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/measurements/expectation_values_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/measurements/expectation_values_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/measurements/measurements_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/measurements/measurements_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/measurements/parities_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/measurements/parities_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_io_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_io_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_openfermion_utils/operator_utils_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_openfermion_utils/operator_utils_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_openfermion_utils/sparse_tools_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_openfermion_utils/sparse_tools_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_operators_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_operators_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/operators/_utils_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/operators/_utils_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/runners/symbolic_simulator_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/runners/symbolic_simulator_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/runners/trackers_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/runners/trackers_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/utils_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/utils_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-quantum-0.8.0/tests/orquestra/quantum/wavefunction_test.py` & `orquestra-quantum-0.9.0/tests/orquestra/quantum/wavefunction_test.py`

 * *Files identical despite different names*

