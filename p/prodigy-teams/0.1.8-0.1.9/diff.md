# Comparing `tmp/prodigy-teams-0.1.8.tar.gz` & `tmp/prodigy-teams-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodigy-teams-0.1.8.tar", last modified: Tue May  9 11:17:47 2023, max compression
+gzip compressed data, was "prodigy-teams-0.1.9.tar", last modified: Tue May  9 14:53:49 2023, max compression
```

## Comparing `prodigy-teams-0.1.8.tar` & `prodigy-teams-0.1.9.tar`

### file list

```diff
@@ -1,133 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.298101 prodigy-teams-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 11:17:47.298101 prodigy-teams-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.254101 prodigy-teams-0.1.8/prodigy_teams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.262101 prodigy-teams-0.1.8/prodigy_teams/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/_recipe_subcommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/_recipes_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/consul.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.266101 prodigy-teams-0.1.8/prodigy_teams/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/files/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/files/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/files/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/files/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/files/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/commands/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.270101 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.274101 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/consul.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/envs2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/full_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/ty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.274101 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.286101 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/broker_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/for_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/full_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/org.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/person.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/recipeplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    52947 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/recipe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/ty.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/read_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.286101 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.286101 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/README.md.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/setup.py.tmpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.290101 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.290101 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.290101 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/example_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/ty.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.294101 prodigy-teams-0.1.8/prodigy_teams/version/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/0.1.5_2023-04-07-13-53-02__e4412009-3dc2-4d23-abc6-755dfb35fef7
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/0.1.5_2023-05-03-10-25-22_patch_d73ea70d-2939-4754-a334-f77d2125ce5c
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/0.1.6_2023-05-03-15-15-23__3d2a988b-fd4e-466c-84cd-8ddb46bd6f4f
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/0.1.6_2023-05-03-15-46-46__3002a5a8-916b-4231-b205-2874dcfe1212
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/0.1.6_2023-05-05-09-59-43_patch_38355b68-f205-4aa7-a97a-3e04a7b4f494
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/0.1.7_2023-05-09-09-18-16_patch_3a77474c-059e-4e79-b71b-7f9437c5287f
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/prodigy_teams/version/read_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.254101 prodigy-teams-0.1.8/prodigy_teams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 11:17:47.000000 prodigy-teams-0.1.8/prodigy_teams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-09 11:17:47.000000 prodigy-teams-0.1.8/prodigy_teams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:17:47.000000 prodigy-teams-0.1.8/prodigy_teams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-09 11:17:47.000000 prodigy-teams-0.1.8/prodigy_teams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:17:46.000000 prodigy-teams-0.1.8/prodigy_teams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-09 11:17:47.000000 prodigy-teams-0.1.8/prodigy_teams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 11:17:47.000000 prodigy-teams-0.1.8/prodigy_teams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-09 11:17:47.298101 prodigy-teams-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:17:47.298101 prodigy-teams-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-09 11:17:35.000000 prodigy-teams-0.1.8/tests/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.581452 prodigy-teams-0.1.9/prodigy_teams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.585452 prodigy-teams-0.1.9/prodigy_teams/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/_recipe_subcommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/_recipes_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.585452 prodigy-teams-0.1.9/prodigy_teams/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/files/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/files/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/files/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/files/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/files/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/commands/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.585452 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.589452 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/envs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/full_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/ty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.589452 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.589452 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/broker_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/for_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/full_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/recipeplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52947 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/recipe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/ty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63413 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/ptc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/read_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.589452 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/README.md.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/setup.py.tmpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/example_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/ty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/prodigy_teams/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/0.1.5_2023-04-07-13-53-02__e4412009-3dc2-4d23-abc6-755dfb35fef7
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/0.1.5_2023-05-03-10-25-22_patch_d73ea70d-2939-4754-a334-f77d2125ce5c
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/0.1.6_2023-05-03-15-15-23__3d2a988b-fd4e-466c-84cd-8ddb46bd6f4f
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/0.1.6_2023-05-03-15-46-46__3002a5a8-916b-4231-b205-2874dcfe1212
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/0.1.6_2023-05-05-09-59-43_patch_38355b68-f205-4aa7-a97a-3e04a7b4f494
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/0.1.7_2023-05-09-09-18-16_patch_3a77474c-059e-4e79-b71b-7f9437c5287f
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/0.1.8_2023-05-09-11-23-54_patch_6cd5dece-ddcb-4c48-8885-85c4020d279b
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/prodigy_teams/version/read_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.585452 prodigy-teams-0.1.9/prodigy_teams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 14:53:49.000000 prodigy-teams-0.1.9/prodigy_teams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-09 14:53:49.000000 prodigy-teams-0.1.9/prodigy_teams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:53:49.000000 prodigy-teams-0.1.9/prodigy_teams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-09 14:53:49.000000 prodigy-teams-0.1.9/prodigy_teams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:53:49.000000 prodigy-teams-0.1.9/prodigy_teams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-09 14:53:49.000000 prodigy-teams-0.1.9/prodigy_teams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 14:53:49.000000 prodigy-teams-0.1.9/prodigy_teams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:53:49.593452 prodigy-teams-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-09 14:53:40.000000 prodigy-teams-0.1.9/tests/test_ui.py
```

### Comparing `prodigy-teams-0.1.8/README.md` & `prodigy-teams-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/__main__.py` & `prodigy-teams-0.1.9/prodigy_teams/__main__.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/about.py` & `prodigy-teams-0.1.9/prodigy_teams/about.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/auth.py` & `prodigy-teams-0.1.9/prodigy_teams/auth.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/cli.py` & `prodigy-teams-0.1.9/prodigy_teams/cli.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/_recipe_subcommand.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/_recipe_subcommand.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/_recipes_meta.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/_recipes_meta.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/actions.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/actions.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/assets.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/assets.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/clusters.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/clusters.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/config.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/config.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/consul.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/consul.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/datasets.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/files/cp.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/files/cp.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/files/ls.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/files/ls.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/files/rm.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/files/rm.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/files/rsync.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/files/rsync.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/files/stats.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/files/stats.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/general.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/general.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/import_export.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/import_export.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/packages.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/packages.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/paths.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/paths.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/projects.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/projects.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/recipes.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/recipes.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/secrets.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/commands/tasks.py` & `prodigy-teams-0.1.9/prodigy_teams/commands/tasks.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/config.py` & `prodigy-teams-0.1.9/prodigy_teams/config.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/errors.py` & `prodigy-teams-0.1.9/prodigy_teams/errors.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/messages.py` & `prodigy-teams-0.1.9/prodigy_teams/messages.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/base.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/base.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/check.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/check.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/consul.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/consul.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/data.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/data.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/envs2.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/envs2.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/files.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/files.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/full_client.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/full_client.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/client/jobs.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/client/jobs.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/errors.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/models.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/models.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_broker_sdk/ty.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_broker_sdk/ty.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/asset.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/asset.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/base.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/base.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/broker.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/broker.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/broker_path.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/broker_path.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/dataset.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/dataset.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/for_cluster.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/for_cluster.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/full_client.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/full_client.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/group.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/group.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/invitation.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/invitation.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/notification.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/notification.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/package.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/package.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/person.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/person.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/recipe.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/recipe.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/recipeplan.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/recipeplan.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/client/secret.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/client/secret.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/errors.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/models.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/models.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/recipe_utils.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/recipe_utils.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/prodigy_teams_pam_sdk/ty.py` & `prodigy-teams-0.1.9/prodigy_teams/prodigy_teams_pam_sdk/ty.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/query.py` & `prodigy-teams-0.1.9/prodigy_teams/query.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/read_version.py` & `prodigy-teams-0.1.9/prodigy_teams/read_version.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/README.md.tmpl` & `prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/README.md.tmpl`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/setup.py.tmpl` & `prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/setup.py.tmpl`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/example_task.py` & `prodigy-teams-0.1.9/prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/example_task.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/ty.py` & `prodigy-teams-0.1.9/prodigy_teams/ty.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/ui.py` & `prodigy-teams-0.1.9/prodigy_teams/ui.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/util.py` & `prodigy-teams-0.1.9/prodigy_teams/util.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams/version/read_version.py` & `prodigy-teams-0.1.9/prodigy_teams/version/read_version.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/prodigy_teams.egg-info/SOURCES.txt` & `prodigy-teams-0.1.9/prodigy_teams.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 prodigy_teams/about.py
 prodigy_teams/auth.py
 prodigy_teams/cli.py
 prodigy_teams/config.py
 prodigy_teams/errors.py
 prodigy_teams/main.py
 prodigy_teams/messages.py
+prodigy_teams/ptc.json
 prodigy_teams/query.py
 prodigy_teams/read_version.py
 prodigy_teams/ty.py
 prodigy_teams/ui.py
 prodigy_teams/util.py
 prodigy_teams.egg-info/PKG-INFO
 prodigy_teams.egg-info/SOURCES.txt
@@ -104,13 +105,14 @@
 prodigy_teams/recipes_cookiecutter/{{cookiecutter.package_dir}}/{{cookiecutter.package_name}}/recipes/example_task.py
 prodigy_teams/version/0.1.5_2023-04-07-13-53-02__e4412009-3dc2-4d23-abc6-755dfb35fef7
 prodigy_teams/version/0.1.5_2023-05-03-10-25-22_patch_d73ea70d-2939-4754-a334-f77d2125ce5c
 prodigy_teams/version/0.1.6_2023-05-03-15-15-23__3d2a988b-fd4e-466c-84cd-8ddb46bd6f4f
 prodigy_teams/version/0.1.6_2023-05-03-15-46-46__3002a5a8-916b-4231-b205-2874dcfe1212
 prodigy_teams/version/0.1.6_2023-05-05-09-59-43_patch_38355b68-f205-4aa7-a97a-3e04a7b4f494
 prodigy_teams/version/0.1.7_2023-05-09-09-18-16_patch_3a77474c-059e-4e79-b71b-7f9437c5287f
+prodigy_teams/version/0.1.8_2023-05-09-11-23-54_patch_6cd5dece-ddcb-4c48-8885-85c4020d279b
 prodigy_teams/version/__init__.py
 prodigy_teams/version/read_version.py
 tests/test_info.py
 tests/test_main.py
 tests/test_projects.py
 tests/test_ui.py
```

### Comparing `prodigy-teams-0.1.8/requirements.txt` & `prodigy-teams-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/setup.py` & `prodigy-teams-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/tests/test_info.py` & `prodigy-teams-0.1.9/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/tests/test_main.py` & `prodigy-teams-0.1.9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-0.1.8/tests/test_ui.py` & `prodigy-teams-0.1.9/tests/test_ui.py`

 * *Files identical despite different names*

