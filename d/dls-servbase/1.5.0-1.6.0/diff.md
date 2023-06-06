# Comparing `tmp/dls-servbase-1.5.0.tar.gz` & `tmp/dls-servbase-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-servbase-1.5.0.tar", last modified: Wed May 31 15:41:59 2023, max compression
+gzip compressed data, was "dls-servbase-1.6.0.tar", last modified: Tue Jun  6 10:15:12 2023, max compression
```

## Comparing `dls-servbase-1.5.0.tar` & `dls-servbase-1.6.0.tar`

### file list

```diff
@@ -1,141 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.664093 dls-servbase-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.648093 dls-servbase-1.5.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.648093 dls-servbase-1.5.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/good_config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:41:59.664093 dls-servbase-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.648093 dls-servbase-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/cookie_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/dataface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/javascript/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/configurations/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/configurations/sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_dataface_takeover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_parse_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.735133 dls-servbase-1.6.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.735133 dls-servbase-1.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.739133 dls-servbase-1.6.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.735133 dls-servbase-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/src/dls_servbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/src/dls_servbase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.743133 dls-servbase-1.6.0/src/dls_servbase_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 10:15:12.000000 dls-servbase-1.6.0/src/dls_servbase_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/cookies/dataface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.747133 dls-servbase-1.6.0/src/dls_servbase_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/guis/html/javascript/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/src/dls_servbase_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:15:12.751133 dls-servbase-1.6.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/configurations/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/configurations/sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_dataface_takeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-06 10:15:03.000000 dls-servbase-1.6.0/tests/test_parse_cookie.py
```

### Comparing `dls-servbase-1.5.0/.dae-devops/Makefile` & `dls-servbase-1.6.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/docs/conventions.rst` & `dls-servbase-1.6.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/docs/developing.rst` & `dls-servbase-1.6.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/docs/devops.rst` & `dls-servbase-1.6.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/docs/docs_structure.rst` & `dls-servbase-1.6.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/docs/documenting.rst` & `dls-servbase-1.6.0/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/docs/installing.rst` & `dls-servbase-1.6.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/docs/testing.rst` & `dls-servbase-1.6.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.dae-devops/project.yaml` & `dls-servbase-1.6.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.devcontainer/Dockerfile` & `dls-servbase-1.6.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.devcontainer/devcontainer.json` & `dls-servbase-1.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/CONTRIBUTING.rst` & `dls-servbase-1.6.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/actions/install_requirements/action.yml` & `dls-servbase-1.6.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/dependabot.yml` & `dls-servbase-1.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/pages/index.html` & `dls-servbase-1.6.0/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/pages/make_switcher.py` & `dls-servbase-1.6.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/workflows/code.yml` & `dls-servbase-1.6.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/workflows/docs.yml` & `dls-servbase-1.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/workflows/docs_clean.yml` & `dls-servbase-1.6.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.github/workflows/linkcheck.yml` & `dls-servbase-1.6.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.gitignore` & `dls-servbase-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.gitlab-ci.yml` & `dls-servbase-1.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/.vscode/launch.json` & `dls-servbase-1.6.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/LICENSE` & `dls-servbase-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/PKG-INFO` & `dls-servbase-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.5.0
+Version: 1.6.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.5.0/docs/conf.py` & `dls-servbase-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/docs/images/dls-favicon.ico` & `dls-servbase-1.6.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/docs/images/dls-logo.svg` & `dls-servbase-1.6.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/pyproject.toml` & `dls-servbase-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase.egg-info/PKG-INFO` & `dls-servbase-1.6.0/src/dls_servbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.5.0
+Version: 1.6.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase.egg-info/SOURCES.txt` & `dls-servbase-1.6.0/src/dls_servbase.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 LICENSE
 README.md
-good_config1.yaml
 pyproject.toml
 .dae-devops/Makefile
 .dae-devops/prepare_git_dependencies.sh
 .dae-devops/project.yaml
 .dae-devops/docs/conventions.rst
 .dae-devops/docs/developing.rst
 .dae-devops/docs/devops.rst
@@ -29,20 +28,32 @@
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/conf.py
 docs/index.rst
 docs/_static/css/custom.css
-docs/api/classes.rst
-docs/api/command_line.rst
-docs/api/index.rst
-docs/api/modules.rst
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
+docs/reference/classes.rst
+docs/reference/command_line.rst
+docs/reference/index.rst
+docs/reference/modules.rst
+docs/tutorials/index.rst
+docs/tutorials/tbd.rst
 src/dls_servbase.egg-info/PKG-INFO
 src/dls_servbase.egg-info/SOURCES.txt
 src/dls_servbase.egg-info/dependency_links.txt
 src/dls_servbase.egg-info/entry_points.txt
 src/dls_servbase.egg-info/requires.txt
 src/dls_servbase.egg-info/top_level.txt
 src/dls_servbase_api/__init__.py
@@ -54,30 +65,31 @@
 src/dls_servbase_api/databases/database_definition.py
 src/dls_servbase_api/databases/table_definitions.py
 src/dls_servbase_api/datafaces/__init__.py
 src/dls_servbase_api/datafaces/aiohttp.py
 src/dls_servbase_api/datafaces/constants.py
 src/dls_servbase_api/datafaces/context.py
 src/dls_servbase_api/datafaces/datafaces.py
+src/dls_servbase_api/guis/__init__.py
+src/dls_servbase_api/guis/aiohttp.py
+src/dls_servbase_api/guis/constants.py
+src/dls_servbase_api/guis/context.py
+src/dls_servbase_api/guis/guis.py
 src/dls_servbase_cli/__init__.py
 src/dls_servbase_cli/main.py
 src/dls_servbase_cli/version.py
 src/dls_servbase_cli/subcommands/__init__.py
 src/dls_servbase_cli/subcommands/base.py
-src/dls_servbase_cli/subcommands/start_services.py
+src/dls_servbase_cli/subcommands/service.py
 src/dls_servbase_lib/__init__.py
 src/dls_servbase_lib/__main__.py
 src/dls_servbase_lib/_version.py
 src/dls_servbase_lib/base_aiohttp.py
 src/dls_servbase_lib/envvar.py
 src/dls_servbase_lib/version.py
-src/dls_servbase_lib/contexts/__init__.py
-src/dls_servbase_lib/contexts/base.py
-src/dls_servbase_lib/contexts/classic.py
-src/dls_servbase_lib/contexts/contexts.py
 src/dls_servbase_lib/cookies/__init__.py
 src/dls_servbase_lib/cookies/base.py
 src/dls_servbase_lib/cookies/cookie_parser.py
 src/dls_servbase_lib/cookies/cookies.py
 src/dls_servbase_lib/cookies/dataface.py
 src/dls_servbase_lib/datafaces/__init__.py
 src/dls_servbase_lib/datafaces/aiohttp.py
@@ -89,20 +101,19 @@
 src/dls_servbase_lib/guis/base.py
 src/dls_servbase_lib/guis/constants.py
 src/dls_servbase_lib/guis/context.py
 src/dls_servbase_lib/guis/guis.py
 src/dls_servbase_lib/guis/html/index.html
 src/dls_servbase_lib/guis/html/javascript/version.js
 tests/__init__.py
-tests/base.py
 tests/base_context_tester.py
-tests/base_specification_tester.py
 tests/base_tester.py
 tests/conftest.py
 tests/test_aiohttp.py
+tests/test_cli.py
 tests/test_database.py
 tests/test_dataface.py
 tests/test_dataface_takeover.py
 tests/test_gui.py
 tests/test_parse_cookie.py
 tests/configurations/mysql.yaml
 tests/configurations/sqlite.yaml
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_api/aiohttp_client.py` & `dls-servbase-1.6.0/src/dls_servbase_api/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_api/databases/database_definition.py` & `dls-servbase-1.6.0/src/dls_servbase_api/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_api/databases/table_definitions.py` & `dls-servbase-1.6.0/src/dls_servbase_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_api/datafaces/aiohttp.py` & `dls-servbase-1.6.0/src/dls_servbase_api/datafaces/aiohttp.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 
 # Dataface protocolj things.
 from dls_servbase_api.datafaces.constants import Commands, Keywords
 
 logger = logging.getLogger(__name__)
 
 
-# ------------------------------------------------------------------------------------------
-class Aiohttp:
+class Aiohttp(AiohttpClient):
     """
     Object implementing client side API for talking to the dls_servbase_dataface server.
-    Please see doctopic [A01].
     """
 
     # ----------------------------------------------------------------------------------------
-    def __init__(self, specification=None):
-        self.__specification = specification
+    def __init__(self, specification):
 
-        self.__aiohttp_client = AiohttpClient(
+        # We will get an umbrella specification which must contain an aiohttp_specification within it.
+        AiohttpClient.__init__(
+            self,
             specification["type_specific_tbd"]["aiohttp_specification"],
         )
 
     # ----------------------------------------------------------------------------------------
     def specification(self):
         return self.__specification
 
@@ -47,19 +46,14 @@
     async def update(self, table_name, record, where, subs=None, why=None):
         """"""
         return await self.__send_protocolj(
             "update", table_name, record, where, subs=subs, why=why
         )
 
     # ----------------------------------------------------------------------------------------
-    async def report_health(self):
-        """"""
-        return await self.__send_protocolj("report_health")
-
-    # ----------------------------------------------------------------------------------------
     async def set_cookie(self, cookie_dict):
         """ """
         return await self.__send_protocolj("set_cookie", cookie_dict)
 
     # ----------------------------------------------------------------------------------------
     async def get_cookie(self, cookie_uuid):
         """
@@ -73,30 +67,22 @@
         """"""
         return await self.__send_protocolj("update_cookie", row)
 
     # ----------------------------------------------------------------------------------------
     async def __send_protocolj(self, function, *args, **kwargs):
         """"""
 
-        return await self.__aiohttp_client.client_protocolj(
+        return await self.client_protocolj(
             {
                 Keywords.COMMAND: Commands.EXECUTE,
                 Keywords.PAYLOAD: {
                     "function": function,
                     "args": args,
                     "kwargs": kwargs,
                 },
             },
         )
 
     # ----------------------------------------------------------------------------------------
-    async def close_client_session(self):
-        """"""
-
-        if self.__aiohttp_client is not None:
-            await self.__aiohttp_client.close_client_session()
-
-    # ----------------------------------------------------------------------------------------
-    async def client_report_health(self):
+    async def report_health(self):
         """"""
-
-        return await self.__aiohttp_client.client_report_health()
+        return await self.__send_protocolj("report_health")
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_api/datafaces/context.py` & `dls-servbase-1.6.0/src/dls_servbase_api/guis/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,43 @@
 import logging
 
+# Base class.
+from dls_utilpack.client_context_base import ClientContextBase
+
 # Things created in the context.
-from dls_servbase_api.datafaces.datafaces import (
-    Datafaces,
-    dls_servbase_datafaces_set_default,
-)
+from dls_servbase_api.guis.guis import Guis, dls_servbase_guis_set_default
 
 logger = logging.getLogger(__name__)
 
 
-class Context:
+class Context(ClientContextBase):
     """
-    Client context for a dls_servbase_dataface object.
+    Client context for a dls_servbase_gui object.
     On entering, it creates the object according to the specification (a dict).
     On exiting, it closes client connection.
 
-    The aenter and aexit methods are exposed for use by an enclosing context.
+    The aenter and aexit methods are exposed for use by an enclosing context and the base class.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
-        self.__specification = specification
-        self.__dls_servbase_dataface = None
-
-    # ----------------------------------------------------------------------------------------
-    async def __aenter__(self):
-        """ """
-
-        await self.aenter()
-
-    # ----------------------------------------------------------------------------------------
-    async def __aexit__(self, type, value, traceback):
-        """ """
-
-        await self.aexit()
+        ClientContextBase.__init__(self, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
         # Build the object according to the specification.
-        self.__dls_servbase_dataface = Datafaces().build_object(self.__specification)
+        self.interface = Guis().build_object(self.specification)
 
-        # If there is more than one dataface, the last one defined will be the default.
-        dls_servbase_datafaces_set_default(self.__dls_servbase_dataface)
+        # If there is more than one gui, the last one defined will be the default.
+        dls_servbase_guis_set_default(self.interface)
 
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
 
-        if self.__dls_servbase_dataface is not None:
-            await self.__dls_servbase_dataface.close_client_session()
+        if self.interface is not None:
+            await self.interface.close_client_session()
 
             # Clear the global variable.  Important between pytests.
-            dls_servbase_datafaces_set_default(None)
+            dls_servbase_guis_set_default(None)
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_api/datafaces/datafaces.py` & `dls-servbase-1.6.0/src/dls_servbase_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_cli/main.py` & `dls-servbase-1.6.0/src/dls_servbase_cli/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python
 
 import argparse
-
-# Use standard python logging
 import logging
 import multiprocessing
 
-# Base class with methods supporting command-line programs.
+# Base class with methods supporting MaxIV command-line programs.
 from dls_mainiac_lib.mainiac import Mainiac
 
 # The subcommands.
-from dls_servbase_cli.subcommands.start_services import StartServices
+from dls_servbase_cli.subcommands.service import Service
 
 # The package version.
 from dls_servbase_cli.version import meta as version_meta
 from dls_servbase_cli.version import version
 
 logger = logging.getLogger(__name__)
 
@@ -24,30 +22,30 @@
     def __init__(self, app_name):
         super().__init__(app_name)
 
     # ----------------------------------------------------------
     def run(self):
         """"""
 
-        if self._args.subcommand == "start_services":
-            StartServices(self._args, self).run()
+        if self._args.subcommand == "service":
+            Service(self._args, self).run()
 
         else:
             raise RuntimeError("unhandled subcommand %s" % (self._args.subcommand))
 
     # ----------------------------------------------------------
     def build_parser(self, arglist=None):
         """
         Method called from mainiac command line parsing.
         Should return argparser for this program.
         """
 
         # Make a parser.
         parser = argparse.ArgumentParser(
-            description="Command line app for checking quality of femtoscan file in progress.",
+            description="Command line interface to dls-servbase.",
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
 
         # --------------------------------------------------------------------
 
         parser.add_argument(
             "--log_name",
@@ -59,16 +57,19 @@
         )
 
         # --------------------------------------------------------------------
         subparsers = parser.add_subparsers(help="subcommands", dest="subcommand")
         subparsers.required = True
 
         # --------------------------------------------------------------------
-        subparser = subparsers.add_parser("start_services", help="Start service(s).")
-        StartServices.add_arguments(subparser)
+        subparser = subparsers.add_parser(
+            "service",
+            help="Start single service and block until ^C or remotely requested shutdown.",
+        )
+        Service.add_arguments(subparser)
 
         return parser
 
     # --------------------------------------------------------------------------
     def configure_logging(self, settings=None):
         """
         Configure runtime logging, override base class.
@@ -88,21 +89,16 @@
         settings = {
             "mpqueue": {"enabled": True},
         }
 
         # Let the base class do most of the work.
         Mainiac.configure_logging(self, settings)
 
-        # See bisstis-maxiv-daqcluster for advanced logging filters.
-
-        # Don't show matplotlib font debug.
-        logging.getLogger("matplotlib.font_manager").setLevel("INFO")
-
-        # Set filter on the ispyb logger to ignore the annoying NOTICE.
-        logging.getLogger("ispyb").addFilter(_ispyb_logging_filter())
+        # Don't show specific asyncio debug.
+        logging.getLogger("asyncio").addFilter(_asyncio_logging_filter())
 
     # ----------------------------------------------------------
     def version(self):
         """
         Method called from mainiac command line parsing.
         Should return string in form of N.N.N.
         """
@@ -115,54 +111,51 @@
         Should return dict which can be serialized by json.
         """
 
         return {"versions": version_meta()}
 
 
 # --------------------------------------------------------------------------------
-class _ispyb_logging_filter:
+class _asyncio_logging_filter:
     """
-    Python logging filter to remove annoying traitlets messages.
+    Python logging filter to remove annoying asyncio messages.
     These are not super useful to see all the time at the DEBUG level.
     """
 
     def filter(self, record):
 
-        if record.msg.startswith(
-            "NOTICE: This code uses __future__ functionality in the ISPyB API."
-        ):
+        if "Using selector" in record.msg:
             return 0
 
         return 1
 
 
-# # --------------------------------------------------------------------------------
-# class _matplotlib_logging_filter:
-#     """
-#     Python logging filter to remove annoying matplotlib messages.
-#     These are not super useful to see all the time at the INIT level.
-#     """
-
-#     def filter(self, record):
-#         if "loaded modules" in record.msg:
-#             return 0
-
-#         return 1
-
-
 # ---------------------------------------------------------------
 def main():
 
     # Instantiate the app.
     main = Main("dls_servbase_cli")
 
     # Configure the app from command line arguments.
     main.parse_args_and_configure_logging()
 
     # Run the main wrapped in a try/catch.
     main.try_run_catch()
 
 
 # ---------------------------------------------------------------
+def get_parser():
+    """
+    Called from sphinx automodule.
+    """
+
+    # Instantiate the app.
+    main = Main("dls_servbase_cli")
+
+    # Configure the app from command line arguments.
+    return main.build_parser()
+
+
+# ---------------------------------------------------------------
 # From command line, invoke the main method.
 if __name__ == "__main__":
     main()
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/__main__.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/base_aiohttp.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/base_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/cookies/base.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/cookies/cookie_parser.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/cookies/cookies.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/cookies/dataface.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/cookies/dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/aiohttp.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/aiohttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain
 from dls_utilpack.require import require
 
 # Basic things.
 from dls_utilpack.thing import Thing
 
+# Class types.
+from dls_servbase_api.constants import ClassTypes
+
 # Dataface protocolj things.
 from dls_servbase_api.datafaces.constants import Commands, Keywords
 
 # Base class for an aiohttp server.
 from dls_servbase_lib.base_aiohttp import BaseAiohttp
 
 # Types of dls_servbase_dataface.
 # Global dls_servbase_dataface.
 from dls_servbase_lib.datafaces.datafaces import Datafaces
 
 logger = logging.getLogger(__name__)
 
-thing_type = "dls_servbase_lib.datafaces.aiohttp"
+thing_type = ClassTypes.AIOHTTP
 
 
 # ------------------------------------------------------------------------------------------
 class Aiohttp(Thing, BaseAiohttp):
     """
     Object implementing remote procedure calls for dls_servbase_dataface methods.
     """
@@ -90,16 +93,14 @@
                     "actual_dataface_specification"
                 ]
             )
 
             # Get the local implementation started.
             await self.__actual_dls_servbase_dataface.start()
 
-            logger.debug(f"calling coro of {callsign(self)}")
-
             await self.activate_coro_base(route_tuples)
 
         except Exception:
             # We managed to get a dataface alive?
             if self.__actual_dls_servbase_dataface is not None:
                 # Need to disconnect it so outer asyncio loop will quit.
                 logger.debug(
@@ -128,17 +129,17 @@
         # Let the base class stop the server listener.
         await self.base_direct_shutdown()
 
     # ----------------------------------------------------------------------------------------
     async def __do_actually(self, function, args, kwargs):
         """"""
 
-        # logger.info(describe("function", function))
-        # logger.info(describe("args", args))
-        # logger.info(describe("kwargs", kwargs))
+        # logger.info(describe("[CLIOPS] function", function))
+        # logger.info(describe("[CLIOPS] args", args))
+        # logger.info(describe("[CLIOPS] kwargs", kwargs))
 
         function = getattr(self.__actual_dls_servbase_dataface, function)
 
         response = await function(*args, **kwargs)
 
         return response
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/context.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 from typing import Dict
 
-# Base class for an asyncio context
-from dls_servbase_lib.contexts.base import Base as ContextBase
+# Base class for an asyncio server context.
+from dls_utilpack.server_context_base import ServerContextBase
 
 # Things created in the context.
 from dls_servbase_lib.datafaces.datafaces import Datafaces
 
 logger = logging.getLogger(__name__)
 
 
 thing_type = "dls_servbase_lib.datafaces.context"
 
 
-class Context(ContextBase):
+class Context(ServerContextBase):
     """
     Asyncio context for a servbase object.
     On entering, it creates the object according to the specification (a dict).
     If specified, it starts the server as a coroutine, thread or process.
     If not a server, then it will instatiate a direct access to a servbase.
     On exiting, it commands the server to shut down and/or releases the direct access resources.
     """
@@ -28,58 +28,61 @@
         Constructor.
 
         Args:
             specification (Dict): specification of the servbase object to be constructed within the context.
                 The only key in the specification that relates to the context is "start_as", which can be "coro", "thread", "process" or None.
                 All other keys in the specification relate to creating the servbase object.
         """
-        ContextBase.__init__(self, thing_type, specification)
+        ServerContextBase.__init__(self, thing_type, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self) -> None:
         """
         Asyncio context entry.
 
         Starts and activates service as specified.
 
         Establishes the global (singleton-like) default servbase.
         """
 
         # Build the object according to the specification.
         self.server = Datafaces().build_object(self.specification())
 
-        if self.context_specification.get("start_as") == "coro":
+        start_as = self.context_specification.get("start_as")
+        if start_as == "coro":
             await self.server.activate_coro()
 
-        elif self.context_specification.get("start_as") == "thread":
+        elif start_as == "thread":
             await self.server.start_thread()
 
-        elif self.context_specification.get("start_as") == "process":
+        elif start_as == "process":
             await self.server.start_process()
 
         # Not running as a service?
-        elif self.context_specification.get("start_as") == "direct":
+        elif start_as == "direct":
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
-            if self.context_specification.get("start_as") == "process":
+            start_as = self.context_specification.get("start_as")
+
+            if start_as == "process":
                 logger.info(
                     "[DISSHU] in context exit, sending shutdown to client process"
                 )
                 # Put in request to shutdown the server.
                 await self.server.client_shutdown()
                 logger.info("[DISSHU] in context exit, sent shutdown to client process")
 
-            if self.context_specification.get("start_as") == "coro":
+            if start_as == "coro":
                 await self.server.direct_shutdown()
 
-            if self.context_specification.get("start_as") == "direct":
+            if start_as == "direct":
                 await self.server.deactivate()
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/datafaces.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/guis/guis.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,55 +3,53 @@
 
 # Class managing list of things.
 from dls_utilpack.things import Things
 
 # Exceptions.
 from dls_servbase_api.exceptions import NotFound
 
+# Types.
+from dls_servbase_api.guis.constants import Types
+
 logger = logging.getLogger(__name__)
 
 
 # -----------------------------------------------------------------------------------------
 
 
-class Datafaces(Things):
+class Guis(Things):
     """
-    List of available dls_servbase_datafaces.
+    List of available dls_servbase_guis.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, name=None):
         Things.__init__(self, name)
 
     # ----------------------------------------------------------------------------------------
     def build_object(self, specification):
         """"""
 
-        dls_servbase_dataface_class = self.lookup_class(specification["type"])
+        dls_servbase_gui_class = self.lookup_class(specification["type"])
 
         try:
-            dls_servbase_dataface_object = dls_servbase_dataface_class(specification)
+            dls_servbase_gui_object = dls_servbase_gui_class(specification)
         except Exception as exception:
             raise RuntimeError(
-                "unable to build dls_servbase_dataface object for type %s"
-                % (dls_servbase_dataface_class)
+                "unable to build dls_servbase_gui object for type %s"
+                % (dls_servbase_gui_class)
             ) from exception
 
-        return dls_servbase_dataface_object
+        return dls_servbase_gui_object
 
     # ----------------------------------------------------------------------------------------
     def lookup_class(self, class_type):
         """"""
 
-        if class_type == "dls_servbase_lib.datafaces.aiohttp":
-            from dls_servbase_lib.datafaces.aiohttp import Aiohttp
+        if class_type == Types.AIOHTTP:
+            from dls_servbase_lib.guis.aiohttp import Aiohttp
 
             return Aiohttp
 
-        elif class_type == "dls_servbase_lib.datafaces.normsql":
-            from dls_servbase_lib.datafaces.normsql import Normsql
-
-            return Normsql
-
         raise NotFound(
-            "unable to get dls_servbase_dataface class for type %s" % (class_type)
+            "unable to get dls_servbase_gui class for type %s" % (class_type)
         )
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/normsql.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/datafaces/normsql.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 # Database manager.
 from dls_normsql.databases import Databases
 
 # Base class for generic things.
 from dls_utilpack.thing import Thing
 
+# Class types.
+from dls_servbase_api.constants import ClassTypes
 from dls_servbase_api.databases.constants import Tablenames
 from dls_servbase_api.databases.database_definition import DatabaseDefinition
 
 logger = logging.getLogger(__name__)
 
-thing_type = "dls_servbase_lib.datafaces.normsql"
+thing_type = ClassTypes.NORMSQL
 
 
 class Normsql(Thing):
     """ """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification=None):
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/guis/aiohttp.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/guis/context.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/guis/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 import logging
 
-# Base class which maps flask requests to methods.
-from dls_servbase_lib.contexts.base import Base as ContextBase
+# Base class for an asyncio server context.
+from dls_utilpack.server_context_base import ServerContextBase
 
 # Things created in the context.
-from dls_servbase_lib.guis.guis import Guis, dls_servbase_guis_set_default
+from dls_servbase_lib.guis.guis import Guis
 
 logger = logging.getLogger(__name__)
 
 
 thing_type = "dls_servbase_lib.dls_servbase_guis.context"
 
 
-class Context(ContextBase):
+class Context(ServerContextBase):
     """
     Object representing an event dls_servbase_dataface connection.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
-        ContextBase.__init__(self, thing_type, specification)
+        ServerContextBase.__init__(self, thing_type, specification)
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
         self.server = Guis().build_object(self.specification())
 
-        # If there is more than one gui, the last one defined will be the default.
-        dls_servbase_guis_set_default(self.server)
-
         if self.context_specification.get("start_as") == "coro":
             await self.server.activate_coro()
 
         elif self.context_specification.get("start_as") == "thread":
             await self.server.start_thread()
 
         elif self.context_specification.get("start_as") == "process":
             await self.server.start_process()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self):
+    async def aexit(self, type, value, traceback):
         """ """
 
         if self.server is not None:
             # Put in request to shutdown the server.
             await self.server.client_shutdown()
 
             # Release a client connection if we had one.
             await self.server.close_client_session()
-
-        dls_servbase_guis_set_default(None)
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/guis/guis.py` & `dls-servbase-1.6.0/src/dls_servbase_api/guis/guis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Use standard logging in this module.
 import logging
 
+# Exceptions.
+from dls_utilpack.exceptions import NotFound
+
 # Class managing list of things.
 from dls_utilpack.things import Things
 
-# Exceptions.
-from dls_servbase_api.exceptions import NotFound
+# Types.
+from dls_servbase_api.guis.constants import Types
 
 logger = logging.getLogger(__name__)
 
 # -----------------------------------------------------------------------------------------
 __default_dls_servbase_gui = None
 
 
@@ -21,19 +24,14 @@
 def dls_servbase_guis_get_default():
     global __default_dls_servbase_gui
     if __default_dls_servbase_gui is None:
         raise RuntimeError("dls_servbase_guis_get_default instance is None")
     return __default_dls_servbase_gui
 
 
-def dls_servbase_guis_has_default():
-    global __default_dls_servbase_gui
-    return __default_dls_servbase_gui is not None
-
-
 # -----------------------------------------------------------------------------------------
 
 
 class Guis(Things):
     """
     List of available dls_servbase_guis.
     """
@@ -48,25 +46,23 @@
 
         dls_servbase_gui_class = self.lookup_class(specification["type"])
 
         try:
             dls_servbase_gui_object = dls_servbase_gui_class(specification)
         except Exception as exception:
             raise RuntimeError(
-                "unable to build dls_servbase_gui object for type %s"
+                "unable to build dls_servbase gui object for type %s"
                 % (dls_servbase_gui_class)
             ) from exception
 
         return dls_servbase_gui_object
 
     # ----------------------------------------------------------------------------------------
     def lookup_class(self, class_type):
         """"""
 
-        if class_type == "dls_servbase_lib.dls_servbase_guis.aiohttp":
-            from dls_servbase_lib.guis.aiohttp import Aiohttp
+        if class_type == Types.AIOHTTP:
+            from dls_servbase_api.guis.aiohttp import Aiohttp
 
             return Aiohttp
 
-        raise NotFound(
-            "unable to get dls_servbase_gui class for type %s" % (class_type)
-        )
+        raise NotFound(f"unable to get dls_servbase gui class for type {class_type}")
```

### Comparing `dls-servbase-1.5.0/src/dls_servbase_lib/version.py` & `dls-servbase-1.6.0/src/dls_servbase_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/tests/base.py` & `dls-servbase-1.6.0/tests/base_tester.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 import multiprocessing
 
 import pytest
 
 logger = logging.getLogger(__name__)
 
 
-class Base:
-
-    # ----------------------------------------------------------------------------------------
-    def main(self, constants, infrastrcuture_context, output_directory):
-        """ """
+# ----------------------------------------------------------------------------------------
+class BaseTester:
+    """
+    Provide asyncio loop and error checking over *Tester classes.
+    """
+
+    def main(self, constants, specification, output_directory):
+        """
+        This is the main program which calls the test using asyncio.
+        """
 
         multiprocessing.current_process().name = "main"
 
         failure_message = None
         try:
             # Run main test in asyncio event loop.
             asyncio.run(
-                self._main_coroutine(
-                    constants, infrastrcuture_context, output_directory
-                )
+                self._main_coroutine(constants, specification, output_directory)
             )
 
         except Exception as exception:
             logger.exception(
                 "unexpected exception in the test method", exc_info=exception
             )
             failure_message = str(exception)
```

### Comparing `dls-servbase-1.5.0/tests/base_context_tester.py` & `dls-servbase-1.6.0/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/tests/configurations/mysql.yaml` & `dls-servbase-1.6.0/tests/configurations/mysql.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                     username: "root"
                     password: "root"
     context:
         start_as: process
 
 # The dls_servbase_gui specification.
 dls_servbase_gui_specification:
-    type: "dls_servbase_lib.dls_servbase_guis.aiohttp"
+    type: "dls_servbase_lib.guis.aiohttp"
     type_specific_tbd:
         # The remote dls_servbase_gui server access.
         aiohttp_specification:
             server: *DLS_SERVBASE_GUI_SERVER
             client: *DLS_SERVBASE_GUI_CLIENT
             search_paths: ["examples/html"]
             cookie_specification:
```

### Comparing `dls-servbase-1.5.0/tests/configurations/sqlite.yaml` & `dls-servbase-1.6.0/tests/configurations/sqlite.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 filename: "${output_directory}/dls_servbase_dataface.sqlite"
                 log_level: "WARNING"
     context:
         start_as: process
 
 # The dls_servbase_gui specification.
 dls_servbase_gui_specification:
-    type: "dls_servbase_lib.dls_servbase_guis.aiohttp"
+    type: "dls_servbase_lib.guis.aiohttp"
     type_specific_tbd:
         # The remote dls_servbase_gui server access.
         aiohttp_specification:
             server: *DLS_SERVBASE_GUI_SERVER
             client: *DLS_SERVBASE_GUI_CLIENT
             search_paths: ["examples/html"]
             cookie_specification:
```

### Comparing `dls-servbase-1.5.0/tests/conftest.py` & `dls-servbase-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/tests/test_aiohttp.py` & `dls-servbase-1.6.0/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/tests/test_database.py` & `dls-servbase-1.6.0/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from dls_normsql.constants import ClassTypes
 from dls_normsql.databases import Databases
 
 from dls_servbase_api.databases.constants import CookieFieldnames, Tablenames
 from dls_servbase_api.databases.database_definition import DatabaseDefinition
-from tests.base_tester import BaseTester2
+from tests.base_tester import BaseTester
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
 class TestDatabaseSqlite:
     def test(self, constants, logging_setup, output_directory):
@@ -57,15 +57,15 @@
             constants,
             database_specification,
             output_directory,
         )
 
 
 # ----------------------------------------------------------------------------------------
-class DatabaseTester(BaseTester2):
+class DatabaseTester(BaseTester):
     """
     Test direct SQL access to the database.
     """
 
     async def _main_coroutine(
         self, constants, database_specification, output_directory
     ):
```

### Comparing `dls-servbase-1.5.0/tests/test_dataface.py` & `dls-servbase-1.6.0/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/tests/test_dataface_takeover.py` & `dls-servbase-1.6.0/tests/test_dataface_takeover.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.5.0/tests/test_gui.py` & `dls-servbase-1.6.0/tests/test_gui.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 
 # Utilities.
 from dls_utilpack.describe import describe
 
 # API constants.
 from dls_servbase_api.constants import Keywords as ProtocoljKeywords
 
-# Context creator.
-from dls_servbase_lib.contexts.contexts import Contexts
+# Client context.
+from dls_servbase_api.guis.context import Context as GuiClientContext
+from dls_servbase_api.guis.guis import dls_servbase_guis_get_default
+
+# Dataface server context.
+from dls_servbase_lib.datafaces.context import Context as DlsServbaseDatafaceContext
+
+# GUI constants.
 from dls_servbase_lib.guis.constants import Commands, Cookies, Keywords
 
-# Object managing gui
-from dls_servbase_lib.guis.guis import dls_servbase_guis_get_default
+# Server context.
+from dls_servbase_lib.guis.context import Context as GuiServerContext
 
 # Base class for the tester.
 from tests.base_context_tester import BaseContextTester
 
 logger = logging.getLogger(__name__)
 
 
@@ -42,139 +48,155 @@
 
     # Called from the base class main method.
     async def _main_coroutine(self, constants, output_directory):
         """ """
 
         # Make a multiconf and load the context configuration file.
         multiconf = self.get_multiconf()
-        context_configuration = await multiconf.load()
+        multiconf_dict = await multiconf.load()
 
-        dls_servbase_gui_specification = context_configuration[
-            "dls_servbase_gui_specification"
-        ]
-        type_specific_tbd = dls_servbase_gui_specification["type_specific_tbd"]
+        dataface_specification = multiconf_dict["dls_servbase_dataface_specification"]
+        dataface_context = DlsServbaseDatafaceContext(dataface_specification)
+
+        gui_specification = multiconf_dict["dls_servbase_gui_specification"]
+        type_specific_tbd = gui_specification["type_specific_tbd"]
         aiohttp_specification = type_specific_tbd["aiohttp_specification"]
         aiohttp_specification["search_paths"] = [output_directory]
 
-        # Make a context instance which can start a service and stop it at the end.
-        dls_servbase_context = Contexts().build_object(context_configuration)
+        # Make the server context.
+        gui_server_context = GuiServerContext(gui_specification)
+
+        # Make the client context.
+        gui_client_context = GuiClientContext(gui_specification)
 
-        async with dls_servbase_context:
+        # Start the dataface the gui uses for cookies.
+        async with dataface_context:
+            # Start the gui client context.
+            async with gui_client_context:
+                # And the gui server context which starts the coro.
+                async with gui_server_context:
+                    await self.__run_the_test(constants, output_directory)
+
+    # ----------------------------------------------------------------------------------------
+
+    async def __run_the_test(self, constants, output_directory):
+        """ """
+        # Reference the xchembku object which the context has set up as the default.
+        gui = dls_servbase_guis_get_default()
 
-            # --------------------------------------------------------------------
-            # Use protocolj to fetch a request from the dataface.
-            # Simulates what javascript would do by ajax.
-
-            # Load tabs, of which there are none at the start.
-            # This establishes the cookie though.
-            load_tabs_request = {
-                Keywords.COMMAND: Commands.LOAD_TABS,
-                ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
-            }
-
-            logger.debug("---------------------- making request 1 --------------------")
-            response = await dls_servbase_guis_get_default().client_protocolj(
-                load_tabs_request, cookies={}
-            )
-
-            # The response is json, with the last saved tab_id, which is None at first.
-            assert Keywords.TAB_ID in response
-            assert response[Keywords.TAB_ID] is None
-
-            # We should also have cookies back.
-            assert "__cookies" in response
-            cookies = response["__cookies"]
-            assert Cookies.TABS_MANAGER in cookies
-
-            # Use the tabs manager cookie value in the next requests.
-            cookie_uuid = cookies[Cookies.TABS_MANAGER].value
-
-            # --------------------------------------------------------------------
-            # Select a tab.
-            # The response is json, but nothing really to see in it.
-
-            select_tab_request = {
-                Keywords.COMMAND: Commands.SELECT_TAB,
-                ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
-                Keywords.TAB_ID: "123",
-            }
-
-            logger.debug("---------------------- making request 2 --------------------")
-            response = await dls_servbase_guis_get_default().client_protocolj(
-                select_tab_request, cookies={Cookies.TABS_MANAGER: cookie_uuid}
-            )
-
-            # --------------------------------------------------------------------
-            # Load tabs again, this time we should get the saved tab_id.
-
-            logger.debug("---------------------- making request 3 --------------------")
-            # Put a deliberately funky cookie string into the header.
-            raw_cookie_header = (
-                'BadCookie={"something"}; ' + f"{Cookies.TABS_MANAGER} = {cookie_uuid};"
-            )
-            response = await dls_servbase_guis_get_default().client_protocolj(
-                load_tabs_request,
-                headers={"Cookie": raw_cookie_header},
-            )
-
-            logger.debug(describe("second load_tabs response", response))
-            assert Keywords.TAB_ID in response
-            assert response[Keywords.TAB_ID] == "123"
-
-            # --------------------------------------------------------------------
-            # Update a tab.
-            # The response is json, but nothing really to see in it.
-
-            select_tab_request = {
-                Keywords.COMMAND: Commands.SELECT_TAB,
-                ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
-                Keywords.TAB_ID: "456",
-            }
-
-            logger.debug("---------------------- making request 4 --------------------")
-            response = await dls_servbase_guis_get_default().client_protocolj(
-                select_tab_request,
-                cookies={Cookies.TABS_MANAGER: cookie_uuid},
-            )
-
-            # --------------------------------------------------------------------
-            # Load tabs again, this time we should get the updated tab_id.
-
-            logger.debug("---------------------- making request 5 --------------------")
-            response = await dls_servbase_guis_get_default().client_protocolj(
-                load_tabs_request,
-                cookies={Cookies.TABS_MANAGER: cookie_uuid},
-            )
-
-            logger.debug(describe("third load_tabs response", response))
-            assert Keywords.TAB_ID in response
-            assert response[Keywords.TAB_ID] == "456"
-
-            # --------------------------------------------------------------------
-            # Write a text file and fetch it through the http server.
-            filename = "test.html"
-            contents = "some test html"
-            with open(f"{output_directory}/{filename}", "wt") as file:
-                file.write(contents)
-            logger.debug(
-                "---------------------- making request 6 (html file) --------------------"
-            )
-            text = await dls_servbase_guis_get_default().client_get_file(filename)
-            # assert text == contents
-
-            # Write a binary file and fetch it through the http server.
-            filename = "test.exe"
-            contents = "some test binary"
-            with open(f"{output_directory}/{filename}", "wt") as file:
-                file.write(contents)
-            binary = await dls_servbase_guis_get_default().client_get_file(filename)
-            # Binary comes back as bytes due to suffix of url filename.
-            assert binary == contents.encode()
-
-            # --------------------------------------------------------------------
-            # Get an html file automatically configured in guis/html.
-            filename = "javascript/version.js"
-            # TODO: Put proper version into javascript somehow during packaging.
-            contents = "dls_servbase___CURRENT_VERSION"
-            text = await dls_servbase_guis_get_default().client_get_file(filename)
-            logger.debug(f"javascript version is {text.strip()}")
-            assert contents in text
+        # --------------------------------------------------------------------
+        # Use protocolj to fetch a request from the dataface.
+        # Simulates what javascript would do by ajax.
+
+        # Load tabs, of which there are none at the start.
+        # This establishes the cookie though.
+        load_tabs_request = {
+            Keywords.COMMAND: Commands.LOAD_TABS,
+            ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
+        }
+
+        logger.debug("---------------------- making request 1 --------------------")
+        logger.debug(describe("gui", gui))
+        response = await gui.client_protocolj(load_tabs_request, cookies={})
+
+        # The response is json, with the last saved tab_id, which is None at first.
+        assert Keywords.TAB_ID in response
+        assert response[Keywords.TAB_ID] is None
+
+        # We should also have cookies back.
+        assert "__cookies" in response
+        cookies = response["__cookies"]
+        assert Cookies.TABS_MANAGER in cookies
+
+        # Use the tabs manager cookie value in the next requests.
+        cookie_uuid = cookies[Cookies.TABS_MANAGER].value
+
+        # --------------------------------------------------------------------
+        # Select a tab.
+        # The response is json, but nothing really to see in it.
+
+        select_tab_request = {
+            Keywords.COMMAND: Commands.SELECT_TAB,
+            ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
+            Keywords.TAB_ID: "123",
+        }
+
+        logger.debug("---------------------- making request 2 --------------------")
+        response = await gui.client_protocolj(
+            select_tab_request, cookies={Cookies.TABS_MANAGER: cookie_uuid}
+        )
+
+        # --------------------------------------------------------------------
+        # Load tabs again, this time we should get the saved tab_id.
+
+        logger.debug("---------------------- making request 3 --------------------")
+        # Put a deliberately funky cookie string into the header.
+        raw_cookie_header = (
+            'BadCookie={"something"}; ' + f"{Cookies.TABS_MANAGER} = {cookie_uuid};"
+        )
+        response = await gui.client_protocolj(
+            load_tabs_request,
+            headers={"Cookie": raw_cookie_header},
+        )
+
+        logger.debug(describe("second load_tabs response", response))
+        assert Keywords.TAB_ID in response
+        assert response[Keywords.TAB_ID] == "123"
+
+        # --------------------------------------------------------------------
+        # Update a tab.
+        # The response is json, but nothing really to see in it.
+
+        select_tab_request = {
+            Keywords.COMMAND: Commands.SELECT_TAB,
+            ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
+            Keywords.TAB_ID: "456",
+        }
+
+        logger.debug("---------------------- making request 4 --------------------")
+        response = await gui.client_protocolj(
+            select_tab_request,
+            cookies={Cookies.TABS_MANAGER: cookie_uuid},
+        )
+
+        # --------------------------------------------------------------------
+        # Load tabs again, this time we should get the updated tab_id.
+
+        logger.debug("---------------------- making request 5 --------------------")
+        response = await gui.client_protocolj(
+            load_tabs_request,
+            cookies={Cookies.TABS_MANAGER: cookie_uuid},
+        )
+
+        logger.debug(describe("third load_tabs response", response))
+        assert Keywords.TAB_ID in response
+        assert response[Keywords.TAB_ID] == "456"
+
+        # --------------------------------------------------------------------
+        # Write a text file and fetch it through the http server.
+        filename = "test.html"
+        contents = "some test html"
+        with open(f"{output_directory}/{filename}", "wt") as file:
+            file.write(contents)
+        logger.debug(
+            "---------------------- making request 6 (html file) --------------------"
+        )
+        text = await gui.client_get_file(filename)
+        # assert text == contents
+
+        # Write a binary file and fetch it through the http server.
+        filename = "test.exe"
+        contents = "some test binary"
+        with open(f"{output_directory}/{filename}", "wt") as file:
+            file.write(contents)
+        binary = await gui.client_get_file(filename)
+        # Binary comes back as bytes due to suffix of url filename.
+        assert binary == contents.encode()
+
+        # --------------------------------------------------------------------
+        # Get an html file automatically configured in guis/html.
+        filename = "javascript/version.js"
+        # TODO: Put proper version into javascript somehow during packaging.
+        contents = "dls_servbase___CURRENT_VERSION"
+        text = await gui.client_get_file(filename)
+        logger.debug(f"javascript version is {text.strip()}")
+        assert contents in text
```

### Comparing `dls-servbase-1.5.0/tests/test_parse_cookie.py` & `dls-servbase-1.6.0/tests/test_parse_cookie.py`

 * *Files identical despite different names*

