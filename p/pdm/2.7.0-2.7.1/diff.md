# Comparing `tmp/pdm-2.7.0.tar.gz` & `tmp/pdm-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.7.0.tar", last modified: Mon May 29 04:11:10 2023, max compression
+gzip compressed data, was "pdm-2.7.1.tar", last modified: Tue Jun  6 03:56:08 2023, max compression
```

## Comparing `pdm-2.7.0.tar` & `pdm-2.7.1.tar`

### file list

```diff
@@ -1,272 +1,272 @@
--rw-r--r--   0        0        0   121652 2023-05-29 04:11:03.270091 pdm-2.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-05-29 04:11:03.270091 pdm-2.7.0/LICENSE
--rw-r--r--   0        0        0     1075 2023-05-29 04:11:03.270091 pdm-2.7.0/LICENSE
--rw-r--r--   0        0        0     7986 2023-05-29 04:11:03.270091 pdm-2.7.0/README.md
--rw-r--r--   0        0        0     7986 2023-05-29 04:11:03.270091 pdm-2.7.0/README.md
--rw-r--r--   0        0        0     4384 2023-05-29 04:11:10.474134 pdm-2.7.0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/__version__.py
--rw-r--r--   0        0        0     3282 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    30077 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     2404 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2174 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6529 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     5812 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     2948 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     1071 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     8510 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3589 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15743 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8027 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     1672 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15445 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9364 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     2392 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     1318 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1683 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6171 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5083 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    38005 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18567 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25089 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10461 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/options.py
--rw-r--r--   0        0        0    24722 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2226 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/compat.py
--rw-r--r--   0        0        0    10647 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8850 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1365 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2400 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7474 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7190 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1390 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10901 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18161 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10990 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4394 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/backends.py
--rw-r--r--   0        0        0    10910 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26568 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1714 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6182 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2195 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    21031 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18068 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/search.py
--rw-r--r--   0        0        0     1340 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2721 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16002 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/config.py
--rw-r--r--   0        0        0    27041 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/py.typed
--rw-r--r--   0        0        0    19876 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13119 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/termui.py
--rw-r--r--   0        0        0    13866 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/conftest.py
--rw-r--r--   0        0        0    12370 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_add.py
--rw-r--r--   0        0        0     5799 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4496 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3872 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8888 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_update.py
--rw-r--r--   0        0        0     2942 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_use.py
--rw-r--r--   0        0        0    10430 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-05-29 04:11:03.290091 pdm-2.7.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-05-29 04:11:03.290091 pdm-2.7.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1329 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_backends.py
--rw-r--r--   0        0        0    13344 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2526 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7190 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_plugin.py
--rw-r--r--   0        0        0    12209 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_signals.py
--rw-r--r--   0        0        0     4419 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_utils.py
--rw-r--r--   0        0        0     9599 1970-01-01 00:00:00.000000 pdm-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0   122599 2023-06-06 03:56:01.064340 pdm-2.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-06-06 03:56:01.064340 pdm-2.7.1/LICENSE
+-rw-r--r--   0        0        0     1075 2023-06-06 03:56:01.064340 pdm-2.7.1/LICENSE
+-rw-r--r--   0        0        0     7986 2023-06-06 03:56:01.064340 pdm-2.7.1/README.md
+-rw-r--r--   0        0        0     7986 2023-06-06 03:56:01.064340 pdm-2.7.1/README.md
+-rw-r--r--   0        0        0     4396 2023-06-06 03:56:08.520348 pdm-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3282 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11850 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    30752 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2404 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2174 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6529 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     5812 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     2948 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     1071 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     8510 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3589 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15743 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8027 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     1672 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15445 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9364 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     2392 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     1318 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1683 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6171 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5083 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    38005 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18567 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25089 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10461 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/options.py
+-rw-r--r--   0        0        0    24722 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2226 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/compat.py
+-rw-r--r--   0        0        0    10647 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8850 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     3560 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1365 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2400 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7358 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1390 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10901 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18161 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10990 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4394 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    11466 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26568 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1714 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6182 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2195 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    21340 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18677 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/search.py
+-rw-r--r--   0        0        0     1344 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2721 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16748 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26273 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/py.typed
+-rw-r--r--   0        0        0    19876 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13119 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/termui.py
+-rw-r--r--   0        0        0    13866 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12377 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5799 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4496 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3872 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     8888 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2942 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10430 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-06-06 03:56:01.084340 pdm-2.7.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      574 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      728 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      332 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo/setup.py
+-rw-r--r--   0        0        0       26 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13344 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2526 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7197 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-06-06 03:56:01.096340 pdm-2.7.1/tests/test_signals.py
+-rw-r--r--   0        0        0     4419 2023-06-06 03:56:01.096340 pdm-2.7.1/tests/test_utils.py
+-rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 pdm-2.7.1/PKG-INFO
```

### Comparing `pdm-2.7.0/CHANGELOG.md` & `pdm-2.7.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Release v2.7.1 (2023-06-06)
+---------------------------
+
+### Features & Improvements
+
+- Switch HTTP data cache to use a split body setup, where the actual body contents are not written to disk unless changed. Previously, any changed headers would write the whole body to disk again. [#1971](https://github.com/pdm-project/pdm/issues/1971)
+- Show the specific install commands for different installations when checking update. This was removed before. [#1972](https://github.com/pdm-project/pdm/issues/1972)
+
+### Bug Fixes
+
+- PDM ignores env vars `PDM_PYPI_USERNAME` and `PDM_PYPI_PASSWORD` when there are no defaults in config. [#1961](https://github.com/pdm-project/pdm/issues/1961)
+- Guess the project name from VCS url if it is missing when importing from requirements.txt. [#1970](https://github.com/pdm-project/pdm/issues/1970)
+- Correctly read the config from environment variables. [#1977](https://github.com/pdm-project/pdm/issues/1977)
+
+
 Release v2.7.0 (2023-05-29)
 ---------------------------
 
 ### Features & Improvements
 
 - When keyring is available, either by importing or by CLI, the credentials of repositories and PyPI indexes will be saved into it. [#1908](https://github.com/pdm-project/pdm/issues/1908)
 - Add support for reading metadata from simple index directly. [#1919](https://github.com/pdm-project/pdm/issues/1919)
```

### Comparing `pdm-2.7.0/LICENSE` & `pdm-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/README.md` & `pdm-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/pyproject.toml` & `pdm-2.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "unearth>=0.9.0",
     "findpython>=0.2.2",
     "tomlkit>=0.11.1,<1",
     "shellingham>=1.3.2",
     "python-dotenv>=0.15",
     "resolvelib>=1.0.1",
     "installer<0.8,>=0.7",
-    "cacheyou[filecache]",
+    "cachecontrol[filecache]>=0.13.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
 readme = "README.md"
 keywords = [
     "packaging",
     "dependency",
@@ -37,15 +37,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.7.0"
+version = "2.7.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.7.0/src/pdm/_types.py` & `pdm-2.7.1/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/builders/base.py` & `pdm-2.7.1/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/builders/editable.py` & `pdm-2.7.1/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/builders/sdist.py` & `pdm-2.7.1/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/builders/wheel.py` & `pdm-2.7.1/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/actions.py` & `pdm-2.7.1/src/pdm/cli/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -730,21 +730,37 @@
     return latest_version
 
 
 def check_update(project: Project) -> None:
     """Check if there is a new version of PDM available"""
     from packaging.version import Version
 
+    from pdm.cli.utils import is_homebrew_installation, is_pipx_installation, is_scoop_installation
+
     this_version = project.core.version
     latest_version = get_latest_version(project)
     if latest_version is None or Version(this_version) >= Version(latest_version):
         return
-    install_command = "pdm self update" + (" --pre" if Version(latest_version).is_prerelease else "")
     disable_command = "pdm config check_update false"
 
+    is_prerelease = Version(latest_version).is_prerelease
+
+    if is_pipx_installation():
+        install_command = f"pipx upgrade {'--pip-args=--pre ' if is_prerelease else ''}pdm"
+    elif is_homebrew_installation():
+        install_command = "brew upgrade pdm"
+    elif is_scoop_installation():
+        install_command = "scoop update pdm"
+    else:
+        install_command = "pdm self update" + (" --pre" if is_prerelease else "")
+        if os.name == "nt":
+            # On Windows, the executable can't replace itself, we add the python prefix to the command
+            # A bit ugly but it works
+            install_command = f"{sys.executable} -m {install_command}"
+
     message = [
         f"\nPDM [primary]{this_version}[/]",
         f" is installed, while [primary]{latest_version}[/]",
         " is available.\n",
         f"Please run [req]`{install_command}`[/]",
         " to upgrade.\n",
         f"Run [req]`{disable_command}`[/]",
```

### Comparing `pdm-2.7.0/src/pdm/cli/commands/add.py` & `pdm-2.7.1/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/base.py` & `pdm-2.7.1/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/build.py` & `pdm-2.7.1/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/cache.py` & `pdm-2.7.1/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/completion.py` & `pdm-2.7.1/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/config.py` & `pdm-2.7.1/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/export.py` & `pdm-2.7.1/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.7.1/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.7.1/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/import_cmd.py` & `pdm-2.7.1/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/info.py` & `pdm-2.7.1/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/init.py` & `pdm-2.7.1/src/pdm/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/install.py` & `pdm-2.7.1/src/pdm/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/list.py` & `pdm-2.7.1/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/lock.py` & `pdm-2.7.1/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.7.1/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/publish/package.py` & `pdm-2.7.1/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/publish/repository.py` & `pdm-2.7.1/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/remove.py` & `pdm-2.7.1/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/run.py` & `pdm-2.7.1/src/pdm/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/search.py` & `pdm-2.7.1/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/self_cmd.py` & `pdm-2.7.1/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/show.py` & `pdm-2.7.1/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/sync.py` & `pdm-2.7.1/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/update.py` & `pdm-2.7.1/src/pdm/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/use.py` & `pdm-2.7.1/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/activate.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/backends.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/create.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/list.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/purge.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/remove.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/commands/venv/utils.py` & `pdm-2.7.1/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/completions/pdm.bash` & `pdm-2.7.1/src/pdm/cli/completions/pdm.bash`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/completions/pdm.fish` & `pdm-2.7.1/src/pdm/cli/completions/pdm.fish`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/completions/pdm.ps1` & `pdm-2.7.1/src/pdm/cli/completions/pdm.ps1`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/completions/pdm.zsh` & `pdm-2.7.1/src/pdm/cli/completions/pdm.zsh`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/filters.py` & `pdm-2.7.1/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/hooks.py` & `pdm-2.7.1/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/options.py` & `pdm-2.7.1/src/pdm/cli/options.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/cli/utils.py` & `pdm-2.7.1/src/pdm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/compat.py` & `pdm-2.7.1/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/core.py` & `pdm-2.7.1/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/environments/__init__.py` & `pdm-2.7.1/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/environments/base.py` & `pdm-2.7.1/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/environments/local.py` & `pdm-2.7.1/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/environments/python.py` & `pdm-2.7.1/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/exceptions.py` & `pdm-2.7.1/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/formats/__init__.py` & `pdm-2.7.1/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/formats/base.py` & `pdm-2.7.1/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/formats/flit.py` & `pdm-2.7.1/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/formats/pipfile.py` & `pdm-2.7.1/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/formats/poetry.py` & `pdm-2.7.1/src/pdm/formats/poetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     def includes(self, source: dict[str, list[str] | str]) -> list[str]:
         includes: list[str] = []
         source_includes: list[str] = []
         for item in source.pop("packages", []):
             assert isinstance(item, dict)
             include = item["include"]
             if item.get("from"):
-                include = f"{item.get('from')}/{include}"
+                include = Path(str(item.get("from")), include).as_posix()
             includes.append(include)
         for item in source.pop("include", []):
             if not isinstance(item, dict):
                 includes.append(item)
             else:
                 dest = source_includes if "sdist" in item.get("format", "") else includes
                 dest.append(item["path"])
```

### Comparing `pdm-2.7.0/src/pdm/formats/requirements.py` & `pdm-2.7.1/src/pdm/formats/requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dataclasses
 import hashlib
 import shlex
 import urllib.parse
 from typing import TYPE_CHECKING, Any, Mapping
 
 from pdm.formats.base import make_array
-from pdm.models.requirements import Requirement, parse_requirement
+from pdm.models.requirements import FileRequirement, Requirement, parse_requirement
 
 if TYPE_CHECKING:
     from argparse import Namespace
     from os import PathLike
 
     from pdm.models.candidates import Candidate
     from pdm.project import Project
@@ -49,15 +49,19 @@
             return ""
         return line.split(" #", 1)[0].strip()
 
     def _parse_line(self, line: str) -> None:
         if not line.startswith("-"):
             # Starts with a requirement, just ignore all per-requirement options
             req_string = line.split(" -", 1)[0].strip()
-            self.requirements.append(parse_requirement(req_string))
+            req = parse_requirement(req_string)
+            if not req.name:
+                assert isinstance(req, FileRequirement)
+                req.name = req.guess_name()
+            self.requirements.append(req)
             return
         args, _ = self._parser.parse_known_args(shlex.split(line))
         if args.index_url:
             self.index_url = args.index_url
         if args.no_index:
             self.no_index = args.no_index
         if args.extra_index_url:
```

### Comparing `pdm-2.7.0/src/pdm/formats/setup_py.py` & `pdm-2.7.1/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/installers/core.py` & `pdm-2.7.1/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/installers/installers.py` & `pdm-2.7.1/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/installers/manager.py` & `pdm-2.7.1/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/installers/packages.py` & `pdm-2.7.1/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/installers/synchronizers.py` & `pdm-2.7.1/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/installers/uninstallers.py` & `pdm-2.7.1/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/auth.py` & `pdm-2.7.1/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/backends.py` & `pdm-2.7.1/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/caches.py` & `pdm-2.7.1/src/pdm/models/caches.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import hashlib
 import json
 import os
 from functools import lru_cache
 from pathlib import Path
 from typing import TYPE_CHECKING, BinaryIO, Generic, Iterable, TypeVar, cast
 
-from cacheyou.cache import BaseCache
-from cacheyou.caches import FileCache
+from cachecontrol.cache import SeparateBodyBaseCache
+from cachecontrol.caches import FileCache
 from packaging.utils import canonicalize_name, parse_wheel_filename
-
 from pdm._types import CandidateInfo
 from pdm.exceptions import PdmException
 from pdm.models.candidates import Candidate
 from pdm.termui import logger
 from pdm.utils import atomic_open_for_write, create_tracked_tempdir
 
 if TYPE_CHECKING:
@@ -243,15 +242,15 @@
             support_min = min(tags_priorities[tag] for tag in tags if tag in tags_priorities)
             candidates.append((support_min, candidate))
         if not candidates:
             return None
         return min(candidates, key=lambda x: x[0])[1]
 
 
-class SafeFileCache(BaseCache):
+class SafeFileCache(SeparateBodyBaseCache):
     """
     A file based cache which is safe to use even when the target directory may
     not be accessible or writable.
     """
 
     def __init__(self, directory: str) -> None:
         super().__init__()
@@ -266,22 +265,39 @@
         return os.path.join(self.directory, *parts)
 
     def get(self, key: str) -> bytes | None:
         path = self._get_cache_path(key)
         with contextlib.suppress(OSError):
             with open(path, "rb") as f:
                 return f.read()
+
+        return None
+
+    def get_body(self, key: str) -> BinaryIO | None:
+        path = self._get_cache_path(key)
+        with contextlib.suppress(OSError):
+            return cast(BinaryIO, open(f"{path}.body", "rb"))
+
         return None
 
     def set(self, key: str, value: bytes, expires: int | None = None) -> None:
         path = self._get_cache_path(key)
         with contextlib.suppress(OSError):
             with atomic_open_for_write(path, mode="wb") as f:
                 cast(BinaryIO, f).write(value)
 
+    def set_body(self, key: str, body: bytes) -> None:
+        if body is None:
+            return
+
+        path = self._get_cache_path(key)
+        with contextlib.suppress(OSError):
+            with atomic_open_for_write(f"{path}.body", mode="wb") as f:
+                cast(BinaryIO, f).write(body)
+
     def delete(self, key: str) -> None:
         path = self._get_cache_path(key)
         with contextlib.suppress(OSError):
             os.remove(path)
 
 
 @lru_cache(maxsize=128)
```

### Comparing `pdm-2.7.0/src/pdm/models/candidates.py` & `pdm-2.7.1/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/in_process/__init__.py` & `pdm-2.7.1/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.7.1/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/in_process/parse_setup.py` & `pdm-2.7.1/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/in_process/pep508.py` & `pdm-2.7.1/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.7.1/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/markers.py` & `pdm-2.7.1/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/project_info.py` & `pdm-2.7.1/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/python.py` & `pdm-2.7.1/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/repositories.py` & `pdm-2.7.1/src/pdm/models/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import posixpath
 import sys
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, TypeVar, cast
+from typing import TYPE_CHECKING, TypeVar, cast
 
 from pdm import termui
 from pdm.exceptions import CandidateInfoNotFound, CandidateNotFound
 from pdm.models.candidates import Candidate, make_candidate
 from pdm.models.requirements import (
     Requirement,
     filter_requirements_with_extras,
@@ -21,19 +21,23 @@
     normalize_name,
     path_to_url,
     url_to_path,
     url_without_fragments,
 )
 
 if TYPE_CHECKING:
+    from typing import Any, Callable, Iterable, Mapping
+
     from unearth import Link
 
     from pdm._types import CandidateInfo, RepositoryConfig, SearchResult
     from pdm.environments import BaseEnvironment
 
+    CandidateKey = tuple[str, str | None, str | None, bool]
+
 ALLOW_ALL_PYTHON = PySpecSet()
 T = TypeVar("T", bound="BaseRepository")
 
 
 def cache_result(func: Callable[[T, Candidate], CandidateInfo]) -> Callable[[T, Candidate], CandidateInfo]:
     @wraps(func)
     def wrapper(self: T, candidate: Candidate) -> CandidateInfo:
@@ -386,17 +390,17 @@
     def __init__(
         self,
         lockfile: Mapping[str, Any],
         sources: list[RepositoryConfig],
         environment: BaseEnvironment,
     ) -> None:
         super().__init__(sources, environment, ignore_compatibility=False)
-        self.packages: dict[tuple, Candidate] = {}
+        self.packages: dict[CandidateKey, Candidate] = {}
         self.file_hashes: dict[tuple[str, str], dict[Link, str]] = {}
-        self.candidate_info: dict[tuple, CandidateInfo] = {}
+        self.candidate_info: dict[CandidateKey, CandidateInfo] = {}
         self._read_lockfile(lockfile)
 
     @property
     def all_candidates(self) -> dict[str, Candidate]:
         return {can.req.identify(): can for can in self.packages.values()}
 
     def _read_lockfile(self, lockfile: Mapping[str, Any]) -> None:
@@ -424,15 +428,15 @@
                 self.candidate_info[can_id] = candidate_info
 
         for key, hashes in lockfile.get("metadata", {}).get("files", {}).items():
             self.file_hashes[tuple(key.split(None, 1))] = {  # type: ignore[index]
                 Link(item["url"]): item["hash"] for item in hashes if "url" in item
             }
 
-    def _identify_candidate(self, candidate: Candidate) -> tuple:
+    def _identify_candidate(self, candidate: Candidate) -> CandidateKey:
         url = getattr(candidate.req, "url", None)
         if url is not None:
             url = url_without_fragments(url)
             url = self.environment.project.backend.expand_line(url)
             if url.startswith("file://"):
                 path = posixpath.normpath(url_to_path(url))
                 url = path_to_url(path)
@@ -448,25 +452,30 @@
 
     def dependency_generators(self) -> Iterable[Callable[[Candidate], CandidateInfo]]:
         return (
             self._get_dependency_from_local_package,
             self._get_dependencies_from_lockfile,
         )
 
-    def _matching_keys(self, requirement: Requirement) -> Iterable[tuple]:
+    def _matching_keys(self, requirement: Requirement) -> Iterable[CandidateKey]:
+        from pdm.models.requirements import FileRequirement
+
         for key in self.candidate_info:
+            can_req = self.packages[key].req
             if requirement.name:
                 if key[0] != requirement.identify():
                     continue
-            elif key[2] is not None:
-                if key[2] != url_without_fragments(getattr(requirement, "url", "")):
-                    continue
             else:
-                can_req = self.packages[key].req
-                if can_req.path != getattr(requirement, "path", None):  # type: ignore[attr-defined]
+                assert isinstance(requirement, FileRequirement)
+                if not isinstance(can_req, FileRequirement):
+                    continue
+                if requirement.path and can_req.path:
+                    if requirement.path != can_req.path:
+                        continue
+                elif key[2] is not None and key[2] != url_without_fragments(requirement.url):
                     continue
 
             yield key
 
     def find_candidates(
         self,
         requirement: Requirement,
```

### Comparing `pdm-2.7.0/src/pdm/models/requirements.py` & `pdm-2.7.1/src/pdm/models/requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,43 @@
         self._parse_url()
         if self.is_local_dir:
             self._check_installable()
 
     def _hash_key(self) -> tuple:
         return (*super()._hash_key(), self.get_full_url(), self.editable)
 
+    def guess_name(self) -> str | None:
+        filename = os.path.basename(urlparse.unquote(url_without_fragments(self.url))).rsplit("@", 1)[0]
+        if self.is_vcs:
+            if self.vcs == "git":  # type: ignore[attr-defined]
+                name = filename
+                if name.endswith(".git"):
+                    name = name[:-4]
+                return name
+            elif self.vcs == "hg":  # type: ignore[attr-defined]
+                return filename
+            else:  # svn and bzr
+                name, in_branch, _ = filename.rpartition("/branches/")
+                if not in_branch and name.endswith("/trunk"):
+                    return name[:-6]
+                return name
+        elif filename.endswith(".whl"):
+            return parse_wheel_filename(filename)[0]
+        else:
+            try:
+                return parse_sdist_filename(filename)[0]
+            except ValueError:
+                match = _egg_info_re.match(filename)
+                # Filename is like `<name>-<version>.tar.gz`, where name will be
+                # extracted and version will be left to be determined from
+                # the metadata.
+                if match:
+                    return match.group(1)
+        return None
+
     @classmethod
     def create(cls: type[T], **kwargs: Any) -> T:
         if kwargs.get("path"):
             kwargs["path"] = Path(kwargs["path"])
         return super().create(**kwargs)
 
     @property
@@ -350,27 +379,15 @@
         if "egg" in fragments:
             egg_info = urlparse.unquote(fragments["egg"])
             name, extras = strip_extras(egg_info)
             self.name = name
             if not self.extras:
                 self.extras = extras
         if not self.name and not self.is_vcs:
-            filename = os.path.basename(urlparse.unquote(url_without_fragments(self.url)))
-            if filename.endswith(".whl"):
-                self.name, *_ = parse_wheel_filename(filename)
-            else:
-                try:
-                    self.name, *_ = parse_sdist_filename(filename)
-                except ValueError:
-                    match = _egg_info_re.match(filename)
-                    # Filename is like `<name>-<version>.tar.gz`, where name will be
-                    # extracted and version will be left to be determined from
-                    # the metadata.
-                    if match:
-                        self.name = match.group(1)
+            self.name = self.guess_name()
 
     def _check_installable(self) -> None:
         assert self.path
         if not (self.path.joinpath("setup.py").exists() or self.path.joinpath("pyproject.toml").exists()):
             raise RequirementError(f"The local path '{self.path}' is not installable.")
         result = Setup.from_directory(self.path.absolute())
         if result.name:
```

### Comparing `pdm-2.7.0/src/pdm/models/search.py` & `pdm-2.7.1/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/session.py` & `pdm-2.7.1/src/pdm/models/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 from pathlib import Path
 from typing import Any
 
-from cacheyou.adapter import CacheControlAdapter
+from cachecontrol.adapter import CacheControlAdapter
 from requests_toolbelt.utils import user_agent
 from unearth.session import InsecureMixin, PyPISession
 
 from pdm.__version__ import __version__
 
 
 class InsecureCacheControlAdapter(InsecureMixin, CacheControlAdapter):
```

### Comparing `pdm-2.7.0/src/pdm/models/setup.py` & `pdm-2.7.1/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/specifiers.py` & `pdm-2.7.1/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/venv.py` & `pdm-2.7.1/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/versions.py` & `pdm-2.7.1/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/models/working_set.py` & `pdm-2.7.1/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/pep582/sitecustomize.py` & `pdm-2.7.1/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/project/config.py` & `pdm-2.7.1/src/pdm/project/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import collections
 import dataclasses
 import os
 from pathlib import Path
-from typing import Any, Callable, Iterator, Mapping, MutableMapping
+from typing import Any, Callable, Iterator, Mapping, MutableMapping, cast
 
 import platformdirs
 import rich.theme
 import tomlkit
 
 from pdm import termui
 from pdm._types import RepositoryConfig
+from pdm.compat import cached_property
 from pdm.exceptions import NoConfigError, PdmUsageError
 
 REPOSITORY = "repository"
 SOURCE = "pypi"
 DEFAULT_REPOSITORIES = {
     "pypi": "https://upload.pypi.org/legacy/",
     "testpypi": "https://test.pypi.org/legacy/",
@@ -224,25 +225,33 @@
     def get_defaults(cls) -> dict[str, Any]:
         defaults = {k: v.default for k, v in cls._config_map.items() if v.should_show()}
         if cls.site is None:
             cls.site = Config(platformdirs.site_config_path("pdm") / "config.toml")
         defaults.update(cls.site)
         return defaults
 
+    @cached_property
+    def env_map(self) -> Mapping[str, Any]:
+        return EnvMap(self._config_map)
+
     @classmethod
     def add_config(cls, name: str, item: ConfigItem) -> None:
         """Add or modify a config item"""
         cls._config_map[name] = item
 
     def __init__(self, config_file: Path, is_global: bool = False):
         self.is_global = is_global
         self.config_file = config_file.resolve()
         self.deprecated = {v.replace: k for k, v in self._config_map.items() if v.replace}
         self._file_data = load_config(self.config_file)
-        self._data = collections.ChainMap(self._file_data, self.get_defaults() if is_global else {})
+        self._data = collections.ChainMap(
+            cast(MutableMapping[str, Any], self.env_map) if is_global else {},
+            self._file_data,
+            self.get_defaults() if is_global else {},
+        )
 
     def load_theme(self) -> rich.theme.Theme:
         if not self.is_global:  # pragma: no cover
             raise PdmUsageError("Theme can only be loaded from global config")
         return rich.theme.Theme({k[6:]: v for k, v in self.items() if k.startswith("theme.")})
 
     @property
@@ -282,24 +291,21 @@
             value = getattr(repo, parts[2]) if len(parts) >= 3 else repo
             return value
 
         if key not in self._config_map and key not in self.deprecated:
             raise NoConfigError(key)
         config_key = self.deprecated.get(key, key)
         config = self._config_map[config_key]
-        env_var = config.env_var
-        if env_var is not None and env_var in os.environ:
-            result = os.environ[env_var]
+
+        if config_key in self._data:
+            result = self._data[config_key]
+        elif config.replace:
+            result = self._data[config.replace]
         else:
-            if config_key in self._data:
-                result = self._data[config_key]
-            elif config.replace:
-                result = self._data[config.replace]
-            else:
-                raise NoConfigError(key) from None
+            raise NoConfigError(key) from None
         return config.coerce(result)
 
     def __setitem__(self, key: str, value: Any) -> None:
         from pdm.models.auth import keyring
 
         parts = key.split(".")
         if parts[0] in (REPOSITORY, SOURCE) and key not in self._config_map:
@@ -320,18 +326,17 @@
             raise NoConfigError(key)
         config_key = self.deprecated.get(key, key)
         config = self._config_map[config_key]
         if not self.is_global and config.global_only:
             raise ValueError(f"Config item '{key}' is not allowed to set in project config.")
 
         value = config.coerce(value)
-        env_var = config.env_var
-        if env_var is not None and env_var in os.environ:
+        if key in self.env_map:
             ui.echo(
-                "WARNING: the config is shadowed by env var '{}', the value set won't take effect.".format(env_var),
+                f"WARNING: the config is shadowed by env var '{config.env_var}', the value set won't take effect.",
                 style="warning",
             )
         self._file_data[config_key] = value
         if config.replace:
             self._file_data.pop(config.replace, None)
         self._save_config()
 
@@ -407,7 +412,32 @@
                     config_prefix=prefix,
                     url=name_or_url,
                 )
             config.passive_update(url=name_or_url)
             if config.name == "__unknown__":
                 config.name = name
         return config
+
+
+class EnvMap(Mapping[str, Any]):
+    def __init__(self, config_items: Mapping[str, ConfigItem]) -> None:
+        self._config_map = config_items
+
+    def __repr__(self) -> str:
+        return repr(dict(self))
+
+    def __getitem__(self, k: str) -> Any:
+        try:
+            item = self._config_map[k]
+            if item.env_var:
+                return item.coerce(os.environ[item.env_var])
+        except KeyError:
+            pass
+        raise KeyError(k)
+
+    def __iter__(self) -> Iterator[str]:
+        for key, item in self._config_map.items():
+            if item.env_var and item.env_var in os.environ:
+                yield key
+
+    def __len__(self) -> int:
+        return sum(1 for _ in self)
```

### Comparing `pdm-2.7.0/src/pdm/project/core.py` & `pdm-2.7.1/src/pdm/project/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import contextlib
 import hashlib
 import os
 import re
 import shutil
 import sys
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Iterable, cast
+from typing import TYPE_CHECKING, Any, Iterable, Mapping, cast
 
 import tomlkit
 from tomlkit.items import Array
 
 from pdm import termui
 from pdm._types import RepositoryConfig
 from pdm.compat import cached_property
@@ -114,20 +114,20 @@
         if self._lockfile is None:
             self._lockfile = Lockfile(self.root / self.LOCKFILE_FILENAME, ui=self.core.ui)
         return self._lockfile
 
     def set_lockfile(self, path: str | Path) -> None:
         self._lockfile = Lockfile(path, ui=self.core.ui)
 
-    @property
-    def config(self) -> dict[str, Any]:
-        """A read-only dict configuration, any modifications won't land in the file."""
-        result = dict(self.global_config)
-        result.update(self.project_config)
-        return result
+    @cached_property
+    def config(self) -> Mapping[str, Any]:
+        """A read-only dict configuration"""
+        import collections
+
+        return collections.ChainMap(self.project_config, self.global_config)
 
     @property
     def scripts(self) -> dict[str, str | dict[str, str]]:
         return self.pyproject.settings.get("scripts", {})
 
     @cached_property
     def project_config(self) -> Config:
@@ -326,35 +326,14 @@
                     req = parse_requirement(line[3:].strip(), True)
                 else:
                     req = parse_requirement(line)
                 # make editable packages behind normal ones to override correctly.
                 result[req.identify()] = req
         return result
 
-    @property
-    def dependencies(self) -> dict[str, Requirement]:
-        return self.get_dependencies()
-
-    @property
-    def dev_dependencies(self) -> dict[str, Requirement]:
-        """All development dependencies"""
-        dev_group = self.pyproject.settings.get("dev-dependencies", {})
-        if not dev_group:
-            return {}
-        result = {}
-        with cd(self.root):
-            for _, deps in dev_group.items():
-                for line in deps:
-                    if line.startswith("-e "):
-                        req = parse_requirement(line[3:].strip(), True)
-                    else:
-                        req = parse_requirement(line)
-                    result[req.identify()] = req
-        return result
-
     def iter_groups(self) -> Iterable[str]:
         groups = {"default"}
         if self.pyproject.metadata.get("optional-dependencies"):
             groups.update(self.pyproject.metadata["optional-dependencies"].keys())
         if self.pyproject.settings.get("dev-dependencies"):
             groups.update(self.pyproject.settings["dev-dependencies"].keys())
         return groups
```

### Comparing `pdm-2.7.0/src/pdm/project/lockfile.py` & `pdm-2.7.1/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/project/project_file.py` & `pdm-2.7.1/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/project/toml_file.py` & `pdm-2.7.1/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/pytest.py` & `pdm-2.7.1/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/resolver/core.py` & `pdm-2.7.1/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/resolver/providers.py` & `pdm-2.7.1/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/resolver/python.py` & `pdm-2.7.1/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/resolver/reporters.py` & `pdm-2.7.1/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/signals.py` & `pdm-2.7.1/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/termui.py` & `pdm-2.7.1/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/src/pdm/utils.py` & `pdm-2.7.1/src/pdm/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/conftest.py` & `pdm-2.7.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_add.py` & `pdm-2.7.1/tests/cli/test_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 @pytest.mark.usefixtures("working_set", "vcs")
 def test_non_editable_override_editable(project, pdm):
     project.environment.python_requires = PySpecSet(">=3.6")
     url = "git+https://github.com/test-root/demo.git#egg=demo"
     pdm(["add", "--dev", "-e", url], obj=project, strict=True)
     pdm(["add", "--dev", url], obj=project, strict=True)
-    assert not project.dev_dependencies["demo"].editable
+    assert not project.get_dependencies("dev")["demo"].editable
 
 
 @pytest.mark.usefixtures("working_set")
 def test_add_remote_package_url(project, dev_option, pdm):
     project.environment.python_requires = PySpecSet(">=3.6")
     url = "http://fixtures.test/artifacts/demo-0.0.1-py2.py3-none-any.whl"
     pdm(["add", *dev_option, url], obj=project, strict=True)
```

### Comparing `pdm-2.7.0/tests/cli/test_build.py` & `pdm-2.7.1/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_cache.py` & `pdm-2.7.1/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_config.py` & `pdm-2.7.1/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_fix.py` & `pdm-2.7.1/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_hooks.py` & `pdm-2.7.1/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_init.py` & `pdm-2.7.1/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_install.py` & `pdm-2.7.1/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_list.py` & `pdm-2.7.1/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_lock.py` & `pdm-2.7.1/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_others.py` & `pdm-2.7.1/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_publish.py` & `pdm-2.7.1/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_remove.py` & `pdm-2.7.1/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_run.py` & `pdm-2.7.1/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_self_command.py` & `pdm-2.7.1/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_update.py` & `pdm-2.7.1/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_use.py` & `pdm-2.7.1/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/cli/test_venv.py` & `pdm-2.7.1/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/conftest.py` & `pdm-2.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.7.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.7.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.7.1/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.7.1/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.7.1/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.7.1/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.7.1/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.7.1/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/pypi.json` & `pdm-2.7.1/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/fixtures/pyproject.toml` & `pdm-2.7.1/tests/fixtures/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 readme = "README.md"
 
 homepage = "https://python-poetry.org/"
 repository = "https://github.com/python-poetry/poetry"
 documentation = "https://python-poetry.org/docs"
 
 packages = [
-    {include="my_package", from="lib"},
+    {include="my_package", from="lib/"},
     {include="tests", format="sdist"}
 ]
 
 include = ["CHANGELOG.md"]
 exclude = ["my_package/excluded.py"]
 
 [tool.poetry.dependencies]
```

### Comparing `pdm-2.7.0/tests/models/test_backends.py` & `pdm-2.7.1/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/models/test_candidates.py` & `pdm-2.7.1/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/models/test_marker.py` & `pdm-2.7.1/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/models/test_requirements.py` & `pdm-2.7.1/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/models/test_setup_parsing.py` & `pdm-2.7.1/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/models/test_specifiers.py` & `pdm-2.7.1/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/models/test_versions.py` & `pdm-2.7.1/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/resolver/test_resolve.py` & `pdm-2.7.1/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/test_formats.py` & `pdm-2.7.1/tests/test_formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 def test_convert_requirements_file_without_name(project, vcs):
     req_file = project.root.joinpath("reqs.txt")
     project.root.joinpath("reqs.txt").write_text("git+https://github.com/test-root/demo.git\n")
     assert requirements.check_fingerprint(project, str(req_file))
     result, _ = requirements.convert(project, str(req_file), Namespace(dev=False, group=None))
 
-    assert result["dependencies"] == ["git+https://github.com/test-root/demo.git"]
+    assert result["dependencies"] == ["demo @ git+https://github.com/test-root/demo.git"]
 
 
 def test_convert_poetry(project):
     golden_file = FIXTURES / "pyproject.toml"
     assert poetry.check_fingerprint(project, golden_file)
     with cd(FIXTURES):
         result, settings = poetry.convert(project, golden_file, Namespace(dev=False, group=None))
```

### Comparing `pdm-2.7.0/tests/test_installer.py` & `pdm-2.7.1/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/test_integration.py` & `pdm-2.7.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/test_plugin.py` & `pdm-2.7.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/test_project.py` & `pdm-2.7.1/tests/test_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,19 +162,17 @@
         "venv": ["virtualenv"],
     }
     project.pyproject.settings["dev-dependencies"] = {
         "test": ["pytest"],
         "doc": ["mkdocs"],
     }
     assert sorted(project.get_dependencies()) == ["requests"]
-    assert sorted(project.dependencies) == ["requests"]
 
     assert sorted(project.get_dependencies("security")) == ["cryptography"]
     assert sorted(project.get_dependencies("test")) == ["pytest"]
-    assert sorted(project.dev_dependencies) == ["mkdocs", "pytest"]
 
     assert sorted(project.iter_groups()) == [
         "default",
         "doc",
         "security",
         "test",
         "venv",
```

### Comparing `pdm-2.7.0/tests/test_signals.py` & `pdm-2.7.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/tests/test_utils.py` & `pdm-2.7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.0/PKG-INFO` & `pdm-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.7.0
+Version: 2.7.1
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -28,15 +28,15 @@
 Requires-Dist: unearth>=0.9.0
 Requires-Dist: findpython>=0.2.2
 Requires-Dist: tomlkit<1,>=0.11.1
 Requires-Dist: shellingham>=1.3.2
 Requires-Dist: python-dotenv>=0.15
 Requires-Dist: resolvelib>=1.0.1
 Requires-Dist: installer<0.8,>=0.7
-Requires-Dist: cacheyou[filecache]
+Requires-Dist: cachecontrol[filecache]>=0.13.0
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
 Requires-Dist: pytest; extra == "pytest"
 Requires-Dist: pytest-mock; extra == "pytest"
 Provides-Extra: pytest
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.7.0 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.7.1 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -11,19 +11,19 @@
 Project-URL: Changelog, https://pdm.fming.dev/latest/dev/changelog/ Requires-
 Python: >=3.7 Requires-Dist: blinker Requires-Dist: certifi Requires-Dist:
 packaging!=22.0,>=20.9 Requires-Dist: platformdirs Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20 Requires-Dist: pyproject-hooks Requires-Dist:
 requests-toolbelt Requires-Dist: unearth>=0.9.0 Requires-Dist:
 findpython>=0.2.2 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
 shellingham>=1.3.2 Requires-Dist: python-dotenv>=0.15 Requires-Dist:
-resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist: cacheyou
-[filecache] Requires-Dist: tomli>=1.1.0; python_version < "3.11" Requires-Dist:
-importlib-metadata>=3.6; python_version < "3.10" Requires-Dist: pytest; extra
-== "pytest" Requires-Dist: pytest-mock; extra == "pytest" Provides-Extra:
-pytest Description-Content-Type: text/markdown
+resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist:
+cachecontrol[filecache]>=0.13.0 Requires-Dist: tomli>=1.1.0; python_version <
+"3.11" Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
+Requires-Dist: pytest; extra == "pytest" Requires-Dist: pytest-mock; extra ==
+"pytest" Provides-Extra: pytest Description-Content-Type: text/markdown
 # PDM A modern Python package and dependency manager supporting the latest PEP
       standards. [ä¸­æçæ¬è¯´æ](README_zh.md) ![PDM logo](https://
 raw.githubusercontent.com/pdm-project/pdm/main/docs/docs/assets/logo_big.png)
  [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=for-the-badge)]
   (https://pdm.fming.dev) [![Twitter Follow](https://img.shields.io/twitter/
    follow/pdm_project?label=get%20updates&logo=twitter&style=for-the-badge)]
  (https://twitter.com/pdm_project) [![Discord](https://img.shields.io/discord/
```

