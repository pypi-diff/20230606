# Comparing `tmp/rockingester-2.3.0.tar.gz` & `tmp/rockingester-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-2.3.0.tar", last modified: Wed May 17 17:46:18 2023, max compression
+gzip compressed data, was "rockingester-3.0.1.tar", last modified: Tue Jun  6 11:16:53 2023, max compression
```

## Comparing `rockingester-2.3.0.tar` & `rockingester-3.0.1.tar`

### file list

```diff
@@ -1,128 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.013771 rockingester-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-17 17:46:06.000000 rockingester-2.3.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-17 17:46:06.000000 rockingester-2.3.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:17.993770 rockingester-2.3.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-17 17:46:06.000000 rockingester-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-17 17:46:06.000000 rockingester-2.3.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 17:46:06.000000 rockingester-2.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 17:46:06.000000 rockingester-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-17 17:46:18.013771 rockingester-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-17 17:46:06.000000 rockingester-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-17 17:46:06.000000 rockingester-2.3.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:17.997770 rockingester-2.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-17 17:46:06.000000 rockingester-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:46:18.013771 rockingester-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:17.997770 rockingester-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17957 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/test_platewait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.343670 rockingester-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-06 11:16:43.000000 rockingester-3.0.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-06 11:16:43.000000 rockingester-3.0.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-06 11:16:43.000000 rockingester-3.0.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-06 11:16:43.000000 rockingester-3.0.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-06 11:16:43.000000 rockingester-3.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-06 11:16:43.000000 rockingester-3.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 11:16:43.000000 rockingester-3.0.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 11:16:43.000000 rockingester-3.0.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 11:16:43.000000 rockingester-3.0.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 11:16:43.000000 rockingester-3.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 11:16:43.000000 rockingester-3.0.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 11:16:43.000000 rockingester-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-06 11:16:53.343670 rockingester-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-06 11:16:43.000000 rockingester-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-06 11:16:43.000000 rockingester-3.0.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 11:16:43.000000 rockingester-3.0.1/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-06 11:16:43.000000 rockingester-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:16:53.343670 rockingester-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.331670 rockingester-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.335671 rockingester-3.0.1/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-06 11:16:53.000000 rockingester-3.0.1/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-06 11:16:53.000000 rockingester-3.0.1/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:16:53.000000 rockingester-3.0.1/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-06 11:16:53.000000 rockingester-3.0.1/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-06 11:16:53.000000 rockingester-3.0.1/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 11:16:53.000000 rockingester-3.0.1/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.339671 rockingester-3.0.1/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.339671 rockingester-3.0.1/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.339671 rockingester-3.0.1/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.339671 rockingester-3.0.1/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.339671 rockingester-3.0.1/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 11:16:53.000000 rockingester-3.0.1/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.339671 rockingester-3.0.1/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/collectors/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/ftrix_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/plate_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-06 11:16:43.000000 rockingester-3.0.1/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.343670 rockingester-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:53.343670 rockingester-3.0.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/configurations/direct_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/configurations/service_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/configurations/service_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/test_ftrix_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/test_plate_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-06 11:16:43.000000 rockingester-3.0.1/tests/test_platewait.py
```

### Comparing `rockingester-2.3.0/.dae-devops/Makefile` & `rockingester-3.0.1/.dae-devops/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint 325d6369d86a2cdf15b3d6b37f5412ac
+# dae_devops_fingerprint 32d9f9bee979f4d231d6b05285af4325
```

### Comparing `rockingester-2.3.0/.dae-devops/docs/conventions.rst` & `rockingester-3.0.1/.dae-devops/docs/conventions.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name rockingester
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint 00ace00f0e95078b5c3b87f58d0d3d10
+.. # dae_devops_fingerprint 1afd29155db2cdc1ab01d6b6c1ac6b2a
```

### Comparing `rockingester-2.3.0/.dae-devops/docs/developing.rst` & `rockingester-3.0.1/.dae-devops/docs/developing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name rockingester
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
+    $ cd <your development area>
     $ git clone https://github.com/diamondlightsource/rockingester/rockingester.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
-Make sure to have at least python version 3.9 then::
+Make sure to have at least python version 3.10 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd rockingester
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
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
-.. # dae_devops_fingerprint 9ed81ab6cfb9cd8a6f7df3d6a8fce3eb
+.. # dae_devops_fingerprint 96d41b708572d1d5049fab9b6abfb97e
```

### Comparing `rockingester-2.3.0/.dae-devops/docs/docs_structure.rst` & `rockingester-3.0.1/.dae-devops/docs/docs_structure.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name rockingester
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint fe2e1c7c54f2d82f4b136eda337d6318
+.. # dae_devops_fingerprint 83174912089972e4482c01462d6d5d84
```

### Comparing `rockingester-2.3.0/.dae-devops/docs/installing.rst` & `rockingester-3.0.1/.dae-devops/docs/installing.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name rockingester
 
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
     $ python3 -m pip install rockingester
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://github.com/diamondlightsource/rockingester/rockingester.git
 
-The library should now be installed and the commandline interface on your path.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ rockingester --version
     $ rockingester --version-json
 
-.. # dae_devops_fingerprint 9cc5938e9a54e77f0bf42f7859b75140
+.. # dae_devops_fingerprint ce67a9b82ccbaa245e0bd24c65a8330b
```

### Comparing `rockingester-2.3.0/.dae-devops/docs/testing.rst` & `rockingester-3.0.1/.dae-devops/docs/testing.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name rockingester
 
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
 
-    /tmp/rockingester/tests/....
+    /tmp/rockingester/tests/*
 
 The tests clear their directory when they start, but not when they finish.
-This allows peeking in there to see what's been written by the test.
+This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint e291ebd21ffbd2fccba82caa307a9a10
+.. # dae_devops_fingerprint b457cd81683b7fef7394412f51fab19b
```

### Comparing `rockingester-2.3.0/.devcontainer/Dockerfile` & `rockingester-3.0.1/.devcontainer/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["rockingester"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 5107e2dc7615b1579db65b5ac08b3a91
+# dae_devops_fingerprint 35139fc4006e8d4d91cada0df5424ab7
```

### Comparing `rockingester-2.3.0/.devcontainer/devcontainer.json` & `rockingester-3.0.1/.devcontainer/devcontainer.json`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.2.
+// ********** It has been generated automatically by dae_devops version 0.5.3.
 // ********** For repository_name rockingester
 
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
 
-// dae_devops_fingerprint d0a924d4e21a12f3ca90dd5c5488155d
+// dae_devops_fingerprint d2bab2d133d445f053d48b13b8cd02ec
```

### Comparing `rockingester-2.3.0/.github/CONTRIBUTING.rst` & `rockingester-3.0.1/.github/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name rockingester
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/rockingester/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 6af4c15a85db612138b071dbd11dde21
+.. # dae_devops_fingerprint 8a36b439242bc5f2a7ed6519355db457
```

### Comparing `rockingester-2.3.0/.github/actions/install_requirements/action.yml` & `rockingester-3.0.1/.github/actions/install_requirements/action.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
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
 
 
-# dae_devops_fingerprint 99ff347e3797c535b265bf65347f69b1
+# dae_devops_fingerprint d48adc639a11ad9f4ef3a948cf0834e6
```

### Comparing `rockingester-2.3.0/.github/dependabot.yml` & `rockingester-3.0.1/.github/dependabot.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
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
 
-# dae_devops_fingerprint f5a7322640608fd00e582daea5f9b272
+# dae_devops_fingerprint 75ea7db79584e4d50fdfc7d140fe5381
```

### Comparing `rockingester-2.3.0/.github/pages/make_switcher.py` & `rockingester-3.0.1/.github/pages/make_switcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
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
 
-# dae_devops_fingerprint c58785ffd04f4bbcdcc6a3025f6e694e
+# dae_devops_fingerprint 5fbfeccf513ac4cfddda72c5285e0f4e
```

### Comparing `rockingester-2.3.0/.github/workflows/code.yml` & `rockingester-3.0.1/.github/workflows/code.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
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
 
-# dae_devops_fingerprint 7eb4f406a3bb52db3bb72e10d546a524
+# dae_devops_fingerprint 449a11e129ac6256bbac38eb0389b13a
```

### Comparing `rockingester-2.3.0/.github/workflows/docs.yml` & `rockingester-3.0.1/.github/workflows/docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
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
 
-# dae_devops_fingerprint 2fc180c8643dbf1692bd9e0819a0335e
+# dae_devops_fingerprint f1faeb67a6fa9307068958663b485f24
```

### Comparing `rockingester-2.3.0/.github/workflows/docs_clean.yml` & `rockingester-3.0.1/.github/workflows/docs_clean.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
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
 
-# dae_devops_fingerprint c9ae67b812184877e541e0abdd8244dd
+# dae_devops_fingerprint 4fedcc7106c9b0c6484db857449564c2
```

### Comparing `rockingester-2.3.0/.gitignore` & `rockingester-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/.gitlab-ci.yml` & `rockingester-3.0.1/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
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
 
-# dae_devops_fingerprint bad18a3b7cc867275610b56fff20dab4
+# dae_devops_fingerprint 65c8ba2b89f0dcde052aaec3f1684f62
```

### Comparing `rockingester-2.3.0/.vscode/launch.json` & `rockingester-3.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/LICENSE` & `rockingester-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/PKG-INFO` & `rockingester-3.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.3.0
-Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
+Version: 3.0.1
+Summary: Service to discover incoming images from the Formulatrix Rockmaker and ingest them into the database.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,100 +204,22 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://github.com/diamondlightsource/rockingester/rockingester
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
 
 rockingester
 =======================================================================
 
-XChem Business Knowledge Unit.  Service, Client, API, persistent store.
+Service to discover incoming images from the Formulatrix Rockmaker and ingest them into the database.
 
-Installation
------------------------------------------------------------------------
-::
-
-    pip install rockingester
-
-    rockingester --version
-
-Legacy information
------------------------------------------------------------------------
-
-The formulatrix pipeline code is here:
-
-    /dls/science/groups/i04-1/software/luigi_pipeline/imager_pipe
-    
-This is a working directory of 
-
-    https://github.com/xchem/formulatrix_pipe
-
-The formulatrix pipeline puts images here:
-
-    /dls/science/groups/i04-1/software/luigi_pipeline/imager_pipe/SubwellImages/9b5j_2023-03-23_RI1000-0276-3drop
-
-Does this have anything useful?
-
-    https://gitlab.diamond.ac.uk/cnp64921/dlsformulatrix.uploader/-/blob/master/formulatrix_uploader.py
-
-
-As for the luigi stuff, one of the scripts in the /dls/science/groups/i04-1/software/luigi_pipeline/imager_pipe/ creates the filename after extracting info from the SQL server on the Formulatrix. I think the 9b5j part is the barcode, yes, but you might have to dig into the scripts there to find out the logic behind it all.
-
-By the way if you want to access the FOrmulatrix /Rockmaker from Windows you can brose to access the RockMaker Imager \\cs04r-nas01-02\rockimager
-
-You see like:
-\\cs04r-nas01-02\rockimager\rockimager\RockMakerStorage\WellImages\539\plateID_14539\batchID_72673
-
-The batch ID proably relates to the inspection... a plate is inspected multiple times and each inspection has a batch ID.
-There may be some clues in the get_barcodes.py script in the imager_pipe directory.
-
-Algorithm
------------------------------------------------------------------------
-Looks in SubwellImages directory.
-
-Uses first 4 letters of each subdirectory as "barcode".
-
-If barcode is NOT in the plates mined from the formulatrix, then it is ignored.
-
-Otherrwise, if name of plate is a valid visit name, and the visit directory exists, then copies the images to the visit directory and inserts them into the database.
-
-Otherwise ignores the subdirectory.
-
-We have to leave all plate directories in SubwellImages since this is where Texrank expects them.
-
-After we don't need Texrank, then we can move the non-visit directories into something like SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/rockingester for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/bxflow/rockingester.git 
-    cd rockingester
-    virtualenv /scratch/$USER/venv/rockingester
-    source /scratch/$USER/venv/rockingester/bin/activate 
-    pip install -e .[dev]
-    make -f .rockingester/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/rockingester/build/html/index.html
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
+Uses xchembku for database interaction.
 
+For documentation see: https://diamondlightsource.github.io/rockingester
```

### Comparing `rockingester-2.3.0/configurations/development.yaml` & `rockingester-3.0.1/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/docs/conf.py` & `rockingester-3.0.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "rockingester",
     "$" + "{package_name}": "rockingester_lib",
     "$" + "{git_url}": "https://github.com/diamondlightsource/rockingester",
-    "$" + "{python_version_at_least}": "3.9",
+    "$" + "{python_version_at_least}": "3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 57cc2679e3536b62d41d3a5952bd47f3
+# dae_devops_fingerprint 828dd6a7f193b8dea97813cc6760f44e
```

### Comparing `rockingester-2.3.0/docs/images/dls-favicon.ico` & `rockingester-3.0.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/docs/images/dls-logo.svg` & `rockingester-3.0.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/pyproject.toml` & `rockingester-3.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name rockingester
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rockingester"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
 ]
-description = "XChem Business Knowledge Unit. Service, Client, API, persistent store."
-dependencies = ["xchembku", "dls_servbase", "dls_mainiac", "dls_multiconf", "dls_utilpack"]
+description = "Service to discover incoming images from the Formulatrix Rockmaker and ingest them into the database."
+dependencies = ["xchembku", "dls_servbase", "dls_mainiac", "dls_multiconf", "dls_utilpack", "python-tds"]
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
 
-# dae_devops_fingerprint 8082a407be92f35eda821c8130b7182b
+# dae_devops_fingerprint 9dc8a98c993bf5a03fa4d5a8e1b8b308
```

### Comparing `rockingester-2.3.0/src/rockingester.egg-info/PKG-INFO` & `rockingester-3.0.1/src/rockingester.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.3.0
-Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
+Version: 3.0.1
+Summary: Service to discover incoming images from the Formulatrix Rockmaker and ingest them into the database.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,100 +204,22 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://github.com/diamondlightsource/rockingester/rockingester
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
 
 rockingester
 =======================================================================
 
-XChem Business Knowledge Unit.  Service, Client, API, persistent store.
+Service to discover incoming images from the Formulatrix Rockmaker and ingest them into the database.
 
-Installation
------------------------------------------------------------------------
-::
-
-    pip install rockingester
-
-    rockingester --version
-
-Legacy information
------------------------------------------------------------------------
-
-The formulatrix pipeline code is here:
-
-    /dls/science/groups/i04-1/software/luigi_pipeline/imager_pipe
-    
-This is a working directory of 
-
-    https://github.com/xchem/formulatrix_pipe
-
-The formulatrix pipeline puts images here:
-
-    /dls/science/groups/i04-1/software/luigi_pipeline/imager_pipe/SubwellImages/9b5j_2023-03-23_RI1000-0276-3drop
-
-Does this have anything useful?
-
-    https://gitlab.diamond.ac.uk/cnp64921/dlsformulatrix.uploader/-/blob/master/formulatrix_uploader.py
-
-
-As for the luigi stuff, one of the scripts in the /dls/science/groups/i04-1/software/luigi_pipeline/imager_pipe/ creates the filename after extracting info from the SQL server on the Formulatrix. I think the 9b5j part is the barcode, yes, but you might have to dig into the scripts there to find out the logic behind it all.
-
-By the way if you want to access the FOrmulatrix /Rockmaker from Windows you can brose to access the RockMaker Imager \\cs04r-nas01-02\rockimager
-
-You see like:
-\\cs04r-nas01-02\rockimager\rockimager\RockMakerStorage\WellImages\539\plateID_14539\batchID_72673
-
-The batch ID proably relates to the inspection... a plate is inspected multiple times and each inspection has a batch ID.
-There may be some clues in the get_barcodes.py script in the imager_pipe directory.
-
-Algorithm
------------------------------------------------------------------------
-Looks in SubwellImages directory.
-
-Uses first 4 letters of each subdirectory as "barcode".
-
-If barcode is NOT in the plates mined from the formulatrix, then it is ignored.
-
-Otherrwise, if name of plate is a valid visit name, and the visit directory exists, then copies the images to the visit directory and inserts them into the database.
-
-Otherwise ignores the subdirectory.
-
-We have to leave all plate directories in SubwellImages since this is where Texrank expects them.
-
-After we don't need Texrank, then we can move the non-visit directories into something like SubwellImages_novisit, and move (instead of copy) them for good visits.  This will keep SubwellImages clean and more efficient to poll.
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/rockingester for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/bxflow/rockingester.git 
-    cd rockingester
-    virtualenv /scratch/$USER/venv/rockingester
-    source /scratch/$USER/venv/rockingester/bin/activate 
-    pip install -e .[dev]
-    make -f .rockingester/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/rockingester/build/html/index.html
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
+Uses xchembku for database interaction.
 
+For documentation see: https://diamondlightsource.github.io/rockingester
```

### Comparing `rockingester-2.3.0/src/rockingester.egg-info/SOURCES.txt` & `rockingester-3.0.1/src/rockingester.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

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
@@ -28,37 +29,40 @@
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
 src/rockingester.egg-info/PKG-INFO
 src/rockingester.egg-info/SOURCES.txt
 src/rockingester.egg-info/dependency_links.txt
 src/rockingester.egg-info/entry_points.txt
 src/rockingester.egg-info/requires.txt
 src/rockingester.egg-info/top_level.txt
 src/rockingester_api/__init__.py
 src/rockingester_api/aiohttp_client.py
-src/rockingester_api/context_base.py
 src/rockingester_api/exceptions.py
 src/rockingester_api/thing.py
 src/rockingester_api/things.py
 src/rockingester_api/collectors/__init__.py
 src/rockingester_api/collectors/aiohttp.py
 src/rockingester_api/collectors/collectors.py
 src/rockingester_api/collectors/constants.py
@@ -71,24 +75,27 @@
 src/rockingester_cli/subcommands/service.py
 src/rockingester_lib/__init__.py
 src/rockingester_lib/__main__.py
 src/rockingester_lib/_version.py
 src/rockingester_lib/base_aiohttp.py
 src/rockingester_lib/envvar.py
 src/rockingester_lib/exceptions.py
+src/rockingester_lib/ftrix_client.py
+src/rockingester_lib/plate_injector.py
 src/rockingester_lib/version.py
 src/rockingester_lib/collectors/__init__.py
 src/rockingester_lib/collectors/aiohttp.py
 src/rockingester_lib/collectors/base.py
 src/rockingester_lib/collectors/collectors.py
 src/rockingester_lib/collectors/constants.py
 src/rockingester_lib/collectors/context.py
 src/rockingester_lib/collectors/direct_poll.py
-src/rockingester_lib/contexts/__init__.py
-src/rockingester_lib/contexts/base.py
 tests/__init__.py
 tests/base.py
 tests/conftest.py
 tests/test_collector.py
+tests/test_ftrix_client.py
+tests/test_plate_injector.py
 tests/test_platewait.py
-tests/configurations/direct_poll.yaml
-tests/configurations/service.yaml
+tests/configurations/direct_sqlite.yaml
+tests/configurations/service_mysql.yaml
+tests/configurations/service_sqlite.yaml
```

### Comparing `rockingester-2.3.0/src/rockingester_api/collectors/aiohttp.py` & `rockingester-3.0.1/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_api/collectors/collectors.py` & `rockingester-3.0.1/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_api/collectors/context.py` & `rockingester-3.0.1/src/rockingester_api/collectors/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import logging
 
+# Base class.
+from dls_utilpack.client_context_base import ClientContextBase
+
 # Things created in the context.
 from rockingester_api.collectors.collectors import (
     Collectors,
     rockingester_collectors_set_default,
 )
 
-# Base class.
-from rockingester_api.context_base import ContextBase
-
 logger = logging.getLogger(__name__)
 
 
-class Context(ContextBase):
+class Context(ClientContextBase):
     """
     Client context for a rockingester_collector object.
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
-        self.interface = Collectors().build_object(self.__specification)
+        self.interface = Collectors().build_object(self.specification)
 
         # If there is more than one collector, the last one defined will be the default.
         rockingester_collectors_set_default(self.interface)
 
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
```

### Comparing `rockingester-2.3.0/src/rockingester_api/exceptions.py` & `rockingester-3.0.1/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_api/thing.py` & `rockingester-3.0.1/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_api/things.py` & `rockingester-3.0.1/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_cli/main.py` & `rockingester-3.0.1/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_cli/subcommands/base.py` & `rockingester-3.0.1/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_cli/subcommands/service.py` & `rockingester-3.0.1/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_cli/version.py` & `rockingester-3.0.1/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_lib/__main__.py` & `rockingester-3.0.1/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-3.0.1/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_lib/collectors/base.py` & `rockingester-3.0.1/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_lib/collectors/collectors.py` & `rockingester-3.0.1/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_lib/collectors/context.py` & `rockingester-3.0.1/src/rockingester_lib/collectors/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 from typing import Dict
 
-# Things created in the context.
-from rockingester_lib.collectors.collectors import Collectors, collectors_set_default
+# Base class for an asyncio server context.
+from dls_utilpack.server_context_base import ServerContextBase
 
-# Base class for an asyncio context.
-from rockingester_lib.contexts.base import Base as ContextBase
+# Things created in the context.
+from rockingester_lib.collectors.collectors import Collectors
 
 logger = logging.getLogger(__name__)
 
 
 thing_type = "rockingester_lib.collectors.context"
 
 
-class Context(ContextBase):
+class Context(ServerContextBase):
     """
     Asyncio context for a collector object.
     On entering, it creates the object according to the specification (a dict).
     If specified, it starts the server as a coroutine, thread or process.
     If not a server, then it will instatiate a direct access to a collector.
     On exiting, it commands the server to shut down and/or releases the direct access resources.
     """
@@ -25,35 +25,32 @@
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification: Dict):
         """
         Constructor.
 
         Args:
             specification (Dict): specification of the collector object to be constructed within the context.
-                The only key in the specification that relates to the context is "start_as", which can be "coro", "thread", "process" or None.
+                The only key in the specification that relates to the context is "start_as", which can be "coro", "thread", "process", "direct", or None.
                 All other keys in the specification relate to creating the collector object.
         """
-        ContextBase.__init__(self, thing_type, specification)
+        ServerContextBase.__init__(self, thing_type, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self) -> None:
         """
         Asyncio context entry.
 
         Starts and activates service as specified.
 
         Establishes the global (singleton-like) default collector.
         """
 
         # Build the object according to the specification.
         self.server = Collectors().build_object(self.specification())
 
-        # If there is more than one collector, the last one defined will be the default.
-        collectors_set_default(self.server)
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

### Comparing `rockingester-2.3.0/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-3.0.1/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 import asyncio
 import logging
 import os
 import shutil
 import time
 from pathlib import Path
-from typing import Dict, List
+from typing import List
 
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain2
 from dls_utilpack.require import require
-from dls_utilpack.visit import VisitNotFound, get_xchem_directory
+from dls_utilpack.visit import get_xchem_directory
 from PIL import Image
 
 # Crystal plate object interface.
 from xchembku_api.crystal_plate_objects.interface import (
     Interface as CrystalPlateInterface,
 )
 
 # Dataface client context.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
-from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 
 # Crystal plate pydantic model.
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 
 # Crystal well pydantic model.
 from xchembku_api.models.crystal_well_model import CrystalWellModel
 
 # Crystal plate objects factory.
 from xchembku_lib.crystal_plate_objects.crystal_plate_objects import CrystalPlateObjects
 
 # Base class for collector instances.
 from rockingester_lib.collectors.base import Base as CollectorBase
 
+# Object able to talk to the formulatrix database.
+from rockingester_lib.ftrix_client import FtrixClient
+
+# Object which can inject new xchembku plate records discovered while looking in subwell images.
+from rockingester_lib.plate_injector import PlateInjector
+
 logger = logging.getLogger(__name__)
 
 thing_type = "rockingester_lib.collectors.direct_poll"
 
 
 # ------------------------------------------------------------------------------------------
 class DirectPoll(CollectorBase):
     """
     Object representing an image collector.
     The behavior is to start a coro task to waken every few seconds and scan for newly created plate directories.
     Image files are pushed to xchembku.
+    Plates for the image files are also pushed to xchembku the first time they are wanted.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification, predefined_uuid=None):
         CollectorBase.__init__(
             self, thing_type, specification, predefined_uuid=predefined_uuid
         )
@@ -65,34 +71,36 @@
         )
 
         # The subdirectory under a visit where to put subwell images that are collected.
         self.__visit_plates_subdirectory = Path(
             require(s, type_specific_tbd, "visit_plates_subdirectory")
         )
 
+        # Reference the dict entry for the ftrix client specification.
+        self.__ftrix_client_specification = require(
+            s, type_specific_tbd, "ftrix_client_specification"
+        )
+
         # Explicit list of barcodes to process (used when testing a deployment).
         self.__ingest_only_barcodes = type_specific_tbd.get("ingest_only_barcodes")
 
         # Maximum time to wait for final image to arrive, relative to time of last arrived image.
         self.__max_wait_seconds = require(s, type_specific_tbd, "max_wait_seconds")
 
         # Database where we will get plate barcodes and add new wells.
         self.__xchembku_client_context = None
         self.__xchembku = None
 
+        # Object able to talk to the formulatrix database.
+        self.__ftrix_client = None
+
         # This flag will stop the ticking async task.
         self.__keep_ticking = True
         self.__tick_future = None
 
-        # This is the last formulatrix plate we have ingested, used to avoid re-handling the same plate.
-        self.__latest_formulatrix__plate__id = 0
-
-        # This is the list of plates indexed by their barcode.
-        self.__crystal_plate_models_by_barcode: Dict[CrystalPlateModel] = {}
-
         # The plate names which we have already finished handling within the current instance.
         self.__handled_plate_names = []
 
     # ----------------------------------------------------------------------------------------
     async def activate(self) -> None:
         """
         Activate the object.
@@ -115,14 +123,24 @@
 
         # Activate the context.
         await self.__xchembku_client_context.aenter()
 
         # Get a reference to the xchembku interface provided by the context.
         self.__xchembku = self.__xchembku_client_context.get_interface()
 
+        # Object able to talk to the formulatrix database.
+        self.__ftrix_client = FtrixClient(
+            self.__ftrix_client_specification,
+        )
+
+        # Object which can inject new xchembku plate records discovered while looking in subwell images.
+        self.__plate_injector = PlateInjector(
+            self.__ftrix_client,
+            self.__xchembku,
+        )
         # Poll periodically.
         self.__tick_future = asyncio.get_event_loop().create_task(self.tick())
 
     # ----------------------------------------------------------------------------------------
     async def deactivate(self) -> None:
         """
         Deactivate the object.
@@ -152,56 +170,37 @@
 
         Stops when flag has been set by other tasks.
 
         # TODO: Use an event to awaken ticker early to handle stop requests sooner.
         """
 
         while self.__keep_ticking:
-            try:
-                # Fetch all the plates we don't have yet.
-                await self.fetch_plates_by_barcode()
-
-                # Scrape all the configured plates directories.
-                await self.scrape()
-            except Exception as exception:
-                logger.error(explain2(exception, "scraping"), exc_info=exception)
+            # Scrape all the configured plates directories.
+            await self.scrape_plates_directories()
 
             # TODO: Make periodic tick period to be configurable.
             await asyncio.sleep(1.0)
 
     # ----------------------------------------------------------------------------------------
-    async def fetch_plates_by_barcode(self) -> None:
-        """
-        Fetch all barcodes in the database which we don't have in memory yet.
-        """
-
-        # Fetch all the plates we don't have yet.
-        plate_models = await self.__xchembku.fetch_crystal_plates(
-            CrystalPlateFilterModel(
-                from_formulatrix__plate__id=self.__latest_formulatrix__plate__id
-            ),
-            why="[ROCKINGESTER POLL]",
-        )
-
-        # Add the plates to the list, assumed sorted by formulatrix__plate__id.
-        for plate_model in plate_models:
-            self.__crystal_plate_models_by_barcode[plate_model.barcode] = plate_model
-
-            # Remember the highest one we got to shorten the query for next time.
-            self.__latest_formulatrix__plate__id = plate_model.formulatrix__plate__id
-
-    # ----------------------------------------------------------------------------------------
-    async def scrape(self) -> None:
+    async def scrape_plates_directories(self) -> None:
         """
         Scrape all the configured directories looking for new files.
         """
 
-        # TODO: Use asyncio tasks to parellize scraping plates directories.
+        # TODO: Use asyncio tasks to paralellize scraping plates directories.
         for directory in self.__plates_directories:
-            await self.scrape_plates_directory(Path(directory))
+            try:
+                await self.scrape_plates_directory(Path(directory))
+            except Exception as exception:
+                # Just log the error, tag as anomaly for reporting, don't die.
+                logger.error(
+                    "[ANOMALY] "
+                    + explain2(exception, f"scraping plates directory {directory}"),
+                    exc_info=exception,
+                )
 
     # ----------------------------------------------------------------------------------------
     async def scrape_plates_directory(
         self,
         plates_directory: Path,
     ) -> None:
         """
@@ -219,72 +218,78 @@
         plate_names.sort()
 
         logger.debug(
             f"[ROCKINGESTER POLL] found {len(plate_names)} plate directories in {plates_directory}"
         )
 
         for plate_name in plate_names:
-            # We already handled this plate name?
-            if plate_name in self.__handled_plate_names:
-                # logger.debug(
-                #     f"[ROCKINGESTER POLL] plate_barcode {plate_barcode}"
-                #     f" is already handled in this instance"
-                # )
-                continue
-
-            # Get the plate's barcode from the directory name.
-            plate_barcode = plate_name[0:4]
-
-            # We have a specific list we want to process?
-            if self.__ingest_only_barcodes is not None:
-                if plate_barcode not in self.__ingest_only_barcodes:
-                    continue
-
-            # Get the matching plate record from the database.
-            crystal_plate_model = self.__crystal_plate_models_by_barcode.get(
-                plate_barcode
-            )
-
-            # This plate directory's barcode is not in the database?
-            if crystal_plate_model is None:
-                logger.debug(
-                    f"[ROCKDIR] plate_barcode {plate_barcode} is not in the database"
-                )
-                self.__handled_plate_names.append(plate_name)
-                continue
             try:
-                # Try to get the visit directory from the visit stored in the database's plate record.
-                visit_directory = Path(
-                    get_xchem_directory(
-                        self.__visits_directory, crystal_plate_model.visit
-                    )
-                )
-            # This is an improperly formatted visit name?
-            except ValueError:
-                logger.debug(
-                    f"[ROCKDIR] plate_barcode {plate_barcode}"
-                    f" is in the database, but visit {crystal_plate_model.visit} is improperly formed"
-                )
-                self.__handled_plate_names.append(plate_name)
-                continue
-            # This visit is not found on disk?
-            except VisitNotFound:
-                logger.debug(
-                    f"[ROCKDIR] plate_barcode {plate_barcode}"
-                    f" is in the database, but cannot find visit directory in {self.__visits_directory}"
+                await self.scrape_plate_directory(plates_directory / plate_name)
+            except Exception as exception:
+                # Just log the error, tag as anomaly for reporting, don't die.
+                logger.error(
+                    "[ANOMALY] "
+                    + explain2(
+                        exception,
+                        f"scraping plate directory {str(plates_directory / plate_name)}",
+                    ),
+                    exc_info=exception,
                 )
-                self.__handled_plate_names.append(plate_name)
-                continue
+
+    # ----------------------------------------------------------------------------------------
+    async def scrape_plate_directory(
+        self,
+        plate_directory: Path,
+    ) -> None:
+        """
+        Scrape a single directory looking for images.
+        """
+
+        plate_name = plate_directory.name
+
+        # We already handled this plate name?
+        if plate_name in self.__handled_plate_names:
+            # logger.debug(
+            #     f"[ROCKINGESTER POLL] plate_barcode {plate_barcode}"
+            #     f" is already handled in this instance"
+            # )
+            return
+
+        # Get the plate's barcode from the directory name.
+        plate_barcode = plate_name[0:4]
+
+        # We have a specific list we want to process?
+        if self.__ingest_only_barcodes is not None:
+            if plate_barcode not in self.__ingest_only_barcodes:
+                return
+
+        # Get the matching plate record from the xchembku or formulatrix database.
+        crystal_plate_model = await self.__plate_injector.find_or_inject_barcode(
+            plate_barcode,
+            self.__visits_directory,
+        )
+
+        logger.debug(
+            f"[CRYERR] for plate_barcode {plate_barcode} crystal_plate_model.error is {crystal_plate_model.error}"
+        )
+
+        if crystal_plate_model.error is None:
+            visit_directory = get_xchem_directory(
+                self.__visits_directory, crystal_plate_model.visit
+            )
 
             # Scrape the directory when all image files have arrived.
             await self.scrape_plate_directory_if_complete(
-                plates_directory / plate_name,
+                plate_directory,
                 crystal_plate_model,
                 visit_directory,
             )
+        else:
+            # Remember we "handled" this one.
+            self.__handled_plate_names.append(plate_name)
 
     # ----------------------------------------------------------------------------------------
     async def scrape_plate_directory_if_complete(
         self,
         plate_directory: Path,
         crystal_plate_model: CrystalPlateModel,
         visit_directory: Path,
```

### Comparing `rockingester-2.3.0/src/rockingester_lib/exceptions.py` & `rockingester-3.0.1/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/src/rockingester_lib/version.py` & `rockingester-3.0.1/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/tests/base.py` & `rockingester-3.0.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/tests/configurations/service.yaml` & `rockingester-3.0.1/tests/configurations/direct_sqlite.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -11,49 +11,80 @@
         enabled: False
         host: 172.23.7.128
         port: 12201
         protocol: UDP
 
 # The external access bits.
 external_access_bits:
-    dataface_port: &ROCKINGESTER_PORT 27821
+    xchembku_dataface_server: &XCHEMBKU_DATAFACE_SERVER http://*:27821
+    xchembku_dataface_client: &XCHEMBKU_DATAFACE_CLIENT http://localhost:27821
 
+visits_directory: &VISITS_DIRECTORY "${output_directory}/visits"
+visit_plates_subdirectory: &VISIT_PLATES_SUBDIRECTORY "processing/rockingester"
+
+# -----------------------------------------------------------------------------
+ftrix_client_specification: &FTRIX_CLIENT_SPECIFICATION
+    mssql:
+        server: dummy
+        database: records1
+        username: na
+        password: na
+        records1:
+            - - 10
+              - 98ab
+              - cm00001-1_scrapable
+              - SWISSci_3Drop
+            - - 11
+              - 98ad
+              - cm00001-badvisit_barcode
+              - SWISSci_3drop
+        records_for_plate_injector:
+            - - 1
+              - 98ab
+              - cm00001-1_something#else
+              - SWISSci_3Drop
+            - - 2
+              - 98ax
+              - cm00001_bad_visit_format
+              - SWISSci_3drop
+
+# -----------------------------------------------------------------------------
 # The xchembku_dataface direct access.
-xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
+xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     type: "xchembku_lib.xchembku_datafaces.direct"
     database:
-        type: "xchembku_lib.xchembku_databases.normsql"
-        filename: "${output_directory}/xchembku.sqlite"
+        type: "dls_normsql.aiosqlite"
+        filename: "${output_directory}/xchembku_dataface.sqlite"
         log_level: "WARNING"
 
-visits_directory: &VISITS_DIRECTORY "${output_directory}/visits"
-visit_plates_subdirectory: &VISIT_PLATES_SUBDIRECTORY "processing/rockingester"
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
+
+# -----------------------------------------------------------------------------
 
 # The rockingester direct access.
-rockingester_collector_specification_direct_poll:
-    &ROCKINGESTER_COLLECTOR_SPECIFICATION_DIRECT_POLL
+rockingester_collector_specification:
     type: "rockingester_lib.collectors.direct_poll"
     type_specific_tbd:
         plates_directories:
             - "${output_directory}/SubwellImages"
         max_wait_seconds: 3.0
         visits_directory: *VISITS_DIRECTORY
         visit_plates_subdirectory: *VISIT_PLATES_SUBDIRECTORY
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
+        ftrix_client_specification: *FTRIX_CLIENT_SPECIFICATION
         ingest_only_barcodes:
             - 98ab
             - 98ac
             - 98ad
-
-# The rockingester client/server composite.
-rockingester_collector_specification:
-    type: "rockingester_lib.collectors.aiohttp"
-    type_specific_tbd:
-        # The remote rockingester server access.
-        aiohttp_specification:
-            server_host: "*"
-            client_host: "127.0.0.1"
-            port: *ROCKINGESTER_PORT
-        # The local implementation of the rockingester.
-        direct_collector_specification: *ROCKINGESTER_COLLECTOR_SPECIFICATION_DIRECT_POLL
     context:
-        start_as: process
+        start_as: direct
```

### Comparing `rockingester-2.3.0/tests/conftest.py` & `rockingester-3.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.3.0/tests/test_collector.py` & `rockingester-3.0.1/tests/test_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 import asyncio
 import logging
 import time
 from pathlib import Path
 
 from dls_utilpack.visit import get_xchem_subdirectory
 
-# Types which the CrystalPlateObjects factory can use to build an instance.
-from xchembku_api.crystal_plate_objects.constants import (
-    ThingTypes as CrystalPlateObjectThingTypes,
-)
-
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
-from xchembku_api.models.crystal_plate_model import CrystalPlateModel
+from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from rockingester_api.collectors.context import Context as CollectorClientContext
 
 # Server context creator.
 from rockingester_lib.collectors.context import Context as CollectorServerContext
 
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCollectorDirectPoll:
+class XTestCollectorDirectMysql:
     """
     Test collector interface by direct call.
     """
 
     def test(self, constants, logging_setup, output_directory):
 
         # Configuration file to use.
-        configuration_file = "tests/configurations/direct_poll.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
 
         CollectorTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCollectorService:
+class TestCollectorServiceSqlite:
     """
     Test collector interface through network interface.
     """
 
     def test(self, constants, logging_setup, output_directory):
 
         # Configuration file to use.
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+
+        CollectorTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestCollectorServiceMysql:
+    """
+    Test collector interface through network interface.
+    """
+
+    def test(self, constants, logging_setup, output_directory):
+
+        # Configuration file to use.
+        configuration_file = "tests/configurations/service_mysql.yaml"
 
         CollectorTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class CollectorTester(Base):
     """
@@ -86,15 +95,19 @@
         multiconf_dict = await multiconf.load()
 
         # Reference the dict entry for the xchembku dataface.
         xchembku_dataface_specification = multiconf_dict[
             "xchembku_dataface_specification"
         ]
 
-        # Make the xchembku client context, expected to be direct (no server).
+        # Make the xchembku server context.
+        xchembku_server_context = XchembkuDatafaceServerContext(
+            xchembku_dataface_specification
+        )
+        # Make the xchembku client context.
         xchembku_client_context = XchembkuDatafaceClientContext(
             xchembku_dataface_specification
         )
 
         collector_specification = multiconf_dict["rockingester_collector_specification"]
         # Make the server context.
         collector_server_context = CollectorServerContext(collector_specification)
@@ -106,72 +119,52 @@
         self.__visits_directory = Path(multiconf_dict["visits_directory"])
         self.__visit_plates_subdirectory = Path(
             multiconf_dict["visit_plates_subdirectory"]
         )
 
         scrapable_image_count = 288
 
-        # Start the client context for the direct access to the xchembku.
+        # Start the client context for the remote access to the xchembku.
         async with xchembku_client_context:
-            # Start the collector client context.
-            async with collector_client_context:
-                # And the collector server context which starts the coro.
-                async with collector_server_context:
-                    await self.__run_part1(
-                        scrapable_image_count, constants, output_directory
-                    )
+            # Start the server context xchembku which starts the process.
+            async with xchembku_server_context:
+                # Start the collector server.
+                async with collector_client_context:
+                    # And the collector server context which starts the coro.
+                    async with collector_server_context:
+                        await self.__run_part1(
+                            scrapable_image_count, constants, output_directory
+                        )
 
-                logger.debug(
-                    "------------ restarting collector server --------------------"
-                )
-
-                # Start the server again.
-                # This covers the case where collector starts by finding existing entries in the database and doesn't double-collect those on disk.
-                async with collector_server_context:
-                    await self.__run_part2(
-                        scrapable_image_count, constants, output_directory
+                    logger.debug(
+                        "------------ restarting collector server --------------------"
                     )
 
+                    # Start the server again.
+                    # This covers the case where collector starts by finding existing entries in the database and doesn't double-collect those on disk.
+                    async with collector_server_context:
+                        await self.__run_part2(
+                            scrapable_image_count, constants, output_directory
+                        )
+
     # ----------------------------------------------------------------------------------------
 
     async def __run_part1(self, scrapable_image_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
 
         # Make the plate on which the wells reside.
         visit = "cm00001-1_otherstuff"
-        created_crystal_plate_models = []
 
         scrabable_barcode = "98ab"
-        created_crystal_plate_models.append(
-            CrystalPlateModel(
-                formulatrix__plate__id=10,
-                barcode=scrabable_barcode,
-                visit=visit,
-                thing_type=CrystalPlateObjectThingTypes.SWISS3,
-            )
-        )
-
         nobarcode_barcode = "98ac"
-
-        # Create a crystal plate model with a good barcode but bad visit.
-        novisit_barcode = "98ad"
-        created_crystal_plate_models.append(
-            CrystalPlateModel(
-                formulatrix__plate__id=11,
-                barcode=novisit_barcode,
-                visit=("X" + visit),
-            )
-        )
-
+        badvisit_barcode = "98ad"
         excluded_barcode = "98ae"
 
-        await xchembku.upsert_crystal_plates(created_crystal_plate_models)
-
         visit_directory = self.__visits_directory / get_xchem_subdirectory(visit)
         visit_directory.mkdir(parents=True)
         rockingester_directory = visit_directory / self.__visit_plates_subdirectory
 
         # Get list of images before we create any of the scrape-able files.
         crystal_well_models = await xchembku.fetch_crystal_wells_filenames()
 
@@ -201,20 +194,20 @@
             filename = plate_directory2 / self.__subwell_filename(nobarcode_barcode, i)
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make yet another scrapable directory with a different barcode.
         # This one gets ignored since it matches a plate with a bad visit name.
         plate_directory3 = (
-            plates_directory / f"{novisit_barcode}_2023-04-06_RI1000-0276-3drop"
+            plates_directory / f"{badvisit_barcode}_2023-04-06_RI1000-0276-3drop"
         )
         plate_directory3.mkdir(parents=True)
         novisit_image_count = 6
         for i in range(novisit_image_count):
-            filename = plate_directory3 / self.__subwell_filename(novisit_barcode, i)
+            filename = plate_directory3 / self.__subwell_filename(badvisit_barcode, i)
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make yet another scrapable directory with a different barcode.
         # This one gets completely ignored because it's not in the explicit list.
         plate_directory4 = (
             plates_directory / f"{excluded_barcode}_2023-04-06_RI1000-0276-3drop"
```

### Comparing `rockingester-2.3.0/tests/test_platewait.py` & `rockingester-3.0.1/tests/test_platewait.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 import asyncio
 import logging
 import time
 from pathlib import Path
 
 from dls_utilpack.visit import get_xchem_subdirectory
 
-# Types which the CrystalPlateObjects factory can use to build an instance.
-from xchembku_api.crystal_plate_objects.constants import (
-    ThingTypes as CrystalPlateObjectThingTypes,
-)
-
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
-from xchembku_api.models.crystal_plate_model import CrystalPlateModel
+from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 # Client context creator.
 from rockingester_api.collectors.context import Context as CollectorClientContext
 
 # Server context creator.
 from rockingester_lib.collectors.context import Context as CollectorServerContext
 
 # Base class for the tester.
 from tests.base import Base
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestPlatewaitDirectPoll:
+class TestPlatewaitDirectMysql:
     """
     Test collector interface by direct call.
     """
 
     def test(self, constants, logging_setup, output_directory):
 
         # Configuration file to use.
-        configuration_file = "tests/configurations/direct_poll.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
 
         PlatewaitTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
-class TestPlatewaitService:
+class TestPlatewaitServiceSqlite:
     """
     Test collector interface through network interface.
     """
 
     def test(self, constants, logging_setup, output_directory):
 
         # Configuration file to use.
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+
+        PlatewaitTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestPlatewaitServiceMysql:
+    """
+    Test collector interface through network interface.
+    """
+
+    def test(self, constants, logging_setup, output_directory):
+
+        # Configuration file to use.
+        configuration_file = "tests/configurations/service_mysql.yaml"
 
         PlatewaitTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class PlatewaitTester(Base):
     """
@@ -75,15 +84,19 @@
         multiconf_dict = await multiconf.load()
 
         # Reference the dict entry for the xchembku dataface.
         xchembku_dataface_specification = multiconf_dict[
             "xchembku_dataface_specification"
         ]
 
-        # Make the xchembku client context, expected to be direct (no server).
+        # Make the xchembku server context.
+        xchembku_server_context = XchembkuDatafaceServerContext(
+            xchembku_dataface_specification
+        )
+        # Make the xchembku client context.
         xchembku_client_context = XchembkuDatafaceClientContext(
             xchembku_dataface_specification
         )
 
         collector_specification = multiconf_dict["rockingester_collector_specification"]
         # Make the server context.
         collector_server_context = CollectorServerContext(collector_specification)
@@ -95,56 +108,46 @@
         self.__visits_directory = Path(multiconf_dict["visits_directory"])
         self.__visit_plates_subdirectory = Path(
             multiconf_dict["visit_plates_subdirectory"]
         )
 
         scrapable_image_count = 4
 
-        # Start the client context for the direct access to the xchembku.
+        # Start the client context for the remote access to the xchembku.
         async with xchembku_client_context:
-            # Start the collector client context.
-            async with collector_client_context:
-                # And the collector server context which starts the coro.
-                async with collector_server_context:
-                    await self.__run_the_test(
-                        scrapable_image_count, constants, output_directory
-                    )
+            # Start the server context xchembku which starts the process.
+            async with xchembku_server_context:
+                # Start the collector client context.
+                async with collector_client_context:
+                    # And the collector server context which starts the coro.
+                    async with collector_server_context:
+                        await self.__run_the_test(
+                            scrapable_image_count, constants, output_directory
+                        )
 
     # ----------------------------------------------------------------------------------------
 
     async def __run_the_test(self, scrapable_image_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
 
         # Make the plate on which the wells reside.
         visit = "cm00001-1_otherstuff"
-        created_crystal_plate_models = []
 
         scrabable_barcode = "98ab"
-        created_crystal_plate_models.append(
-            CrystalPlateModel(
-                formulatrix__plate__id=10,
-                barcode=scrabable_barcode,
-                visit=visit,
-                thing_type=CrystalPlateObjectThingTypes.SWISS3,
-            )
-        )
-
-        await xchembku.upsert_crystal_plates(created_crystal_plate_models)
 
         visit_directory = self.__visits_directory / get_xchem_subdirectory(visit)
         visit_directory.mkdir(parents=True)
         rockingester_directory = visit_directory / self.__visit_plates_subdirectory
 
         # Source directory which gets scraped for plates.
         plates_directory = Path(output_directory) / "SubwellImages"
 
-        # Make the scrapable directory with some files, fewer than the total.
-        # This one gets scraped as normal.
+        # Make the scrapable directory with some files, fewer than the total for the plate type.
         plate_directory1 = plates_directory / "98ab_2023-04-06_RI1000-0276-3drop"
         plate_directory1.mkdir(parents=True)
         for i in range(scrapable_image_count):
             filename = plate_directory1 / self.__subwell_filename(scrabable_barcode, i)
             with open(filename, "w") as stream:
                 stream.write("")
```

