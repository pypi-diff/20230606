# Comparing `tmp/xchembku-1.8.0.tar.gz` & `tmp/xchembku-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.8.0.tar", last modified: Fri May 26 10:46:39 2023, max compression
+gzip compressed data, was "xchembku-1.9.1.tar", last modified: Tue Jun  6 04:48:55 2023, max compression
```

## Comparing `xchembku-1.8.0.tar` & `xchembku-1.9.1.tar`

### file list

```diff
@@ -1,156 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.478142 xchembku-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-26 10:46:28.000000 xchembku-1.8.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-26 10:46:28.000000 xchembku-1.8.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.450141 xchembku-1.8.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-26 10:46:28.000000 xchembku-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-26 10:46:28.000000 xchembku-1.8.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 10:46:28.000000 xchembku-1.8.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 10:46:28.000000 xchembku-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-26 10:46:39.478142 xchembku-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-26 10:46:28.000000 xchembku-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-26 10:46:28.000000 xchembku-1.8.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.450141 xchembku-1.8.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-26 10:46:28.000000 xchembku-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:46:39.478142 xchembku-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.454141 xchembku-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_plate_report_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17383 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.478142 xchembku-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.478142 xchembku-1.8.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/direct_mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/direct_sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/service_mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/service_sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_plate_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_well_droplocation1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_well_droplocation2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_soakdb3_crystal_well.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.205511 xchembku-1.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.181511 xchembku-1.9.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.185511 xchembku-1.9.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-06 04:48:45.000000 xchembku-1.9.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.185511 xchembku-1.9.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-06 04:48:45.000000 xchembku-1.9.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-06 04:48:45.000000 xchembku-1.9.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.185511 xchembku-1.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.177511 xchembku-1.9.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.185511 xchembku-1.9.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.185511 xchembku-1.9.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.185511 xchembku-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-06 04:48:45.000000 xchembku-1.9.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-06 04:48:45.000000 xchembku-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-06 04:48:45.000000 xchembku-1.9.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 04:48:45.000000 xchembku-1.9.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.185511 xchembku-1.9.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 04:48:45.000000 xchembku-1.9.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 04:48:45.000000 xchembku-1.9.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 04:48:45.000000 xchembku-1.9.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 04:48:45.000000 xchembku-1.9.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 04:48:45.000000 xchembku-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-06-06 04:48:55.201511 xchembku-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-06 04:48:45.000000 xchembku-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-06 04:48:45.000000 xchembku-1.9.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.177511 xchembku-1.9.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.189511 xchembku-1.9.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-06 04:48:45.000000 xchembku-1.9.1/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-06 04:48:45.000000 xchembku-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 04:48:55.205511 xchembku-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.181511 xchembku-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.193511 xchembku-1.9.1/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-06-06 04:48:55.000000 xchembku-1.9.1/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-06 04:48:55.000000 xchembku-1.9.1/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 04:48:55.000000 xchembku-1.9.1/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 04:48:55.000000 xchembku-1.9.1/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-06 04:48:55.000000 xchembku-1.9.1/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 04:48:55.000000 xchembku-1.9.1/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.193511 xchembku-1.9.1/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.193511 xchembku-1.9.1/src/xchembku_api/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/crystal_plate_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/crystal_plate_objects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/crystal_plate_objects/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.193511 xchembku-1.9.1/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.193511 xchembku-1.9.1/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12365 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.197511 xchembku-1.9.1/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_plate_report_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.197511 xchembku-1.9.1/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.197511 xchembku-1.9.1/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.197511 xchembku-1.9.1/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 04:48:55.000000 xchembku-1.9.1/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.197511 xchembku-1.9.1/src/xchembku_lib/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/crystal_plate_objects/swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.201511 xchembku-1.9.1/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-06 04:48:45.000000 xchembku-1.9.1/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.201511 xchembku-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 04:48:55.201511 xchembku-1.9.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/configurations/direct_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/configurations/direct_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/configurations/service_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/configurations/service_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/test_crystal_plate_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/test_crystal_well_droplocation1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/test_crystal_well_droplocation2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/test_soakdb3_crystal_well.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-06 04:48:45.000000 xchembku-1.9.1/tests/test_swiss3.py
```

### Comparing `xchembku-1.8.0/.dae-devops/Makefile` & `xchembku-1.9.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.dae-devops/docs/conventions.rst` & `xchembku-1.9.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.dae-devops/docs/developing.rst` & `xchembku-1.9.1/.dae-devops/docs/developing.rst`

 * *Files 11% similar despite different names*

```diff
@@ -5,34 +5,27 @@
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
+    $ cd <your development area>
     $ git clone https://github.com/diamondlightsource/xchembku/xchembku.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
-Make sure to have at least python version 3.9 then::
+Make sure to have at least python version 3.10 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd xchembku
-    $ pip install -e .[dev]
+    $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
-|
 
-If you plan to modify the docs, you will need to::
-
-    $ pip install -e .[docs]
-
-    
-
-
-.. # dae_devops_fingerprint b8e50fbfb03247dcba32527a1bce43ac
+.. # dae_devops_fingerprint 7ed6884248b751dc449fb414a1ca82e1
```

### Comparing `xchembku-1.8.0/.dae-devops/docs/devops.rst` & `xchembku-1.9.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.dae-devops/docs/docs_structure.rst` & `xchembku-1.9.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.dae-devops/docs/installing.rst` & `xchembku-1.9.1/.dae-devops/docs/installing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 .. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
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
 
     $ python3 -m pip install xchembku
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://github.com/diamondlightsource/xchembku/xchembku.git
 
-The library should now be installed and the commandline should be available.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ xchembku --version
     $ xchembku --version-json
 
-.. # dae_devops_fingerprint b0dd26d8e2897f65f63f81a16b0a8e29
+.. # dae_devops_fingerprint e17b07ee438d265975080254e6435145
```

### Comparing `xchembku-1.8.0/.dae-devops/docs/testing.rst` & `xchembku-1.9.1/.dae-devops/docs/testing.rst`

 * *Files 17% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 If you want to see more output of the test while it's running you can do::
 
     $ pytest -sv -ra --tb=line tests/the_test_you_want.py
 
 Each test will write files into its own directory::
 
-    /tmp/xchembku/tests/....
+    /tmp/xchembku/tests/*
 
 The tests clear their directory when they start, but not when they finish.
-This allows peeking in there to see what's been written by the test.
+This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint a8eba26c733cc75e40ad8560dd959093
+.. # dae_devops_fingerprint e60d69a5aa7ae4acb6ba6e90dcff15cb
```

### Comparing `xchembku-1.8.0/.dae-devops/project.yaml` & `xchembku-1.9.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.devcontainer/Dockerfile` & `xchembku-1.9.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.devcontainer/devcontainer.json` & `xchembku-1.9.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.github/CONTRIBUTING.rst` & `xchembku-1.9.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.github/actions/install_requirements/action.yml` & `xchembku-1.9.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.github/dependabot.yml` & `xchembku-1.9.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.github/pages/make_switcher.py` & `xchembku-1.9.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.github/workflows/code.yml` & `xchembku-1.9.1/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,14 @@
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
         python: ["3.10"]
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
@@ -212,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint b95f4d599ba467ac167ad6ea2a446537
+# dae_devops_fingerprint fd9227ec7552b75511373c7ecd644d4d
```

### Comparing `xchembku-1.8.0/.github/workflows/docs.yml` & `xchembku-1.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.github/workflows/docs_clean.yml` & `xchembku-1.9.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.github/workflows/linkcheck.yml` & `xchembku-1.9.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.gitignore` & `xchembku-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.gitlab-ci.yml` & `xchembku-1.9.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/.vscode/launch.json` & `xchembku-1.9.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/LICENSE` & `xchembku-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/PKG-INFO` & `xchembku-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.8.0
+Version: 1.9.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,19 +204,17 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://github.com/diamondlightsource/xchembku/xchembku
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
 
 xchembku
 =======================================================================
```

### Comparing `xchembku-1.8.0/README.rst` & `xchembku-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/configurations/development.yaml` & `xchembku-1.9.1/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/docs/conf.py` & `xchembku-1.9.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "xchembku",
     "$" + "{package_name}": "xchembku_lib",
     "$" + "{git_url}": "https://github.com/diamondlightsource/xchembku",
-    "$" + "{python_version_at_least}": "3.9",
+    "$" + "{python_version_at_least}": "3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 3e5f08df87ebb37ddf17572d476185a2
+# dae_devops_fingerprint c1c571c112da8688ea81070cffde5401
```

### Comparing `xchembku-1.8.0/docs/images/dls-favicon.ico` & `xchembku-1.9.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/docs/images/dls-logo.svg` & `xchembku-1.9.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/docs/index.rst` & `xchembku-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.9.1/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/docs/user/index.rst` & `xchembku-1.9.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/pyproject.toml` & `xchembku-1.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchembku"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
 ]
 description = "XChem Business Knowledge Unit. Service, Client, API, persistent store."
 dependencies = ["dls_servbase", "dls_mainiac", "dls_multiconf", "dls_utilpack", "soakdb3", "pydantic"]
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
 
-# dae_devops_fingerprint c6a28d0d6afaffc18e6857fe4c60799f
+# dae_devops_fingerprint 0e49b85fe4d7a2a5abd589d879846417
```

### Comparing `xchembku-1.8.0/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.9.1/src/xchembku.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.8.0
+Version: 1.9.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,19 +204,17 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://github.com/diamondlightsource/xchembku/xchembku
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
 
 xchembku
 =======================================================================
```

### Comparing `xchembku-1.8.0/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.9.1/src/xchembku.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

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
@@ -49,15 +50,14 @@
 src/xchembku.egg-info/SOURCES.txt
 src/xchembku.egg-info/dependency_links.txt
 src/xchembku.egg-info/entry_points.txt
 src/xchembku.egg-info/requires.txt
 src/xchembku.egg-info/top_level.txt
 src/xchembku_api/__init__.py
 src/xchembku_api/aiohttp_client.py
-src/xchembku_api/context_base.py
 src/xchembku_api/exceptions.py
 src/xchembku_api/crystal_plate_objects/__init__.py
 src/xchembku_api/crystal_plate_objects/constants.py
 src/xchembku_api/crystal_plate_objects/interface.py
 src/xchembku_api/databases/__init__.py
 src/xchembku_api/databases/constants.py
 src/xchembku_api/databases/database_definition.py
@@ -83,16 +83,14 @@
 src/xchembku_cli/subcommands/service.py
 src/xchembku_lib/__init__.py
 src/xchembku_lib/__main__.py
 src/xchembku_lib/_version.py
 src/xchembku_lib/base_aiohttp.py
 src/xchembku_lib/envvar.py
 src/xchembku_lib/version.py
-src/xchembku_lib/contexts/__init__.py
-src/xchembku_lib/contexts/base.py
 src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
 src/xchembku_lib/crystal_plate_objects/swiss3.py
 src/xchembku_lib/datafaces/__init__.py
 src/xchembku_lib/datafaces/aiohttp.py
 src/xchembku_lib/datafaces/context.py
 src/xchembku_lib/datafaces/datafaces.py
 src/xchembku_lib/datafaces/direct.py
```

### Comparing `xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/constants.py` & `xchembku-1.9.1/src/xchembku_api/crystal_plate_objects/constants.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/interface.py` & `xchembku-1.9.1/src/xchembku_api/crystal_plate_objects/interface.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/databases/database_definition.py` & `xchembku-1.9.1/src/xchembku_api/databases/database_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     # ----------------------------------------------------------------------------------------
     def __init__(self):
         """
         Construct object.  Do not connect to database.
         """
 
-        self.LATEST_REVISION = 4
+        self.LATEST_REVISION = 5
 
     # ----------------------------------------------------------------------------------------
     async def apply_revision(self, database, revision):
 
         logger.debug(f"applying revision {revision}")
 
         if revision == 3:
@@ -60,14 +60,21 @@
                     "crystal_well_droplocations",
                     "is_exported_to_soakdb3",
                     "crystal_well_droplocations",
                     "is_exported_to_soakdb3",
                 )
             )
 
+        if revision == 5:
+            # Add crytal plate error field.
+            await database.execute(
+                "ALTER TABLE crystal_plates ADD COLUMN error TEXT",
+                why="revision {revision}: new column",
+            )
+
     # ----------------------------------------------------------------------------------------
     async def add_table_definitions(self, database):
         """
         Make all the table definitions.
         """
 
         # Table schemas in our database.
```

### Comparing `xchembku-1.8.0/src/xchembku_api/databases/table_definitions.py` & `xchembku-1.9.1/src/xchembku_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.9.1/src/xchembku_api/datafaces/aiohttp.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,24 @@
             record,
             where,
             subs=subs,
             why=why,
         )
 
     # ----------------------------------------------------------------------------------------
+    async def commit(self, why: Optional[str] = None):
+        """
+        Commit is exposed on the API for use in testing when database states must be deterministic.
+        """
+        return await self.__send_protocolj(
+            "commit",
+            why=why,
+        )
+
+    # ----------------------------------------------------------------------------------------
     async def upsert_crystal_plates(
         self,
         models: List[CrystalPlateModel],
         why: Optional[str] = None,
     ) -> None:
         """"""
```

### Comparing `xchembku-1.8.0/src/xchembku_api/datafaces/context.py` & `xchembku-1.9.1/src/xchembku_api/datafaces/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 import logging
 
-from dls_utilpack.callsign import callsign
-
 # Base class.
-from xchembku_api.context_base import ContextBase
+from dls_utilpack.client_context_base import ClientContextBase
 
 # Things created in the context.
 from xchembku_api.datafaces.datafaces import Datafaces, xchembku_datafaces_set_default
 
 logger = logging.getLogger(__name__)
 
 
-class Context(ContextBase):
+class Context(ClientContextBase):
     """
     Client context for a xchembku_dataface object.
     On entering, it creates the object according to the specification (a dict).
     On exiting, it closes client connection.
 
-    The aenter and aexit methods are exposed for use by an enclosing context.
+    The aenter and aexit methods are exposed for use by an enclosing context and the base class.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
-        self.__specification = specification
+        ClientContextBase.__init__(self, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
         # Build the object according to the specification.
-        self.interface = Datafaces().build_object(self.__specification)
+        self.interface = Datafaces().build_object(self.specification)
 
         # If there is more than one dataface, the last one defined will be the default.
         xchembku_datafaces_set_default(self.interface)
 
         # Open client session to the service or direct connection.
         await self.interface.open_client_session()
 
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
-        logger.debug(f"[DISSHU] {callsign(self)} in aexit")
-
         if self.interface is not None:
-            logger.debug(
-                f"[DISSHU] {callsign(self)} calling close_client_session on {callsign(self.interface)}"
-            )
             # Close client session to the service or direct connection.
             await self.interface.close_client_session()
-            logger.debug(f"[DISSHU] {callsign(self)} called close_client_session")
 
             # Clear the global variable.  Important between pytests.
             xchembku_datafaces_set_default(None)
```

### Comparing `xchembku-1.8.0/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.9.1/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/exceptions.py` & `xchembku-1.9.1/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_plate_filter_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_plate_filter_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     """
     Model containing crystal plate query filter.
     """
 
     uuid: Optional[str] = None
     visit: Optional[str] = None
     barcode: Optional[str] = None
+    include_errors: Optional[bool] = None
     limit: Optional[int] = None
     direction: Optional[int] = None
 
     # Allow searching starting from a particular plate id.
     from_formulatrix__plate__id: Optional[int] = None
 
     # These choices are only used in the report query.
```

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_plate_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,26 +9,28 @@
     Model containing plate information.
 
     Typically this structure is populated and transmitted by the rockminer package.
     """
 
     uuid: str
     # ID from the Plate table.
-    formulatrix__plate__id: int
+    formulatrix__plate__id: Optional[int]
     # Name from the formulatrix "experiment" tree node.
     formulatrix__experiment__name: Optional[str]
     # Directory stem where wells were mined from.
     # Also used by echolocator to format the export csv filename.
     rockminer_collected_stem: Optional[str] = None
     # The 4-letter barcode.
     barcode: str
     # The visit gleaned from the Formulatrix database.
-    visit: str
+    visit: Optional[str]
     # A string which allows the CrytsalPlateObjects factory to make an instance.
     thing_type: Optional[str] = None
+    # Error string.
+    error: Optional[str] = None
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
         if "uuid" not in kwargs:
```

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_plate_report_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_plate_report_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_well_filter_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_well_filter_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.9.1/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_cli/main.py` & `xchembku-1.9.1/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_cli/subcommands/base.py` & `xchembku-1.9.1/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_cli/subcommands/service.py` & `xchembku-1.9.1/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_cli/version.py` & `xchembku-1.9.1/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/__main__.py` & `xchembku-1.9.1/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py` & `xchembku-1.9.1/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/swiss3.py` & `xchembku-1.9.1/src/xchembku_lib/crystal_plate_objects/swiss3.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/context.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
 
-# Base class for an asyncio context
-from xchembku_lib.contexts.base import Base as ContextBase
+# Base class for an asyncio server context.
+from dls_utilpack.server_context_base import ServerContextBase
 
 # Things created in the context.
 from xchembku_lib.datafaces.datafaces import Datafaces
 
 logger = logging.getLogger(__name__)
 
 
 thing_type = "xchembku_lib.xchembku_datafaces.context"
 
 
-class Context(ContextBase):
+class Context(ServerContextBase):
     """
     Asyncio context for a xchembku_dataface server object.
     On entering, it creates the object according to the specification (a dict).
     If configured, it starts the server as a coroutine, thread or process.
     On exiting, it commands the server to shut down.
 
     The enter and exit methods are exposed for use during testing.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
-        ContextBase.__init__(self, thing_type, specification)
+        ServerContextBase.__init__(self, thing_type, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
         # Build the object according to the specification.
         self.server = Datafaces().build_object(self.specification())
@@ -42,15 +42,15 @@
         elif self.context_specification.get("start_as") == "thread":
             await self.server.start_thread()
 
         elif self.context_specification.get("start_as") == "process":
             await self.server.start_process()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self):
+    async def aexit(self, type, value, traceback):
         """ """
 
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
                 # Put in request to shutdown the server.
                 await self.server.client_shutdown()
```

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/direct_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,32 @@
         return {
             "count": await self.__database.update(
                 table_name, record, where, subs=subs, why=why
             )
         }
 
     # ----------------------------------------------------------------------------------------
+    async def commit_serialized(
+        self,
+        why=None,
+    ) -> None:
+        """
+        Commit is exposed on the API for use in testing when database states must be deterministic.
+        """
+        # Return the method doing the work.
+        return await self.commit(why=why)
+
+    # ----------------------------------------------------------------------------------------
+    async def commit(self, why=None) -> None:
+        """"""
+        await self.establish_database_connection()
+
+        return await self.__database.commit()
+
+    # ----------------------------------------------------------------------------------------
     async def report_health(self):
         """"""
 
         report = {}
 
         report["alive"] = True
```

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,20 @@
             where = "AND"
 
         if filter.barcode is not None:
             sql += f"\n{where} barcode = ?"
             subs.append(filter.barcode)
             where = "AND"
 
+        if filter.barcode is None:
+            # Default, if not specified, is to exclude plates with errors.
+            if filter.include_errors is None or filter.include_errors is False:
+                sql += f"\n{where} error IS NULL"
+                where = "AND"
+
         if filter.from_formulatrix__plate__id is not None:
             if filter.direction == -1:
                 sql += f"\n{where} formulatrix__plate__id < ?"
             else:
                 sql += f"\n{where} formulatrix__plate__id > ?"
             subs.append(filter.from_formulatrix__plate__id)
             where = "AND"
```

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,28 @@
 
         return {
             "updated_count": updated_count,
             "inserted_count": inserted_count,
         }
 
     # ----------------------------------------------------------------------------------------
+    async def fetch_crystal_wells_filenames_serialized(
+        self, limit: int = 1, why=None
+    ) -> List[Dict]:
+        """ """
+
+        # Get the models from the direct call.
+        models = await self.fetch_crystal_wells_filenames(limit=limit, why=why)
+
+        # Serialize models into dicts to give to the response.
+        records = [model.dict() for model in models]
+
+        return records
+
+    # ----------------------------------------------------------------------------------------
     async def fetch_crystal_wells_filenames(
         self, limit: int = 1, why=None
     ) -> List[CrystalWellModel]:
         """
         Filenams for ALL wells ever.
         """
 
@@ -408,15 +422,15 @@
                 f"\n{where} crystal_well_droplocations.is_usable = True"
             )
             where = "AND"
 
         # Caller wants just the anchor record?
         if filter.anchor is not None and filter.direction is None:
             sql += (
-                "\n/* Get the crystal well at the anchor. */"
+                f"\n/* Get the crystal well at the anchor {filter.anchor}. */"
                 f"\n{where} crystal_wells.uuid = ?"
             )
             subs.append(filter.anchor)
             where = "AND"
 
         # Caller wants those in direction from the anchor record?
         # This means we ne need the anchor to be in the rows,
```

### Comparing `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py` & `xchembku-1.9.1/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/src/xchembku_lib/version.py` & `xchembku-1.9.1/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/base.py` & `xchembku-1.9.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/configurations/direct_mysql.yaml` & `xchembku-1.9.1/tests/configurations/direct_mysql.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/configurations/direct_sqlite.yaml` & `xchembku-1.9.1/tests/configurations/direct_sqlite.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/configurations/service_mysql.yaml` & `xchembku-1.9.1/tests/configurations/service_sqlite.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         enabled: False
         host: 172.23.7.128
         port: 12201
         protocol: UDP
 
 # The external access bits.
 external_access_bits:
-    dataface_port: &DATAFACE_PORT 27821
+    xchembku_dataface_server: &XCHEMBKU_DATAFACE_SERVER http://*:27821
+    xchembku_dataface_client: &XCHEMBKU_DATAFACE_CLIENT http://localhost:27821
     soakdb3_dataface_server: &SOAKDB3_DATAFACE_SERVER http://*:27824
     soakdb3_dataface_client: &SOAKDB3_DATAFACE_CLIENT http://localhost:27824
     soakdb3_puck_barcodes_filename: &SOAKDB3_PUCK_BARCODES_FILENAME /dls/science/groups/i04-1/software/barcode-store/store/store.csv
 
 # -----------------------------------------------------------------------------
 # The soakdb3 dataface via direct.
 soakdb3_dataface_specification_direct: &SOAKDB3_DATAFACE_SPECIFICATION_DIRECT
@@ -64,30 +65,24 @@
         start_as: process
 
 # -----------------------------------------------------------------------------
 # The xchembku_dataface direct access.
 xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     type: "xchembku_lib.xchembku_datafaces.direct"
     soakdb3_dataface_specification: *SOAKDB3_DATAFACE_SPECIFICATION
-    should_drop_database: True
     database:
-        type: "dls_normsql.aiomysql"
-        type_specific_tbd:
-            database_name: "xchembku_pytest"
-            host: $MYSQL_HOST
-            port: $MYSQL_PORT
-            username: "root"
-            password: "root"
+        type: "dls_normsql.aiosqlite"
+        filename: "${output_directory}/xchembku_dataface.sqlite"
+        log_level: "WARNING"
 
 # The xchembku_dataface client/server composite.
 xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
     type: "xchembku_lib.xchembku_datafaces.aiohttp"
     type_specific_tbd:
         # The remote xchembku_dataface server access.
         aiohttp_specification:
-            server_host: "*"
-            client_host: "127.0.0.1"
-            port: *DATAFACE_PORT
+            server: *XCHEMBKU_DATAFACE_SERVER
+            client: *XCHEMBKU_DATAFACE_CLIENT
         # The local implementation of the xchembku_dataface.
         actual_xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     context:
         start_as: process
```

### Comparing `xchembku-1.8.0/tests/configurations/service_sqlite.yaml` & `xchembku-1.9.1/tests/configurations/service_mysql.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         enabled: False
         host: 172.23.7.128
         port: 12201
         protocol: UDP
 
 # The external access bits.
 external_access_bits:
-    dataface_port: &DATAFACE_PORT 27821
+    xchembku_dataface_server: &XCHEMBKU_DATAFACE_SERVER http://*:27821
+    xchembku_dataface_client: &XCHEMBKU_DATAFACE_CLIENT http://localhost:27821
     soakdb3_dataface_server: &SOAKDB3_DATAFACE_SERVER http://*:27824
     soakdb3_dataface_client: &SOAKDB3_DATAFACE_CLIENT http://localhost:27824
     soakdb3_puck_barcodes_filename: &SOAKDB3_PUCK_BARCODES_FILENAME /dls/science/groups/i04-1/software/barcode-store/store/store.csv
 
 # -----------------------------------------------------------------------------
 # The soakdb3 dataface via direct.
 soakdb3_dataface_specification_direct: &SOAKDB3_DATAFACE_SPECIFICATION_DIRECT
@@ -64,25 +65,29 @@
         start_as: process
 
 # -----------------------------------------------------------------------------
 # The xchembku_dataface direct access.
 xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     type: "xchembku_lib.xchembku_datafaces.direct"
     soakdb3_dataface_specification: *SOAKDB3_DATAFACE_SPECIFICATION
+    should_drop_database: True
     database:
-        type: "dls_normsql.aiosqlite"
-        filename: "${output_directory}/xchembku_dataface.sqlite"
-        log_level: "WARNING"
+        type: "dls_normsql.aiomysql"
+        type_specific_tbd:
+            database_name: "xchembku_pytest"
+            host: $MYSQL_HOST
+            port: $MYSQL_PORT
+            username: "root"
+            password: "root"
 
 # The xchembku_dataface client/server composite.
 xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
     type: "xchembku_lib.xchembku_datafaces.aiohttp"
     type_specific_tbd:
         # The remote xchembku_dataface server access.
         aiohttp_specification:
-            server_host: "*"
-            client_host: "127.0.0.1"
-            port: *DATAFACE_PORT
+            server: *XCHEMBKU_DATAFACE_SERVER
+            client: *XCHEMBKU_DATAFACE_CLIENT
         # The local implementation of the xchembku_dataface.
         actual_xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     context:
         start_as: process
```

### Comparing `xchembku-1.8.0/tests/conftest.py` & `xchembku-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/test_crystal_plate.py` & `xchembku-1.9.1/tests/test_crystal_plate.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/test_crystal_plate_report.py` & `xchembku-1.9.1/tests/test_crystal_plate_report.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/test_crystal_well_autolocation.py` & `xchembku-1.9.1/tests/test_crystal_well_autolocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/test_crystal_well_droplocation1.py` & `xchembku-1.9.1/tests/test_crystal_well_droplocation1.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/test_crystal_well_droplocation2.py` & `xchembku-1.9.1/tests/test_crystal_well_droplocation2.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/test_soakdb3_crystal_well.py` & `xchembku-1.9.1/tests/test_soakdb3_crystal_well.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.8.0/tests/test_swiss3.py` & `xchembku-1.9.1/tests/test_swiss3.py`

 * *Files identical despite different names*

