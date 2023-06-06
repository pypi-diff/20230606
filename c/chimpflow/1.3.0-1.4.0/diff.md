# Comparing `tmp/chimpflow-1.3.0.tar.gz` & `tmp/chimpflow-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chimpflow-1.3.0.tar", last modified: Mon May 22 14:01:46 2023, max compression
+gzip compressed data, was "chimpflow-1.4.0.tar", last modified: Tue Jun  6 11:26:25 2023, max compression
```

## Comparing `chimpflow-1.3.0.tar` & `chimpflow-1.4.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.796072 chimpflow-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.772072 chimpflow-1.3.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.772072 chimpflow-1.3.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.772072 chimpflow-1.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.772072 chimpflow-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.764072 chimpflow-1.3.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.772072 chimpflow-1.3.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.772072 chimpflow-1.3.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.776072 chimpflow-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.776072 chimpflow-1.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 14:01:36.000000 chimpflow-1.3.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 14:01:36.000000 chimpflow-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-05-22 14:01:46.796072 chimpflow-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-22 14:01:36.000000 chimpflow-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.776072 chimpflow-1.3.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-22 14:01:36.000000 chimpflow-1.3.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.776072 chimpflow-1.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.764072 chimpflow-1.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.776072 chimpflow-1.3.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.776072 chimpflow-1.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.776072 chimpflow-1.3.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.780072 chimpflow-1.3.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.780072 chimpflow-1.3.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.780072 chimpflow-1.3.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.780072 chimpflow-1.3.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.780072 chimpflow-1.3.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 14:01:36.000000 chimpflow-1.3.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-22 14:01:36.000000 chimpflow-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:01:46.796072 chimpflow-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.768072 chimpflow-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.780072 chimpflow-1.3.0/src/chimpflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-05-22 14:01:46.000000 chimpflow-1.3.0/src/chimpflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-22 14:01:46.000000 chimpflow-1.3.0/src/chimpflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:01:46.000000 chimpflow-1.3.0/src/chimpflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 14:01:46.000000 chimpflow-1.3.0/src/chimpflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-22 14:01:46.000000 chimpflow-1.3.0/src/chimpflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-22 14:01:46.000000 chimpflow-1.3.0/src/chimpflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.784072 chimpflow-1.3.0/src/chimpflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.784072 chimpflow-1.3.0/src/chimpflow_api/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.784072 chimpflow-1.3.0/src/chimpflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.788072 chimpflow-1.3.0/src/chimpflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.788072 chimpflow-1.3.0/src/chimpflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 14:01:46.000000 chimpflow-1.3.0/src/chimpflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/base_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/chimp_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.788072 chimpflow-1.3.0/src/chimpflow_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.792072 chimpflow-1.3.0/src/chimpflow_lib/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/miners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/miners/direct_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 14:01:36.000000 chimpflow-1.3.0/src/chimpflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.792072 chimpflow-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.792072 chimpflow-1.3.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:01:46.796072 chimpflow-1.3.0/tests/echo_test_imgs/
--rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/echo_test_imgs/97wo_01A_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/echo_test_imgs/97wo_01A_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/echo_test_imgs/97wo_01A_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/test_chimp_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-22 14:01:36.000000 chimpflow-1.3.0/tests/test_miner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.060840 chimpflow-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.020843 chimpflow-1.4.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.024843 chimpflow-1.4.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.024843 chimpflow-1.4.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.024843 chimpflow-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.008844 chimpflow-1.4.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.028843 chimpflow-1.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 11:26:13.000000 chimpflow-1.4.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 11:26:13.000000 chimpflow-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-06 11:26:25.060840 chimpflow-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-06 11:26:13.000000 chimpflow-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-06 11:26:13.000000 chimpflow-1.4.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.012844 chimpflow-1.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.032842 chimpflow-1.4.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.036842 chimpflow-1.4.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.036842 chimpflow-1.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.036842 chimpflow-1.4.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.040842 chimpflow-1.4.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 11:26:13.000000 chimpflow-1.4.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-06 11:26:13.000000 chimpflow-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:26:25.060840 chimpflow-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.016843 chimpflow-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.040842 chimpflow-1.4.0/src/chimpflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-06 11:26:25.000000 chimpflow-1.4.0/src/chimpflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.044841 chimpflow-1.4.0/src/chimpflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.044841 chimpflow-1.4.0/src/chimpflow_api/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.048841 chimpflow-1.4.0/src/chimpflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.048841 chimpflow-1.4.0/src/chimpflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.052841 chimpflow-1.4.0/src/chimpflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 11:26:24.000000 chimpflow-1.4.0/src/chimpflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/base_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/chimp_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/src/chimpflow_lib/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 11:26:13.000000 chimpflow-1.4.0/src/chimpflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/configurations/direct_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/configurations/service_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/configurations/service_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:26:25.056841 chimpflow-1.4.0/tests/echo_test_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/test_chimp_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-06 11:26:13.000000 chimpflow-1.4.0/tests/test_miner.py
```

### Comparing `chimpflow-1.3.0/.dae-devops/Makefile` & `chimpflow-1.4.0/.dae-devops/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint e7dd1051580ffa0ed1b6a5a9ce3e6290
+# dae_devops_fingerprint 2cf2414f1b8c1b09c1141588f1f4e6ca
```

### Comparing `chimpflow-1.3.0/.dae-devops/docs/conventions.rst` & `chimpflow-1.4.0/.dae-devops/docs/conventions.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name chimpflow
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint 1584b2ca3962a352d751931fba1af516
+.. # dae_devops_fingerprint 0b606baa538d6630ee8110b0ceb8ddde
```

### Comparing `chimpflow-1.3.0/.dae-devops/docs/docs_structure.rst` & `chimpflow-1.4.0/.dae-devops/docs/docs_structure.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name chimpflow
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint b2ecceb2057aa129a1ee55c76c58e867
+.. # dae_devops_fingerprint 5459e53455f7e8e1536898e915c8a69f
```

### Comparing `chimpflow-1.3.0/.dae-devops/docs/installing.rst` & `chimpflow-1.4.0/.dae-devops/docs/installing.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name chimpflow
 
 Installing
 =======================================================================
 
 
-You will need python 3.9 or later. 
+You will need python 3.10 or later. 
 
-On a Diamond Light Source internal computer, you can achieve Python 3.9 by::
+On a Diamond Light Source internal computer, you can achieve Python 3.10 by::
 
-    $ module load python/3.9
+    $ module load python/3.10
 
 You can check your version of python by typing into a terminal::
 
     $ python3 --version
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 
-You can now use ``pip`` to install the library and its dependencies::
+You can now use ``pip`` to install the package and its dependencies::
 
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ python3 -m pip install chimpflow
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://github.com/diamondlightsource/chimpflow/chimpflow.git
 
-The library should now be installed and the commandline interface on your path.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ chimpflow --version
     $ chimpflow --version-json
 
-.. # dae_devops_fingerprint f4209c13d354b457d8cc21ddf076df26
+.. # dae_devops_fingerprint 9eb5999388b437ecec6c6b841f3294ae
```

### Comparing `chimpflow-1.3.0/.dae-devops/docs/testing.rst` & `chimpflow-1.4.0/.dae-devops/docs/testing.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name chimpflow
 
 Testing
 =======================================================================
 
 The package uses pytest for unit testing.
 
 If you want to run the tests, first get a copy of the code per the instructions in the Developing section.
 
 Then you can run all tests by::
 
-    $ pytest
-
-Or this, which is the command used by the CI runner.
-
-    $ make -f .dae-devops/Makefile validate_pytest
+    $ tox -q -e pytest
 
 To run a single test you can do::
 
     $ pytest tests/the_test_you_want.py
 
-If you want to see more output of the test while it's running you can do:
+If you want to see more output of the test while it's running you can do::
 
     $ pytest -sv -ra --tb=line tests/the_test_you_want.py
 
 Each test will write files into its own directory::
 
-    /tmp/chimpflow/tests/....
+    /tmp/chimpflow/tests/*
 
 The tests clear their directory when they start, but not when they finish.
-This allows peeking in there to see what's been written by the test.
+This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint 3787294ef4eef4f87161e07806f1f417
+.. # dae_devops_fingerprint e9f6ebe8b344e5282c25bc3ba9775f39
```

### Comparing `chimpflow-1.3.0/.dae-devops/project.yaml` & `chimpflow-1.4.0/.dae-devops/project.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Primary information needed for devops.
 primary:
     repository_name: chimpflow
     package_name: chimpflow_lib
-    one_line_description: "XChem Business Knowledge Unit. Service, Client, API, persistent store."
+    one_line_description: "Service which polls the database for subwell images which need to have the chimp detector run on them."
     author:
         name: David Erb
         email: david.erb@diamond.ac.uk
     project_urls:
         GitLab: https://github.com/diamondlightsource/chimpflow
     project_scripts:
         chimpflow: "chimpflow_lib.__main__:main"
@@ -17,8 +17,7 @@
               # TODO: Dependency should be on xchembku_api, not xchembku complete.
               - xchem-chimp
               - xchembku
               - dls_servbase
               - dls_mainiac
               - dls_multiconf
               - dls_utilpack
-              - requests
```

### Comparing `chimpflow-1.3.0/.devcontainer/Dockerfile` & `chimpflow-1.4.0/.devcontainer/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["chimpflow"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 5785b1775d09431a8a064cb67aa564cf
+# dae_devops_fingerprint 7d93d36ee7ace632caa5eb0c17a91b1f
```

### Comparing `chimpflow-1.3.0/.devcontainer/devcontainer.json` & `chimpflow-1.4.0/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.2.
+// ********** It has been generated automatically by dae_devops version 0.5.3.
 // ********** For repository_name chimpflow
 
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "Dockerfile",
@@ -53,8 +53,8 @@
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
     "postCreateCommand": "pip install -e .[dev]"
 }
 
-// dae_devops_fingerprint 045d41997d413a169ed082821ce0dccf
+// dae_devops_fingerprint c663450ade9da0f217afbaa7770a418a
```

### Comparing `chimpflow-1.3.0/.github/CONTRIBUTING.rst` & `chimpflow-1.4.0/.github/CONTRIBUTING.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name chimpflow
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/chimpflow/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 303160a2b536f20a8c1a1ec134e82f71
+.. # dae_devops_fingerprint e109cdf66466d29dc10364ab076c97f3
```

### Comparing `chimpflow-1.3.0/.github/actions/install_requirements/action.yml` & `chimpflow-1.4.0/.github/actions/install_requirements/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 name: Install requirements
 description: Run pip install with requirements and upload resulting requirements
 inputs:
   requirements_file:
     description: Name of requirements file to use and upload
@@ -57,8 +57,8 @@
             echo "Error: ${{ inputs.requirements_file }} need the above changes to be exhaustive"
             exit 1
           fi
         fi
       shell: bash
 
 
-# dae_devops_fingerprint e7e586c2794a8c6979edef0f62c7ba89
+# dae_devops_fingerprint d0dc7cda2625644ebd227600a40b9b87
```

### Comparing `chimpflow-1.3.0/.github/dependabot.yml` & `chimpflow-1.4.0/.github/dependabot.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 # To get started with Dependabot version updates, you'll need to specify which
 # package ecosystems to update and where the package manifests are located.
 # Please see the documentation for all configuration options:
 # https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates
 
@@ -15,8 +15,8 @@
       interval: "weekly"
 
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
       interval: "weekly"
 
-# dae_devops_fingerprint f732df8e00cb502c9de0f1a614c9351e
+# dae_devops_fingerprint b6ca8f2a21711ee2c5f52928628a3eaf
```

### Comparing `chimpflow-1.3.0/.github/pages/make_switcher.py` & `chimpflow-1.4.0/.github/pages/make_switcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
@@ -98,8 +98,8 @@
     versions = get_versions("origin/gh-pages", args.add, args.remove)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
 
-# dae_devops_fingerprint bf1e6514a2184d0710558edb524fb309
+# dae_devops_fingerprint 3dc2f67ed5164090274eaaa1ec757290
```

### Comparing `chimpflow-1.3.0/.github/workflows/code.yml` & `chimpflow-1.4.0/.github/workflows/code.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -35,21 +35,16 @@
 
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python: ["3.10", "3.11"]
+        python: ["3.10"]
         install: ["-e .[dev,docs]"]
-        # Make one version be non-editable to test both paths of version code
-        include:
-          - os: "ubuntu-latest"
-            python: "3.9"
-            install: ".[dev,docs]"
 
     runs-on: ${{ matrix.os }}
     env:
       # https://github.com/pytest-dev/pytest/issues/2042
       PY_IGNORE_IMPORTMISMATCH: "1"
 
     steps:
@@ -65,14 +60,18 @@
           python_version: ${{ matrix.python }}
           requirements_file: requirements-test-${{ matrix.os }}-${{ matrix.python }}.txt
           install_options: ${{ matrix.install }}
 
       - name: List dependency tree
         run: pipdeptree
 
+      # TODO: Make startup of MySQL able to be configured.
+      - name: Start up the MySQL that comes with Unbuntu
+        run: sudo /etc/init.d/mysql start
+
       - name: Run tests
         run: |
           sudo apt install environment-modules
           export MODULESHOME=/usr/share/modules
           source $MODULESHOME/init/bash
           pytest
 
@@ -208,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint 618b4ddc2d21af6824e6444a1c40caa7
+# dae_devops_fingerprint 8bfd4754775b0f120cc9aaf3baa87f5d
```

### Comparing `chimpflow-1.3.0/.github/workflows/docs.yml` & `chimpflow-1.4.0/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 name: Docs CI
 
 on:
   push:
   pull_request:
@@ -52,8 +52,8 @@
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
         uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
 
-# dae_devops_fingerprint a146e4a2bb02a7386ed24898b5d29200
+# dae_devops_fingerprint b4232ae6fae06078f660c3d8e9e17de8
```

### Comparing `chimpflow-1.3.0/.github/workflows/docs_clean.yml` & `chimpflow-1.4.0/.github/workflows/docs_clean.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 name: Docs Cleanup CI
 
 # delete branch documentation when a branch is deleted
 # also allow manually deleting a documentation version
 on:
@@ -42,8 +42,8 @@
           rm -r $DOCS_VERSION
           python make_switcher.py --remove $DOCS_VERSION ${{ github.repository }} switcher.json
           git config --global user.name 'GitHub Actions Docs Cleanup CI'
           git config --global user.email 'GithubActionsCleanup@noreply.github.com'
           git commit -am "Removing redundant docs version $DOCS_VERSION"
           git push
 
-# dae_devops_fingerprint 9d06f858b84de2523c688330e687075b
+# dae_devops_fingerprint 75becafa6319ee221942a3f56df14baa
```

### Comparing `chimpflow-1.3.0/.gitignore` & `chimpflow-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/.gitlab-ci.yml` & `chimpflow-1.4.0/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -83,8 +83,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint 8ef619190b6341d741696f65e16ef3d5
+# dae_devops_fingerprint e989098c901515f755ea8e5f066d81e8
```

### Comparing `chimpflow-1.3.0/.vscode/launch.json` & `chimpflow-1.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/LICENSE` & `chimpflow-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/PKG-INFO` & `chimpflow-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.3.0
-Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
+Version: 1.4.0
+Summary: Service which polls the database for subwell images which need to have the chimp detector run on them.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,36 +204,29 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://github.com/diamondlightsource/chimpflow/chimpflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 chimpflow
 =======================================================================
 
-XChem Business Knowledge Unit.  Service, Client, API, persistent store.
+Service which polls the database for subwell images which need to have the chimp detector run on them.
 
-Installation
------------------------------------------------------------------------
-::
-
-    pip install chimpflow
-
-    chimpflow --version
+Uses xchembku for database interaction.
 
+For documentation see: https://diamondlightsource.github.io/chimpflow
 
 
 Model file for xchem-chimp
 -----------------------------------------------------------------------
 
 The model file is saved in::
 
@@ -243,33 +236,7 @@
 This file is too large for github.
 
 For GitHub pytest to find the file in its CI/CD Actions, this file has been uploaded to zenodo:
 
     https://zenodo.org/record/7810708/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch
 
 The tests/conftest.py fetches this file automatically.
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/chimpflow for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/bxflow/chimpflow.git 
-    cd chimpflow
-    virtualenv /scratch/$USER/venv/chimpflow
-    source /scratch/$USER/venv/chimpflow/bin/activate 
-    pip install -e .[dev]
-    make -f .chimpflow/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/chimpflow/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
-
```

### Comparing `chimpflow-1.3.0/configurations/development.yaml` & `chimpflow-1.4.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/docs/conf.py` & `chimpflow-1.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "chimpflow",
     "$" + "{package_name}": "chimpflow_lib",
     "$" + "{git_url}": "https://github.com/diamondlightsource/chimpflow",
-    "$" + "{python_version_at_least}": "3.9",
+    "$" + "{python_version_at_least}": "3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint b80ddf31fa2e6cb77cfd3f049739c5c3
+# dae_devops_fingerprint 2454d977ead961b176ee3b27ab8bf6ef
```

### Comparing `chimpflow-1.3.0/docs/images/dls-favicon.ico` & `chimpflow-1.4.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/docs/images/dls-logo.svg` & `chimpflow-1.4.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/pyproject.toml` & `chimpflow-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name chimpflow
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chimpflow"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
 ]
-description = "XChem Business Knowledge Unit. Service, Client, API, persistent store."
-dependencies = ["xchem-chimp", "xchembku", "dls_servbase", "dls_mainiac", "dls_multiconf", "dls_utilpack", "requests"]
+description = "Service which polls the database for subwell images which need to have the chimp detector run on them."
+dependencies = ["xchem-chimp", "xchembku", "dls_servbase", "dls_mainiac", "dls_multiconf", "dls_utilpack"]
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
-requires-python = ">=3.9"
+readme = "README.md"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
     "black==22.12.0",
     "mypy",
     "flake8-isort",
     "Flake8-pyproject",
@@ -99,8 +97,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 6a9a79b1bad8cb6709ce1e2c603b64b0
+# dae_devops_fingerprint 40e120808487c93f2e5299ac8d1ae3c0
```

### Comparing `chimpflow-1.3.0/src/chimpflow.egg-info/PKG-INFO` & `chimpflow-1.4.0/src/chimpflow.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.3.0
-Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
+Version: 1.4.0
+Summary: Service which polls the database for subwell images which need to have the chimp detector run on them.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,36 +204,29 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://github.com/diamondlightsource/chimpflow/chimpflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 chimpflow
 =======================================================================
 
-XChem Business Knowledge Unit.  Service, Client, API, persistent store.
+Service which polls the database for subwell images which need to have the chimp detector run on them.
 
-Installation
------------------------------------------------------------------------
-::
-
-    pip install chimpflow
-
-    chimpflow --version
+Uses xchembku for database interaction.
 
+For documentation see: https://diamondlightsource.github.io/chimpflow
 
 
 Model file for xchem-chimp
 -----------------------------------------------------------------------
 
 The model file is saved in::
 
@@ -243,33 +236,7 @@
 This file is too large for github.
 
 For GitHub pytest to find the file in its CI/CD Actions, this file has been uploaded to zenodo:
 
     https://zenodo.org/record/7810708/2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch
 
 The tests/conftest.py fetches this file automatically.
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/chimpflow for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/bxflow/chimpflow.git 
-    cd chimpflow
-    virtualenv /scratch/$USER/venv/chimpflow
-    source /scratch/$USER/venv/chimpflow/bin/activate 
-    pip install -e .[dev]
-    make -f .chimpflow/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/chimpflow/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
-
```

### Comparing `chimpflow-1.3.0/src/chimpflow.egg-info/SOURCES.txt` & `chimpflow-1.4.0/src/chimpflow.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 LICENSE
-README.rst
+README.md
 pyproject.toml
 .dae-devops/Makefile
 .dae-devops/prepare_git_dependencies.sh
 .dae-devops/project.yaml
 .dae-devops/docs/conventions.rst
 .dae-devops/docs/developing.rst
 .dae-devops/docs/devops.rst
 .dae-devops/docs/docs_structure.rst
+.dae-devops/docs/documenting.rst
 .dae-devops/docs/installing.rst
 .dae-devops/docs/testing.rst
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/CONTRIBUTING.rst
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
@@ -28,38 +29,41 @@
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 configurations/development.yaml
 docs/conf.py
 docs/index.rst
 docs/_static/css/custom.css
+docs/explanations/conventions.rst
+docs/explanations/docs_structure.rst
+docs/explanations/index.rst
+docs/explanations/todo.rst
+docs/how-to/developing.rst
+docs/how-to/devops.rst
+docs/how-to/documenting.rst
+docs/how-to/index.rst
+docs/how-to/installing.rst
+docs/how-to/testing.rst
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
-docs/user/index.rst
-docs/user/explanations/22-developing.rst
-docs/user/explanations/23-testing.rst
-docs/user/explanations/24-devops.rst
-docs/user/explanations/25-docs-structure.rst
-docs/user/explanations/51-todo.rst
-docs/user/how-to/01-installing_development.rst
-docs/user/reference/api.rst
-docs/user/reference/api/classes.rst
-docs/user/reference/api/command_line.rst
-docs/user/reference/api/modules.rst
-docs/user/tutorials/tbd.rst
+docs/reference/classes.rst
+docs/reference/command_line.rst
+docs/reference/index.rst
+docs/reference/modules.rst
+docs/tutorials/index.rst
+docs/tutorials/tbd.rst
 src/chimpflow.egg-info/PKG-INFO
 src/chimpflow.egg-info/SOURCES.txt
 src/chimpflow.egg-info/dependency_links.txt
 src/chimpflow.egg-info/entry_points.txt
 src/chimpflow.egg-info/requires.txt
 src/chimpflow.egg-info/top_level.txt
 src/chimpflow_api/__init__.py
 src/chimpflow_api/aiohttp_client.py
 src/chimpflow_api/constants.py
-src/chimpflow_api/context_base.py
 src/chimpflow_api/exceptions.py
 src/chimpflow_api/thing.py
 src/chimpflow_api/things.py
 src/chimpflow_api/miners/__init__.py
 src/chimpflow_api/miners/aiohttp.py
 src/chimpflow_api/miners/constants.py
 src/chimpflow_api/miners/context.py
@@ -74,26 +78,25 @@
 src/chimpflow_lib/__main__.py
 src/chimpflow_lib/_version.py
 src/chimpflow_lib/base_aiohttp.py
 src/chimpflow_lib/chimp_adapter.py
 src/chimpflow_lib/envvar.py
 src/chimpflow_lib/exceptions.py
 src/chimpflow_lib/version.py
-src/chimpflow_lib/contexts/__init__.py
-src/chimpflow_lib/contexts/base.py
 src/chimpflow_lib/miners/__init__.py
 src/chimpflow_lib/miners/aiohttp.py
 src/chimpflow_lib/miners/base.py
 src/chimpflow_lib/miners/constants.py
 src/chimpflow_lib/miners/context.py
 src/chimpflow_lib/miners/direct_poll.py
 src/chimpflow_lib/miners/miners.py
 tests/__init__.py
 tests/base.py
 tests/conftest.py
 tests/test_chimp_adapter.py
 tests/test_miner.py
-tests/configurations/direct_poll.yaml
-tests/configurations/service.yaml
+tests/configurations/direct_sqlite.yaml
+tests/configurations/service_mysql.yaml
+tests/configurations/service_sqlite.yaml
 tests/echo_test_imgs/97wo_01A_1.jpg
 tests/echo_test_imgs/97wo_01A_2.jpg
 tests/echo_test_imgs/97wo_01A_3.jpg
```

### Comparing `chimpflow-1.3.0/src/chimpflow_api/exceptions.py` & `chimpflow-1.4.0/src/chimpflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_api/miners/aiohttp.py` & `chimpflow-1.4.0/src/chimpflow_api/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_api/miners/context.py` & `chimpflow-1.4.0/src/chimpflow_api/miners/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import logging
 
 # Base class.
-from chimpflow_api.context_base import ContextBase
+from dls_utilpack.client_context_base import ClientContextBase
 
 # Things created in the context.
 from chimpflow_api.miners.miners import Miners, chimpflow_miners_set_default
 
 logger = logging.getLogger(__name__)
 
 
-class Context(ContextBase):
+class Context(ClientContextBase):
     """
     Client context for a chimpflow_miner object.
     On entering, it creates the object according to the specification (a dict).
     On exiting, it closes client connection.
 
-    The aenter and aexit methods are exposed for use by an enclosing context.
+    The aenter and aexit methods are exposed for use by an enclosing context and the base class.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
-        ContextBase.__init__(self, specification)
+        ClientContextBase.__init__(self, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
         # Build the object according to the specification.
         self.interface = Miners().build_object(self.specification)
```

### Comparing `chimpflow-1.3.0/src/chimpflow_api/miners/miners.py` & `chimpflow-1.4.0/src/chimpflow_api/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_api/thing.py` & `chimpflow-1.4.0/src/chimpflow_api/thing.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_api/things.py` & `chimpflow-1.4.0/src/chimpflow_api/things.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_cli/main.py` & `chimpflow-1.4.0/src/chimpflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_cli/subcommands/base.py` & `chimpflow-1.4.0/src/chimpflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_cli/subcommands/service.py` & `chimpflow-1.4.0/src/chimpflow_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_cli/version.py` & `chimpflow-1.4.0/src/chimpflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/__main__.py` & `chimpflow-1.4.0/src/chimpflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/chimp_adapter.py` & `chimpflow-1.4.0/src/chimpflow_lib/chimp_adapter.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/exceptions.py` & `chimpflow-1.4.0/src/chimpflow_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/miners/aiohttp.py` & `chimpflow-1.4.0/src/chimpflow_lib/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/miners/base.py` & `chimpflow-1.4.0/src/chimpflow_lib/miners/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/miners/context.py` & `chimpflow-1.4.0/src/chimpflow_lib/miners/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 from typing import Dict
 
-# Base class for an asyncio context.
-from chimpflow_lib.contexts.base import Base as ContextBase
+# Base class for an asyncio server context.
+from dls_utilpack.server_context_base import ServerContextBase
 
 # Things created in the context.
-from chimpflow_lib.miners.miners import Miners, miners_set_default
+from chimpflow_lib.miners.miners import Miners
 
 logger = logging.getLogger(__name__)
 
 
 thing_type = "chimpflow_lib.miners.context"
 
 
-class Context(ContextBase):
+class Context(ServerContextBase):
     """
     Asyncio context for a miner object.
     On entering, it creates the object according to the specification (a dict).
     If specified, it starts the server as a coroutine, thread or process.
     If not a server, then it will instatiate a direct access to a miner.
     On exiting, it commands the server to shut down and/or releases the direct access resources.
     """
@@ -25,35 +25,32 @@
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification: Dict):
         """
         Constructor.
 
         Args:
             specification (Dict): specification of the miner object to be constructed within the context.
-                The only key in the specification that relates to the context is "start_as", which can be "coro", "thread", "process" or None.
+                The only key in the specification that relates to the context is "start_as", which can be "coro", "thread", "process", "direct", or None.
                 All other keys in the specification relate to creating the miner object.
         """
-        ContextBase.__init__(self, thing_type, specification)
+        ServerContextBase.__init__(self, thing_type, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self) -> None:
         """
         Asyncio context entry.
 
         Starts and activates service as specified.
 
         Establishes the global (singleton-like) default miner.
         """
 
         # Build the object according to the specification.
         self.server = Miners().build_object(self.specification())
 
-        # If there is more than one miner, the last one defined will be the default.
-        miners_set_default(self.server)
-
         if self.context_specification.get("start_as") == "coro":
             await self.server.activate_coro()
 
         elif self.context_specification.get("start_as") == "thread":
             await self.server.start_thread()
 
         elif self.context_specification.get("start_as") == "process":
@@ -61,28 +58,24 @@
 
         # Not running as a service?
         elif self.context_specification.get("start_as") == "direct":
             # We need to activate the tick() task.
             await self.server.activate()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self) -> None:
+    async def aexit(self, type, value, traceback) -> None:
         """
         Asyncio context exit.
 
         Stop service if one was started and releases any client resources.
         """
 
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
-                logger.info(
-                    "[DISSHU] in context exit, sending shutdown to client process"
-                )
                 # Put in request to shutdown the server.
                 await self.server.client_shutdown()
-                logger.info("[DISSHU] in context exit, sent shutdown to client process")
 
             if self.context_specification.get("start_as") == "coro":
                 await self.server.direct_shutdown()
 
             if self.context_specification.get("start_as") == "direct":
                 await self.server.deactivate()
```

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/miners/direct_poll.py` & `chimpflow-1.4.0/src/chimpflow_lib/miners/direct_poll.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/miners/miners.py` & `chimpflow-1.4.0/src/chimpflow_lib/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/src/chimpflow_lib/version.py` & `chimpflow-1.4.0/src/chimpflow_lib/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/tests/base.py` & `chimpflow-1.4.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/tests/configurations/service.yaml` & `chimpflow-1.4.0/tests/configurations/service_mysql.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -11,24 +11,47 @@
         enabled: False
         host: 172.23.7.128
         port: 12201
         protocol: UDP
 
 # The external access bits.
 external_access_bits:
-    dataface_port: &CHIMPFLOW_PORT 27821
+    xchembku_dataface_server: &XCHEMBKU_DATAFACE_SERVER http://*:27821
+    xchembku_dataface_client: &XCHEMBKU_DATAFACE_CLIENT http://localhost:27821
+    chimpflow_miner_server: &CHIMPFLOW_MINER_SERVER http://*:27825
+    chimpflow_miner_client: &CHIMPFLOW_MINER_CLIENT http://localhost:27825
 
+# -----------------------------------------------------------------------------
 # The xchembku_dataface direct access.
-xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
+xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     type: "xchembku_lib.xchembku_datafaces.direct"
+    should_drop_database: True
     database:
-        type: "xchembku_lib.xchembku_databases.normsql"
-        filename: "${output_directory}/xchembku.sqlite"
-        log_level: "WARNING"
+        type: "dls_normsql.aiomysql"
+        type_specific_tbd:
+            database_name: "xchembku_pytest"
+            host: $MYSQL_HOST
+            port: $MYSQL_PORT
+            username: "root"
+            password: "root"
+
+# The xchembku_dataface client/server composite.
+xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
+    type: "xchembku_lib.xchembku_datafaces.aiohttp"
+    type_specific_tbd:
+        # The remote xchembku_dataface server access.
+        aiohttp_specification:
+            server: *XCHEMBKU_DATAFACE_SERVER
+            client: *XCHEMBKU_DATAFACE_CLIENT
+        # The local implementation of the xchembku_dataface.
+        actual_xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
+    context:
+        start_as: process
 
+# -----------------------------------------------------------------------------
 # The chimpflow direct access.
 chimpflow_miner_specification_direct_poll:
     &CHIMPFLOW_COLLECTOR_SPECIFICATION_DIRECT_POLL
     type: "chimpflow_lib.miners.direct_poll"
     type_specific_tbd:
         chimp_adapter:
             # In pytest conftest.py, this file gets downloaded from Zenodo.
@@ -38,14 +61,13 @@
 
 # The chimpflow client/server composite.
 chimpflow_miner_specification:
     type: "chimpflow_lib.miners.aiohttp"
     type_specific_tbd:
         # The remote chimpflow server access.
         aiohttp_specification:
-            server_host: "*"
-            client_host: "127.0.0.1"
-            port: *CHIMPFLOW_PORT
+            server: *CHIMPFLOW_MINER_SERVER
+            client: *CHIMPFLOW_MINER_CLIENT
         # The local implementation of the chimpflow.
         direct_miner_specification: *CHIMPFLOW_COLLECTOR_SPECIFICATION_DIRECT_POLL
     context:
         start_as: process
```

### Comparing `chimpflow-1.3.0/tests/conftest.py` & `chimpflow-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/tests/echo_test_imgs/97wo_01A_1.jpg` & `chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_1.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/tests/echo_test_imgs/97wo_01A_2.jpg` & `chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_2.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/tests/echo_test_imgs/97wo_01A_3.jpg` & `chimpflow-1.4.0/tests/echo_test_imgs/97wo_01A_3.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/tests/test_chimp_adapter.py` & `chimpflow-1.4.0/tests/test_chimp_adapter.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.3.0/tests/test_miner.py` & `chimpflow-1.4.0/tests/test_miner.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import logging
 import multiprocessing
 import os
 import time
 
 # Crystal plate constants.
 from xchembku_api.crystal_plate_objects.constants import ThingTypes
-from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 
 # Things xchembku provides.
+from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 from xchembku_api.models.crystal_well_model import CrystalWellModel
+from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from chimpflow_api.miners.context import Context as MinerClientContext
 
 # Server context creator.
 from chimpflow_lib.miners.context import Context as MinerServerContext
 
@@ -31,15 +32,15 @@
     """
     Test miner interface by direct call.
     """
 
     def test(self, constants, logging_setup, output_directory):
 
         # Configuration file to use.
-        configuration_file = "tests/configurations/direct_poll.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
 
         # Do the work in a separate process so that the Service test
         # can also be run in the same pytest invocation.
         # TODO: Figure out how to release resources from torchvision in process.
         p = multiprocessing.Process(
             target=self.__process,
             args=[constants, configuration_file, output_directory],
@@ -50,23 +51,37 @@
     # ----------------------------------------------------------------------------------------
     def __process(self, constants, configuration_file, output_directory):
 
         MinerTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
-class TestMinerService:
+class TestMinerServiceSqlite:
     """
     Test miner interface through network interface.
     """
 
     def test(self, constants, logging_setup, output_directory):
 
         # Configuration file to use.
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+
+        MinerTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestMinerServiceMysql:
+    """
+    Test miner interface through network interface.
+    """
+
+    def test(self, constants, logging_setup, output_directory):
+
+        # Configuration file to use.
+        configuration_file = "tests/configurations/service_mysql.yaml"
 
         MinerTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class MinerTester(Base):
     """
@@ -84,35 +99,41 @@
         multiconf_dict = await multiconf.load()
 
         # Reference the dict entry for the xchembku dataface.
         xchembku_dataface_specification = multiconf_dict[
             "xchembku_dataface_specification"
         ]
 
-        # Reference the dict entry for the xchembku dataface.
+        # Make the xchembku server context.
+        xchembku_server_context = XchembkuDatafaceServerContext(
+            xchembku_dataface_specification
+        )
+        # Make the xchembku client context.
         xchembku_client_context = XchembkuDatafaceClientContext(
             xchembku_dataface_specification
         )
 
         miner_specification = multiconf_dict["chimpflow_miner_specification"]
         # Make the server context.
         miner_server_context = MinerServerContext(miner_specification)
 
         # Make the client context.
         miner_client_context = MinerClientContext(miner_specification)
 
         image_count = 1
 
-        # Start the client context for the direct access to the xchembku.
+        # Start the client context for the remote access to the xchembku.
         async with xchembku_client_context:
-            # Start the matching xchembku client context.
-            async with miner_client_context:
-                # Start the miner server context.
-                async with miner_server_context:
-                    await self.__run_part1(image_count, constants, output_directory)
+            # Start the server context xchembku which starts the process.
+            async with xchembku_server_context:
+                # Start the miner client context.
+                async with miner_client_context:
+                    # Start the miner server context.
+                    async with miner_server_context:
+                        await self.__run_part1(image_count, constants, output_directory)
 
     # ----------------------------------------------------------------------------------------
 
     async def __run_part1(self, image_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
```

