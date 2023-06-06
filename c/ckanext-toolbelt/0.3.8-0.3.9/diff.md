# Comparing `tmp/ckanext-toolbelt-0.3.8.tar.gz` & `tmp/ckanext-toolbelt-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-toolbelt-0.3.8.tar", last modified: Mon Apr 10 08:49:36 2023, max compression
+gzip compressed data, was "ckanext-toolbelt-0.3.9.tar", last modified: Thu Apr 13 18:04:17 2023, max compression
```

## Comparing `ckanext-toolbelt-0.3.8.tar` & `ckanext-toolbelt-0.3.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/search_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_gh_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_gulp-sass.js
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_black.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_commitizen.toml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_isort.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_pyright.toml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_pytest.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/magic/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/magic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/cascade_organization_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/safe_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.418228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.422228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/types/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:49:36.000000 ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-10 08:49:36.426228 ckanext-toolbelt-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-10 08:49:24.000000 ckanext-toolbelt-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/search_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_gh_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_gulp-sass.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_black.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_commitizen.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_isort.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_pyright.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_pytest.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/magic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/cascade_organization_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/safe_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.490736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.494736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:04:17.000000 ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-13 18:04:17.498736 ckanext-toolbelt-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-13 18:04:05.000000 ckanext-toolbelt-0.3.9/setup.py
```

### Comparing `ckanext-toolbelt-0.3.8/LICENSE` & `ckanext-toolbelt-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/PKG-INFO` & `ckanext-toolbelt-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.3.8/README.md` & `ckanext-toolbelt-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/_shared.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/_shared.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/db.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/db.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/ckan/search_index.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/ckan/search_index.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/dev.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_config.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_gh_action.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_gh_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_readme.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_readme.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/make_template.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/make_template.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/action_test.yaml` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/action_test.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_gulp-sass.js` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_gulp-sass.js`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/config_pre-commit.yaml` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/config_pre-commit.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -33,36 +33,21 @@
 # ## Ruff
 # - repo: https://github.com/charliermarsh/ruff-pre-commit
 #   rev: v0.0.260
 #   hooks:
 #   - id: ruff
 #     stages: [pre-commit]
 
-# ## PEP257: Python docstring conventions
-# - repo: https://github.com/PyCQA/pydocstyle
-#   rev: 6.3.0
-#   hooks:
-#   - id: pydocstyle
-#     stages: [pre-push]
-
 # ## Detect passwords, api-tokens, secrets within a code base
 # - repo: https://github.com/Yelp/detect-secrets
 #   rev: v1.4.0
 #   hooks:
 #   - id: detect-secrets
 #     stages: [pre-push]
 #     # args: ['--baseline', '.secrets.baseline']
 
-# ## Conventional commit message(basic)
-# - repo: https://github.com/compilerla/conventional-pre-commit
-#   rev: v2.1.1
-#   hooks:
-#   - id: conventional-pre-commit
-#     stages: [commit-msg]
-#     args: [] # list of Conventional Commits types to allow. default: ["build", "chore", "ci", "docs", "feat", "fix", "perf", "refactor", "revert", "style", "test"]
-
 # ## Conventional commit message(commitizen)
 # - repo: https://github.com/commitizen-tools/commitizen
 #   rev: v2.42.1
 #   hooks:
 #   - id: commitizen
 #     stages: [commit-msg]
```

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/cli/templates/template_pyright.toml` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/cli/templates/template_pyright.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.pyright]
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 include = ["ckanext"]
 exclude = [
     "**/test*",
     "**/migration",
 ]
 strict = []
```

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/magic/__init__.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/cascade_organization_updates.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_changes.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_changes.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/group_composite.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/group_composite.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/safe_upload.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/safe_upload.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/__init__.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/cache.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/collector.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/collector.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/fs.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/hierarchy.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext/toolbelt/utils/structures.py` & `ckanext-toolbelt-0.3.9/ckanext/toolbelt/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/PKG-INFO` & `ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/SOURCES.txt` & `ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/ckanext_toolbelt.egg-info/entry_points.txt` & `ckanext-toolbelt-0.3.9/ckanext_toolbelt.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/pyproject.toml` & `ckanext-toolbelt-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.3.8/setup.cfg` & `ckanext-toolbelt-0.3.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-toolbelt
-version = 0.3.8
+version = 0.3.9
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-toolbelt
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

