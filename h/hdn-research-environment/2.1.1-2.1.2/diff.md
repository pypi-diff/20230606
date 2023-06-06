# Comparing `tmp/hdn-research-environment-2.1.1.tar.gz` & `tmp/hdn-research-environment-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.1.1.tar", last modified: Mon Jun  5 16:43:53 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.1.2.tar", last modified: Tue Jun  6 14:41:50 2023, max compression
```

## Comparing `hdn-research-environment-2.1.1.tar` & `hdn-research-environment-2.1.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.1/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.1/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.1/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.1/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3074 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.1/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-05 16:43:26.000000 hdn-research-environment-2.1.1/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1600 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.1/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.1/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.1/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    18751 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.1/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.1/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.1/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.1/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.1/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     7616 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.1/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.1.1/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      251 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.1/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.1/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.1/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.1/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1467 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.1/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.1/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.1/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    13857 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.1/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     3100 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.1/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-05 16:43:53.000000 hdn-research-environment-2.1.1/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.1/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.2/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.2/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.2/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.2/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3074 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.2/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.2/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-05 16:43:26.000000 hdn-research-environment-2.1.2/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.2/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.2/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.2/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    18751 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.2/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.2/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.2/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.2/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.2/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7616 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.2/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.2/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.2/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.1.2/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      251 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.2/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.2/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.2/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.2/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.2/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.2/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.2/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.2/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.2/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.2/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.2/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13857 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.2/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3100 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-06 14:41:49.000000 hdn-research-environment-2.1.2/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.2/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-06 14:41:50.000000 hdn-research-environment-2.1.2/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.2/setup.py
```

### Comparing `hdn-research-environment-2.1.1/LICENSE` & `hdn-research-environment-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/PKG-INFO` & `hdn-research-environment-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.1/environment/api/v1/__init__.py` & `hdn-research-environment-2.1.2/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/api/v1/auth.py` & `hdn-research-environment-2.1.2/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/api/v1/decorators.py` & `hdn-research-environment-2.1.2/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/api/v2/__init__.py` & `hdn-research-environment-2.1.2/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/api/v2/decorators.py` & `hdn-research-environment-2.1.2/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/constants.py` & `hdn-research-environment-2.1.2/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/decorators.py` & `hdn-research-environment-2.1.2/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/deserializers.py` & `hdn-research-environment-2.1.2/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/entities.py` & `hdn-research-environment-2.1.2/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/exceptions.py` & `hdn-research-environment-2.1.2/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/forms.py` & `hdn-research-environment-2.1.2/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/mailers.py` & `hdn-research-environment-2.1.2/environment/mailers.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.apps import apps
 from django.db.models import Model
 from django.conf import settings
 from django.urls import reverse
 from django.template import loader
 from django.core.mail import send_mail
+from django.utils.html import strip_tags
 
 from environment.models import BillingAccountSharingInvite
 
 
 PublishedProject = apps.get_model("project", "PublishedProject")
 
 User = Model
@@ -23,24 +24,25 @@
     )
     subject = f"{settings.SITE_NAME} Billing Account Shared"
     email_context = {
         "site_name": settings.SITE_NAME,
         "signature": settings.EMAIL_SIGNATURE,
         "confirmation_url": f"https://{site_domain}{confirmation_path}",
     }
-    body = loader.render_to_string(
+    html_body = loader.render_to_string(
         "environment/email/billing_sharing_confirmation.html", email_context
     )
-
+    text_body = strip_tags(html_body)
     return send_mail(
         subject,
-        body,
+        text_body,
         settings.DEFAULT_FROM_EMAIL,
         [invite.user_contact_email],
         fail_silently=False,
+        html_message=html_body,
     )
 
 
 def send_environment_access_expired(user: User, projects: Iterable[PublishedProject]):
     subject = f"{settings.SITE_NAME} Environment Access Expired"
     email_context = {
         "signature": settings.EMAIL_SIGNATURE,
```

### Comparing `hdn-research-environment-2.1.1/environment/migrations/0001_initial.py` & `hdn-research-environment-2.1.2/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.1.2/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.1.2/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.1.2/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.1.2/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/models.py` & `hdn-research-environment-2.1.2/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/services.py` & `hdn-research-environment-2.1.2/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/signals.py` & `hdn-research-environment-2.1.2/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.1.2/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.1.2/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.1.2/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.1.2/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tasks.py` & `hdn-research-environment-2.1.2/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.1.2/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.1.2/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.1.2/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.1.2/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.1.2/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.1.2/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.1.2/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.1.2/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-2.1.2/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.1.2/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.1.2/environment/templates/tag/environment_modal_button.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
           <span aria-hidden="true">&times;</span>
         </button>
       </div>
       <div class="modal-body">
         {% if instances_dict != None %}
             <select class="form-select" id="form-select" size="5" aria-label="size 5 select example">
               {% for instance_type, instance_specification in instances_dict.items %}
-                <option value="{{ instance_type }}">{{ instance_specification }}</option>
+                <option value="{{ instance_type.value }}">{{ instance_specification }}</option>
               {% endfor %}
             </select>
         {% else %}
             <p>{{ modal_body }}</p>
         {% endif %}
       </div>
       <div class="modal-footer">
```

### Comparing `hdn-research-environment-2.1.1/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.1.2/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/helpers.py` & `hdn-research-environment-2.1.2/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/mocks.py` & `hdn-research-environment-2.1.2/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/test_decorators.py` & `hdn-research-environment-2.1.2/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/test_services.py` & `hdn-research-environment-2.1.2/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/test_signals.py` & `hdn-research-environment-2.1.2/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/test_utilities.py` & `hdn-research-environment-2.1.2/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/test_validators.py` & `hdn-research-environment-2.1.2/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/tests/test_views.py` & `hdn-research-environment-2.1.2/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/urls.py` & `hdn-research-environment-2.1.2/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/utilities.py` & `hdn-research-environment-2.1.2/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/environment/views.py` & `hdn-research-environment-2.1.2/environment/views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.1.2/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.1/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.1.2/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.1/setup.cfg` & `hdn-research-environment-2.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.1.1
+version = 2.1.2
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

