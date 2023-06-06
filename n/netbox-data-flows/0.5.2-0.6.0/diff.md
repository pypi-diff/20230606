# Comparing `tmp/netbox-data-flows-0.5.2.tar.gz` & `tmp/netbox-data-flows-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-data-flows-0.5.2.tar", last modified: Thu May 11 20:32:05 2023, max compression
+gzip compressed data, was "netbox-data-flows-0.6.0.tar", last modified: Tue Jun  6 20:55:18 2023, max compression
```

## Comparing `netbox-data-flows-0.5.2.tar` & `netbox-data-flows-0.6.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.302914 netbox-data-flows-0.5.2/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/graphql/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/models/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.302914 netbox-data-flows-0.5.2/netbox_data_flows/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.310914 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/netbox_data_flows/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/netbox_data_flows/views/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:32:05.306914 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:32:05.000000 netbox-data-flows-0.5.2/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-11 20:31:48.000000 netbox-data-flows-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:32:05.314914 netbox-data-flows-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/graphql/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.982302 netbox-data-flows-0.6.0/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.986302 netbox-data-flows-0.6.0/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.986302 netbox-data-flows-0.6.0/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.986302 netbox-data-flows-0.6.0/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.974301 netbox-data-flows-0.6.0/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:55:18.978301 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 20:55:18.000000 netbox-data-flows-0.6.0/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-06 20:54:59.000000 netbox-data-flows-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:55:18.990302 netbox-data-flows-0.6.0/setup.cfg
```

### Comparing `netbox-data-flows-0.5.2/LICENSE` & `netbox-data-flows-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/PKG-INFO` & `netbox-data-flows-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.5.2
+Version: 0.6.0
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.5.2/README.md` & `netbox-data-flows-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/applications.py` & `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/dataflows.py` & `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/groups.py` & `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/nested.py` & `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/nested.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/api/serializers/objectaliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/api/urls.py` & `netbox-data-flows-0.6.0/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/api/views.py` & `netbox-data-flows-0.6.0/netbox_data_flows/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/choices.py` & `netbox-data-flows-0.6.0/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/addins.py` & `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/addins.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/applications.py` & `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/dataflows.py` & `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/filters.py` & `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/groups.py` & `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/filtersets/objectaliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/filtersets/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/forms/applicationroles.py` & `netbox-data-flows-0.6.0/netbox_data_flows/forms/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/forms/applications.py` & `netbox-data-flows-0.6.0/netbox_data_flows/forms/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/forms/dataflows.py` & `netbox-data-flows-0.6.0/netbox_data_flows/forms/dataflows.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,18 @@
     CommentField,
     CSVChoiceField,
     CSVModelChoiceField,
     CSVModelMultipleChoiceField,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
     MultipleChoiceField,  # TODO: deprecated, remove for 3.6.0
+    NumericArrayField,
     TagFilterField,
 )
 
-try:  # >=3.5.0
-    from utilities.forms.fields import NumericArrayField
-except ImportError:  # <3.5.0
-    from utilities.forms import NumericArrayField
-
-# TODO: Cleanup of StaticSelect
-try:  # <3.5.0
-    from utilities.forms import StaticSelect
-except ImportError:  # >=3.5.0
-    StaticSelect = forms.Select
-
 from dcim.models import Device
 from ipam.models import Prefix, IPRange, IPAddress
 from ipam.constants import SERVICE_PORT_MIN, SERVICE_PORT_MAX
 from virtualization.models import VirtualMachine
 
 from netbox_data_flows import models, choices
 
@@ -126,15 +116,15 @@
             "protocol",
             "source_ports",
             "destination_ports",
             "sources",
             "destinations",
         )
         widgets = {
-            "protocol": StaticSelect(),
+            "protocol": forms.Select(),
         }
         help_texts = {
             "status": "Status of the data group. If its group is disabled, the data flow will also be disabled."
         }
 
 
 #
@@ -156,20 +146,20 @@
             "application_id": "$application",
         },
     )
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
     )
     protocol = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowProtocolChoices),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
     )
     source_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
         help_text="Comma-separated list of one or more port numbers. A range may be specified using a hyphen.",
         required=False,
@@ -322,21 +312,21 @@
         help_text="Recursive group(s)",
     )
     tag = TagFilterField(model)
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
         help_text="Status of the data flows themselves",
     )
     inherited_status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
         help_text="Status inherited from the data flow groups",
     )
 
     protocol = MultipleChoiceField(
         choices=choices.DataFlowProtocolChoices,
         required=False,
     )
@@ -352,15 +342,15 @@
         required=False,
         help_text="Use the API or repeat the URL parameter to select several",
     )
 
     source_is_null = forms.ChoiceField(
         choices=add_blank_choice(choices.TargetIsEmptyChoice),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
         help_text="No sources are defined?",
     )
     source_aliases = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
         label="Source Object Aliases",
     )
@@ -391,15 +381,15 @@
         label="Source Virtual Machines",
         help_text="Any IP address of the virtual machine",
     )
 
     destination_is_null = forms.ChoiceField(
         choices=add_blank_choice(choices.TargetIsEmptyChoice),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
         help_text="No destinations are defined?",
     )
     destination_aliases = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
         label="Destination Object Aliases",
     )
```

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/forms/groups.py` & `netbox-data-flows-0.6.0/netbox_data_flows/forms/groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,19 @@
 from utilities.forms.fields import (
     CommentField,
     CSVChoiceField,
     CSVModelChoiceField,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
     MultipleChoiceField,  # TODO: deprecated, remove for 3.6.0
+    NumericArrayField,
     SlugField,
     TagFilterField,
 )
 
-try:  # >=3.5.0
-    from utilities.forms.fields import NumericArrayField
-except ImportError:  # <3.5.0
-    from utilities.forms import NumericArrayField
-
-try:  # <3.5.0
-    from utilities.forms import StaticSelect
-except ImportError:  # >=3.5.0
-    StaticSelect = forms.Select
-
 from netbox_data_flows import models, choices
 
 
 __all__ = (
     "DataFlowGroupForm",
     "DataFlowGroupBulkEditForm",
     "DataFlowGroupFilterForm",
@@ -107,15 +98,15 @@
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
     )
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
     )
 
     fieldsets = (
         (
             "Data Flow Groups",
             (
                 "application",
@@ -187,20 +178,20 @@
         label="Ancestor group",
         help_text="Recursive parent group(s)",
     )
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
     )
     inherited_status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=StaticSelect(),
+        widget=forms.Select(),
     )
 
     fieldsets = (
         (
             None,
             (
                 "filter_id",  # Saved Filter
```

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/forms/objectaliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/forms/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/graphql/__init__.py` & `netbox-data-flows-0.6.0/netbox_data_flows/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/graphql/applications.py` & `netbox-data-flows-0.6.0/netbox_data_flows/graphql/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/graphql/objectaliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/graphql/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0001_initial.py` & `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py` & `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/models/applications.py` & `netbox-data-flows-0.6.0/netbox_data_flows/models/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/models/dataflows.py` & `netbox-data-flows-0.6.0/netbox_data_flows/models/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/models/groups.py` & `netbox-data-flows-0.6.0/netbox_data_flows/models/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/models/objectaliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/models/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/navigation.py` & `netbox-data-flows-0.6.0/netbox_data_flows/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/search.py` & `netbox-data-flows-0.6.0/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/tables/applications.py` & `netbox-data-flows-0.6.0/netbox_data_flows/tables/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/tables/dataflows.py` & `netbox-data-flows-0.6.0/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/tables/groups.py` & `netbox-data-flows-0.6.0/netbox_data_flows/tables/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/tables/objectaliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/tables/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
       </div>
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
-      {% include 'inc/panels/contacts.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
 
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
```

#### html2text {}

```diff
@@ -5,15 +5,14 @@
 {% endblock %} {% block content %}
 ** Application **
 Name        {{ object.name }}
 Role        {{ object.role|placeholder|linkify }}
 Description {{ object.description|placeholder }}
 {% include 'inc/panels/comments.html' %} {% include 'inc/panels/
 custom_fields.html' %} {% plugin_left_page object %}
-{% include 'inc/panels/tags.html' %} {% include 'inc/panels/contacts.html' %}
-{% plugin_right_page object %}
+{% include 'inc/panels/tags.html' %} {% plugin_right_page object %}
 ** Data Flow Groups **
 {% render_table dataflowgroups_table %}
 ** Data Flows **
 {% render_table dataflows_table %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/inc/dataflow_specifications.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox-data-flows-0.6.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/urls.py` & `netbox-data-flows-0.6.0/netbox_data_flows/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/utils/aliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/utils/helpers.py` & `netbox-data-flows-0.6.0/netbox_data_flows/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/views/applicationroles.py` & `netbox-data-flows-0.6.0/netbox_data_flows/views/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/views/applications.py` & `netbox-data-flows-0.6.0/netbox_data_flows/views/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django.db.models import Count
 
 from netbox.views import generic
 from utilities.views import register_model_view
 
+from tenancy.views import ObjectContactsView
+
 from netbox_data_flows import filtersets, forms, models, tables
 
 
 __all__ = (
     "ApplicationView",
     "ApplicationListView",
     "ApplicationEditView",
@@ -77,7 +79,12 @@
 
 class ApplicationBulkDeleteView(generic.BulkDeleteView):
     queryset = models.Application.objects.annotate(
         dataflow_count=Count("dataflows", distinct=True),
     )
     filterset = filtersets.ApplicationFilterSet
     table = tables.ApplicationTable
+
+
+@register_model_view(models.Application, "contacts")
+class ApplicationContactsView(ObjectContactsView):
+    queryset = models.Application.objects.all()
```

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/views/dataflows.py` & `netbox-data-flows-0.6.0/netbox_data_flows/views/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/views/groups.py` & `netbox-data-flows-0.6.0/netbox_data_flows/views/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows/views/objectaliases.py` & `netbox-data-flows-0.6.0/netbox_data_flows/views/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows.egg-info/PKG-INFO` & `netbox-data-flows-0.6.0/netbox_data_flows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.5.2
+Version: 0.6.0
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.5.2/netbox_data_flows.egg-info/SOURCES.txt` & `netbox-data-flows-0.6.0/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.5.2/pyproject.toml` & `netbox-data-flows-0.6.0/pyproject.toml`

 * *Files identical despite different names*

