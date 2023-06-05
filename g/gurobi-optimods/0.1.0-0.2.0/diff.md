# Comparing `tmp/gurobi_optimods-0.1.0.tar.gz` & `tmp/gurobi_optimods-0.2.0.tar.gz`

## Comparing `gurobi_optimods-0.1.0.tar` & `gurobi_optimods-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,92 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/Makefile
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tox.ini
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/ISSUE_TEMPLATE/new_mod.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/doc-build.yml
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/doc-tests.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.github/workflows/wheel-tests.yml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/adding.rst
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/api.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/beyond.rst
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/contact.rst
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/contributing.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/dev-reference.rst
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/extending.rst
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/gallery.rst
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/installation.rst
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/license.rst
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/usage.rst
--rw-r--r--   0        0        0     9474 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/bipartite-matching.rst
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/diet.rst
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/l1-regression.rst
--rw-r--r--   0        0        0    11332 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/min-cost-flow.rst
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/mwis.rst
--rw-r--r--   0        0        0    27437 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/portfolio.rst
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/qubo.rst
--rw-r--r--   0        0        0    16213 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/workforce.rst
--rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-example.png
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-figs.py
--rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-flow.png
--rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-result.png
--rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/lad-outlier-coeffs.png
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/lad-outlier-errors.png
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/lad-regression-coeffs.png
--rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/min-cost-flow-result.png
--rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/mvp.png
--rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/mwis.png
--rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/pie.png
--rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/qubo.png
--rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/figures/shortest-path-result.png
--rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/mods/icons/lad-regression.png
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/refs/graphs.bib
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/refs/portfolio.bib
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/refs/qubo.bib
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/docs/source/refs/regression.bib
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/__init__.py
--rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/bipartite_matching.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/datasets.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/diet.py
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/min_cost_flow.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/mwis.py
--rw-r--r--   0        0        0    13528 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/portfolio.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/qubo.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/regression.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/utils.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/workforce.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/diet/diet-categories.csv
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/diet/diet-foods.csv
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/diet/diet-values.csv
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/graphs/edge_data1.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/graphs/edge_data2.csv
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/graphs/node_data1.csv
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/graphs/node_data2.csv
--rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/portfolio/portfolio.csv
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/workforce/preferences.csv
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/workforce/shift_requirements.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/src/gurobi_optimods/data/workforce/worker_limits.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0    10863 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_bipartite_matching.py
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_diet.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_min_cost_flow.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_mwis.py
--rw-r--r--   0        0        0    28263 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_portfolio.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_qubo.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_regression.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/tests/test_workforce.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/NOTICE
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 gurobi_optimods-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/Makefile
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tox.ini
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/ISSUE_TEMPLATE/new_mod.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/doc-build.yml
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/doc-tests.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/wheel-tests.yml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/adding.rst
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/api.rst
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/contact.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/dev-reference.rst
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/gallery.rst
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/license.rst
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/usage.rst
+-rw-r--r--   0        0        0     8660 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/bipartite-matching.rst
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/lad-regression.rst
+-rw-r--r--   0        0        0     9861 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/min-cost-flow.rst
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/mwis.rst
+-rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/portfolio.rst
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/qubo.rst
+-rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/workforce.rst
+-rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-example.png
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-figs.py
+-rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-flow.png
+-rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-result.png
+-rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-coeffs.png
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-errors.png
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/lad-regression-coeffs.png
+-rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/min-cost-flow-result.png
+-rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/mvp.png
+-rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/mwis.png
+-rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/pie.png
+-rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/qubo.png
+-rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/shortest-path-result.png
+-rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/icons/lad-regression.png
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/graphs.bib
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/portfolio.bib
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/qubo.bib
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/regression.bib
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/workforce.bib
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/__init__.py
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/bipartite_matching.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/datasets.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/min_cost_flow.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/mwis.py
+-rw-r--r--   0        0        0    14692 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/portfolio.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/qubo.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/regression.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/utils.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/workforce.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/edge_data1.csv
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/edge_data2.csv
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/node_data1.csv
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/node_data2.csv
+-rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/portfolio/portfolio.csv
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/preferences.csv
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/shift_requirements.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/worker_limits.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_bipartite_matching.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_graph_utils.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_min_cost_flow.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_mwis.py
+-rw-r--r--   0        0        0    31002 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_portfolio.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_qubo.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_regression.py
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_workforce.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/NOTICE
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/README.md
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/PKG-INFO
```

### Comparing `gurobi_optimods-0.1.0/CODE_OF_CONDUCT.md` & `gurobi_optimods-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/CONTRIBUTING.md` & `gurobi_optimods-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/pull_request_template.md` & `gurobi_optimods-0.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/ISSUE_TEMPLATE/new_mod.md` & `gurobi_optimods-0.2.0/.github/ISSUE_TEMPLATE/new_mod.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/workflows/code-quality.yml` & `gurobi_optimods-0.2.0/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/workflows/doc-build.yml` & `gurobi_optimods-0.2.0/.github/workflows/doc-build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,8 @@
       - name: Install docs build dependencies
         run: |
           python -m pip install -rdocs/requirements.txt
           python -m pip install .
       - name: Build docs (fail on warnings)
         run: |
           cd docs
-          make clean html SPHINXOPTS="-W --keep-going"
+          make clean html SPHINXOPTS="-W --keep-going -n"
```

### Comparing `gurobi_optimods-0.1.0/.github/workflows/doc-tests.yml` & `gurobi_optimods-0.2.0/.github/workflows/doc-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/workflows/publish-pypi.yml` & `gurobi_optimods-0.2.0/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/workflows/python-tests.yml` & `gurobi_optimods-0.2.0/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/workflows/release.yml` & `gurobi_optimods-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/.github/workflows/wheel-tests.yml` & `gurobi_optimods-0.2.0/.github/workflows/wheel-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/Makefile` & `gurobi_optimods-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/make.bat` & `gurobi_optimods-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/adding.rst` & `gurobi_optimods-0.2.0/docs/source/adding.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Adding a New Mod
+Adding a new Mod
 ================
 
 The goal of the OptiMods is to create and maintain an open-source Python
 repository of implemented optimization use cases. Each use case will have clear,
 informative, and pretty documentation that explains both how to use it and the
 mathematical model behind it for interested readers.
 
@@ -13,15 +13,15 @@
 Proposing a new Mod
 -------------------
 
 To propose a new mod, create an issue in our repository using the 'New Mod
 Proposal' template to gather the required details. One of the maintainers will
 reach out to you on the issue to discuss the proposed topic and design.
 
-A good mod:
+A good Mod:
 
 - solves well-known, well-defined problem from a non-optimization field;
 - has a simple interface which shields the user from interacting with gurobipy
   directly;
 - is self-contained, and follows a clean data-in data-out style leaning on
   standard packages from the python ecosystem (``numpy``, ``scipy``, and
   ``pandas`` are our first-class citizens);
@@ -64,20 +64,14 @@
         """An optimod which solves an important problem
 
         :param data: Description of argument
         :type data: Type of argument
 
         ... describe additional arguments ...
 
-        :param silent: ``silent=True`` suppresses all console output. Defaults
-            to ``False``.
-        :type silent: bool
-        :param logfile: Write all mod output to the given file path. Defaults
-            to ``None`` (no log file produced)
-        :type logfile: str
         :return: Description of returned result
         :rtype: Type of returned result
         """
 
         # ... Prepare data ...
 
         with create_env() as env, gp.Model(env=env) as model:
@@ -92,16 +86,16 @@
 
 Mods should be stateless with respect to ``gurobipy`` objects. This means Gurobi
 environments and models are created within a mod function, and closed before the
 function returns using context managers. Gurobi environments should be created
 by calling ``create_env``. This function is provided to your mod by the
 ``@optimod()`` decorator and supplies some necessary parameters to Gurobi to
 handle console output and log files consistently across mods. The standard
-parameters ``silent`` and ``logfile`` are also handled by the decorator, but you
-should include them in the docstring as above.
+parameters ``verbose`` and ``logfile`` are also handled by the decorator and will
+be included automatically in the API documentation.
 
 If your mod needs to produce any output, use the in-built python logging call
 ``logger.info``.
 
 You should also include your mod in the :doc:`api` by adding appropriate
 `autodoc <https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html>`_
 references to ``docs/source/api.rst``.
@@ -113,14 +107,24 @@
 each mod is different, there is no specific template for this, but please use
 the existing mod pages as a guide.
 
 A reference to your page must also be added to ``docs/source/gallery.rst`` to
 include it in the gallery page and toctree when the documentation is built. You
 should also add an icon to the gallery card for your mod.
 
+Your documentation page must contain example codes that new users can
+immediately used, with presentation of the results included in the documentation
+page.
+
+The implementation of the Mod (description of the mathematical model or
+algorithms used) should be hidden from the user at first glance. We use tabs to
+do this. Any mathematical and algorithmic details should be placed in a tab and
+clearly indicate that this is advanced detail the user does not need to fully
+understand in order to use the Mod.
+
 Including datasets
 ------------------
 
 Some of your examples may rely on datasets. These can be packaged with the
 optimods to enable users to quickly reproduce the examples in your documentation.
 
 - Any data files should live under a subdirectory
```

### Comparing `gurobi_optimods-0.1.0/docs/source/api.rst` & `gurobi_optimods-0.2.0/docs/source/api.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 API Reference
 =============
 
 .. automodule:: gurobi_optimods.bipartite_matching
    :members: maximum_bipartite_matching
 
-.. automodule:: gurobi_optimods.diet
-   :members: solve_diet_problem
-
 .. automodule:: gurobi_optimods.min_cost_flow
    :members: min_cost_flow, min_cost_flow_networkx, min_cost_flow_scipy
 
 .. automodule:: gurobi_optimods.mwis
    :members: maximum_weighted_independent_set
 
 .. automodule:: gurobi_optimods.portfolio
-   :members: MeanVariancePortfolio
+   :members: MeanVariancePortfolio, PortfolioResult
 
 .. automodule:: gurobi_optimods.qubo
-   :members: solve_qubo
+   :members: solve_qubo, QuboResult
 
 .. automodule:: gurobi_optimods.regression
    :members: LADRegression
 
 .. automodule:: gurobi_optimods.workforce
    :members: solve_workforce_scheduling
```

### Comparing `gurobi_optimods-0.1.0/docs/source/contributing.rst` & `gurobi_optimods-0.2.0/docs/source/contributing.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Contributing to OptiMods
 ========================
 
 We welcome contributions from the commumnity: bug fixes, doc corrections,
-extensions to existing mods, or development of new mods. This page describes
+extensions to existing Mods, or development of new Mods. This page describes
 conventions to follow when contributing, and the development process we follow
 for the project, which is applicable to all contributors. For guidelines on
-proposing and implementing new mods, see :doc:`adding`. For discussion on
-extending existing mods, see :doc:`extending`.
+proposing and implementing new Mods, see :doc:`adding`.
 
 Coding Standards
 ----------------
 
 We use `black <https://github.com/psf/black>`_ to format all source code.
 ``pre-commit`` takes care of this formatting when installed (see
-:ref:`contributing:development environment`) and runs checks automatically when you commit
-changes. To run code quality checks manually, run the following and ensure no
-issues are reported::
+:ref:`contributing:development environment`) and runs checks automatically when
+you commit changes. To run code quality checks manually, run the following and
+ensure no issues are reported::
 
     pre-commit run --all-files
     python -m flake8 . --select=E9,F63,F7,F82,F811,F401 --show-source
 
+We follow the `numpydoc <https://numpydoc.readthedocs.io/en/latest/format.html>`_
+style guide for docstrings of all public API functions.
+
 Testing
 -------
 
-All new additions, including bug fixes, mod extensions, or brand new mods `must`
+All new additions, including bug fixes, Mod extensions, or brand new Mods `must`
 include unit tests to verify their functionality. We use
-:external+python:std:doc:`unittest <library/unittest>` to test mod functionality
+:external+python:std:doc:`unittest <library/unittest>` to test Mod functionality
 and :doc:`sphinx doctest <sphinx:usage/extensions/doctest>` to ensure code
 snippets provided in the documentation work as expected.
 
 Documentation
 -------------
 
-Documentation is a core part of the OptiMods project. All mods must be
+Documentation is a core part of the OptiMods project. All Mods must be
 accompanied by a documentation page explaining their use and providing
-appropriate background information.
+appropriate background information. If new mod features are added, the
+documentation must reflect the changes.
 
 Development Environment
 -----------------------
 
 To set up your development environment:
 
 1. Create and activate a Python 3.8 virtual environment using your preferred
@@ -68,9 +71,9 @@
 ------------------
 
 We use issues and pull requests to manage and review contributions.
 
 - Minor doc fixes can be submitted directly as pull requests.
 - Bugs should first be reported as issues before submitting a pull request to
   fix them. Use the 'Bug report' issue template.
-- New mod proposals should first be submitted as issues for discussion, see
+- New Mod proposals should first be submitted as issues for discussion, see
   :doc:`adding` for further details.
```

### Comparing `gurobi_optimods-0.1.0/docs/source/dev-reference.rst` & `gurobi_optimods-0.2.0/docs/source/dev-reference.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/gallery.rst` & `gurobi_optimods-0.2.0/docs/source/gallery.rst`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,16 @@
 
     .. grid-item-card:: Maximum Bipartite Matching
         :link: mods/bipartite-matching
         :link-type: doc
         :text-align: center
         :img-top: mods/figures/bipartite-matching-example.png
 
-    .. grid-item-card:: Stigler Diet Problem
-        :link: mods/diet
-        :link-type: doc
-        :text-align: center
-        :img-top: mods/figures/pie.png
-
     .. grid-item-card:: Least Absolute Deviation Regression
-        :link: mods/l1-regression
+        :link: mods/lad-regression
         :link-type: doc
         :text-align: center
         :img-top: mods/icons/lad-regression.png
 
     .. grid-item-card:: Minimum-Cost Flow
         :link: mods/min-cost-flow
         :link-type: doc
@@ -56,14 +50,13 @@
 
 
 .. toctree::
    :maxdepth: 1
    :hidden:
 
    mods/bipartite-matching
-   mods/diet
-   mods/l1-regression
+   mods/lad-regression
    mods/min-cost-flow
    mods/mwis
    mods/portfolio
    mods/qubo
    mods/workforce
```

### Comparing `gurobi_optimods-0.1.0/docs/source/installation.rst` & `gurobi_optimods-0.2.0/docs/source/installation.rst`

 * *Files 20% similar despite different names*

```diff
@@ -4,13 +4,12 @@
 ``gurobi-optimods`` can be installed directly from PyPI::
 
     python -m pip install gurobi-optimods
 
 This will also install ``gurobipy``, ``numpy``, ``scipy``, ``pandas``, and
 ``gurobipy-pandas`` as dependencies.
 
-Please note that gurobipy is commercial software and requires a license (which
-you can get `for free as an academic
-<https://www.gurobi.com/academia/academic-program-and-licenses/>`_). When
+Please note that gurobipy is commercial software and requires a license. When
 installed via pip or conda, gurobipy ships with an evaluation license which is
 only for testing and can only solve models of limited size. You will be able to
 run all the examples given in this documentation using this evaluation license.
+Please see :doc:`license` for details on obtaining a full license for Gurobi.
```

### Comparing `gurobi_optimods-0.1.0/docs/source/usage.rst` & `gurobi_optimods-0.2.0/docs/source/usage.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 
 The best way to get started with the optimods is to try one out! Check out the
 :doc:`gallery` first to find a mod that suits you. Each mod comes complete with
 a page of explanatory documentation which provides background on the problem it
 is intended to solve. The docs also include runnable example codes and datasets
 to get you started.
 
-Note that you may need to install additonal dependencies for some examples. The
+Note that you may need to install additional dependencies for some examples. The
 quick way to ensure you have a Python environment which can execute all the
 example snippets in the docs is to run the following::
 
    python -m pip install gurobi-optimods[examples]
 
 Each mod is designed to be self-contained, with a clean data-in data-out API.
 Munge your data into the appropriate format using Python tools you already know,
 and run the mod as outlined in its documentation page to get back a solution.
 
-If you are interested to learn more about the mathematical model underlying a
-mod, the documentation page explains the model. You can also browse :ghsrc:`the
-mod source<src/gurobi_optimods>` to find out how the model is implemented in
-code.
+The documentation pages also included details of the mathematical model
+underlying the mod, should you be interested to learn more about the
+implementation. These details are explained in sections marked "Background". It
+is not necessary to read and understand these sections in order to use the mod
+effectively. You can also browse :ghsrc:`the mod source <src/gurobi_optimods>`
+to find out how the model is implemented in code.
 
 Finally, we welcome contributions of new mods, bug fixes and new features for
 existing mods, and improvements to the documentation. This is intended to be a
 community project that grows over time to handle a wide range of optimization
 use-cases across a different fields. See :doc:`contributing` for more details.
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/bipartite-matching.rst` & `gurobi_optimods-0.2.0/docs/source/mods/bipartite-matching.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,36 +31,37 @@
 are disjoint vertex sets, and the edge set :math:`E \subseteq U \times V`
 joins only between, not within, the sets. A matching on this graph is any
 subset of edges such that no vertex is incident to more than one edge.
 Equivalently, the matching is a subgraph of :math:`G` where all vertices
 have degree at most one. A maximum matching is the largest possible matching
 on :math:`G`.
 
-Algorithm
----------
+.. dropdown:: Background: Mathematical Model
 
-The bipartite matching problem can be reduced to a maximum flow problem by
-introducing a source vertex as a predecessor to all vertices in :math:`U`,
-and a sink vertex as a successor to all vertices in :math:`V`. Giving every
-edge unit capacity, a maximum matching is found by maximizing flow from the
-source to the sink. All edges with non-zero flow in the max flow solution
-are part of the matching.
-
-.. Figure generated using networkx, see bipartite-matching-figs.py
-.. figure:: figures/bipartite-matching-flow.png
-    :width: 400
-    :alt: Bipartite matching flow network
-
-    A maximum flow network for the bipartite matching problem
-
-
-We do not describe the mathematical formulation here, see the max flow mod (ref)
-for details. The important point to note is that when this continuous model is
-solved using the simplex algorithm, we are guaranteed to get an integral solution
-and thus the solution can be used to select a set of edges for the matching.
+    The bipartite matching Mod is implemented by reducing the basic version of
+    the problem to a minimum-cost flow problem. To do so, we introduce a source
+    vertex as a predecessor to all vertices in :math:`U`, and a sink vertex as a
+    successor to all vertices in :math:`V`. Giving every edge unit capacity, a
+    maximum matching is found by maximizing flow from the source to the sink. As
+    a min-cost flow, this is equivalent to adding an edge with a negative cost
+    from the sink to the source and assigning zero cost to all other edges. All
+    edges with non-zero flow in the min-cost flow solution are part of the
+    matching.
+
+    .. Figure generated using networkx, see bipartite-matching-figs.py
+    .. figure:: figures/bipartite-matching-flow.png
+        :width: 400
+        :alt: Bipartite matching flow network
+
+        A maximum flow network for the bipartite matching problem
+
+    We do not describe the mathematical formulation here, see :doc:`/mods/min-cost-flow`
+    for details. The important point to note is that when this continuous model is
+    solved using the simplex algorithm, we are guaranteed to get an integral solution
+    and thus the solution can be used to select a set of edges for the matching.
 
 Interface
 ---------
 
 The ``maximum_bipartite_matching`` function supports scipy sparse arrays, pandas
 dataframes, and networkx graphs as possible inputs. The user must also provide
 the bipartite partitioning of the input graph. In all cases, the matching is
@@ -159,45 +160,14 @@
 
 
 The ``maximum_bipartite_matching`` function formulates a linear program for the
 the network flow model corresponding to the given bipartite graph. Since the
 model is formulated as a network flow, Gurobi will in most cases solve the model
 using a network primal simplex algorithm.
 
-.. collapse:: View Gurobi logs
-
-    .. code-block:: text
-
-        Solving maximum matching n1=5 n2=4 |E|=11
-        Gurobi Optimizer version 10.0.1 build v10.0.1rc0 (mac64[x86])
-
-        CPU model: Intel(R) Core(TM) i5-1038NG7 CPU @ 2.00GHz
-        Thread count: 4 physical cores, 8 logical processors, using up to 8 threads
-
-        Optimize a model with 11 rows, 21 columns and 42 nonzeros
-        Model fingerprint: 0x6966afa3
-        Coefficient statistics:
-          Matrix range     [1e+00, 1e+00]
-          Objective range  [1e+00, 1e+00]
-          Bounds range     [1e+00, 1e+00]
-          RHS range        [0e+00, 0e+00]
-        Presolve removed 2 rows and 3 columns
-        Presolve time: 0.00s
-        Presolved: 9 rows, 18 columns, 36 nonzeros
-
-        Iteration    Objective       Primal Inf.    Dual Inf.      Time
-               0    4.0000000e+00   8.000000e+00   0.000000e+00      0s
-               6    4.0000000e+00   0.000000e+00   0.000000e+00      0s
-
-        Solved in 6 iterations and 0.00 seconds (0.00 work units)
-        Optimal objective  4.000000000e+00
-        Max bipartite matching |E|=4
-
-|
-
 Solution
 --------
 
 .. tabs::
 
     .. group-tab:: scipy
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/l1-regression.rst` & `gurobi_optimods-0.2.0/docs/source/mods/lad-regression.rst`

 * *Files 14% similar despite different names*

```diff
@@ -23,47 +23,41 @@
 
 Problem Specification
 ---------------------
 
 Scikit-learn's documentation gives a general explanation of `Linear Models
 <https://scikit-learn.org/stable/modules/linear_model.html>`_. The distinction
 between this mod and the Ordinary Least Squares regression from scikit-learn is the
-loss function.
-
-.. tabs::
-
-    .. tab:: Loss Function
-
-        :code:`LADRegression` chooses coefficients :math:`w` of a linear model
-        :math:`y = Xw` to minimize the sum of absolute errors on a training
-        dataset :math:`(X, y)`. In other words, it aims to minimize the
-        following loss function:
-
-        .. math::
-
-            \min_w \lvert Xw - y \rvert
-
-    .. tab:: Optimization Model
-
-        To model the L1 regression loss function using linear programming, a a
-        number of auxiliary variables are introduced. Here :math:`I` is the set
-        of observations and :math:`J` the set of fields. Response values
-        :math:`y_i` are predicted from predictor values :math:`x_{ij}` by
-        fitting coefficients :math:`w_j`. To handle the absolute value in the
-        loss function, non-negative variables :math:`u_i` and :math:`v_i` are
-        introduced.
-
-        .. math::
-
-            \begin{alignat}{2}
-            \min \quad        & \sum_i u_i + v_i \\
-            \mbox{s.t.} \quad & \sum_j w_j x_{ij} + u_i - v_i = y_i \quad & \forall i \in I \\
-                              & u_i, v_i \ge 0                      \quad & \forall i \in I \\
-                              & w_j \,\, \text{free}                \quad & \forall j \in J \\
-            \end{alignat}
+loss function. ``LADRegression`` chooses coefficients :math:`w` of a linear model
+:math:`y = Xw` to minimize the sum of absolute errors on a training
+dataset :math:`(X, y)`. In other words, it aims to minimize the
+following loss function:
+
+.. math::
+
+    \min_w \lvert Xw - y \rvert
+
+.. dropdown:: Background: Mathematical Model
+
+    The fitting algorithm of the LAD regression Mod is implemented by
+    formulating the loss function as a Linear Program (LP), which is then solved
+    using Gurobi. Here :math:`I` is the set of observations and :math:`J` the
+    set of fields. Response values :math:`y_i` are predicted from predictor
+    values :math:`x_{ij}` by fitting coefficients :math:`w_j`. To handle the
+    absolute value in the loss function, auxiliary non-negative variables
+    :math:`u_i` and :math:`v_i` are introduced.
+
+    .. math::
+
+        \begin{alignat}{2}
+        \min \quad        & \sum_i u_i + v_i \\
+        \mbox{s.t.} \quad & \sum_j w_j x_{ij} + u_i - v_i = y_i \quad & \forall i \in I \\
+                          & u_i, v_i \ge 0                      \quad & \forall i \in I \\
+                          & w_j \,\, \text{free}                \quad & \forall j \in J \\
+        \end{alignat}
 
 Example Code
 ------------
 
 This mod implements the fit-predict API used by all predictive models in
 scikit-learn (including the :code:`sklearn.linear_model.LinearRegression`
 class). The example below reads in the diabetes dataset from scikit-learn,
@@ -110,50 +104,19 @@
     >>> y_train.shape
     (331,)
     >>> X_test.shape
     (111, 10)
     >>> y_test.shape
     (111,)
 
-The formulated model is solved as a linear program by Gurobi. Logs provided for
-interested parties:
-
-.. collapse:: View Gurobi logs
-
-    .. code-block:: text
-
-        Gurobi Optimizer version 10.0.1 build v10.0.1rc0 (mac64[x86])
-
-        CPU model: Intel(R) Core(TM) i5-1038NG7 CPU @ 2.00GHz
-        Thread count: 4 physical cores, 8 logical processors, using up to 8 threads
-
-        Optimize a model with 331 rows, 673 columns and 4303 nonzeros
-        Model fingerprint: 0xb54fc171
-        Coefficient statistics:
-          Matrix range     [6e-05, 1e+00]
-          Objective range  [1e+00, 1e+00]
-          Bounds range     [0e+00, 0e+00]
-          RHS range        [2e+01, 3e+02]
-        Presolve time: 0.00s
-        Presolved: 331 rows, 673 columns, 4303 nonzeros
-
-        Iteration    Objective       Primal Inf.    Dual Inf.      Time
-               0      handle free variables                          0s
-             354    1.4473274e+04   0.000000e+00   0.000000e+00      0s
-
-        Solved in 354 iterations and 0.01 seconds (0.01 work units)
-        Optimal objective  1.447327363e+04
-
-|
-
-Comparison with OLS
--------------------
+Comparison with Ordinary Least Squares
+--------------------------------------
 
 Here we extract the coefficients of the fitted model and compare them with the
-coefficients found using OLS.
+coefficients found using Ordinary Least Squares (OLS).
 
 .. testcode:: lad_regression
 
     import pandas as pd
     import matplotlib.pyplot as plt
     from sklearn.linear_model import LinearRegression
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/min-cost-flow.rst` & `gurobi_optimods-0.2.0/docs/source/mods/min-cost-flow.rst`

 * *Files 20% similar despite different names*

```diff
@@ -13,71 +13,64 @@
 larger networks include cost-scaling methods (e.g. variants of the push-relabel
 algorithm by :footcite:t:`goldberg1990finding`). For a more detailed comparison
 see, for example, :footcite:t:`kovacs2015minimum`.
 
 Problem Specification
 ---------------------
 
-We provide the graph theory and mathematical definition of this problem.
+For a given graph :math:`G` with set of vertices :math:`V` and edges
+:math:`E`. Each edge :math:`(i,j)\in E` has the following attributes:
 
-.. tabs::
-
-    .. tab:: Graph Theory
-
-        For a given graph :math:`G` with set of vertices :math:`V` and edges
-        :math:`E`. Each edge :math:`(i,j)\in E` has the following attributes:
-
-        - cost: :math:`c_{ij}\in \mathbb{R}`;
-        - and capacity: :math:`B_{ij}\in\mathbb{R}`.
+- cost: :math:`c_{ij}\in \mathbb{R}`;
+- and capacity: :math:`B_{ij}\in\mathbb{R}`.
 
-        Also, each vertex :math:`i\in V` has a demand :math:`d_i\in\mathbb{R}`.
-        This value can be positive (requesting flow), negative (supplying
-        flow), or 0.
+Each vertex :math:`i\in V` has a demand :math:`d_i\in\mathbb{R}` which can be
+positive (requesting flow), negative (supplying flow), or zero (a transshipment
+node).
 
-        The problem can be stated as finding the flow with minimal total cost
-        such that:
+The problem can be stated as finding the flow with minimal total cost
+such that:
 
-        - the demand at each vertex is met;
-        - and, the flow is capacity feasible.
+- the demand at each vertex is met exactly; and
+- the flow is capacity feasible.
 
-    .. tab:: Optimization Model
+.. dropdown:: Background: Optimization Model
 
-        Let us define a set of continuous variables :math:`x_{ij}` to represent
-        the amount of non-negative (:math:`\geq 0`) flow going through an edge
-        :math:`(i,j)\in E`.
+    This Mod is implemented by formulating a Linear Program (LP) and solving it
+    using Gurobi. Let us define a set of continuous variables :math:`x_{ij}` to
+    represent the amount of non-negative (:math:`\geq 0`) flow going through an
+    edge :math:`(i,j)\in E`.
 
+    The formulation can be stated as follows:
 
-        The mathematical formulation can be stated as follows:
+    .. math::
 
-        .. math::
+        \begin{alignat}{2}
+            \min \quad        & \sum_{(i, j) \in E} c_{ij} x_{ij} \\
+            \mbox{s.t.} \quad & \sum_{j \in \delta^+(i)} x_{ij} - \sum_{j \in \delta^-(i)} x_{ji} = d_i & \forall i \in V \\
+                            & 0 \leq x_{ij} \le B_{ij} & \forall (i, j) \in E \\
+        \end{alignat}
 
-            \begin{alignat}{2}
-              \min \quad        & \sum_{(i, j) \in E} c_{ij} x_{ij} \\
-              \mbox{s.t.} \quad & \sum_{j \in \delta^+(i)} x_{ij} - \sum_{j \in \delta^-(i)} x_{ji} = d_i & \forall i \in V \\
-                                & 0 \leq x_{ij} \le B_{ij} & \forall (i, j) \in E \\
-            \end{alignat}
+    Where :math:`\delta^+(\cdot)` (:math:`\delta^-(\cdot)`) denotes the
+    outgoing (incoming) neighbours.
 
-        Where :math:`\delta^+(\cdot)` (:math:`\delta^-(\cdot)`) denotes the
-        outgoing (incoming) neighbours.
+    The objective minimises the total cost over all edges.
 
-        The objective minimises the total cost over all edges.
+    The first constraints ensure flow balance for all vertices. That is, for
+    a given node, the incoming flow (sum over all incoming edges to this
+    node) minus the outgoing flow (sum over all outgoing edges from this
+    node) is equal to the demand. Clearly, in the case when the demand is 0,
+    the outgoing flow must be equal to the incoming flow. When the demand is
+    negative, this node can supply flow to the network (outgoing term is
+    larger), and conversely when the demand is negative, this node can
+    request flow from the network (incoming term is larger).
 
-        The first constraints ensure flow balance for all vertices. That is, for
-        a given node, the incoming flow (sum over all incoming edges to this
-        node) minus the outgoing flow (sum over all outgoing edges from this
-        node) is equal to the demand. Clearly, in the case when the demand is 0,
-        the outgoing flow must be equal to the incoming flow. When the demand is
-        negative, this node can supply flow to the network (outgoing term is
-        larger), and conversely when the demand is negative, this node can
-        request flow from the network (incoming term is larger).
+    The last constraints ensure non-negativity of the variables and that the
+    capacity per edge is not exceeded.
 
-        The last constraints ensure non-negativity of the variables and that the
-        capacity per edge is not exceeded.
-
-|
 
 Code and Inputs
 ---------------
 
 For this mod, one can use input graphs of different types:
 
 * pandas: using a ``pd.DataFrame``;
@@ -149,20 +142,14 @@
           (3, {'demand': 1})
           (4, {'demand': 0})
           (5, {'demand': 2})
 
       Edges have attributes ``capacity`` and ``cost`` and nodes have
       attributes ``demand``.
 
-      We assume that nodes labels are integers from :math:`0,\dots,|V|-1`.
-      NetworkX has a handy function for this
-      `nx.convert_node_labels_to_integers`_.
-
-      .. _nx.convert_node_labels_to_integers: https://networkx.org/documentation/stable/reference/generated/networkx.relabel.convert_node_labels_to_integers.html
-
   .. group-tab:: scipy.sparse
 
       .. doctest:: load_graph_scipy
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
           >>> G, capacities, cost, demands = datasets.load_graph_scipy()
@@ -213,59 +200,59 @@
 
       .. doctest:: min_cost_flow
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
           >>> from gurobi_optimods.min_cost_flow import min_cost_flow
           >>> edge_data, node_data = datasets.load_graph()
-          >>> obj, sol = min_cost_flow(edge_data, node_data, silent=True)
+          >>> obj, sol = min_cost_flow(edge_data, node_data, verbose=False)
           >>> obj
           31.0
           >>> sol
           source  target
           0       1         1.0
                   2         1.0
           1       3         1.0
           2       3         0.0
                   4         2.0
           3       5         0.0
           4       5         2.0
-          dtype: float64
+          Name: flow, dtype: float64
 
       The ``min_cost_flow`` function returns the cost of the solution as well
       as ``pd.Series`` with the flow per edge. Similarly as the input
       DataFrame the resulting series is indexed by ``source`` and ``target``.
 
 
   .. group-tab:: NetworkX
 
       .. doctest:: min_cost_flow_networkx
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
           >>> from gurobi_optimods.min_cost_flow import min_cost_flow_networkx
           >>> G = datasets.load_graph_networkx()
-          >>> obj, sol = min_cost_flow_networkx(G, silent=True)
+          >>> obj, sol = min_cost_flow_networkx(G, verbose=False)
           >>> obj
           31.0
-          >>> sol
-          {(0, 1): 1.0, (0, 2): 1.0, (1, 3): 1.0, (2, 4): 2.0, (4, 5): 2.0}
+          >>> list(sol.edges(data=True))
+          [(0, 1, {'flow': 1.0}), (0, 2, {'flow': 1.0}), (1, 3, {'flow': 1.0}), (2, 4, {'flow': 2.0}), (4, 5, {'flow': 2.0})]
 
       The ``min_cost_flow_networkx`` function returns the cost of the solution
       as well as a dictionary indexed by edge with the non-zero flow.
 
   .. group-tab:: scipy.sparse
 
       .. doctest:: min_cost_flow_networkx
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
           >>> from gurobi_optimods.min_cost_flow import min_cost_flow_scipy
           >>> G, capacities, cost, demands = datasets.load_graph_scipy()
-          >>> obj, sol = min_cost_flow_scipy(G, capacities, cost, demands, silent=True)
+          >>> obj, sol = min_cost_flow_scipy(G, capacities, cost, demands, verbose=False)
           >>> obj
           31.0
           >>> sol
           <5x6 sparse matrix of type '<class 'numpy.float64'>'
                   with 5 stored elements in COOrdinate format>
           >>> print(sol)
             (0, 1)        1.0
@@ -286,38 +273,8 @@
 .. image:: figures/min-cost-flow-result.png
   :width: 600
   :alt: Sample network.
 
 In all these cases, the model is solved as an LP by Gurobi (typically using the
 NS algorithm).
 
-.. collapse:: View Gurobi Logs
-
-    .. code-block:: text
-
-        Solving min-cost flow with 6 nodes and 7 edges
-        Gurobi Optimizer version 10.0.1 build v10.0.1rc0 (mac64[arm])
-
-        CPU model: Apple M1
-        Thread count: 8 physical cores, 8 logical processors, using up to 8 threads
-
-        Optimize a model with 6 rows, 7 columns and 14 nonzeros
-        Model fingerprint: 0xc6fc382e
-        Coefficient statistics:
-          Matrix range     [1e+00, 1e+00]
-          Objective range  [1e+00, 1e+01]
-          Bounds range     [1e+00, 2e+00]
-          RHS range        [1e+00, 2e+00]
-        Presolve removed 4 rows and 4 columns
-        Presolve time: 0.00s
-        Presolved: 2 rows, 3 columns, 6 nonzeros
-
-        Iteration    Objective       Primal Inf.    Dual Inf.      Time
-               0    2.7994000e+01   1.002000e+00   0.000000e+00      0s
-               1    3.1000000e+01   0.000000e+00   0.000000e+00      0s
-
-        Solved in 1 iterations and 0.00 seconds (0.00 work units)
-        Optimal objective  3.100000000e+01
-
-----
-
 .. footbibliography::
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/mwis.rst` & `gurobi_optimods-0.2.0/docs/source/mods/mwis.rst`

 * *Files 18% similar despite different names*

```diff
@@ -27,44 +27,42 @@
 
 Consider an undirected graph :math:`G` with :math:`n` vertices and :math:`m`
 edges where each vertex is associated with a positive weight :math:`w`. Find a
 maximum weighted independent set, i.e., select a set of vertices in graph
 :math:`G` where there is no edge between any pair of vertices and the sum of the
 vertex weight is maximum.
 
-.. tabs::
-
-    .. tab:: Domain-Specific Description
-
-        Let :math:`G = (V, E, w)` be an undirected graph where each vertex
-        :math:`i \in V` has a positive weight :math:`w_i`. Find a
-        subset :math:`S \subseteq V` such that:
-
-        * no two vertices in :math:`S` are connected by an edge, and
-        * among all such independent sets, the set :math:`S` has the maximum total vertex weight.
-
-    .. tab:: Optimization Model
-
-        For each vertex :math:`i \in V`, define a binary decision variable
-        :math:`x_i` as below:
-
-        .. math::
-            x_i = \begin{cases}
-                1 & \text{if vertex}\,i\,\text{belongs to set}\,S\,\\
-                0 & \text{otherwise.} \\
-            \end{cases}
-
-        The binary integer programming model of the MWIS is then given below:
-
-        .. math::
-            \begin{align}
-            \max \quad        & \sum_{i \in V} w_i x_i \\
-            \mbox{s.t.} \quad & x_i + x_j \leq 1 & \forall (i, j) \in E \\
-                              & x_i \in \{0, 1\} & \forall i \in V
-            \end{align}
+Formally stated, let :math:`G = (V, E, w)` be an undirected graph where each
+vertex :math:`i \in V` has a positive weight :math:`w_i`. Find a subset :math:`S
+\subseteq V` such that:
+
+* no two vertices in :math:`S` are connected by an edge; and
+* among all such independent sets, the set :math:`S` has the maximum total
+  vertex weight.
+
+.. dropdown:: Background: Optimization Model
+
+    This mod is implemented by formulating a Binary Integer Programming (BIP)
+    model and solving it using Gurobi. For each vertex :math:`i \in V`, define a
+    binary decision variable :math:`x_i` as below:
+
+    .. math::
+        x_i = \begin{cases}
+            1 & \text{if vertex}\,i\,\text{belongs to set}\,S\,\\
+            0 & \text{otherwise.} \\
+        \end{cases}
+
+    The formulation of the MWIS is then given below:
+
+    .. math::
+        \begin{align}
+        \max \quad        & \sum_{i \in V} w_i x_i \\
+        \mbox{s.t.} \quad & x_i + x_j \leq 1 & \forall (i, j) \in E \\
+                            & x_i \in \{0, 1\} & \forall i \in V
+        \end{align}
 
 The input data for this mod includes a scipy sparse matrix in CSR format
 representing the graph :math:`G` adjacency matrix (upper triangular) and a
 numpy array representing the weights of the vertices.
 
 
 Code
@@ -91,46 +89,14 @@
 
 .. testoutput:: mwis
     :hide:
 
     ...
     Best objective 1.650000000000e+02, best bound 1.650000000000e+02, gap 0.0000%
 
-
-The model is solved as a MIP by Gurobi.
-
-.. collapse:: View Gurobi Logs
-
-    .. code-block:: text
-
-        Gurobi Optimizer version 10.0.1 build v10.0.1rc0 (mac64[arm])
-        Thread count: 8 physical cores, 8 logical processors, using up to 8 threads
-        Optimize a model with 12 rows, 8 columns and 24 nonzeros
-        Model fingerprint: 0x31a65d0e
-        Variable types: 0 continuous, 8 integer (8 binary)
-        Coefficient statistics:
-        Matrix range     [1e+00, 1e+00]
-        Objective range  [1e+00, 1e+02]
-        Bounds range     [1e+00, 1e+00]
-        RHS range        [1e+00, 1e+00]
-        Found heuristic solution: objective 165.0000000
-        Presolve removed 12 rows and 8 columns
-        Presolve time: 0.00s
-        Presolve: All rows and columns removed
-
-        Explored 0 nodes (0 simplex iterations) in 0.00 seconds (0.00 work units)
-        Thread count was 1 (of 8 available processors)
-
-        Solution count 1: 165
-
-        Optimal solution found (tolerance 1.00e-04)
-        Best objective 1.650000000000e+02, best bound 1.650000000000e+02, gap 0.0000%
-
-|
-
 Solution
 --------
 
 The solution is a numpy array containing the vertices in set :math:`S`.
 
 .. doctest:: mwis
     :options: +NORMALIZE_WHITESPACE
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/portfolio.rst` & `gurobi_optimods-0.2.0/docs/source/mods/portfolio.rst`

 * *Files 8% similar despite different names*

```diff
@@ -17,39 +17,38 @@
 This mod returns portfolios on the
 efficient frontier given expected returns and variances.
 
 
 Problem Specification
 ---------------------
 
-.. tabs::
-
-    .. tab:: Description
-
-        We consider a single-period portfolio optimization problem where want
-        to allocate wealth into :math:`n` risky assets. The returned portfolio
-        :math:`x` is an efficient mean-variance portfolio for given returns
-        :math:`\mu`, covariance matrix :math:`\Sigma` and risk aversion
-        :math:`\gamma`.
-
-
-    .. tab:: Mathematical Formulation
-
-        .. math::
-
-            \begin{alignat}{2}
-            \max \quad        & \mu^\top x - \tfrac12 \gamma\ x^\top\Sigma x \\
-            \mbox{s.t.} \quad & 1^\top x = 1 \\
-            \end{alignat}
-
-        * :math:`\mu` is the vector of expected returns.
-        * :math:`\Sigma` is the return covariance matrix.
-        * :math:`x` is the portfolio where :math:`x_i` denotes the fraction of
-          wealth invested in the risky asset :math:`i`.
-        * :math:`\gamma\geq0` is the risk aversion coefficient.
+We consider a single-period portfolio optimization problem where want
+to allocate wealth into :math:`n` risky assets. The returned portfolio
+:math:`x` is an efficient mean-variance portfolio for given returns
+:math:`\mu`, covariance matrix :math:`\Sigma` and risk aversion
+:math:`\gamma`.
+
+
+.. dropdown:: Background: Mathematical Formulation
+
+    The most basic version of this Mod is implemented by formulating a Quadratic
+    Program (QP) and solving it using Gurobi. The formulation is as follows:
+
+    .. math::
+
+        \begin{alignat}{2}
+        \max \quad        & \mu^\top x - \tfrac12 \gamma\ x^\top\Sigma x \\
+        \mbox{s.t.} \quad & 1^\top x = 1 \\
+        \end{alignat}
+
+    * :math:`\mu` is the vector of expected returns.
+    * :math:`\Sigma` is the return covariance matrix.
+    * :math:`x` is the portfolio where :math:`x_i` denotes the fraction of
+        wealth invested in the risky asset :math:`i`.
+    * :math:`\gamma\geq0` is the risk aversion coefficient.
 
 
 This description refers only to the simple base model.  Further down in
 `Enforcing more portfolio features`_ we explain how to enforce additional
 features, such as leverage or transaction fees.
 
 
@@ -118,101 +117,67 @@
 
     data = load_portfolio()
     cov_matrix = data.cov()
     mu = data.mean()
     gamma = 100.0
 
     mvp = MeanVariancePortfolio(mu, cov_matrix)
-    x = mvp.efficient_portfolio(gamma)
+    pf = mvp.efficient_portfolio(gamma)
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 82 rows, 90 columns and 190 nonzeros
+    Optimize a model with 82 rows, 91 columns and 190 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 1 rows, 10 columns, 10 nonzeros
     ...
 
-
-..  You can include the full Gurobi log output here for the curious reader.
-    It will be visible as a collapsible section.
-
-.. collapse:: View Gurobi Logs
-
-    .. code-block:: text
-
-        Gurobi Optimizer version 10.0.1 build v10.0.1rc0 (mac64[rosetta2])
-
-        CPU model: Apple M1
-        Thread count: 8 physical cores, 8 logical processors, using up to 8 threads
-
-        Optimize a model with 1 rows, 10 columns and 10 nonzeros
-        Model fingerprint: 0x7edd9de0
-        Model has 55 quadratic objective terms
-        Coefficient statistics:
-        Matrix range     [1e+00, 1e+00]
-        Objective range  [7e-04, 1e-02]
-        QObjective range [7e-06, 2e-03]
-        Bounds range     [0e+00, 0e+00]
-        RHS range        [1e+00, 1e+00]
-        Presolve time: 0.01s
-        Presolved: 1 rows, 10 columns, 10 nonzeros
-        Presolved model has 55 quadratic objective terms
-        Ordering time: 0.00s
-
-        Barrier statistics:
-        Free vars  : 9
-        AA' NZ     : 4.500e+01
-        Factor NZ  : 5.500e+01
-        Factor Ops : 3.850e+02 (less than 1 second per iteration)
-        Threads    : 1
-
-                          Objective                Residual
-        Iter       Primal          Dual         Primal    Dual     Compl     Time
-           0  -2.08348238e+05  2.08383773e+05  1.00e+04 1.43e-02  1.00e+06     0s
-           1  -1.91482256e-01  4.99463850e+02  1.08e+01 9.88e-09  1.12e+03     0s
-           2  -1.94725618e-02  4.56374984e+02  1.08e-05 9.88e-15  4.56e+01     0s
-           3  -1.94685319e-02  4.71448851e-01  8.14e-10 1.39e-17  4.91e-02     0s
-           4  -1.63767350e-02  1.14105476e-02  2.04e-11 6.94e-18  2.78e-03     0s
-           5  -7.58352892e-03  1.59186002e-04  3.89e-16 2.08e-17  7.74e-04     0s
-           6  -5.59221914e-03 -4.72740622e-03  1.67e-16 6.94e-18  8.65e-05     0s
-           7  -5.18009820e-03 -5.10195350e-03  9.30e-16 1.04e-17  7.81e-06     0s
-           8  -5.12692872e-03 -5.12414839e-03  6.11e-16 3.47e-18  2.78e-07     0s
-           9  -5.12425311e-03 -5.12424841e-03  4.84e-15 6.94e-18  4.70e-10     0s
-
-        Barrier solved model in 9 iterations and 0.00 seconds (0.00 work units)
-        Optimal objective -5.12425311e-03
-
-
 Solution
 --------
 
-The returned Series contains the relative investment for each asset;
-here the solution suggests to spread the investments over five positions
-(AA, DD, GG, HH, II).  The other allocations are negligible.
+The return value of the ``efficient_portfolio`` method is a data class instance
+containing information on the computed portfolio.  It has the following
+attributes:
+
+* ``x`` : The relative investments :math:`x` for each asset
+* ``ret`` : The estimated return :math:`\mu^T x`
+* ``risk`` : The estimated risk :math:`x^T \Sigma x`
+
+In this example the solution suggests to spread the investments over five
+positions (AA, DD, GG, HH, II).  The other allocations are negligible.
 
 .. doctest:: mod
     :options: +NORMALIZE_WHITESPACE
 
-    >>> x
+    >>> pf.x
     AA    4.236507e-01
     BB    1.743570e-07
     CC    7.573610e-10
     DD    2.430104e-01
     EE    1.017732e-07
     FF    2.760531e-09
     GG    2.937307e-02
     HH    2.350833e-01
     II    6.888222e-02
     JJ    1.248442e-08
     dtype: float64
 
+The estimated risk and return are:
+
+.. doctest:: mod
+    :options: +NORMALIZE_WHITESPACE
+
+    >>> round(pf.risk, ndigits=8)
+    0.00017552
+    >>> round(pf.ret, ndigits=8)
+    0.00365177
+
 .. _factor models:
 
 Using factor models as input
 ----------------------------
 
 In the preceding discussion we have assumed that we the covariance matrix
 :math:`\Sigma` was explicitly given.  In many cases, however, the covariance is
@@ -228,15 +193,16 @@
 is known.  Examples for this are single- or multi-factor models that divide the
 individual covariances into a general market movement, and an idiosyncratic
 risk component for each asset.  See `Efficient frontier(s) with cardinality
 constraints`_ for an example.
 
 Rather than computing the covariance matrix explcitly from the decomposition,
 it is adivised to input the individual factor matrices directly through the
-``cov_factors`` keyword argurment as in the following example:
+``cov_factors`` keyword argurment as in the following example, which mimicks a
+single-factor model:
 
 .. testcode:: mod
 
     import numpy as np
     from gurobi_optimods.portfolio import MeanVariancePortfolio
 
     mu = np.array([0.23987036, 0.24402181, 0.15069203])
@@ -245,33 +211,33 @@
     beta = np.array([[0.93797928], [1.71942161], [1.15652896]])
     # Idiosyncratic risk
     asset_risk = np.array([0.23745675, 0.19140259, 0.34325066])
 
     # Full covariance matrix according to single factor model
     Sigma = beta @ beta.T * market_variance**2 + np.diag(asset_risk**2)
     mvp_matrix = MeanVariancePortfolio(mu, cov_matrix=Sigma)
-    x_matrix = mvp_matrix.efficient_portfolio(20)
+    x_matrix = mvp_matrix.efficient_portfolio(20).x
 
     # Better use known factorization
     F1 = beta * market_variance
     F2 = np.diag(asset_risk)
     mvp_factors = MeanVariancePortfolio(mu, cov_factors=(F1, F2))
-    x_factors = mvp_factors.efficient_portfolio(20)
+    x_factors = mvp_factors.efficient_portfolio(20).x
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 26 rows, 27 columns and 57 nonzeros
+    Optimize a model with 26 rows, 28 columns and 57 nonzeros
     ...
     Model has 6 quadratic objective terms
     ...
     Presolved: 1 rows, 3 columns, 3 nonzeros
     ...
-    Optimize a model with 30 rows, 31 columns and 67 nonzeros
+    Optimize a model with 30 rows, 32 columns and 67 nonzeros
     ...
     Model has 4 quadratic objective terms
     ...
     Presolved: 2 rows, 4 columns, 6 nonzeros
     ...
 
 The two computed portfolios are the same, up to numerical noise.
@@ -311,21 +277,21 @@
     from gurobi_optimods.datasets import load_portfolio
     from gurobi_optimods.portfolio import MeanVariancePortfolio
     data = load_portfolio()
     cov_matrix = data.cov()
     mu = data.mean()
     gamma = 100.0
     mvp = MeanVariancePortfolio(mu, cov_matrix)
-    x = mvp.efficient_portfolio(gamma, max_total_short=0.3)
+    x = mvp.efficient_portfolio(gamma, max_total_short=0.3).x
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 82 rows, 90 columns and 200 nonzeros
+    Optimize a model with 82 rows, 91 columns and 200 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 62 rows, 70 columns, 160 nonzeros
     ...
 
 By incorporating leverage, we now obtain an optimal portfolio with three short
@@ -366,21 +332,21 @@
 
     data = load_portfolio()
     cov_matrix = data.cov()
     mu = data.mean()
     gamma = 100.0
 
     mvp = MeanVariancePortfolio(mu, cov_matrix)
-    x = mvp.efficient_portfolio(gamma, fees_buy=0.005)
+    x = mvp.efficient_portfolio(gamma, fees_buy=0.005).x
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 82 rows, 90 columns and 200 nonzeros
+    Optimize a model with 82 rows, 91 columns and 200 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 26 rows, 25 columns, 65 nonzeros
     ...
 
 Transaction fees can be provided either as a constant fee, applying the
@@ -423,21 +389,21 @@
 
     data = load_portfolio()
     cov_matrix = data.cov()
     mu = data.mean()
     gamma = 100.0
 
     mvp = MeanVariancePortfolio(mu, cov_matrix)
-    x = mvp.efficient_portfolio(gamma, costs_buy=0.0025)
+    x = mvp.efficient_portfolio(gamma, costs_buy=0.0025).x
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 82 rows, 90 columns and 200 nonzeros
+    Optimize a model with 82 rows, 91 columns and 200 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 1 rows, 10 columns, 10 nonzeros
     ...
 
 Transaction costs can be provided either as a constant value, applying
@@ -479,28 +445,28 @@
     from gurobi_optimods.datasets import load_portfolio
     from gurobi_optimods.portfolio import MeanVariancePortfolio
     data = load_portfolio()
     cov_matrix = data.cov()
     mu = data.mean()
     gamma = 100.0
     mvp = MeanVariancePortfolio(mu, cov_matrix)
-    x_plain = mvp.efficient_portfolio(gamma, max_total_short=0.3)
-    x_minpos = mvp.efficient_portfolio(gamma, max_total_short=0.3, min_long=0.05, min_short=0.05)
+    x_plain = mvp.efficient_portfolio(gamma, max_total_short=0.3).x
+    x_minpos = mvp.efficient_portfolio(gamma, max_total_short=0.3, min_long=0.05, min_short=0.05).x
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 82 rows, 90 columns and 200 nonzeros
+    Optimize a model with 82 rows, 91 columns and 200 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 62 rows, 70 columns, 160 nonzeros
     ...
-    Optimize a model with 102 rows, 90 columns and 240 nonzeros
+    Optimize a model with 102 rows, 91 columns and 240 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 82 rows, 70 columns, 210 nonzeros
     ...
 
 Comparing the two portfolios ``x_plain``, which has no minimum position
@@ -541,21 +507,21 @@
 
     data = load_portfolio()
     cov_matrix = data.cov()
     mu = data.mean()
     gamma = 100.0
 
     mvp = MeanVariancePortfolio(mu, cov_matrix)
-    x = mvp.efficient_portfolio(gamma, max_positions=3)
+    x = mvp.efficient_portfolio(gamma, max_positions=3).x
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 83 rows, 90 columns and 210 nonzeros
+    Optimize a model with 83 rows, 91 columns and 210 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 27 rows, 25 columns, 65 nonzeros
     ...
 
 The returned solution now suggests to trade only the assets "AA", "DD", "HH".
@@ -584,14 +550,68 @@
 that only a limited number of positions can be traded.  This can be set through
 the ``max_trades`` keyword parameter.  Without a starting portfolio (see
 `Starting portfolio & rebalancing`_) this is equivalent to limiting the number
 of positions (via ``max_positions``).  But with a starting portfolio defined,
 this parameter will limit the number of trades changing it.
 
 
+Including a risk-free asset
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+A risk-free asset can be included in the optimal choice of portfolio through
+the ``rf_return`` parameter.  Its value specifies the risk-free return rate.
+For example, here we compute an efficient portfolio under the assumption that
+the risk-free return rate is 0.25%:
+
+.. testcode:: mod
+
+    import pandas as pd
+
+    from gurobi_optimods.datasets import load_portfolio
+    from gurobi_optimods.portfolio import MeanVariancePortfolio
+
+    data = load_portfolio()
+    cov_matrix = data.cov()
+    mu = data.mean()
+    gamma = 12.5
+
+    mvp = MeanVariancePortfolio(mu, cov_matrix)
+    pf = mvp.efficient_portfolio(gamma, rf_return=0.0025)
+
+.. testoutput:: mod
+    :hide:
+
+    ...
+    Optimize a model with 82 rows, 91 columns and 191 nonzeros
+    ...
+    Model has 55 quadratic objective terms
+    ...
+    Presolved: 1 rows, 11 columns, 11 nonzeros
+    ...
+
+If a risk-free return rate has been specified, the returned
+:class:`~gurobi_optimods.portfolio.PortfolioResult` instance's ``x_rf``
+attribute tells the proportion of
+investment into the risk-free asset.  In this example the optimal portfolio
+allocates about 17% into the risk-free asset:
+
+.. testcode:: mod
+
+   print(f"risky     investment: {100*pf.x.sum():.2f}%")
+   print(f"risk-less investment: {100*pf.x_rf:.2f}%")
+
+.. testoutput:: mod
+
+   risky     investment: 83.18%
+   risk-less investment: 16.82%
+
+
+Note that the contribution of ``rf_return * pf.x_rf`` to the portfolio's expected
+value is already included in ``pf.ret``.
+
 Starting portfolio & rebalancing
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Alternatively to computing an optimal portfolio out of an all-cash position,
 one can specify a *starting portfolio*, referred to as :math:`x^0` in the
 following, via the ``initial_holdings`` keyword parameter.  In this case, an
 optimal *rebalancing* of the given portfolio is computed.
@@ -638,21 +658,21 @@
     # A random starting portfolio
     x0 = pd.Series(
         [0.06, 0.0, 0.0, 0.23, 0.37, 0.18, 0.0, 0.09, 0.07, 0.0],
         index=mu.index
     )
 
     x = mvp.efficient_portfolio(gamma, initial_holdings=x0, max_trades=2,
-        fees_buy=0.001, fees_sell=0.002)
+        fees_buy=0.001, fees_sell=0.002).x
 
 .. testoutput:: mod
     :hide:
 
     ...
-    Optimize a model with 83 rows, 90 columns and 230 nonzeros
+    Optimize a model with 83 rows, 91 columns and 230 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 37 rows, 43 columns, 125 nonzeros
     ...
 
 .. doctest:: mod
@@ -773,42 +793,39 @@
     from gurobi_optimods.portfolio import MeanVariancePortfolio
     gammas = np.logspace(-1, 1, 256)**2
     rr_pairs_unc = []
     rr_pairs_con = {1: [], 2: [], 3: []}
 
     for g in gammas:
         mvp = MeanVariancePortfolio(mu, cov_factors=(F, risk_specific))
-        # No cardinality constraints
-        x = mvp.efficient_portfolio(g, silent=True)
-        ret = mu @ x
-        risk = ((F.T @ x)**2).sum() + (x**2 * risk_specific**2).sum()
-        rr_pairs_unc.append((ret, risk))
+        # Optimal portfolio w/o cardinality constraints
+        pf = mvp.efficient_portfolio(g, verbose=False)
+        rr_pairs_unc.append((pf.risk, pf.ret))
         for max_positions in [1, 2, 3]:
-            # Some cardinality constraints
-            x = mvp.efficient_portfolio(g, max_positions=max_positions, silent=True)
-            ret = mu @ x
-            risk = ((F.T @ x)**2).sum() + (x**2 * risk_specific**2).sum()
-            rr_pairs_con[max_positions].append((ret, risk))
+            # Optimal portfolio with cardinality constraints
+            pf = mvp.efficient_portfolio(g, max_positions=max_positions, verbose=False)
+            rr_pairs_con[max_positions].append((pf.risk, pf.ret))
 
 Comparison
 ~~~~~~~~~~
 
 All risk/return pairs are now recorded in ``rr_pairs_unc`` (unconstrained
 portfolios) and ``rr_pairs_con`` (constrained portfolios). The corresponding
 efficient frontiers look like this:
 
 .. code-block:: python
 
     from matplotlib import pyplot as plt
     fig, ax = plt.subplots()
 
-    ax.scatter(list(t[1] for t in rr_pairs_unc), list(t[0] for t in rr_pairs_unc), label="unconstrained")
+    risk, ret = zip(*rr_pairs_unc)
+    ax.scatter(risk, ret, label="unconstrained")
     for k in rr_pairs_con:
-        v = rr_pairs_con[k]
-        ax.scatter(list(t[1] for t in v), list(t[0] for t in v), label=f"{k:d} asset{'' if k==1 else 's':s}")
+        risk, ret = zip(*rr_pairs_con[k])
+        ax.scatter(risk, ret, label=f"{k:d} asset{'' if k==1 else 's':s}")
         ax.legend(loc='lower right')
         plt.xlabel("risk")
         plt.ylabel("return")
 
     plt.show()
 
 .. _efficient frontiers:
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/qubo.rst` & `gurobi_optimods-0.2.0/docs/source/mods/qubo.rst`

 * *Files 23% similar despite different names*

```diff
@@ -23,64 +23,62 @@
 problems. Therefore, it is more efficient to avoid QUBO translations, if possible, and
 solve the problem as a MIP where the constraints are directly represented.
 
 
 Problem Specification
 ---------------------
 
-.. tabs::
+We are given a set :math:`I` of :math:`n` items, weights :math:`q_i \in
+\mathbb{R}` for each single item :math:`i \in I`, and weights :math:`q_{ij} \in
+\mathbb{R}` for each pair of distinct items :math:`i,j \in I,~ i \neq j`.
+
+The objective is to find a subset :math:`S^* \subseteq I` of items such that the
+sum of weights of all single items in :math:`S^*` and all pairs of distinct
+items in :math:`S^*` is minimal, i.e.,
 
-    .. tab:: Domain-Specific Description
-
-        We are given a set :math:`I` of :math:`n` items,
-        weights :math:`q_i \in \mathbb{R}`
-        for each single item :math:`i \in I`,
-        and weights :math:`q_{ij} \in \mathbb{R}` for each pair of distinct items
-        :math:`i,j \in I,~ i \neq j`.
-
-        The objective is to find a subset :math:`S^* \subseteq I` of items such that the sum of weights
-        of all single items in :math:`S^*` and all pairs of distinct items in :math:`S^*` is
-        minimal, i.e.,
-
-        .. math::
-            S^* = \arg \min_{S \subseteq I} \sum_{i \in S} q_i + \sum_{i,j \in S,~ i \neq j} q_{ij}
-
-        We arrange the weights in an upper triangular matrix :math:`Q \in \mathbb{R}^{n \times n}`
-        where entry :math:`q_{ij}` with :math:`i < j` is the weight for item pair :math:`i,j`, and
-        entry :math:`q_{ii} = q_i` is the weight for single item :math:`i`.
-
-        Note that the input matrix does not necessarily need to be in upper triangular format.
-        We accept matrices :math:`Q'` that are populated in an arbitrary way and accumulate symmetric entries,
-        i.e., :math:`q_{ij} = q'_{ij} + q'_{ji}` for all item pairs :math:`i,j` with :math:`i < j`.
-
-    .. tab:: Optimization Model
-
-        We define a binary decision vector :math:`x \in \{0,1\}^n` with variables
-
-        .. math::
-            x_i = \begin{cases}
-                1 & \text{if item}\,i \in S^*\\
-                0 & \text{otherwise.} \\
-            \end{cases}
-
-        The QUBO model is then given as:
-
-        .. math::
-            \begin{align}
-            \max \quad        & x' Q x = \sum_{i \in I} \sum_{j \in I} q_{ij} x_i x_j & \\
-            \mbox{s.t.} \quad & x \in \{0, 1\}^n &
-            \end{align}
+.. math::
+    S^* = \arg \min_{S \subseteq I} \sum_{i \in S} q_i + \sum_{i,j \in S,~ i \neq j} q_{ij}
 
-        Note that weights :math:`q_i = q_{ii}` for single items :math:`i \in I` are
-        correctly considered in the objective function since :math:`x_i x_i = x_i` holds
-        for binary variables.
+We arrange the weights in an upper triangular matrix :math:`Q \in \mathbb{R}^{n
+\times n}` where entry :math:`q_{ij}` with :math:`i < j` is the weight for item
+pair :math:`i,j`, and entry :math:`q_{ii} = q_i` is the weight for single item
+:math:`i`.
+
+Note that the input matrix does not necessarily need to be in upper triangular
+format. We accept matrices :math:`Q'` that are populated in an arbitrary way and
+accumulate symmetric entries, i.e., :math:`q_{ij} = q'_{ij} + q'_{ji}` for all
+item pairs :math:`i,j` with :math:`i < j`.
+
+.. dropdown:: Background: Optimization Model
+
+    This Mod is implemented by formulating the QUBO problem as a Binary
+    Quadratic Program (BQP). To do so, we define a binary decision vector
+    :math:`x \in \{0,1\}^n` with variables
+
+    .. math::
+        x_i = \begin{cases}
+            1 & \text{if item}\,i \in S^*\\
+            0 & \text{otherwise.} \\
+        \end{cases}
+
+    The BQP is then formulated as:
+
+    .. math::
+        \begin{align}
+        \max \quad        & x' Q x = \sum_{i \in I} \sum_{j \in I} q_{ij} x_i x_j & \\
+        \mbox{s.t.} \quad & x \in \{0, 1\}^n &
+        \end{align}
+
+    Note that weights :math:`q_i = q_{ii}` for single items :math:`i \in I` are
+    correctly considered in the objective function since :math:`x_i x_i = x_i` holds
+    for binary variables.
 
 The input data consisting of the item (pair) weights is defined as a matrix (see the
-domain-specific description), either as a NumPy array :class:`numpy.ndarray`
-or as a SciPy sparse matrix :class:`scipy.sparse`.
+description), either as a NumPy array :class:`~numpy.ndarray`
+or as a SciPy sparse matrix :class:`~scipy.sparse.spmatrix`.
 
 Code
 ----
 
 The example below solves a QUBO problem instance based on 3 items
 with single-item weights :math:`q_1 = 0,~ q_2 = -3,~ q_3 = 2`, and
 item-pair weights :math:`q_{12} = -1,~ q_{13} = -2,~ q_{23} = 3`,
@@ -113,57 +111,14 @@
 
 .. testoutput:: qubo
     :hide:
 
     ...
     New QUBO solution found with objective -4.0
 
-The model is solved as an MIQP by Gurobi.
-
-.. collapse:: View Gurobi Logs
-
-    .. code-block:: text
-
-        Gurobi 10.0.1 (linux64) logging started Fri Apr 28 17:24:54 2023
-
-        Set parameter LogFile to value "gurobi.log"
-        Gurobi Optimizer version 10.0.1 build v10.0.1rc0 (linux64)
-
-        CPU model: Intel(R) Core(TM) i7-8665U CPU @ 1.90GHz, instruction set [SSE2|AVX|AVX2]
-        Thread count: 4 physical cores, 8 logical processors, using up to 8 threads
-
-        Optimize a model with 0 rows, 3 columns and 0 nonzeros
-        Model fingerprint: 0x0d77f9fa
-        Model has 5 quadratic objective terms
-        Variable types: 0 continuous, 3 integer (3 binary)
-        Coefficient statistics:
-        Matrix range     [0e+00, 0e+00]
-        Objective range  [0e+00, 0e+00]
-        QObjective range [2e+00, 6e+00]
-        Bounds range     [1e+00, 1e+00]
-        RHS range        [0e+00, 0e+00]
-        Found heuristic solution: objective 0.0000000
-        Found heuristic solution: objective -1.0000000
-        Found heuristic solution: objective -4.0000000
-        Presolve removed 0 rows and 3 columns
-        Presolve time: 0.00s
-        Presolve: All rows and columns removed
-
-        Explored 0 nodes (0 simplex iterations) in 0.00 seconds (0.00 work units)
-        Thread count was 1 (of 8 available processors)
-
-        Solution count 3: -4 -1 0
-        No other solutions better than -4
-
-        Optimal solution found (tolerance 1.00e-04)
-        Best objective -4.000000000000e+00, best bound -4.000000000000e+00, gap 0.0000%
-
-        User-callback calls 84, time in user-callback 0.00 sec
-
-
 Solution
 --------
 
 The returned result is a data class containing the objective value and
 the solution itself as a NumPy ndarray.
 
 .. doctest:: qubo
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/workforce.rst` & `gurobi_optimods-0.2.0/docs/source/mods/workforce.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,120 +1,125 @@
 Workforce Scheduling
 ====================
 
 Workforce scheduling is an extremely widely-used application of optimization in
-practice. It involves balancing many competing concerns, including worker
-availability and preferences, shift coverage requirements, conditions on
-consecutive shifts or rest breaks, and so on. Implementation can become quite
+practice. It involves balancing many competing concerns such as worker
+availability, cost, and preferences; shift coverage requirements; conditions on
+consecutive shifts or rest breaks; and so on. Implementation can become quite
 involved as worker requirements and entitlements become more complex.
 
-This mod implements a relatively simple case. Workers provide their availability
-and preferences, while rest requirements and work entitlements are handled
-through lower and upper limits on the number of shifts a worker is rostered on
-for in a given period. The scheduler aims to maximize satisfaction by finding a
-feasible roster which maximizes the sum of preference scores.
+This Mod implements several basic variants of workforce scheduling. The initial
+example is deliberately simple, while later sections progressively add more
+complexity and enforce additional requirements on the generated schedule. If the
+initial example appears too simple for your use-case, please, read on!
 
 Problem Specification
 ---------------------
 
-Consider a service business, such as a restaurant, that develops its roster for
-a two week period. The service requires only one set of skills. There are a
-number of employed workers with the same set of skills and with identical
-productivity that are available to work on some of the days during the two-week
-planning horizon. There is only one shift per workday, however each shift may
-require a different number of workers. The business requests preferences from
-all workers for shifts they are available for, and aims to maximize the sum of
-preference scores of assigned shifts as a proxy for worker happiness.
+This first example covers a simple case for a business developing a two-week
+roster. Each shift requires a given number of workers who have identical skills
+and productivity. In other words, any work can cover any shift, and all workers
+are considered equivalent. Workers provide their availability for shifts, and
+rest requirements and minimum work entitlements are handled through upper and
+lower limits, respectively, on the number of shifts a worker is rostered on for
+in the schedule. Optionally, preferences can be provided, in which case the
+scheduler aims to maximize satisfaction by finding a feasible roster which
+maximizes the sum of preference scores of the assigned shifts.
+
+The workforce scheduling Mod takes the following three dataframes as input:
+
+* The ``availability`` dataframe has two columns: ``Worker`` and
+  ``Shift``. Each row in dataframe specifies that the given worker is
+  available to work the given shift. If the optional ``preferences`` argument
+  is provided, it must refer to an additional column in the ``availability``
+  dataframe containing preferences.
+* The ``shift_requirements`` dataframe has two columns: ``Shift`` and
+  ``Required``. Each row specifies the number of workers required for a given
+  shift. There must be one row for every unique shift in
+  ``availability["Shift"]``.
+* The ``worker_limits`` dataframe has three columns: ``Worker``,
+  ``MinShifts``, and ``MaxShifts``. Each row specifies the minimum and maximum
+  number of shifts the given worker may be assigned in the schedule. There
+  must be one row for every unique worker in ``availability["Worker"]``.
+
+When ``solve_workforce_scheduling`` is called, a model is formulated and solved
+immediately using Gurobi. Workers will be assigned only to shifts they are
+available for, in such a way that all requirements are covered, minimum and
+maximum shift numbers are respected, and the total sum of worker preference
+scores is maximised. If ``preferences=None``, preferences are omitted and any
+feasible schedule will be returned.
+
+The returned assignment dataframe is a subset of the availability dataframe,
+with the same columns. A row in the returned dataframe specifies that the given
+worker has been assigned to the given shift.
+
+.. dropdown:: Background: Mathematical Model
+
+    The set of shifts :math:`S` is to be covered using the set of workers
+    :math:`W`. Workers :math:`w \in W_{s} \subseteq W` are available to work
+    a given shift `s`, and have a preference :math:`p_{ws}` for each
+    assigned shift. Shift :math:`s` requires :math:`r_{s}` workers assigned.
+    Each worker must be assigned between :math:`l_{w}` and :math:`u_{w}`
+    shifts in total. The model is defined on binary variables :math:`x_{ws}`
+    which satisfy the condition
+
+    .. math::
+
+        x_{ws} = \begin{cases}
+            1 & \text{if worker w is given shift s} \\
+            0 & \text{otherwise.} \\
+        \end{cases}
+
+    The mathematical model is then expressed as:
+
+    .. math::
+
+        \begin{alignat}{2}
+        \max \quad        & \sum_{s \in S} \sum_{w \in W_{s}} p_{ws} x_{ws} \\
+        \mbox{s.t.} \quad & \sum_{w \in W_{s}} x_{ws} = r_{s} & \forall s \in S \\
+                            & l_{w} \le \sum_{s \in S} x_{ws} \le u_{w} & \forall w \in W \\
+                            & x_{ws} \in \lbrace 0, 1 \rbrace & \forall s \in S, w \in W_{s} \\
+        \end{alignat}
+
+    The objective computes the total cost of all shift assignments based on
+    worker pay rates. The first constraint ensures that all shifts are
+    assigned the required number of workers, while the second constraint
+    ensures workers are assigned to an acceptable number of shifts.
 
-.. tabs::
-
-    .. tab:: Data Specification
-
-        The workforce scheduling model takes the following three dataframes as
-        input:
-
-        * The ``preferences`` dataframe has three columns: ``Worker``, ``Shift``,
-          and ``Preference``. Each row in dataframe specifies that the given worker
-          is available to work the given shift.
-        * The ``shift_requirements`` dataframe has two columns: ``Shift`` and
-          ``Required``. Each row specifies the number of workers required for a
-          given shift. There must be one row for every unique shift in
-          ``preferences["Shift"]``.
-        * The ``worker_limits`` dataframe has three columns: ``Worker``,
-          ``MinShifts``, and ``MaxShifts``. Each row specifies the minimum and
-          maximum number of shifts the given worker may be assigned in the
-          schedule. There must be one row for every unique worker in
-          ``preferences["Worker"]``.
-
-        When ``solve_workforce_scheduling`` is called, a model is formulated and
-        solved immediately using Gurobi. Workers will be assigned only to shifts
-        they are available for, in such a way that all requirements are covered,
-        minimum and maximum shift numbers are respected, and the total sum of
-        worker preference scores is maximised.
-
-        The returned assignment dataframe is a subset of the preferences
-        dataframe, with the same columns. A row in the returned dataframe
-        specifies that the given worker has been assigned to the given shift.
-
-    .. tab:: Optimization Model
-
-        The set of shifts :math:`S` is to be covered using the set of workers
-        :math:`W`. Workers :math:`w \in W_{s} \subseteq W` are available to work
-        a given shift `s`, and have a preference :math:`p_{ws}` for each
-        assigned shift. Shift :math:`s` requires :math:`r_{s}` workers assigned.
-        Each worker must be assigned between :math:`l_{w}` and :math:`u_{w}`
-        shifts in total. The model is defined on binary variables :math:`x_{ws}`
-        which satisfy the condition
-
-        .. math::
-
-            x_{ws} = \begin{cases}
-                1 & \text{if worker w is given shift s} \\
-                0 & \text{otherwise.} \\
-            \end{cases}
-
-        The mathematical model is then expressed as:
-
-        .. math::
-
-            \begin{alignat}{2}
-            \max \quad        & \sum_{s \in S} \sum_{w \in W_{s}} p_{ws} x_{ws} \\
-            \mbox{s.t.} \quad & \sum_{w \in W_{s}} x_{ws} = r_{s} & \forall s \in S \\
-                              & l_{w} \le \sum_{s \in S} x_{ws} \le u_{w} & \forall w \in W \\
-                              & x_{ws} \in \lbrace 0, 1 \rbrace & \forall s \in S, w \in W_{s} \\
-            \end{alignat}
-
-        The objective computes the total cost of all shift assignments based on
-        worker pay rates. The first constraint ensures that all shifts are
-        assigned the required number of workers, while the second constraint
-        ensures workers are assigned to an acceptable number of shifts.
+A Simple Example
+----------------
 
-All input data is given as pandas dataframes, following the layout described in
-the Data Specification above. The tabs below show example data for each frame.
+This section shows the simplest possible input dataset for the Mod, comprising
+seven workers covering daily shifts over a two week period, each with defined
+availability. All input data is given as pandas dataframes, following the layout
+described in the :ref:`mods/workforce:problem specification` above. The tabs
+below show example data for each frame.
 
 .. testsetup:: workforce
 
     # Set pandas options
     import pandas as pd
     pd.options.display.max_rows = 10
 
 .. tabs::
 
-    .. tab:: ``preferences``
+    .. tab:: ``availability``
 
         The following example table lists worker availability and preferences.
         For example, Siva is available on July 2nd, 3rd, 5th, and so on, with a
-        stronger preference to be assigned the shift on the 5th.
+        stronger preference to be assigned the shift on the 5th. To use the
+        preference data, the optional argument ``preferences="Preference"`` must
+        be supplied.
 
         .. doctest:: workforce
             :options: +NORMALIZE_WHITESPACE
 
             >>> from gurobi_optimods import datasets
             >>> data = datasets.load_workforce()
-            >>> data.preferences
+            >>> data.availability
                  Worker      Shift  Preference
             0      Siva 2023-05-02         2.0
             1      Siva 2023-05-03         2.0
             2      Siva 2023-05-05         5.0
             3      Siva 2023-05-07         3.0
             4      Siva 2023-05-09         2.0
             ..      ...        ...         ...
@@ -177,90 +182,47 @@
             4  Vincent          6          8
             5   Marisa          5          8
             6  Pauline          6          8
 
         In the mathematical model, this table provides the values :math:`l_w`
         and :math:`u_w`.
 
-Solving a Model
----------------
-
-The example code below solves the workforce scheduling problem for a simple
-example dataset comprising seven workers covering daily shifts over a two week
-period.
+The example code below solves the workforce scheduling problem for the above
+dataset. The dataset can be imported directly in the environment where
+``gurobi-optimods`` is installed.
 
 .. testcode:: workforce
 
     from gurobi_optimods.datasets import load_workforce
     from gurobi_optimods.workforce import solve_workforce_scheduling
 
     # Load example data
     data = load_workforce()
 
     # Solve the mod, get back a schedule
     assigned_shifts = solve_workforce_scheduling(
-        preferences=data.preferences,
+        availability=data.availability,
         shift_requirements=data.shift_requirements,
         worker_limits=data.worker_limits,
+        preferences="Preference",
     )
 
 .. testoutput:: workforce
     :hide:
 
     ...
     Optimize a model with 28 rows, 72 columns and 216 nonzeros
     ...
     Best objective 1.850000000000e+02, best bound 1.850000000000e+02, gap 0.0000%
 
-.. collapse:: View Gurobi logs for solving this example
-
-    .. code-block:: text
-
-        Gurobi Optimizer version 10.0.1 build v10.0.1rc0 (mac64[x86])
-
-        CPU model: Intel(R) Core(TM) i5-1038NG7 CPU @ 2.00GHz
-        Thread count: 4 physical cores, 8 logical processors, using up to 8 threads
-
-        Optimize a model with 28 rows, 72 columns and 216 nonzeros
-        Model fingerprint: 0x595b329f
-        Variable types: 0 continuous, 72 integer (72 binary)
-        Coefficient statistics:
-          Matrix range     [1e+00, 1e+00]
-          Objective range  [1e+00, 5e+00]
-          Bounds range     [1e+00, 1e+00]
-          RHS range        [2e+00, 8e+00]
-        Found heuristic solution: objective 170.0000000
-        Presolve removed 6 rows and 22 columns
-        Presolve time: 0.00s
-        Presolved: 22 rows, 50 columns, 145 nonzeros
-        Variable types: 0 continuous, 50 integer (50 binary)
-        Found heuristic solution: objective 177.0000000
-
-        Root relaxation: objective 1.850000e+02, 24 iterations, 0.00 seconds (0.00 work units)
-
-            Nodes    |    Current Node    |     Objective Bounds      |     Work
-         Expl Unexpl |  Obj  Depth IntInf | Incumbent    BestBd   Gap | It/Node Time
-
-        *    0     0               0     185.0000000  185.00000  0.00%     -    0s
-
-        Explored 1 nodes (24 simplex iterations) in 0.00 seconds (0.00 work units)
-        Thread count was 8 (of 8 available processors)
-
-        Solution count 3: 185 177 170
-
-        Optimal solution found (tolerance 1.00e-04)
-        Best objective 1.850000000000e+02, best bound 1.850000000000e+02, gap 0.0000%
-
-|
-
 Inspecting the Solution
 -----------------------
 
 The solution to this workforce scheduling problem is a selection of shift
-assignments. The returned dataframe is a subset of the original preferences
+assignments. The returned dataframe is a subset of the original availability
 dataframe.
 
 .. doctest:: workforce
     :options: +NORMALIZE_WHITESPACE
 
     >>> assigned_shifts
           Worker      Shift  Preference
@@ -351,19 +313,20 @@
 required. When solving this variant of the problem, ``rolling_limits`` must be
 set to ``True`` to enforce the new requirement.
 
 .. doctest:: workforce
     :options: +NORMALIZE_WHITESPACE +ELLIPSIS
 
     >>> assigned_shifts = solve_workforce_scheduling(
-    ...     preferences=data.preferences,
+    ...     availability=data.availability,
     ...     shift_requirements=data.shift_requirements,
     ...     worker_limits=worker_limits,
+    ...     preferences="Preference",
     ...     rolling_limits=True,
-    ...     silent=True,
+    ...     verbose=False,
     ... )
     >>> shifts_table = pd.pivot_table(
     ...     assigned_shifts.assign(value=1),
     ...     values="value",
     ...     index="Shift",
     ...     columns="Worker",
     ...     fill_value="-",
@@ -385,7 +348,18 @@
     2023-05-11     Y      -       -       Y    -       Y       Y
     2023-05-12     Y      Y       Y       Y    Y       -       -
     2023-05-13     Y      Y       Y       Y    Y       Y       Y
     2023-05-14     -      Y       Y       Y    Y       Y       -
 
 Notice that Siva's shifts have been adjusted so as to avoid any worker working
 more than 5 consecutive days.
+
+Further Requirements
+--------------------
+
+As mentioned in the introduction, this Mod implements some basic cases of
+workforce scheduling, and is limited in scope. However, similar modelling
+approaches to those described here can be applied to handle more complex
+requirements. For further information, see :footcite:t:`ERNST20043` (among many,
+many other references on the topic).
+
+.. footbibliography::
```

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-example.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-example.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-figs.py` & `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-figs.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-flow.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-flow.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/bipartite-matching-result.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/lad-outlier-coeffs.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/lad-outlier-errors.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-errors.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/lad-regression-coeffs.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/lad-regression-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/min-cost-flow-result.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/min-cost-flow-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/mvp.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/mvp.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/mwis.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/mwis.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/pie.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/pie.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/qubo.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/qubo.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/figures/shortest-path-result.png` & `gurobi_optimods-0.2.0/docs/source/mods/figures/shortest-path-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/mods/icons/lad-regression.png` & `gurobi_optimods-0.2.0/docs/source/mods/icons/lad-regression.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/refs/graphs.bib` & `gurobi_optimods-0.2.0/docs/source/refs/graphs.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/docs/source/refs/qubo.bib` & `gurobi_optimods-0.2.0/docs/source/refs/qubo.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/bipartite_matching.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/bipartite_matching.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Bipartite Matching
 ------------------
 """
 
 
 import logging
-from typing import List, Optional, overload
+from typing import List, overload
 
+import gurobipy as gp
+import gurobipy_pandas as gppd
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
-
-import gurobipy as gp
 from gurobipy import GRB
-import gurobipy_pandas as gppd
 
 try:
     import networkx as nx
 except ImportError:
     nx = None
 
 from gurobi_optimods.utils import optimod
@@ -26,62 +25,62 @@
 
 
 @overload
 def maximum_bipartite_matching(
     graph: sp.spmatrix,
     nodes1: np.ndarray,
     nodes2: np.ndarray,
-    silent: bool = False,
-    logfile: Optional[str] = None,
 ) -> sp.spmatrix:
     ...
 
 
 @overload
 def maximum_bipartite_matching(
     graph: pd.DataFrame,
     nodes1: str,
     nodes2: str,
-    silent: bool = False,
-    logfile: Optional[str] = None,
 ) -> pd.DataFrame:
     ...
 
 
 if nx is not None:
 
     @overload
     def maximum_bipartite_matching(
         graph: nx.Graph,
         nodes1: List,
         nodes2: List,
-        silent: bool = False,
-        logfile: Optional[str] = None,
     ) -> nx.Graph:
         ...
 
 
 @optimod()
 def maximum_bipartite_matching(graph, nodes1, nodes2, *, create_env):
     """Solve a maximum cardinality bipartite matching problem on the
     given graph.
 
-    :param graph: A graph, specified either as a scipy.sparse adjacency matrix, networkx
-        graph, or pandas dataframe
-    :type graph: :class:`sp.sparray|nx.Graph|pd.DataFrame`
-    :param nodes1: Nodes in the first bipartite set. If ``graph`` is a pandas dataframe,
-        nodes1 must be a column name. Otherwise, it is a numpy array of nodes in the first
-        bipartite set.
-    :type nodes1: :class:`np.array|List|str`
-    :param nodes2: Nodes in the second bipartite set. If ``graph`` is a pandas dataframe,
-        nodes2 must be a column name. Otherwise, it is a numpy array of nodes in the second
-        bipartite set.
-    :type nodes2: :class:`np.array|List|str`
-    :return: A subgraph of the original graph specifying the maximum matching
-    :rtype: :class:`sp.sparray|nx.Graph|pd.DataFrame`
+    Parameters
+    ----------
+    graph : spmatrix or Graph or DataFrame
+        A graph, specified either as a scipy.sparse adjacency matrix, networkx
+        graph, or pandas dataframe.
+    nodes1 : ndarray or str
+        Nodes in the first bipartite set. If ``graph`` is a pandas dataframe,
+        nodes1 must be a column name. Otherwise, it is a numpy array of nodes in
+        the first bipartite set.
+    nodes2 : ndarray or str
+        Nodes in the second bipartite set. If ``graph`` is a pandas dataframe,
+        nodes2 must be a column name. Otherwise, it is a numpy array of nodes in
+        the second bipartite set.
+
+    Returns
+    -------
+    DataFrame or Graph
+        A subgraph of the original ``graph`` (with the same data type) specifying
+        the maximum matching
     """
     if isinstance(graph, sp.spmatrix):
         return _maximum_bipartite_matching_scipy(graph, nodes1, nodes2, create_env)
     elif isinstance(graph, pd.DataFrame):
         return _maximum_bipartite_matching_pandas(graph, nodes1, nodes2, create_env)
     elif nx is not None and isinstance(graph, nx.Graph):
         return _maximum_bipartite_matching_networkx(graph, nodes1, nodes2, create_env)
@@ -90,57 +89,40 @@
 
 
 def _maximum_bipartite_matching_pandas(frame, n1_column, n2_column, create_env):
     """This implementation uses gurobipy-pandas, which suits the input data
     already in a pandas dataframe."""
 
     with create_env() as env, gp.Model(env=env) as model:
-        df = (
-            pd.concat(
-                [
-                    frame.assign(_original_edge=True),
-                    pd.DataFrame(
-                        {
-                            n1_column: "source",
-                            n2_column: frame[n1_column].unique(),
-                            "_original_edge": False,
-                        }
-                    ),
-                    pd.DataFrame(
-                        {
-                            n1_column: frame[n2_column].unique(),
-                            n2_column: "sink",
-                            "_original_edge": False,
-                        }
-                    ),
-                ]
-            )
-            .set_index([n1_column, n2_column])
-            .gppd.add_vars(model, ub=1, name="flow")
-        )
-        df.loc[("sink", "source"), "flow"] = model.addVar(
-            obj=1, name="flow[sink,source]"
+        # Directed flow variables between bipartite sets
+        df = frame.set_index([n1_column, n2_column]).gppd.add_vars(
+            model, ub=1, name="flow"
         )
-        df.loc[("sink", "source"), "_original_edge"] = False
-        model.ModelSense = GRB.MAXIMIZE
 
-        gppd.add_constrs(
-            model,
-            df["flow"].groupby(n1_column).sum(),
-            GRB.EQUAL,
-            df["flow"].groupby(n2_column).sum(),
-            name="balance",
-        )
-        model.optimize()
+        # Inflow variables and flow balance on n1
+        n1_outflows = df["flow"].groupby(n1_column).sum()
+        n1_inflows = gppd.add_vars(model, n1_outflows.index, ub=1, name="src_flow")
+        gppd.add_constrs(model, n1_inflows, GRB.EQUAL, n1_outflows, name="n1_balance")
+
+        # Outflow variables and flow balance on n2
+        n2_inflows = df["flow"].groupby(n2_column).sum()
+        n2_outflows = gppd.add_vars(model, n2_inflows.index, ub=1, name="sink_flow")
+        gppd.add_constrs(model, n2_inflows, GRB.EQUAL, n2_outflows, name="n2_balance")
+
+        # sink-source flow variable and flow balances
+        sink_source_flow = model.addVar(name="sink_source_flow")
+        model.addConstr(sink_source_flow == n1_inflows.sum(), name="src_balance")
+        model.addConstr(n2_outflows.sum() == sink_source_flow, name="sink_balance")
 
-        return (
-            df[df["flow"].gppd.X.gt(0.1) & df._original_edge]
-            .drop(columns=["flow", "_original_edge"])
-            .reset_index()
-        )
+        # max flow
+        model.setObjective(sink_source_flow, sense=GRB.MAXIMIZE)
+
+        # solve and extract solution
+        model.optimize()
+        return df.loc[df["flow"].gppd.X.gt(0.1)].reset_index().drop(columns=["flow"])
 
 
 def _maximum_bipartite_matching_networkx(graph, nodes1, nodes2, create_env):
     """This implementation uses gurobipy's term-based API, which suits the
     iterator-based API for reading data from networkx graphs."""
 
     logger.info(
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/datasets.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
 
 def load_workforce():
     return AttrDict(
-        preferences=pd.read_csv(
+        availability=pd.read_csv(
             DATA_FILE_DIR / "workforce/preferences.csv", parse_dates=["Shift"]
         ),
         shift_requirements=pd.read_csv(
             DATA_FILE_DIR / "workforce/shift_requirements.csv", parse_dates=["Shift"]
         ),
         worker_limits=pd.read_csv(
             DATA_FILE_DIR / "workforce/worker_limits.csv",
@@ -86,22 +86,14 @@
 
 
 def load_graph2_scipy():
     edge_data, node_data = load_graph2()
     return _convert_pandas_to_scipy(edge_data, node_data)
 
 
-def load_diet():
-    return AttrDict(
-        categories=pd.read_csv(DATA_FILE_DIR / "diet/diet-categories.csv"),
-        foods=pd.read_csv(DATA_FILE_DIR / "diet/diet-foods.csv"),
-        nutrition_values=pd.read_csv(DATA_FILE_DIR / "diet/diet-values.csv"),
-    )
-
-
 def load_portfolio():
     fn = DATA_FILE_DIR / "portfolio/portfolio.csv"
     return pd.read_csv(fn, index_col=0)
 
 
 def _convert_pandas_to_digraph(
     edge_data, node_data, capacity=True, cost=True, demand=True
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/mwis.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/mwis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """
 Maximum Weighted Independent Set
 --------------------------------
 """
 
-import numpy as np
-
 import gurobipy as gp
+import numpy as np
 from gurobipy import GRB
 
 from gurobi_optimods.utils import optimod
 
 
 @optimod()
 def maximum_weighted_independent_set(adjacency_matrix, weights, *, create_env):
     """Find a set of mutually non-adjacent vertices with maximum weighted sum.
 
-    :param adjacency_matrix: The upper triangular adjacency matrix.
-    :type adjacency_matrix: :class:`sp.sparray`
-    :param weights: Vertex weight array.
-    :type weights: :class:`np.array`
-    :return: The maximum weighted independent set array.
-    :rtype: :class:`np.array`
+    Parameters
+    ----------
+    adjacency_matrix : spmatrix
+        The upper triangular adjacency matrix.
+    weights : ndarray
+        Vertex weight array.
+
+    Returns
+    -------
+    ndarray
+        The maximum weighted independent set array.
     """
     with create_env() as env, gp.Model("mwis", env=env) as model:
         # x_i: 1 if vertex i is in the independent set and 0 otherwise
         x = model.addMVar(len(weights), vtype=GRB.BINARY, name="x")
         # Maximize the sum of the vertex weights in the independent set
         model.setObjective(weights @ x, sense=GRB.MAXIMIZE)
         # The independent set contains non-adjacent vertices
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/portfolio.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/portfolio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 """
 Mean-Variance Portfolio
 -----------------------
 """
 
+from dataclasses import dataclass
+from typing import Optional
+
 import gurobipy as gp
-from gurobipy import GRB
 import numpy as np
 import pandas as pd
+from gurobipy import GRB
 
 from gurobi_optimods.utils import optimod
 
 
 class MeanVariancePortfolio:
     """Optimal mean-variance portfolio solver.
 
     Instantiate an object of :class:`MeanVariancePortfolio` for given
     covariance matrix and return vector.  Use
     :meth:`MeanVariancePortfolio.efficient_portfolio` to solve for efficient
     portfolios with given parameters.
 
-    :param mu: Return vector
-    :type mu: 1-d :class:`np.ndarray`
-    :param cov_matrix: Covariance matrix :math:`\Sigma`
-    :type cov_matrix: 2-d :class:`np.ndarray`
-    :param cov_factors: Covariance factors that constitute :math:`\Sigma`,
-        see :ref:`factor models`
-    :type cov_factors: 2-d :class:`tuple` of :class:`np.ndarray`
+    Parameters
+    ----------
+    mu : 1-d ndarray
+        Vector of expected returns for each asset
+    cov_matrix : 2-d ndarray
+        Covariance matrix :math:`\Sigma`
+    cov_factors : tuple of ndarray
+        Covariance factors that constitute :math:`\Sigma`. Typically each
+        element ``F`` of ``cov_matrix`` will either be a
+
+            * n-by-k dense matrix, or a
+            * n-by-n diagonal matrix.
+
+        Each element ``F`` of ``cov_factors`` contributes the term ``F @ F.T``
+        to :math:`\Sigma`; see also :ref:`factor models`
 
     """
 
     def __init__(
         self,
         mu,
         cov_matrix=None,
@@ -73,57 +84,79 @@
         fees_sell=None,
         costs_buy=None,
         costs_sell=None,
         min_long=None,
         min_short=None,
         max_total_short=0.0,
         initial_holdings=None,
+        rf_return=None,
         *,
         create_env,
     ):
-        """
-        Compute efficient portfolio for given paramters
+        """Compute efficient portfolio for given parameters
 
-        :param gamma: Risk aversion cofficient for balancing risk and return;
-            the resulting objective functions is
-            :math:`\mu^T x - 0.5 \gamma x^T \Sigma x`
-        :type gamma: :class:`float` >= 0
-        :param max_trades: Upper limit on the number of trades
-        :type max_trades: :class:`int` >= 0
-        :param max_positions: Upper limit on the number of open positions
-        :type max_positions: :class:`int` >= 0
-        :param fees_buy: Fixed-charge fee for each buy transaction, relative
-            to total portfolio value
-        :type fees_buy: :class:`float` or :class:`np.ndarray` >= 0
-        :param fees_sell: Fixed-charge fee for each sell transaction, relative
-            to total portfolio value
-        :type fees_buy: :class:`float` or :class:`np.ndarray` >= 0
-        :param costs_buy: Variable transaction costs for each buy transaction, relative
-            to trade value
-        :type fees_buy: :class:`float` or :class:`np.ndarray` >= 0
-        :param costs_sell: Variable transaction costs for each sell transaction, relative
-            to trade value
-        :type fees_buy: :class:`float` or :class:`np.ndarray` >= 0
-        :param min_long: Lower bound on the volume on a traded long position,
-            relative to total portfolio value
-        :type min_long: :class:`float` >= 0
-        :param min_short: Lower bound on the volume on a traded short position,
-            relative to total portfolio value
-        :type min_long: :class:`float` >= 0
-        :param max_total_short: Maximum total short positions, relative to
-            total investment.
-        :type max_total_short: :class:`float` >= 0
-        :param max_total_short: Maximum total short positions, relative to
-            total investment.
-        :type max_total_short: :class:`float` >= 0
-        :param initial_holdings: Initial portfolio holdings (sum needs to be <= 1)
-        :type initial_holdings: 1-d :class:`np.ndarray`
+        Parameters
+        ----------
 
-        Refer to :ref:`portfolio features` for a detailed discussion of these
+        gamma : float >= 0
+            Risk aversion cofficient for balancing risk and return; the
+            resulting objective functions is
+            :math:`\mu^T x - 0.5 \gamma x^T \Sigma x`
+        max_trades : int >= 0, optional
+            Upper limit on the number of trades
+        max_positions : int >= 0, optional
+            Upper limit on the number of open positions
+        fees_buy : float or ndarray >= 0, optional
+            Fixed-charge fee for each buy transaction, relative to total
+            portfolio value
+        fees_sell : float or ndarray >= 0, optional
+            Fixed-charge fee for each sell transaction, relative to total
+            portfolio value
+        costs_buy : float or ndarray >= 0, optional
+            Variable transaction costs for each buy transaction, relative to
+            trade value
+        costs_sell : float or ndarray >= 0, optional
+            Variable transaction costs for each sell transaction, relative to
+            trade value
+        min_long : float >= 0, optional
+            Lower bound on the volume on a traded long position, relative to
+            total portfolio value
+        min_short : float >= 0, optional
+            Lower bound on the volume on a traded short position, relative to
+            total portfolio value
+        max_total_short : float >= 0, optional
+            Maximum total short positions, relative to total investment.
+        initial_holdings : 1-d ndarray, optional
+            Initial portfolio holdings (sum needs to be <= 1)
+        rf_return : float, optional
+            Include a risk-free asset having return rate ``rf_return``.
+
+        Returns
+        -------
+        mvp_result : PortfolioResult
+            A dataclass containing the efficient portfolio, along with auxiliary
+            information:
+
+            * ``mvp_result.x``: The portfolio vector :math:`x`
+            * ``mvp_result.risk``: The estimated risk :math:`x^T \Sigma x`
+              of the portfolio
+            * ``mvp_result.return``: The estimated return :math:`\mu^T x` of
+              the portfolio
+            * ``mvp.x_rf`` relative investment in the risk-free asset.
+              Present only if ``rf_return`` was non-None on input
+
+            Some combinations of requested portfolio features may rule out
+            **all** possible portfolios.  In this corner case the value
+            ``None`` is returned.
+
+        Notes
+        -----
+        Refer to :ref:`portfolio features` for a detailed discussion of all
         parameters.
+
         """
 
         fees_buy = self._homogenize_input(fees_buy)
         fees_sell = self._homogenize_input(fees_sell)
         costs_buy = self._homogenize_input(costs_buy)
         costs_sell = self._homogenize_input(costs_sell)
         initial_holdings = self._homogenize_input(initial_holdings)
@@ -131,96 +164,73 @@
         if initial_holdings is not None:
             if initial_holdings.sum() > 1.0:
                 raise ValueError("Initial holding's sum must not exceed 1.0")
         else:
             initial_holdings = np.zeros(self.mu.shape)
 
         with create_env() as env, gp.Model("efficient_portfolio", env=env) as m:
-            x = self._populate_model(
+            x, x_rf = self._populate_model(
                 m,
                 gamma,
                 max_trades,
                 max_positions,
                 fees_buy,
                 fees_sell,
                 costs_buy,
                 costs_sell,
                 min_long,
                 min_short,
                 max_total_short,
                 initial_holdings,
+                rf_return,
             )
 
             m.optimize()
             status = m.Status
             if status == GRB.OPTIMAL:
-                xvals = x.X
+                x_vals = x.X
+                x_rf_val = x_rf.X
 
         if status == GRB.OPTIMAL:
-            return self._convert_result(xvals)
+            return self._construct_result(x_vals, x_rf_val, rf_return)
         elif status in [GRB.INFEASIBLE, GRB.INF_OR_UNBD]:
             print("No portfolio satisfies the constraints!")
             return None
         else:
             return None
 
-    # Just boilerplate, waiting to be filled with life
-    def _minimize_risk(self, expected_return):
-        with gp.Env() as env, gp.Model("min_risk", env=env) as m:
-            x = m.addMVar(shape=self.mu.shape, name="x")
-
-            m.addConstr(x.sum() == 1, name="fully_invested")
-            m.addConstr(self.mu @ x >= expected_return, name="expected_return")
-            m.setObjective(x @ self.covariance @ x)
-
-            m.optimize()
-
-            if m.Status == GRB.OPTIMAL:
-                return self._convert_result(x.X)
-
-    # Just boilerplate, waiting to be filled with life
-    def _maximize_return(self, max_risk):
-        with gp.Env() as env, gp.Model("max_return", env=env) as m:
-            x = m.addMVar(shape=self.mu.shape, name="x")
-            m.addConstr(x.sum() == 1, name="fully_invested")
-            m.addConstr(x @ self.covariance @ x <= max_risk, name="max_risk")
-            m.setObjective(self.mu @ x, GRB.MAXIMIZE)
-
-            m.optimize()
-
-            if m.Status == GRB.OPTIMAL:
-                return self._convert_result(x.X)
-
     def _populate_model(
         self,
         m,
         gamma,
         max_trades,
         max_positions,
         fees_buy,
         fees_sell,
         costs_buy,
         costs_sell,
         min_long,
         min_short,
         max_total_short,
         initial_holdings,
+        rf_return,
     ):
-        # max x' * mu - gamma * x' * cov_matrix * x
+        # max rf_return * x_rf + x' * mu - gamma * x' * cov_matrix * x
         # s.t.
         #      x = x_long - x_short  (x is split in positive/negative parts)
         #
         #      x_long = initial_holdings_long + x_long_buy - x_long_sell
         #      x_short == initial_holdings_short - x_short_buy + x_short_sell
         #      x - initial_holdings == x_buy - x_sell
         #
         #      sum(x)   + sum(b_buy) * fees_buy
         #               + sum(b_sell) * fees_sell
         #               + sum(x_buy) * costs_buy
         #               + sum(x_sell) * costs_sell
+        #               + x_rf
         #      = 1
         #                             (fully invested, minus transaction costs and fees)
         #
         #      x_long  <= M b_long    (force x_long to zero if not traded long)
         #                             (M >= 1 + max_total_short)
         #
         #      b_short + b_long <= 1  (cannot go long and short at the same time)
@@ -247,25 +257,30 @@
 
         # Portfolio vector x is split into long and short positions
         x = m.addMVar(shape=self.mu.shape, lb=-float("inf"), name="x")
         x_long = m.addMVar(shape=self.mu.shape, name="x_long")
         x_short = m.addMVar(shape=self.mu.shape, name="x_short")
         m.addConstr(x == x_long - x_short)
 
+        # Dummy variable for investment in risk-free asset,
+        x_rf = m.addVar(lb=0.0, ub=0.0, name="x_rf")
+
         x_buy = m.addMVar(shape=self.mu.shape, name="x_buy")
         x_sell = m.addMVar(shape=self.mu.shape, name="x_sell")
         m.addConstr(x - initial_holdings == x_buy - x_sell)
 
         # Binaries used to enforce VUB and minimum position/trade size
         b_long = m.addMVar(shape=self.mu.shape, vtype="B", name="position_long")
         b_short = m.addMVar(shape=self.mu.shape, vtype="B", name="position_short")
 
         b_buy = m.addMVar(shape=self.mu.shape, vtype="B", name="trade_buy")
         b_sell = m.addMVar(shape=self.mu.shape, vtype="B", name="trade_sell")
 
+        m.update()
+
         # Define VUB constraints for x_long and x_short.
         #
         # Going short by alpha means that each long position is upper
         # bounded by 1 + alpha, and each short position by alpha.
         # This is implied by the sum(x) == 1 constraint.
         m.addConstr(x_long <= (1.0 + max_total_short) * b_long)
         m.addConstr(x_short <= max_total_short * b_short)
@@ -296,28 +311,29 @@
             investment += (b_sell * fees_sell).sum()
 
         if costs_buy is not None:
             investment += (x_buy * costs_buy).sum()
         if costs_sell is not None:
             investment += (x_sell * costs_sell).sum()
 
+        if rf_return is not None:
+            x_rf.ub = 1.0
+            investment += x_rf
+
         if min_long is not None:
             m.addConstr(x_buy >= min_long * b_buy, name="min_buy")
 
         if min_short is not None:
             m.addConstr(x_sell >= min_short * b_sell, name="min_sell")
 
         m.addConstr(investment == 1, name="fully_invested")
 
         if not isinstance(self.covariance, tuple):
             # Basic mean-variance weighted objective
-            m.setObjective(
-                self.mu @ x - 0.5 * gamma * x @ self.covariance @ x,
-                GRB.MAXIMIZE,
-            )
+            objexpr = self.mu @ x - 0.5 * gamma * x @ self.covariance @ x
         else:
             # Idea:   We have given  Sigma =
             #
             #   factors[0] @ factors[0].T + ... + factors[l] @ factors[l].T
             #   =: F_0 @ F_0.T + ... + F_l @ F_l
             #
             # so that for each contributing term we can set
@@ -332,30 +348,76 @@
             objexpr = self.mu @ x
 
             for idx, F in enumerate(self.covariance):
                 y = m.addMVar(F.shape[1], lb=-float("inf"), name=f"factor{idx:d}")
                 m.addConstr(F.T @ x == y, name=f"link_factor{idx:d}_x")
                 objexpr -= 0.5 * gamma * y @ y
 
-            m.setObjective(objexpr, GRB.MAXIMIZE)
+        if rf_return is not None:
+            objexpr += rf_return * x_rf
 
-        return x
+        m.setObjective(objexpr, GRB.MAXIMIZE)
+        return (x, x_rf)
 
-    def _convert_result(self, x):
+    def _construct_result(self, x, x_rf, rf_return):
         if self.resultType == "numpy":
-            return x
+            pass
         elif self.resultType == "pandas":
-            return pd.Series(x, index=self.index)
+            x = pd.Series(x, index=self.index)
         else:
             assert False
 
+        ret = self.mu @ x
+
+        if not isinstance(self.covariance, tuple):
+            risk = x @ self.covariance @ x
+        else:
+            risk = 0.0
+            for F in self.covariance:
+                y = x @ F
+                risk += y @ y
+
+        if rf_return is not None:
+            x_rf = x_rf
+            ret += rf_return * x_rf
+        else:
+            x_rf = None
+
+        return PortfolioResult(x, ret, risk, x_rf)
+
     def _homogenize_input(self, input_data):
         # Check and unpack if input_data is a Series
         if isinstance(input_data, pd.Series):
             if self.index is not None:
                 if any(self.index != input_data.index):
                     raise ValueError("Misaligned Series indexes: " + input_data.index)
             else:
                 self.index = input_data.index
             input_data = input_data.to_numpy()
 
         return input_data
+
+
+@dataclass
+class PortfolioResult:
+    """
+    Data class representing computed portfolios.
+
+
+    Attributes
+    ----------
+    x : 1-d ndarray
+        The vector of relative investments into each asset
+    ret : float
+        The (estimated) return of the portfolio
+    risk : float
+        The (estimated) risk of the portfolio
+    x_rf : float, optional
+        The relative investment into the risk-free asset.  Equals to None if no
+        risk-free return rate was specified upon input
+
+    """
+
+    x: np.ndarray
+    ret: float
+    risk: float
+    x_rf: Optional[float] = None
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/qubo.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/qubo.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,40 @@
 --------------------------------------------------
 """
 
 import logging
 from dataclasses import dataclass
 
 import gurobipy as gp
-from gurobipy import GRB
 import numpy as np
+from gurobipy import GRB
 
 from gurobi_optimods.utils import optimod
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class QuboResult:
+    """
+    Solution to a QUBO problem.
+
+    Attributes
+    ----------
+    solution : ndarray
+        0/1 array of variable values in the solution
+    objective_value : float
+        The objective function value for this solution
+    """
+
     solution: np.ndarray
     objective_value: float
 
 
 def callback(model, where):
-
     if where == GRB.Callback.MIP:
         runtime = model.cbGet(GRB.Callback.RUNTIME)
         if runtime >= model._next_output_time:
             primal_bound = model.cbGet(GRB.Callback.MIP_OBJBST)
             dual_bound = model.cbGet(GRB.Callback.MIP_OBJBND)
             logger.info(
                 f"Time: {runtime:.0f}s, "
@@ -41,39 +51,43 @@
         obj = model.cbGet(GRB.Callback.MIPSOL_OBJ)
         logger.info(f"New QUBO solution found with objective {obj}")
 
 
 @optimod()
 def solve_qubo(coeff_matrix, time_limit=GRB.INFINITY, *, create_env) -> QuboResult:
     """
-    Solve a quadratic unconstrained binary optimization (QUBO) problem,
-    i.e., minimize quadratic function :math:`x'Qx` defined by coefficient matrix :math:`Q`
-    over a binary decision variable vector :math:`x`
-
-    :param coeffMatrix: Quadratic coefficient matrix
-    :type coeffMatrix: :class:`numpy.ndarray` or :class:`scipy.sparse`
-    :param timeLimit: Time limit in seconds
-    :type timeLimit: :class:`int`
-    :return: 0/1 solution array, objective value
-    :rtype: :class:`QuboResult`
+    Solve a quadratic unconstrained binary optimization (QUBO) problem, i.e.,
+    minimize quadratic function :math:`x'Qx` defined by coefficient matrix
+    :math:`Q` over a binary decision variable vector :math:`x`
+
+    Parameters
+    ----------
+    coeff_matrix : spmatrix
+        Quadratic coefficient matrix
+    time_limit : float
+        Time limit in seconds (optional, default no limit)
+
+    Returns
+    -------
+    QuboResult
+        A dataclass containing a 0/1 solution array and its objective value
     """
 
     if coeff_matrix.ndim != 2:
         raise ValueError("Matrix is not 2-dimensional.")
 
     shape = coeff_matrix.shape
     if shape[0] != shape[1]:
         raise ValueError("Matrix is not quadratic.")
 
     n = shape[0]
 
     params = {"TimeLimit": time_limit, "LogToConsole": 0}
 
     with create_env(params=params) as env, gp.Model(env=env) as model:
-
         x = model.addMVar(n, vtype=GRB.BINARY)
         model.setObjective(x @ coeff_matrix @ x, GRB.MINIMIZE)
 
         model._next_output_time = 5
         model.optimize(callback)
 
         if model.SolCount == 0:
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/regression.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/regression.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,26 +31,28 @@
 class LADRegression(RegressionBase):
     """Least absolute deviations (L1-norm) regressor"""
 
     @optimod()
     def fit(self, X_train, y_train, *, create_env):
         """Fit the model to training data.
 
-        :param X_train: Training set feature values
-        :type X_train: :class:`np.array`
-        :param y_train: Training set output values
-        :type y_train: :class:`np.array`
+        Parameters
+        ----------
+
+        X_train : ndarray
+            Training set feature values
+        y_train : ndarray
+            Training set output values
         """
 
         # Metadata about the input data
         records, n_features_in = X_train.shape
 
         # Create model
         with create_env() as env, gp.Model(env=env) as model:
-
             # Create unbounded variables for each column coefficient, and bound
             # magnitudes using additional variables. Keep intercept separate.
             intercept = model.addVar(lb=-GRB.INFINITY, name="intercept")
             coeff = model.addMVar(n_features_in, lb=-GRB.INFINITY, name="coeff")
             pos_error = model.addMVar(records, name="pos_error")
             neg_error = model.addMVar(records, name="neg_error")
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/utils.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # factory function should be used to create the mod's gurobi environments.
 #
 #   @optimod(mod_logger=logger)  # pass the mod's module logger
 #   def my_mod(inputs, *, create_env):
 #       with create_env() as env, gp.Model(env=env) as model:
 #           # do stuff with model
 #
-# The mod then gets two arguments for free: `silent`, where `silent=True`
-# suppresses all output, and logfile=<file-path> creates a log file including
-# logger output from the mod and gurobi output.
+# The mod then gets two arguments for free: `verbose`, where `verbose=False`
+# suppresses all output, and logfile=<file-path>, which creates a log file
+# including logger output from the mod and gurobi output.
 #
-# FIXME this won't handle multi-threaded stuff well (context manipulates
+# Note that this won't handle multi-threaded stuff well (context manipulates
 # global logger handlers). But it's simpler to implement in the mods than
 # passing some funky log collecting object around.
 
 import functools
 import logging
 import re
 import sys
@@ -103,21 +103,38 @@
 def optimod(mod_logger=None):
     if mod_logger is None:
         mod_logger = global_mod_logger
 
     def optimod_decorator(func):
         @functools.wraps(func)
         def optimod_decorated(
-            *args, silent=False, logfile=None, solver_params=None, **kwargs
+            *args, verbose=True, logfile=None, solver_params=None, **kwargs
         ):
             with _mod_context(
                 mod_logger=mod_logger,
-                log_to_console=not silent,
+                log_to_console=verbose,
                 log_to_file=logfile,
                 user_params=solver_params,
             ) as create_env:
-                return func(*args, create_env=create_env, **kwargs)
+                try:
+                    return func(*args, create_env=create_env, **kwargs)
+
+                except gp.GurobiError as ge:
+                    if ge.errno == gp.GRB.ERROR_SIZE_LIMIT_EXCEEDED:
+                        pass  # fall through
+                    else:
+                        raise
+
+                # We can only fall through to here due to SIZE_LIMIT_EXCEEDED,
+                # so raise a more optimods-appropriate error. Raise here
+                # (instead of directly in the except block above) to avoid a
+                # confusing double stack trace.
+                raise ValueError(
+                    "Given data exceeds Gurobi trial license limits; please see "
+                    "https://support.gurobi.com/hc/en-us/articles/15801588452241 "
+                    "to resolve this issue"
+                )
 
         optimod_decorated._decorated_mod = True
         return optimod_decorated
 
     return optimod_decorator
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/workforce.py` & `gurobi_optimods-0.2.0/src/gurobi_optimods/workforce.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 """
 Workforce Scheduling
 --------------------
 """
 
 import logging
+from typing import Optional
 
 import gurobipy as gp
 import gurobipy_pandas as gppd
 import pandas as pd
 from gurobipy import GRB
 
 from gurobi_optimods.utils import optimod
 
 logger = logging.getLogger(__name__)
 
 
 @optimod()
 def solve_workforce_scheduling(
-    preferences: pd.DataFrame,
+    availability: pd.DataFrame,
     shift_requirements: pd.DataFrame,
     worker_limits: pd.DataFrame,
+    preferences: Optional[str] = None,
     rolling_limits: bool = False,
     *,
     create_env,
 ) -> pd.DataFrame:
     """Solve a workforce scheduling model.
 
-    :param preferences: Dataframe with columns 'Worker' and 'Shift' defining
-        all allowable worker-shift combinations
-    :type preferences: :class:`pd.DataFrame`
-    :param shift_requirements: Dataframe with columns 'Shift' and 'Required'
-        specifying the number of staff required for every shift
-    :type shift_requirements: :class:`pd.DataFrame`
-    :param worker_limits: Dataframe with columns 'Worker', 'MinShifts', and
-        'MaxShifts' specifying the maximum and minimum number of shifts each
-        worker may be assigned
-    :type worker_limits: :class:`pd.DataFrame`
-    :param rolling_limits: Whether to enforce worker shift limits on a rolling
-        window basis. If True, worker_limits must contain an additional 'Window'
-        column specifying the rolling window for each worker
-    :type rolling_limits: :class:`bool`
-    :return: Assigned shifts as a subset of the preferences dataframe
-    :rtype: :class:`pd.DataFrame`
+    Parameters
+    ----------
+    availability : DataFrame
+        Dataframe with columns 'Worker' and 'Shift' defining all allowable
+        worker-shift combinations. The 'Preference' column optionally assigns a
+        preference value to the given combination.
+    shift_requirements : DataFrame
+        Dataframe with columns 'Shift' and 'Required' specifying the number of
+        staff required for every shift.
+    worker_limits : DataFrame
+        Dataframe with columns 'Worker', 'MinShifts', and 'MaxShifts' specifying
+        the maximum and minimum number of shifts each worker may be assigned in
+        the schedule.
+    preferences : str, optional
+        The name of a column in the availability dataframe containing preference
+        values. If provided, the mod returns a schedule which maximises the sum
+        of preference values of assigned shifts.
+    rolling_limits : bool
+        Whether to enforce worker shift limits on a rolling window basis. If
+        True, worker_limits must contain an additional 'Window' column
+        specifying the rolling window for each worker.
+
+    Returns
+    -------
+    DataFrame
+        Shift assignments as a subset of the availability dataframe
+
+    Raises
+    ------
+    ValueError
+        If a feasible set of shift assignments cannot be constructed from the
+        input data
     """
     with create_env() as env, gp.Model(env=env) as m:
-
         # Create binary variables for all valid shift assignments and
         # create preference maximization objective
         m.ModelSense = GRB.MAXIMIZE
-        assignments = preferences.set_index(["Worker", "Shift"]).gppd.add_vars(
-            m, obj="Preference", vtype=GRB.BINARY, name="assign"
+        preference_value = 0.0 if preferences is None else preferences
+        assignments = availability.set_index(["Worker", "Shift"]).gppd.add_vars(
+            m, obj=preference_value, vtype=GRB.BINARY, name="assign"
         )
 
         # Enforce shift coverage requirements
         gppd.add_constrs(
             m,
             assignments.groupby("Shift")["assign"].sum(),
             GRB.EQUAL,
@@ -96,15 +114,15 @@
                 assignments.groupby("Worker")["assign"].sum(),
                 GRB.GREATER_EQUAL,
                 worker_limits.set_index("Worker")["MinShifts"],
                 name="min_shifts",
             )
 
         # Solve the model and return the shift assignments as a subset of the
-        # input preferences dataframe. Raise an exception if a feasible schedule
+        # input availability dataframe. Raise an exception if a feasible schedule
         # does not exist.
 
         m.optimize()
         if m.Status == GRB.INFEASIBLE:
             raise ValueError("Infeasible roster")
 
         return (
```

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/data/portfolio/portfolio.csv` & `gurobi_optimods-0.2.0/src/gurobi_optimods/data/portfolio/portfolio.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/src/gurobi_optimods/data/workforce/preferences.csv` & `gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/preferences.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/tests/test_bipartite_matching.py` & `gurobi_optimods-0.2.0/tests/test_bipartite_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,41 @@
         matching = maximum_bipartite_matching(frame, "n1", "n2")
 
         self.assertIsInstance(matching, pd.DataFrame)
         self.assertIsNot(matching, frame)
         self.assert_is_unweighted_matching(matching, columns=["n1", "n2"])
         assert_frame_equal(matching, expected_result)
 
+    def test_integer_types(self):
+        frame = pd.DataFrame(
+            {
+                "a": list(range(100)),
+                "b": list(range(100, 200)),
+            }
+        )
+
+        matching = maximum_bipartite_matching(frame, "a", "b")
+        self.assertIsInstance(matching, pd.DataFrame)
+        self.assertIsNot(matching, frame)
+        assert_frame_equal(matching, frame)
+
+    def test_datetime_types(self):
+        start = pd.Timestamp("2022-01-01")
+        frame = pd.DataFrame(
+            {
+                "date": pd.date_range(start, freq="D", periods=10),
+                "activity": [f"a{i}" for i in range(10)],
+            }
+        )
+
+        matching = maximum_bipartite_matching(frame, "date", "activity")
+        self.assertIsInstance(matching, pd.DataFrame)
+        self.assertIsNot(matching, frame)
+        assert_frame_equal(matching, frame)
+
 
 @unittest.skipIf(nx is None, "networkx is not installed")
 class TestBipartiteMatchingNetworkx(unittest.TestCase):
     def assert_is_unweighted_matching(self, matching):
         # Verify that the given networkx graph is a matching
         incidence_count = Counter(chain(*matching.edges))
         self.assertTrue(all(count == 1 for count in incidence_count.values()))
```

### Comparing `gurobi_optimods-0.1.0/tests/test_min_cost_flow.py` & `gurobi_optimods-0.2.0/tests/test_min_cost_flow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,176 @@
 import unittest
 
-import gurobipy as gp
 import numpy as np
-from gurobipy import GRB
+import pandas as pd
+import scipy.sparse as sp
 
 try:
     import networkx as nx
 except ImportError:
     nx = None
 
-from numpy.testing import assert_array_equal, assert_allclose
-
 import gurobi_optimods.datasets as datasets
 import gurobi_optimods.min_cost_flow as mcf
-from gurobi_optimods.min_cost_flow import solve_min_cost_flow
+
+from .test_graph_utils import (
+    check_solution_networkx,
+    check_solution_pandas,
+    check_solution_scipy,
+)
 
 
 class TestMinCostFlow(unittest.TestCase):
     def test_pandas(self):
         edge_data, node_data = datasets.load_graph()
         cost, sol = mcf.min_cost_flow(edge_data, node_data)
         sol = sol[sol > 0]
         self.assertEqual(cost, 31)
-        self.assertEqual(sol.tolist(), [1.0, 1.0, 1.0, 2.0, 2.0])
-        self.assertEqual(sol.index.tolist(), [(0, 1), (0, 2), (1, 3), (2, 4), (4, 5)])
+        candidate = {(0, 1): 1.0, (0, 2): 1.0, (1, 3): 1.0, (2, 4): 2.0, (4, 5): 2.0}
+        self.assertIsInstance(sol, pd.Series)
+        self.assertTrue(check_solution_pandas(sol, [candidate]))
 
     def test_infeasible(self):
         edge_data, node_data = datasets.load_graph()
         # Add a node requesting more flow than is available.
         node_data["demand"].values[-1] = 10.0
         with self.assertRaisesRegex(ValueError, "Unsatisfiable flows"):
             obj, sol = mcf.min_cost_flow(edge_data, node_data)
 
     def test_scipy(self):
         G, cap, cost, demands = datasets.load_graph_scipy()
         cost, sol = mcf.min_cost_flow_scipy(G, cap, cost, demands)
         self.assertEqual(cost, 31)
-        expected = np.array(
+        candidate = np.array(
             [
                 [0.0, 1.0, 1.0, 0.0, 0.0, 0.0],
                 [0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
                 [0.0, 0.0, 0.0, 0.0, 2.0, 0.0],
                 [0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
                 [0.0, 0.0, 0.0, 0.0, 0.0, 2.0],
             ]
         )
-        assert_array_equal(sol.toarray(), expected)
+        self.assertIsInstance(sol, sp.spmatrix)
+        self.assertTrue(check_solution_scipy(sol, [candidate]))
 
     @unittest.skipIf(nx is None, "networkx is not installed")
     def test_networkx(self):
         G = datasets.load_graph_networkx()
         cost, sol = mcf.min_cost_flow_networkx(G)
         self.assertEqual(cost, 31)
-        self.assertEqual(
-            sol, {(0, 1): 1.0, (0, 2): 1.0, (1, 3): 1.0, (2, 4): 2.0, (4, 5): 2.0}
-        )
+        expected = {
+            (0, 1): {"flow": 1.0},
+            (0, 2): {"flow": 1.0},
+            (1, 3): {"flow": 1.0},
+            (2, 4): {"flow": 2.0},
+            (4, 5): {"flow": 2.0},
+        }
+        self.assertIsInstance(sol, nx.Graph)
+        self.assertTrue(check_solution_networkx(sol, [expected]))
+
+    @unittest.skipIf(nx is None, "networkx is not installed")
+    def test_networkx_renamed(self):
+        G = datasets.load_graph_networkx()
+        G = nx.relabel_nodes(G, {0: "s", 5: "t"})
+        cost, sol = mcf.min_cost_flow_networkx(G)
+        self.assertEqual(cost, 31)
+        expected = {
+            ("s", 1): {"flow": 1.0},
+            ("s", 2): {"flow": 1.0},
+            (1, 3): {"flow": 1.0},
+            (2, 4): {"flow": 2.0},
+            (4, "t"): {"flow": 2.0},
+        }
+        self.assertIsInstance(sol, nx.Graph)
+        self.assertTrue(check_solution_networkx(sol, [expected]))
 
 
 class TestMinCostFlow2(unittest.TestCase):
     def test_pandas(self):
         edge_data, node_data = datasets.load_graph2()
         cost, sol = mcf.min_cost_flow(edge_data, node_data)
         sol = sol[sol > 0]
         self.assertEqual(cost, 150)
-        self.assertEqual(sol.tolist(), [12.0, 8.0, 4.0, 8.0, 11.0, 5.0, 10.0])
-        self.assertEqual(
-            sol.index.tolist(),
-            [(0, 1), (0, 2), (1, 3), (1, 2), (2, 3), (2, 4), (3, 4)],
-        )
+        candidate = {
+            (0, 1): 12.0,
+            (0, 2): 8.0,
+            (1, 3): 4.0,
+            (1, 2): 8.0,
+            (2, 3): 15.0,
+            (2, 4): 1.0,
+            (3, 4): 14.0,
+        }
+        candidate2 = {
+            (0, 1): 12.0,
+            (0, 2): 8.0,
+            (1, 3): 4.0,
+            (1, 2): 8.0,
+            (2, 3): 11.0,
+            (2, 4): 5.0,
+            (3, 4): 10.0,
+        }
+        self.assertTrue(check_solution_pandas(sol, [candidate, candidate2]))
 
     def test_scipy(self):
         G, cap, cost, demands = datasets.load_graph2_scipy()
         cost, sol = mcf.min_cost_flow_scipy(G, cap, cost, demands)
         self.assertEqual(cost, 150)
         expected = np.array(
             [
                 [0.0, 12.0, 8.0, 0.0, 0.0],
                 [0.0, 0.0, 8.0, 4.0, 0.0],
                 [0.0, 0.0, 0.0, 11.0, 5.0],
                 [0.0, 0.0, 0.0, 0.0, 10.0],
-                [0.0, 0.0, 0.0, 0.0, 0.0],
             ]
         )
-        assert_array_equal(sol.toarray(), expected)
+        self.assertTrue(check_solution_scipy(sol, [expected]))
 
     @unittest.skipIf(nx is None, "networkx is not installed")
     def test_networkx(self):
         G = datasets.load_graph2_networkx()
         cost, sol = mcf.min_cost_flow_networkx(G)
         self.assertEqual(cost, 150)
-        self.assertEqual(
-            sol,
-            {
-                (0, 1): 12.0,
-                (0, 2): 8.0,
-                (1, 3): 4.0,
-                (1, 2): 8.0,
-                (2, 3): 11.0,
-                (2, 4): 5.0,
-                (3, 4): 10.0,
-            },
-        )
-
+        candidate = {
+            (0, 1): {"flow": 12.0},
+            (0, 2): {"flow": 8.0},
+            (1, 2): {"flow": 8.0},
+            (1, 3): {"flow": 4.0},
+            (2, 3): {"flow": 11.0},
+            (2, 4): {"flow": 5.0},
+            (3, 4): {"flow": 10.0},
+        }
+        candidate2 = {
+            (0, 1): {"flow": 12.0},
+            (0, 2): {"flow": 8.0},
+            (1, 3): {"flow": 4.0},
+            (1, 2): {"flow": 8.0},
+            (2, 3): {"flow": 15.0},
+            (2, 4): {"flow": 1.0},
+            (3, 4): {"flow": 14.0},
+        }
+        self.assertTrue(check_solution_networkx(sol, [candidate, candidate2]))
 
-class TestSolveMinCostFlowUtil(unittest.TestCase):
-    # FIXME repurpose these to target the mod
-
-    def setUp(self):
-        self.env = gp.Env()
-
-    def tearDown(self):
-        self.env.close()
-
-    def test_max_flow(self):
-        # Max flow network from a small bipartite matching model, augmented
-        # with a sink->source edge to create a min-cost flow
-        cost, flows = solve_min_cost_flow(
-            env=self.env,
-            edge_source=np.array([5, 5, 0, 1, 1, 2, 3, 4, 6]),
-            edge_target=np.array([0, 1, 4, 2, 4, 6, 6, 6, 5]),
-            capacity=np.array([1.0] * 8 + [GRB.INFINITY]),
-            cost=np.array([0.0] * 8 + [-1.0]),
-            demand=np.zeros(7),
-        )
-        # Max flow is 2. Any optimal solution has 2 units along the sink->source
-        # arc and 2 units in each of the 3 network layers.
-        self.assertEqual(cost, -2.0)
-        self.assertEqual(flows[-1], 2.0)
-        self.assertEqual(flows.sum(), 8.0)
-
-    def test_linear(self):
-        # Silly example to get the demand direction right
-        cost, flows = solve_min_cost_flow(
-            env=self.env,
-            edge_source=np.array([0, 1, 2, 3]),
-            edge_target=np.array([1, 2, 3, 4]),
-            capacity=np.ones(4),
-            cost=np.ones(4),
-            demand=np.array([-1.0, 0.0, 0.0, 0.0, 1.0]),
-        )
-        self.assertEqual(cost, 4.0)
-        assert_allclose(flows, np.ones(4))
-
-    def test_infeasible(self):
-        # A very silly example
-        with self.assertRaisesRegex(ValueError, "Unsatisfiable flows"):
-            solve_min_cost_flow(
-                env=self.env,
-                edge_source=np.array([0]),
-                edge_target=np.array([1]),
-                capacity=np.array([1.0]),
-                cost=np.array([1.0]),
-                demand=np.array([-1.0, 2.0]),
-            )
+    @unittest.skipIf(nx is None, "networkx is not installed")
+    def test_networkx_renamed(self):
+        G = datasets.load_graph2_networkx()
+        G = nx.relabel_nodes(G, {0: "s", 4: "t"})
+        cost, sol = mcf.min_cost_flow_networkx(G)
+        self.assertEqual(cost, 150)
+        candidate = {
+            ("s", 1): {"flow": 12.0},
+            ("s", 2): {"flow": 8.0},
+            (1, 2): {"flow": 8.0},
+            (1, 3): {"flow": 4.0},
+            (2, 3): {"flow": 11.0},
+            (2, "t"): {"flow": 5.0},
+            (3, "t"): {"flow": 10.0},
+        }
+        candidate2 = {
+            ("s", 1): {"flow": 12.0},
+            ("s", 2): {"flow": 8.0},
+            (1, 3): {"flow": 4.0},
+            (1, 2): {"flow": 8.0},
+            (2, 3): {"flow": 15.0},
+            (2, "t"): {"flow": 1.0},
+            (3, "t"): {"flow": 14.0},
+        }
+        self.assertTrue(check_solution_networkx(sol, [candidate, candidate2]))
```

### Comparing `gurobi_optimods-0.1.0/tests/test_mwis.py` & `gurobi_optimods-0.2.0/tests/test_mwis.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
-
 from itertools import combinations
-import scipy.sparse as sp
+
 import numpy as np
+import scipy.sparse as sp
 from numpy.testing import assert_array_equal
 
 from gurobi_optimods.mwis import maximum_weighted_independent_set
 
 
 def get_adjacency_matrix(num_vertices, density, seed):
     """Create the upper triangular adjacency matrix for a random graph
```

### Comparing `gurobi_optimods-0.1.0/tests/test_portfolio.py` & `gurobi_optimods-0.2.0/tests/test_portfolio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from contextlib import redirect_stdout
 import io
+import os
+import tempfile
 import unittest
+from contextlib import redirect_stdout
+
 import numpy as np
 import pandas as pd
 from numpy.testing import assert_allclose, assert_array_equal
 
 from gurobi_optimods.datasets import load_portfolio
-from gurobi_optimods.portfolio import MeanVariancePortfolio
+from gurobi_optimods.portfolio import MeanVariancePortfolio, PortfolioResult
 
 
 class TestMVPBasic(unittest.TestCase):
     # All tests that focus on construction, data checks etc. go here
 
     def test_datasets(self):
         data = load_portfolio()
@@ -21,15 +24,15 @@
 
     def test_example_data(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x = mvp.efficient_portfolio(0.5)
+        pf = mvp.efficient_portfolio(0.5)
 
     def test_init_0(self):
         # Specifying neither cov_matrix nor cov_factors is disallowed
         data = load_portfolio()
         mu = data.mean()
 
         with self.assertRaises(TypeError):
@@ -58,204 +61,234 @@
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         with redirect_stdout(io.StringIO()) as console:
-            x = mvp.efficient_portfolio(0.5, solver_params={})
+            pf = mvp.efficient_portfolio(0.5, solver_params={})
         consoleContent = console.getvalue()
         self.assertIn("Gurobi Optimizer", consoleContent)
 
         solver_params = {"OutputFlag": 0}
         with redirect_stdout(io.StringIO()) as console:
-            x = mvp.efficient_portfolio(0.5, solver_params=solver_params)
+            pf = mvp.efficient_portfolio(0.5, solver_params=solver_params)
         consoleContent = console.getvalue()
         self.assertEqual(consoleContent, "")
 
-    def test_silent(self):
+    def test_non_verbose(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         with redirect_stdout(io.StringIO()) as console:
-            x = mvp.efficient_portfolio(0.5, solver_params={})
+            pf = mvp.efficient_portfolio(0.5, solver_params={})
         consoleContent = console.getvalue()
         self.assertIn("Gurobi Optimizer", consoleContent)
 
         with redirect_stdout(io.StringIO()) as console:
-            x = mvp.efficient_portfolio(0.5, silent=True)
+            pf = mvp.efficient_portfolio(0.5, verbose=False)
         consoleContent = console.getvalue()
         self.assertEqual(consoleContent, "")
 
     def test_logfile(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
-        x = mvp.efficient_portfolio(0.5, logfile="more_bananas.log")
-        with open("more_bananas.log", "rt") as fh:
-            content = fh.read()
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            logfile = os.path.join(tmpdirname, "more_bananas.log")
+            pf = mvp.efficient_portfolio(0.5, logfile=logfile)
+            with open(logfile, "rt") as fh:
+                content = fh.read()
         self.assertIn("Gurobi Optimizer", content)
 
     def test_params(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         solver_params = {"MIPFocus": 1}
         with redirect_stdout(io.StringIO()) as console:
-            x = mvp.efficient_portfolio(0.5, solver_params=solver_params)
+            pf = mvp.efficient_portfolio(0.5, solver_params=solver_params)
         consoleContent = console.getvalue()
         self.assertIn("Set parameter MIPFocus to value 1", consoleContent)
 
 
 class TestMVPFeatures(unittest.TestCase):
     # All tests that focus portfolio feature correctness go here
 
-    def test_two_assets(self):
+    def test_two_assets_x(self):
+        cov_matrix = np.array([[3, 0.5], [0.5, 2]])
+        mu = np.array([1, -0.1])
+        mvp = MeanVariancePortfolio(mu, cov_matrix)
+        pf = mvp.efficient_portfolio(0.5)
+        assert_allclose(pf.x, [0.925, 0.075], atol=1e-6)
+
+    def test_two_assets_return(self):
         cov_matrix = np.array([[3, 0.5], [0.5, 2]])
         mu = np.array([1, -0.1])
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x = mvp.efficient_portfolio(0.5)
-        assert_allclose(x, [0.925, 0.075], atol=1e-6)
+        pf = mvp.efficient_portfolio(0.5)
+        self.assertAlmostEqual(pf.ret, pf.x @ mu)
+
+    def test_two_assets_risk(self):
+        cov_matrix = np.array([[3, 0.5], [0.5, 2]])
+        mu = np.array([1, -0.1])
+        mvp = MeanVariancePortfolio(mu, cov_matrix)
+        pf = mvp.efficient_portfolio(0.5)
+        self.assertAlmostEqual(pf.risk, pf.x @ cov_matrix @ pf.x)
+
+    def test_example_data_result(self):
+        data = load_portfolio()
+        cov_matrix = data.cov()
+        mu = data.mean()
+        gamma = 100.0
+
+        mvp = MeanVariancePortfolio(mu, cov_matrix)
+        pf = mvp.efficient_portfolio(gamma)
+        self.assertIsInstance(pf, PortfolioResult)
+
+        self.assertAlmostEqual(pf.ret, pf.x @ mu)
+        self.assertAlmostEqual(pf.risk, pf.x @ cov_matrix @ pf.x)
+        self.assertIsNone(pf.x_rf)
 
     def test_number_of_trades(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x_unconstrained = mvp.efficient_portfolio(gamma)
+        x_unconstrained = mvp.efficient_portfolio(gamma).x
         self.assertGreater((x_unconstrained > 1e-4).sum(), 3)
 
-        x_3 = mvp.efficient_portfolio(gamma, max_trades=3)
+        x_3 = mvp.efficient_portfolio(gamma, max_trades=3).x
         self.assertLessEqual((x_3 > 1e-4).sum(), 3)
 
     def test_transaction_fees_long(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         fees_buy = 1e-4
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x = mvp.efficient_portfolio(gamma, fees_buy=fees_buy)
+        x = mvp.efficient_portfolio(gamma, fees_buy=fees_buy).x
         n_trades = (x > 1e-4).sum()
         self.assertLessEqual(x.sum(), 1 - n_trades * fees_buy)
 
     def test_transaction_fees_short(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         fees_sell = 1e-4
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         # Ensure that we go short somewhere
-        x = mvp.efficient_portfolio(gamma, max_total_short=0.3)
+        x = mvp.efficient_portfolio(gamma, max_total_short=0.3).x
         n_trades = (x < 0).sum()
         self.assertGreater(n_trades, 0)
         self.assertAlmostEqual(x.sum(), 1)
 
         # Ensure that transaction fees are paid out of the portfolio
-        x = mvp.efficient_portfolio(gamma, max_total_short=0.3, fees_sell=fees_sell)
+        x = mvp.efficient_portfolio(gamma, max_total_short=0.3, fees_sell=fees_sell).x
         n_trades = (x < 0).sum()
         self.assertGreater(n_trades, 0)
         self.assertLessEqual(x.sum(), 1 - n_trades * fees_sell + 1e-8)
 
     def test_min_long(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         # Ensure that we _have_ a small trade w/o minimum buy in
-        x = mvp.efficient_portfolio(gamma, min_long=0.0)
+        x = mvp.efficient_portfolio(gamma, min_long=0.0).x
         small_trades = (x > 1e-6) & (x < (0.03 - 1e-6))
         self.assertGreater(small_trades.sum(), 0)
 
         # Ensure that we _don't_ have a small trade w minimum buy in
-        x = mvp.efficient_portfolio(gamma, min_long=0.03)
+        x = mvp.efficient_portfolio(gamma, min_long=0.03).x
         small_trades = (x > 1e-6) & (x < (0.03 - 1e-6))
         self.assertEqual(small_trades.sum(), 0)
 
     def test_max_total_short(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         # Ensure that by default we don't go short
-        x = mvp.efficient_portfolio(gamma)
+        x = mvp.efficient_portfolio(gamma).x
         self.assertEqual((x < 0).sum(), 0)
 
         # Ensure that we take advantage of leverage
-        x = mvp.efficient_portfolio(gamma, max_total_short=0.1)
+        x = mvp.efficient_portfolio(gamma, max_total_short=0.1).x
         self.assertGreaterEqual(x[x < 0].sum(), -0.1 - 1e-6)
         self.assertLess(x[x < 0].sum(), -1e-3)
         self.assertAlmostEqual(x.sum(), 1.0)
         self.assertAlmostEqual(np.abs(x).sum(), 1.0 + 2 * 0.1)
 
     def test_min_short_0(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         # Ensure that by default we don't go short
-        x = mvp.efficient_portfolio(gamma)
+        x = mvp.efficient_portfolio(gamma).x
         self.assertEqual((x < 0).sum(), 0)
 
         # Adding a min_short constraint doesn't change a thing
-        x_other = mvp.efficient_portfolio(gamma, min_short=0.01)
+        x_other = mvp.efficient_portfolio(gamma, min_short=0.01).x
         assert_allclose(x.to_numpy(), x_other.to_numpy())
 
     def test_min_short_1(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x = mvp.efficient_portfolio(gamma, max_total_short=0.5)
+        x = mvp.efficient_portfolio(gamma, max_total_short=0.5).x
 
         # Ensure that we do have tiny short positions
         small_trades = (x < -1e-6) & (x > (-0.05 + 1e-6))
         self.assertGreater(small_trades.sum(), 0)
 
         # Ensure that we still have short positions but beyond the threshold
-        x = mvp.efficient_portfolio(gamma, max_total_short=0.5, min_short=0.05)
+        x = mvp.efficient_portfolio(gamma, max_total_short=0.5, min_short=0.05).x
         self.assertGreater((x <= -0.05).sum(), 0)
         small_trades = (x < -1e-6) & (x > (-0.05 + 1e-6))
         self.assertEqual(small_trades.sum(), 0)
 
     def test_start_portfolio_empty(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
         x0 = np.zeros(mu.shape)
-        x_with = mvp.efficient_portfolio(gamma, initial_holdings=x0)
-        x_without = mvp.efficient_portfolio(gamma, initial_holdings=None)
+        x_with = mvp.efficient_portfolio(gamma, initial_holdings=x0).x
+        x_without = mvp.efficient_portfolio(gamma, initial_holdings=None).x
         assert_array_equal(x_with, x_without)
 
     def test_start_portfolio_invalid(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
@@ -272,47 +305,49 @@
         mu = data.mean()
         gamma = 100.0
 
         # If there are no additional restrictions, the resulting portfolio
         # should be the same as without initial holdings sunk-cost-fallacy
         mvp = MeanVariancePortfolio(mu, cov_matrix)
         x0 = 1.0 / mu.size * np.ones(mu.size)
-        x_with = mvp.efficient_portfolio(gamma, initial_holdings=x0)
-        x_without = mvp.efficient_portfolio(gamma, initial_holdings=None)
+        x_with = mvp.efficient_portfolio(gamma, initial_holdings=x0).x
+        x_without = mvp.efficient_portfolio(gamma, initial_holdings=None).x
         assert_allclose(x_with, x_without, atol=1e-6)
 
     def test_start_portfolio_not_fully_invested(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         # If there are no additional restrictions, the resulting portfolio
         # should be the same as without initial holdings sunk-cost-fallacy
         mvp = MeanVariancePortfolio(mu, cov_matrix)
         x0 = 0.5 / mu.size * np.ones(mu.size)
-        x_with = mvp.efficient_portfolio(gamma, initial_holdings=x0)
-        x_without = mvp.efficient_portfolio(gamma, initial_holdings=None)
+        x_with = mvp.efficient_portfolio(gamma, initial_holdings=x0).x
+        x_without = mvp.efficient_portfolio(gamma, initial_holdings=None).x
         assert_allclose(x_with, x_without, atol=1e-6)
 
     def test_start_portfolio_limit_trades(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
         x0 = 1.0 / mu.size * np.ones(mu.size)
         # Ensure that we use more than 3 trades if there is no limit
-        x1_nomaxtrades = mvp.efficient_portfolio(gamma, initial_holdings=x0)
+        x1_nomaxtrades = mvp.efficient_portfolio(gamma, initial_holdings=x0).x
         trades = ((x1_nomaxtrades - x0) > 1e-4) | ((x1_nomaxtrades - x0) < -1e-4)
         self.assertGreater(trades.sum(), 3)
 
         # Ensure that we only use 3 trades with the limit
-        x1_maxtrades = mvp.efficient_portfolio(gamma, initial_holdings=x0, max_trades=3)
+        x1_maxtrades = mvp.efficient_portfolio(
+            gamma, initial_holdings=x0, max_trades=3
+        ).x
         trades = ((x1_maxtrades - x0) > 1e-4) | ((x1_maxtrades - x0) < -1e-4)
         self.assertLessEqual(trades.sum(), 3)
 
     def test_start_portfolio_max_total_short_max_trades(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
@@ -320,15 +355,15 @@
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
         x0 = 1.0 / mu.size * np.ones(mu.size)
 
         # Ensure that we take advantage of leverage
         x = mvp.efficient_portfolio(
             gamma, initial_holdings=x0, max_trades=6, max_total_short=0.1
-        )
+        ).x
 
         self.assertGreaterEqual((x[x < 0]).sum(), -0.1 - 1e-6)
         self.assertLess(x[x < 0].sum(), -1e-3)
         self.assertAlmostEqual(x.sum(), 1.0)
 
         trades = ((x - x0) > 1e-4) | ((x - x0) < -1e-4)
         self.assertLessEqual(trades.sum(), 6)
@@ -339,50 +374,50 @@
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
         x0 = np.array([0.4, 0, 0, 0.2, 0, 0.1, 0.03, 0.2, 0.07, 0])
         x0 /= x0.sum()  # To avoid 1+eps results due to rounding
         # Ensure that we _do_ have a small trade w/o minimum buy
-        x = mvp.efficient_portfolio(gamma, min_long=0.0, initial_holdings=x0)
+        x = mvp.efficient_portfolio(gamma, min_long=0.0, initial_holdings=x0).x
         trades = x - x0
         small_trades = (trades > 1e-6) & (trades < (0.03 - 1e-6))
         self.assertGreater(small_trades.sum(), 0)
 
         # Ensure that we _don't_ have a small trade w/ minimum buy
-        x = mvp.efficient_portfolio(gamma, min_long=0.03, initial_holdings=x0)
+        x = mvp.efficient_portfolio(gamma, min_long=0.03, initial_holdings=x0).x
         trades = x - x0
         small_trades = (trades > 1e-6) & (trades < (0.03 - 1e-6))
         self.assertEqual(small_trades.sum(), 0)
 
     def test_start_portfolio_no_fees(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         fees = 1e-4
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         # Determine efficient portfolio without fees
-        x0 = mvp.efficient_portfolio(gamma, max_total_short=0.1)
+        x0 = mvp.efficient_portfolio(gamma, max_total_short=0.1).x
 
         # Ensure that this is not changed when we compute the portfolio again
         # with x0 as start and fees.  We need min_long and min_short to avoid
         # that paying fees is seen as a "risk-free loss" which might improve
         # our objective
         x = mvp.efficient_portfolio(
             gamma,
             max_total_short=0.1,
             initial_holdings=x0.to_numpy(),
             fees_buy=fees,
             fees_sell=fees,
             min_long=0.02,
             min_short=0.02,
-        )
+        ).x
         assert_allclose(x0, x, atol=1e-6)
 
     def test_start_portfolio_fees_buy(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
@@ -394,15 +429,15 @@
         x = mvp.efficient_portfolio(
             gamma,
             max_total_short=0.1,
             initial_holdings=x0,
             fees_buy=fees,
             min_long=0.02,
             min_short=0.02,
-        )
+        ).x
         buy_trades = (x - x0) > 1e-4
         # Ensure that there have been buy trades
         self.assertGreater(buy_trades.sum(), 0)
         self.assertLessEqual(x.sum(), 1 - buy_trades.sum() * fees + 1e-6)
 
     def test_start_portfolio_fees_sell(self):
         data = load_portfolio()
@@ -417,28 +452,28 @@
         x = mvp.efficient_portfolio(
             gamma,
             max_total_short=0.1,
             initial_holdings=x0,
             fees_sell=fees,
             min_long=0.02,
             min_short=0.02,
-        )
+        ).x
         sell_trades = (x0 - x) > 1e-4
         # Ensure that there have been sell trades
         self.assertGreater(sell_trades.sum(), 0)
         self.assertLessEqual(x.sum(), 1 - sell_trades.sum() * fees + 1e-6)
 
     def test_max_positions(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x = mvp.efficient_portfolio(gamma, max_positions=3)
+        x = mvp.efficient_portfolio(gamma, max_positions=3).x
         self.assertLessEqual((x > 1e-4).sum(), 3)
 
     def test_max_positions_start_portfolio(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
@@ -447,15 +482,15 @@
         x0 = 1.0 / mu.size * np.ones(mu.size)
 
         x = mvp.efficient_portfolio(
             gamma,
             initial_holdings=x0,
             max_positions=6,
             max_trades=5,
-        )
+        ).x
 
         self.assertLessEqual((x > 1e-4).sum(), 6)
         # In order to satisfy max_positions=6 with max_trades=5,
         # we need to sell 4 positions and invest the surplus into one of the remaining open positions.
         self.assertEqual((x >= (5.0 / mu.size - 1e-6)).sum(), 1)
 
     def test_max_positions_infeasible(self):
@@ -463,45 +498,45 @@
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
         x0 = 1.0 / mu.size * np.ones(mu.size)
 
-        x = mvp.efficient_portfolio(
+        pf = mvp.efficient_portfolio(
             gamma,
             initial_holdings=x0,
             max_positions=6,
             max_trades=3,
         )
         # This needs to be infeasible.
-        self.assertIsNone(x)
+        self.assertIsNone(pf)
 
     def test_transaction_costs_long(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         costs = 0.0025
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x = mvp.efficient_portfolio(gamma, costs_buy=costs)
+        x = mvp.efficient_portfolio(gamma, costs_buy=costs).x
         value_trades = x.sum()
         self.assertAlmostEqual(x.sum(), 1 - costs * value_trades, delta=1e-6)
 
     def test_transaction_fees_costs_long(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         costs = 0.0025
         fees = 1e-4
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
-        x = mvp.efficient_portfolio(gamma, costs_buy=costs, fees_buy=fees)
+        x = mvp.efficient_portfolio(gamma, costs_buy=costs, fees_buy=fees).x
         n_trades = (x > 1e-4).sum()
         value_trades = x.sum()
         self.assertAlmostEqual(
             x.sum(), 1 - n_trades * fees - value_trades * costs, delta=1e-3
         )
 
     def test_transaction_fees_costs_short(self):
@@ -514,15 +549,15 @@
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         x = mvp.efficient_portfolio(
             gamma,
             max_total_short=0.3,
             fees_sell=fees,
             costs_sell=costs,
-        )
+        ).x
         n_trades = (x < 0).sum()
         value_trades = -x[x < 0].sum()
 
         # Ensure that we go short somewhere
         self.assertGreater(n_trades, 0)
         # Ensure that transaction fees and costs are paid out of the portfolio
         self.assertAlmostEqual(x.sum(), 1 - n_trades * fees - value_trades * costs)
@@ -539,15 +574,15 @@
         x = mvp.efficient_portfolio(
             gamma,
             max_total_short=0.3,
             fees_buy=fees,
             fees_sell=fees,
             costs_buy=costs,
             costs_sell=costs,
-        )
+        ).x
         trades = (x < -1e-6) | (x > 1e-6)
         n_trades = trades.sum()
         long_trades_value = x[x > 0].sum()
         short_trades_value = -x[x < 0].sum()
         self.assertAlmostEqual(
             x.sum(),
             1 - n_trades * fees - (long_trades_value + short_trades_value) * costs,
@@ -570,15 +605,15 @@
             fees_buy=fees,
             fees_sell=fees,
             costs_buy=costs,
             costs_sell=costs,
             min_long=0.02,
             min_short=0.02,
             max_trades=6,
-        )
+        ).x
         trades = x - x0
         buy_trades = trades > 1e-4
         sell_trades = trades < -1e-4
         n_trades = buy_trades.sum() + sell_trades.sum()
         buy_trades_value = trades[buy_trades].sum()
         sell_trades_value = -trades[sell_trades].sum()
         trades_value = buy_trades_value + sell_trades_value
@@ -600,35 +635,48 @@
             gamma,
             initial_holdings=x0,
             min_short=0.01,
             min_long=0.015,
             max_total_short=0.1,
             fees_buy=0.001,
             fees_sell=0.002,
-        )
+        ).x
 
         self.assertAlmostEqual(x[x < 0].sum(), -0.1)
 
-    def test_risk_factors_0(self):
+    def test_risk_factors_equivalent_0(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         L = np.linalg.cholesky(cov_matrix)
         mu = data.mean()
         gamma = 100.0
 
         # Two equivalent setups: Sigma itself, and its Cholesky factor
         mvp_factors = MeanVariancePortfolio(mu, None, cov_factors=(L,))
         mvp_Sigma = MeanVariancePortfolio(mu, cov_matrix)
 
-        x_factors = mvp_factors.efficient_portfolio(gamma)
-        x_Sigma = mvp_Sigma.efficient_portfolio(gamma)
+        x_factors = mvp_factors.efficient_portfolio(gamma).x
+        x_Sigma = mvp_Sigma.efficient_portfolio(gamma).x
 
         assert_allclose(x_factors, x_Sigma, atol=1e-6)
 
-    def test_risk_factors_1(self):
+    def test_risk_factors_auxdata_0(self):
+        data = load_portfolio()
+        cov_matrix = data.cov()
+        L = np.linalg.cholesky(cov_matrix)
+        mu = data.mean()
+        gamma = 100.0
+
+        mvp = MeanVariancePortfolio(mu, None, cov_factors=(L,))
+        pf = mvp.efficient_portfolio(gamma)
+
+        self.assertAlmostEqual(pf.ret, mu.to_numpy() @ pf.x)
+        self.assertAlmostEqual(pf.risk, cov_matrix.to_numpy() @ pf.x @ pf.x)
+
+    def test_risk_factors_equivalent_1(self):
         # Use case: Data that would emerge from a Single factor model
         # R = alpha + beta * R_m + e.
         #
         # Letting s = beta * R_m, the resulting covariance matrix would then
         # become Sigma = s @ s.T + diag(...) where the second term captures the
         # variances of the specific returns.
         #
@@ -643,42 +691,57 @@
         cov_matrix = s @ s.T + np.diag(d**2)
 
         # Two equivalent setups: Sigma itself, and its Cholesky factor
         gamma = 20
         mvp_factors = MeanVariancePortfolio(mu, None, cov_factors=(s, D))
         mvp_Sigma = MeanVariancePortfolio(mu, cov_matrix)
 
-        x_factors = mvp_factors.efficient_portfolio(gamma)
-        x_Sigma = mvp_Sigma.efficient_portfolio(gamma)
+        x_factors = mvp_factors.efficient_portfolio(gamma).x
+        x_Sigma = mvp_Sigma.efficient_portfolio(gamma).x
 
         assert_allclose(x_factors, x_Sigma, atol=1e-5)
 
+    def test_risk_factors_auxdata_1(self):
+        n = 3
+        mu = 0.2 + (0.2 * np.random.rand(3) - 0.1)
+        s = (0.1 + 0.2 * np.random.rand(3)).reshape((3, 1))
+        d = 0.05 + 0.3 * np.random.rand(3)
+        D = np.diag(d)
+        cov_matrix = s @ s.T + np.diag(d**2)
+
+        gamma = 20
+        mvp = MeanVariancePortfolio(mu, None, cov_factors=(s, D))
+        pf = mvp.efficient_portfolio(gamma)
+
+        self.assertAlmostEqual(pf.ret, mu @ pf.x)
+        self.assertAlmostEqual(pf.risk, cov_matrix @ pf.x @ pf.x)
+
     def test_costs_per_asset_long(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         costs = np.array(
             [0.01, 0.01, 0.01, 0.02, 0.02, 0.02, 0.0025, 0.0025, 0.0025, 0.0025]
         )
-        x = mvp.efficient_portfolio(gamma, costs_buy=costs)
+        x = mvp.efficient_portfolio(gamma, costs_buy=costs).x
 
         self.assertAlmostEqual(x.sum(), 1 - (costs * x.to_numpy()).sum(), delta=1e-6)
 
     def test_costs_per_asset_long_random(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         costs = np.random.rand(mu.size) * 0.05
-        x = mvp.efficient_portfolio(gamma, costs_buy=costs)
+        x = mvp.efficient_portfolio(gamma, costs_buy=costs).x
 
         self.assertAlmostEqual(x.sum(), 1 - (costs * x.to_numpy()).sum(), delta=1e-6)
 
     def test_costs_per_asset_long_and_short(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
@@ -689,15 +752,15 @@
             [0.01, 0.01, 0.01, 0.02, 0.02, 0.02, 0.0025, 0.0025, 0.0025, 0.0025]
         )
         costs_sell = np.array(
             [0.01, 0.01, 0.01, 0.02, 0.02, 0.02, 0.0025, 0.0025, 0.0025, 0.0025]
         )
         x = mvp.efficient_portfolio(
             gamma, costs_buy=costs_buy, costs_sell=costs_sell, max_total_short=0.1
-        )
+        ).x
 
         df_buy = pd.Series(costs_buy, index=mu.index)
         df_sell = pd.Series(costs_sell, index=mu.index)
         total_costs_buy = (df_buy[x > 1e-6] * x[x > 1e-6]).sum()
         total_costs_sell = -(df_sell[x < -1e-6] * x[x < -1e-6]).sum()
         self.assertAlmostEqual(
             x.sum(), 1 - total_costs_buy - total_costs_sell, delta=1e-6
@@ -711,15 +774,15 @@
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         # costs = np.array([0.00832292, 0.00295583, 0.00353887, 0.0044858 , 0.00337871, 0.00924592, 0.00339121, 0.00391734, 0.00773179, 0.00425846])
         costs_buy = np.random.rand(mu.size) * 0.05
         costs_sell = np.random.rand(mu.size) * 0.05
         x = mvp.efficient_portfolio(
             gamma, costs_buy=costs_buy, costs_sell=costs_sell, max_total_short=0.1
-        )
+        ).x
 
         df_buy = pd.Series(costs_buy, index=mu.index)
         df_sell = pd.Series(costs_sell, index=mu.index)
         total_costs_buy = (df_buy[x > 1e-6] * x[x > 1e-6]).sum()
         total_costs_sell = -(df_sell[x < -1e-6] * x[x < -1e-6]).sum()
         self.assertAlmostEqual(
             x.sum(), 1 - total_costs_buy - total_costs_sell, delta=1e-6
@@ -731,29 +794,29 @@
         mu = data.mean()
         gamma = 100.0
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         fees = np.array(
             [0.01, 0.003, 0.01, 0.004, 0.001, 0.0002, 0.002, 0.006, 0.005, 0.004]
         )
-        x = mvp.efficient_portfolio(gamma, fees_buy=fees, max_trades=4)
+        x = mvp.efficient_portfolio(gamma, fees_buy=fees, max_trades=4).x
         df_buy = pd.Series(fees, index=mu.index)
         total_fees = df_buy[x > 1e-6].sum()
 
         self.assertAlmostEqual(x.sum(), 1 - total_fees, delta=1e-6)
 
     def test_fees_per_asset_long_random(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         fees = np.random.rand(10) * 0.01
-        x = mvp.efficient_portfolio(gamma, fees_buy=fees, max_trades=4)
+        x = mvp.efficient_portfolio(gamma, fees_buy=fees, max_trades=4).x
         df_buy = pd.Series(fees, index=mu.index)
         total_fees = df_buy[x > 1e-6].sum()
 
         self.assertAlmostEqual(x.sum(), 1 - total_fees, delta=1e-6)
 
     def test_fees_per_asset_long_and_short_random(self):
         data = load_portfolio()
@@ -766,15 +829,15 @@
         fees_sell = np.random.rand(10) * 0.01
         x = mvp.efficient_portfolio(
             gamma,
             fees_buy=fees_buy,
             fees_sell=fees_sell,
             max_trades=4,
             max_total_short=0.1,
-        )
+        ).x
         df_buy = pd.Series(fees_buy, index=mu.index)
         df_sell = pd.Series(fees_sell, index=mu.index)
         total_fees = df_buy[x > 1e-6].sum() + df_sell[x < -1e-6].sum()
 
         self.assertAlmostEqual(x.sum(), 1 - total_fees, delta=1e-6)
 
     def test_input_wrong_index(self):
@@ -782,28 +845,41 @@
         cov_matrix = data.cov()
         mu = data.mean()
         gamma = 100.0
         mvp = MeanVariancePortfolio(mu, cov_matrix)
 
         fees_buy = pd.Series(index=mu.index[::-1], data=np.linspace(0.0, 0.1, mu.size))
         with self.assertRaises(ValueError):
-            x = mvp.efficient_portfolio(gamma, fees_buy=fees_buy)
+            _ = mvp.efficient_portfolio(gamma, fees_buy=fees_buy)
 
         fees_sell = pd.Series(index=mu.index[::-1], data=np.linspace(0.0, 0.1, mu.size))
         with self.assertRaises(ValueError):
-            x = mvp.efficient_portfolio(gamma, fees_sell=fees_sell)
+            _ = mvp.efficient_portfolio(gamma, fees_sell=fees_sell)
 
         costs_buy = pd.Series(index=mu.index[::-1], data=np.linspace(0.0, 0.1, mu.size))
         with self.assertRaises(ValueError):
-            x = mvp.efficient_portfolio(gamma, costs_buy=costs_buy)
+            _ = mvp.efficient_portfolio(gamma, costs_buy=costs_buy)
 
         costs_sell = pd.Series(
             index=mu.index[::-1], data=np.linspace(0.0, 0.1, mu.size)
         )
         with self.assertRaises(ValueError):
-            x = mvp.efficient_portfolio(gamma, costs_sell=costs_sell)
+            _ = mvp.efficient_portfolio(gamma, costs_sell=costs_sell)
 
         initial_holdings = pd.Series(
             index=mu.index[::-1], data=np.linspace(0.0, 0.01, mu.size)
         )
         with self.assertRaises(ValueError):
-            x = mvp.efficient_portfolio(gamma, initial_holdings=initial_holdings)
+            _ = mvp.efficient_portfolio(gamma, initial_holdings=initial_holdings)
+
+    def test_risk_free_asset(self):
+        data = load_portfolio()
+        cov_matrix = data.cov()
+        mu = data.mean()
+        gamma = 12.5
+
+        # Parameters chosen such that some fraction is invested in cash
+        mvp = MeanVariancePortfolio(mu, cov_matrix)
+        pf = mvp.efficient_portfolio(gamma, rf_return=0.0025)
+
+        self.assertGreater(pf.x_rf, 0.1)
+        self.assertAlmostEqual(pf.ret, mu @ pf.x + 0.0025 * pf.x_rf)
```

### Comparing `gurobi_optimods-0.1.0/tests/test_qubo.py` & `gurobi_optimods-0.2.0/tests/test_qubo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
+
 import numpy as np
-from numpy.testing import assert_array_equal
 import scipy.sparse as sp
+from numpy.testing import assert_array_equal
 
 from gurobi_optimods.qubo import solve_qubo
 
 
 class TestQubo(unittest.TestCase):
     def test_none(self):
         Q = None
```

### Comparing `gurobi_optimods-0.1.0/tests/test_regression.py` & `gurobi_optimods-0.2.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/tests/test_workforce.py` & `gurobi_optimods-0.2.0/tests/test_workforce.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import unittest
 from io import StringIO
 from textwrap import dedent
 
 import pandas as pd
-from pandas.api.types import is_object_dtype, is_datetime64_any_dtype, is_numeric_dtype
+from pandas.api.types import is_datetime64_any_dtype, is_numeric_dtype, is_object_dtype
 from pandas.testing import assert_frame_equal
 
-from gurobi_optimods.workforce import solve_workforce_scheduling
 from gurobi_optimods.datasets import load_workforce
+from gurobi_optimods.workforce import solve_workforce_scheduling
 
 
 def read_csv(text):
     return pd.read_csv(StringIO(dedent(text)))
 
 
 class TestWorkforceScheduling(unittest.TestCase):
     def test_dataset(self):
         # Check that the example dataset has the expected structure
         data = load_workforce()
         self.assertEqual(
-            set(data.keys()), {"preferences", "shift_requirements", "worker_limits"}
+            set(data.keys()), {"availability", "shift_requirements", "worker_limits"}
         )
 
         self.assertEqual(
-            set(data.preferences.columns), {"Worker", "Shift", "Preference"}
+            set(data.availability.columns), {"Worker", "Shift", "Preference"}
         )
-        self.assertTrue(is_object_dtype(data.preferences["Worker"]))
-        self.assertTrue(is_numeric_dtype(data.preferences["Preference"]))
-        self.assertTrue(is_datetime64_any_dtype(data.preferences["Shift"]))
+        self.assertTrue(is_object_dtype(data.availability["Worker"]))
+        self.assertTrue(is_numeric_dtype(data.availability["Preference"]))
+        self.assertTrue(is_datetime64_any_dtype(data.availability["Shift"]))
 
         self.assertEqual(set(data.shift_requirements.columns), {"Shift", "Required"})
         self.assertTrue(is_datetime64_any_dtype(data.shift_requirements["Shift"]))
         self.assertTrue(is_numeric_dtype(data.shift_requirements["Required"]))
 
         self.assertEqual(
             set(data.worker_limits.columns),
             {"Worker", "MinShifts", "MaxShifts"},
         )
         self.assertTrue(is_numeric_dtype(data.worker_limits["MinShifts"]))
         self.assertTrue(is_numeric_dtype(data.worker_limits["MaxShifts"]))
 
     def test_no_option(self):
         # Simple example where there is only one way to cover requirements
-        preferences = read_csv(
+        availability = read_csv(
             """
             Worker,Shift,Preference
             Bob,2022-07-02,1.0
             Alice,2022-07-03,1.0
             """
         )
         shift_requirements = read_csv(
@@ -61,27 +61,28 @@
             Worker,MinShifts,MaxShifts
             Bob,1,1
             Alice,1,1
             """
         )
 
         assignments = solve_workforce_scheduling(
-            preferences=preferences,
+            availability=availability,
             shift_requirements=shift_requirements,
             worker_limits=worker_limits,
+            preferences="Preference",
         )
 
         self.assertIsInstance(assignments, pd.DataFrame)
-        self.assertIsNot(assignments, preferences)
-        assert_frame_equal(assignments, preferences)
+        self.assertIsNot(assignments, availability)
+        assert_frame_equal(assignments, availability)
 
     def test_preferences(self):
         # Choose an assignment which maximises sum of preferences (worker
         # limits are redundant in this example)
-        preferences = read_csv(
+        availability = read_csv(
             """
             Worker,Shift,Preference
             Alice,2022-07-02,1.0
             Alice,2022-07-03,2.0
             Bob,2022-07-02,2.0
             Bob,2022-07-03,1.0
             """
@@ -98,38 +99,86 @@
             Worker,MinShifts,MaxShifts
             Bob,0,2
             Alice,0,2
             """
         )
 
         assignments = solve_workforce_scheduling(
-            preferences=preferences,
+            availability=availability,
             shift_requirements=shift_requirements,
             worker_limits=worker_limits,
+            preferences="Preference",
         )
 
         expected = read_csv(
             """
             Worker,Shift,Preference
             Alice,2022-07-03,2.0
             Bob,2022-07-02,2.0
             """
         )
         self.assertIsInstance(assignments, pd.DataFrame)
-        self.assertIsNot(assignments, preferences)
+        self.assertIsNot(assignments, availability)
+        assert_frame_equal(
+            assignments.sort_values(["Worker", "Shift"]).reset_index(drop=True),
+            expected,
+        )
+
+    def test_no_preferences(self):
+        # Choose a feasible assignment, no preferences provided
+        availability = read_csv(
+            """
+            Worker,Shift
+            Alice,2022-07-02
+            Alice,2022-07-03
+            Bob,2022-07-02
+            Bob,2022-07-03
+            """
+        )
+        shift_requirements = read_csv(
+            """
+            Shift,Required
+            2022-07-02,1
+            2022-07-03,1
+            """
+        )
+        # Bob is unavailable
+        worker_limits = read_csv(
+            """
+            Worker,MinShifts,MaxShifts
+            Bob,0,0
+            Alice,0,2
+            """
+        )
+
+        assignments = solve_workforce_scheduling(
+            availability=availability,
+            shift_requirements=shift_requirements,
+            worker_limits=worker_limits,
+        )
+
+        expected = read_csv(
+            """
+            Worker,Shift
+            Alice,2022-07-02
+            Alice,2022-07-03
+            """
+        )
+        self.assertIsInstance(assignments, pd.DataFrame)
+        self.assertIsNot(assignments, availability)
         assert_frame_equal(
             assignments.sort_values(["Worker", "Shift"]).reset_index(drop=True),
             expected,
         )
 
     def test_constrained(self):
         # Test min/max shifts per worker constraints
-        preferences = read_csv(
+        availability = read_csv(
             """
-            Worker,Shift,Preference
+            Worker,Shift,ThePreferences
             Alice,2022-07-01,1.0
             Alice,2022-07-02,1.0
             Alice,2022-07-03,1.0
             Bob,2022-07-01,2.0
             Bob,2022-07-02,2.0
             Bob,2022-07-03,2.0
             Joy,2022-07-01,3.0
@@ -143,79 +192,79 @@
             2022-07-01,1
             2022-07-02,1
             2022-07-03,1
             """
         )
 
         with self.subTest("upperlimits"):
-
             worker_limits = read_csv(
                 """
                 Worker,MinShifts,MaxShifts
                 Alice,0,3
                 Bob,0,1
                 Joy,0,2
                 """
             )
 
             assignments = solve_workforce_scheduling(
-                preferences=preferences,
+                availability=availability,
                 shift_requirements=shift_requirements,
                 worker_limits=worker_limits,
+                preferences="ThePreferences",
             )
             expected = read_csv(
                 """
-                Worker,Shift,Preference
+                Worker,Shift,ThePreferences
                 Bob,2022-07-01,2.0
                 Joy,2022-07-02,3.1
                 Joy,2022-07-03,3.1
                 """
             )
             self.assertIsInstance(assignments, pd.DataFrame)
-            self.assertIsNot(assignments, preferences)
+            self.assertIsNot(assignments, availability)
             assert_frame_equal(
                 assignments.sort_values(["Shift"]).reset_index(drop=True),
                 expected,
             )
 
         with self.subTest("lowerlimits"):
-
             worker_limits = read_csv(
                 """
                 Worker,MinShifts,MaxShifts
                 Alice,1,3
                 Bob,0,3
                 Joy,0,3
                 """
             )
 
             assignments = solve_workforce_scheduling(
-                preferences=preferences,
+                availability=availability,
                 shift_requirements=shift_requirements,
                 worker_limits=worker_limits,
+                preferences="ThePreferences",
             )
             expected = read_csv(
                 """
-                Worker,Shift,Preference
+                Worker,Shift,ThePreferences
                 Alice,2022-07-01,1.0
                 Joy,2022-07-02,3.1
                 Joy,2022-07-03,3.1
                 """
             )
             self.assertIsInstance(assignments, pd.DataFrame)
-            self.assertIsNot(assignments, preferences)
+            self.assertIsNot(assignments, availability)
             assert_frame_equal(
                 assignments.sort_values(["Shift"]).reset_index(drop=True),
                 expected,
             )
 
     def test_rolling_limits(self):
         # Test enforcement of limits on a rolling window basis
 
-        preferences = read_csv(
+        availability = read_csv(
             """
             Worker,Shift,Preference
             Alice,2022-07-01,1.0
             Alice,2022-07-02,2.0
             Alice,2022-07-03,3.0
             Alice,2022-07-04,4.0
             Bob,2022-07-01,5.1
@@ -238,40 +287,41 @@
             Worker,Window,MinShifts,MaxShifts
             Alice,2D,0,1
             Bob,2D,0,1
             """
         ).assign(Window=lambda df: pd.to_timedelta(df["Window"]))
 
         assignments = solve_workforce_scheduling(
-            preferences=preferences,
+            availability=availability,
             shift_requirements=shift_requirements,
             worker_limits=worker_limits,
+            preferences="Preference",
             rolling_limits=True,
         )
 
         expected = read_csv(
             """
             Worker,Shift,Preference
             Alice,2022-07-01,1.0
             Bob,2022-07-02,6.2
             Alice,2022-07-03,3.0
             Bob,2022-07-04,8.4
             """
         ).assign(Shift=lambda df: pd.to_datetime(df["Shift"]))
         self.assertIsInstance(assignments, pd.DataFrame)
-        self.assertIsNot(assignments, preferences)
+        self.assertIsNot(assignments, availability)
         assert_frame_equal(
             assignments.sort_values(["Shift"]).reset_index(drop=True),
             expected,
         )
 
     def test_infeasibility(self):
         # Infeasibility should raise an exception
 
-        preferences = read_csv(
+        availability = read_csv(
             """
             Worker,Shift,Preference
             Bob,2022-07-02,1.0
             """
         )
         shift_requirements = read_csv(
             """
@@ -284,11 +334,12 @@
             Worker,MinShifts,MaxShifts
             Bob,1,1
             """
         )
 
         with self.assertRaises(ValueError):
             solve_workforce_scheduling(
-                preferences=preferences,
+                availability=availability,
                 shift_requirements=shift_requirements,
                 worker_limits=worker_limits,
+                preferences="Preference",
             )
```

### Comparing `gurobi_optimods-0.1.0/.gitignore` & `gurobi_optimods-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/LICENSE` & `gurobi_optimods-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/NOTICE` & `gurobi_optimods-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/README.md` & `gurobi_optimods-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.1.0/pyproject.toml` & `gurobi_optimods-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -36,7 +36,10 @@
     "networkx",
     "matplotlib",
     "scikit-learn"
 ]
 
 [tool.hatch.version]
 path = "src/gurobi_optimods/__init__.py"
+
+[tool.isort]
+profile = "black"
```

### Comparing `gurobi_optimods-0.1.0/PKG-INFO` & `gurobi_optimods-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-optimods
-Version: 0.1.0
+Version: 0.2.0
 Summary: Nice APIs for common optimization tasks
 Author-email: Simon Bowly <bowly@gurobi.com>, Robert Luce <luce@gurobi.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
 Keywords: gurobipy,optimization,pandas
 Classifier: Development Status :: 4 - Beta
```

