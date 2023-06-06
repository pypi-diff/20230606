# Comparing `tmp/aws-service-catalog-puppet-0.99.1.tar.gz` & `tmp/aws-service-catalog-puppet-0.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-service-catalog-puppet-0.99.1.tar", max compression
+gzip compressed data, was "aws-service-catalog-puppet-0.99.2.tar", max compression
```

## Comparing `aws-service-catalog-puppet-0.99.1.tar` & `aws-service-catalog-puppet-0.99.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0    10142 2021-03-10 19:25:39.810363 aws-service-catalog-puppet-0.99.1/LICENSE
--rw-r--r--   0        0        0     1575 2021-03-10 19:25:39.810363 aws-service-catalog-puppet-0.99.1/README.md
--rw-r--r--   0        0        0     2085 2021-03-10 19:28:59.410247 aws-service-catalog-puppet-0.99.1/pyproject.toml
--rw-r--r--   0        0        0      112 2021-03-10 19:25:39.834363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/__init__.py
--rw-r--r--   0        0        0      229 2021-03-10 19:25:39.834363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/asset_helpers.py
--rw-r--r--   0        0        0     1007 2021-03-10 19:25:39.834363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/asset_helpers_unit_test.py
--rw-r--r--   0        0        0    20738 2021-03-10 19:25:39.834363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/aws.py
--rw-r--r--   0        0        0    24018 2021-03-10 19:26:45.058363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/cli.py
--rw-r--r--   0        0        0     7924 2021-03-10 19:25:39.834363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/config.py
--rw-r--r--   0        0        0     5095 2021-03-10 19:25:39.834363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/config_unit_test.py
--rw-r--r--   0        0        0     3146 2021-03-10 19:25:39.834363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/constants.py
--rw-r--r--   0        0        0    48405 2021-03-10 19:26:46.362363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/core.py
--rw-r--r--   0        0        0      693 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/all-tasks-for-launch-b.json
--rw-r--r--   0        0        0     2946 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/all-tasks.json
--rw-r--r--   0        0        0     4317 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/deployment-map.json
--rw-r--r--   0        0        0      633 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-a.json
--rw-r--r--   0        0        0      635 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-b.json
--rw-r--r--   0        0        0     2580 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-c.json
--rw-r--r--   0        0        0      891 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-details-for-launch-b.json
--rw-r--r--   0        0        0     9974 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/manifest-tasks.json
--rw-r--r--   0        0        0     8484 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/manifest.json
--rw-r--r--   0        0        0     1745 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/manifest_with_numbers.json
--rw-r--r--   0        0        0      739 2021-03-10 19:25:39.838363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all.yaml
--rw-r--r--   0        0        0      739 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all_expected.yaml
--rw-r--r--   0        0        0      750 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region.yaml
--rw-r--r--   0        0        0      738 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml
--rw-r--r--   0        0        0      716 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty.yaml
--rw-r--r--   0        0        0      738 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty_expected.yaml
--rw-r--r--   0        0        0      743 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled.yaml
--rw-r--r--   0        0        0     1477 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml
--rw-r--r--   0        0        0      751 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml
--rw-r--r--   0        0        0     1477 2021-03-10 19:25:39.842363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml
--rw-r--r--   0        0        0      783 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists.yaml
--rw-r--r--   0        0        0     1478 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists_expected.yaml
--rw-r--r--   0        0        0      751 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml
--rw-r--r--   0        0        0     1479 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml
--rw-r--r--   0        0        0      739 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml
--rw-r--r--   0        0        0      723 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all.yaml
--rw-r--r--   0        0        0      739 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all_expected.yaml
--rw-r--r--   0        0        0      734 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region.yaml
--rw-r--r--   0        0        0      738 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml
--rw-r--r--   0        0        0      700 2021-03-10 19:25:39.846363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty.yaml
--rw-r--r--   0        0        0      738 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty_expected.yaml
--rw-r--r--   0        0        0      727 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled.yaml
--rw-r--r--   0        0        0     1477 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml
--rw-r--r--   0        0        0      735 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml
--rw-r--r--   0        0        0     1477 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml
--rw-r--r--   0        0        0      767 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists.yaml
--rw-r--r--   0        0        0     1478 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists_expected.yaml
--rw-r--r--   0        0        0      735 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml
--rw-r--r--   0        0        0     1479 2021-03-10 19:25:39.850363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml
--rw-r--r--   0        0        0      723 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml
--rw-r--r--   0        0        0     1849 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks.yaml
--rw-r--r--   0        0        0     3975 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks_expected.yaml
--rw-r--r--   0        0        0     2438 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248.yaml
--rw-r--r--   0        0        0     2479 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248_1.yaml
--rw-r--r--   0        0        0      573 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils_for_spoke_local_portfolios/simple.yaml
--rw-r--r--   0        0        0      186 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/example-config-small.yaml
--rw-r--r--   0        0        0      272 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/macros.py
--rw-r--r--   0        0        0     1047 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest.yaml
--rw-r--r--   0        0        0    25357 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils.py
--rw-r--r--   0        0        0    13186 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_for_explode_unit_test.py
--rw-r--r--   0        0        0     3126 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_for_launches.py
--rw-r--r--   0        0        0     1353 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_for_spoke_local_portfolios.py
--rw-r--r--   0        0        0     3840 2021-03-10 19:25:39.854363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_unit_test.py
--rw-r--r--   0        0        0     2443 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifests/manifest-quickstart.yaml
--rw-r--r--   0        0        0      690 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifests/manifest-simple.yaml
--rw-r--r--   0        0        0     1657 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/puppet_schema_extensions.py
--rw-r--r--   0        0        0     4001 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/schema.yaml
--rw-r--r--   0        0        0     7546 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/sdk.py
--rw-r--r--   0        0        0    15543 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-initialiser.template.yaml
--rw-r--r--   0        0        0     1740 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-org-master.template.yaml
--rw-r--r--   0        0        0     2033 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-regional.template.yaml
--rw-r--r--   0        0        0     9858 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-spoke.template.yaml
--rw-r--r--   0        0        0    30956 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet.template.yaml
--rw-r--r--   0        0        0        0 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/__init__.py
--rw-r--r--   0        0        0        0 2021-03-10 19:25:39.858363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/__init__.py
--rw-r--r--   0        0        0    38467 2021-03-10 19:26:47.426363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/bootstrap.py
--rw-r--r--   0        0        0     3158 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/bootstrap_region.py
--rw-r--r--   0        0        0        0 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/bootstrap_region_unit_test.py
--rw-r--r--   0        0        0     1045 2021-03-10 19:26:46.458363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/bootstrap_unit_test.py
--rw-r--r--   0        0        0      598 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/associations.template.yaml.j2
--rw-r--r--   0        0        0      903 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/launch_role_constraints.template.yaml.j2
--rw-r--r--   0        0        0     4198 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/policies.template.yaml.j2
--rw-r--r--   0        0        0      560 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/product.template.yaml.j2
--rw-r--r--   0        0        0       72 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/unittest_utils.py
--rw-r--r--   0        0        0      202 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/utils.py
--rw-r--r--   0        0        0        0 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/__init__.py
--rw-r--r--   0        0        0     1342 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/general.py
--rw-r--r--   0        0        0     1164 2021-03-10 19:25:39.862363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/general_c_unit_test.py
--rw-r--r--   0        0        0    10264 2021-03-10 19:25:39.866363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/generate.py
--rw-r--r--   0        0        0     4419 2021-03-10 19:25:39.866363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/generate_c_unit_test.py
--rw-r--r--   0        0        0    13548 2021-03-10 19:25:39.866363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/lambda_invocations.py
--rw-r--r--   0        0        0     4265 2021-03-10 19:25:39.866363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/launch.py
--rw-r--r--   0        0        0     1309 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/launch_c_unit_test.py
--rw-r--r--   0        0        0     1101 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/management.py
--rw-r--r--   0        0        0      934 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/management_c_unit_test.py
--rw-r--r--   0        0        0     1279 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/manifest.py
--rw-r--r--   0        0        0    71959 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/portfoliomanagement.py
--rw-r--r--   0        0        0    19386 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/portfoliomanagement_c_unit_test.py
--rw-r--r--   0        0        0    67296 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/provisioning.py
--rw-r--r--   0        0        0    14997 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/provisioning_c_unit_test.py
--rw-r--r--   0        0        0    14546 2021-03-10 19:25:39.870363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/runner.py
--rw-r--r--   0        0        0     2429 2021-03-10 19:25:39.874363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/spoke_local_portfolios.py
--rw-r--r--   0        0        0      584 2021-03-10 19:25:39.874363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/spoke_local_portfolios_c_unit_test.py
--rw-r--r--   0        0        0     8177 2021-03-10 19:25:39.874363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/tasks.py
--rw-r--r--   0        0        0      885 2021-03-10 19:25:39.874363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/tasks_c_unit_test.py
--rw-r--r--   0        0        0     1934 2021-03-10 19:25:39.874363 aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/tasks_unit_tests.py
--rw-r--r--   0        0        0     3675 2021-03-10 19:29:01.591027 aws-service-catalog-puppet-0.99.1/setup.py
--rw-r--r--   0        0        0     3657 2021-03-10 19:29:01.591397 aws-service-catalog-puppet-0.99.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2021-03-18 09:19:01.570500 aws-service-catalog-puppet-0.99.2/LICENSE
+-rw-r--r--   0        0        0     1575 2021-03-18 09:19:01.570500 aws-service-catalog-puppet-0.99.2/README.md
+-rw-r--r--   0        0        0     2085 2021-03-18 09:22:13.398500 aws-service-catalog-puppet-0.99.2/pyproject.toml
+-rw-r--r--   0        0        0      112 2021-03-18 09:19:01.590500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/__init__.py
+-rw-r--r--   0        0        0      229 2021-03-18 09:19:01.590500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/asset_helpers.py
+-rw-r--r--   0        0        0     1007 2021-03-18 09:19:01.594500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/asset_helpers_unit_test.py
+-rw-r--r--   0        0        0    20738 2021-03-18 09:19:01.594500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/aws.py
+-rw-r--r--   0        0        0    24018 2021-03-18 09:20:04.282500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/cli.py
+-rw-r--r--   0        0        0     7924 2021-03-18 09:19:01.594500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/config.py
+-rw-r--r--   0        0        0     5095 2021-03-18 09:19:01.594500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/config_unit_test.py
+-rw-r--r--   0        0        0     3146 2021-03-18 09:19:01.594500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/constants.py
+-rw-r--r--   0        0        0    47720 2021-03-18 09:20:05.542500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/core.py
+-rw-r--r--   0        0        0      693 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/all-tasks-for-launch-b.json
+-rw-r--r--   0        0        0     2946 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/all-tasks.json
+-rw-r--r--   0        0        0     4317 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/deployment-map.json
+-rw-r--r--   0        0        0      633 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-a.json
+-rw-r--r--   0        0        0      635 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-b.json
+-rw-r--r--   0        0        0     2580 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-c.json
+-rw-r--r--   0        0        0      891 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-details-for-launch-b.json
+-rw-r--r--   0        0        0     9974 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/manifest-tasks.json
+-rw-r--r--   0        0        0     8484 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/manifest.json
+-rw-r--r--   0        0        0     1745 2021-03-18 09:19:01.598500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/manifest_with_numbers.json
+-rw-r--r--   0        0        0      739 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all.yaml
+-rw-r--r--   0        0        0      739 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all_expected.yaml
+-rw-r--r--   0        0        0      750 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region.yaml
+-rw-r--r--   0        0        0      738 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml
+-rw-r--r--   0        0        0      716 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty.yaml
+-rw-r--r--   0        0        0      738 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty_expected.yaml
+-rw-r--r--   0        0        0      743 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled.yaml
+-rw-r--r--   0        0        0     1477 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml
+-rw-r--r--   0        0        0      751 2021-03-18 09:19:01.602500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml
+-rw-r--r--   0        0        0     1477 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml
+-rw-r--r--   0        0        0      783 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists.yaml
+-rw-r--r--   0        0        0     1478 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists_expected.yaml
+-rw-r--r--   0        0        0      751 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml
+-rw-r--r--   0        0        0     1479 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml
+-rw-r--r--   0        0        0      739 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml
+-rw-r--r--   0        0        0      723 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all.yaml
+-rw-r--r--   0        0        0      739 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all_expected.yaml
+-rw-r--r--   0        0        0      734 2021-03-18 09:19:01.606500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region.yaml
+-rw-r--r--   0        0        0      738 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml
+-rw-r--r--   0        0        0      700 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty.yaml
+-rw-r--r--   0        0        0      738 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty_expected.yaml
+-rw-r--r--   0        0        0      727 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled.yaml
+-rw-r--r--   0        0        0     1477 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml
+-rw-r--r--   0        0        0      735 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml
+-rw-r--r--   0        0        0     1477 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml
+-rw-r--r--   0        0        0      767 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists.yaml
+-rw-r--r--   0        0        0     1478 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists_expected.yaml
+-rw-r--r--   0        0        0      735 2021-03-18 09:19:01.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml
+-rw-r--r--   0        0        0     1479 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml
+-rw-r--r--   0        0        0      723 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml
+-rw-r--r--   0        0        0     1849 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks.yaml
+-rw-r--r--   0        0        0     3975 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks_expected.yaml
+-rw-r--r--   0        0        0     2438 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248.yaml
+-rw-r--r--   0        0        0     2479 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248_1.yaml
+-rw-r--r--   0        0        0      573 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils_for_spoke_local_portfolios/simple.yaml
+-rw-r--r--   0        0        0      186 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/example-config-small.yaml
+-rw-r--r--   0        0        0      272 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/macros.py
+-rw-r--r--   0        0        0     1047 2021-03-18 09:19:01.614500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest.yaml
+-rw-r--r--   0        0        0    25357 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils.py
+-rw-r--r--   0        0        0    13186 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_for_explode_unit_test.py
+-rw-r--r--   0        0        0     3126 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_for_launches.py
+-rw-r--r--   0        0        0     1353 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_for_spoke_local_portfolios.py
+-rw-r--r--   0        0        0     3840 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_unit_test.py
+-rw-r--r--   0        0        0     2443 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifests/manifest-quickstart.yaml
+-rw-r--r--   0        0        0      690 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifests/manifest-simple.yaml
+-rw-r--r--   0        0        0     1657 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/puppet_schema_extensions.py
+-rw-r--r--   0        0        0     4001 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/schema.yaml
+-rw-r--r--   0        0        0     7546 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/sdk.py
+-rw-r--r--   0        0        0    15621 2021-03-18 09:19:01.618500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-initialiser.template.yaml
+-rw-r--r--   0        0        0     1740 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-org-master.template.yaml
+-rw-r--r--   0        0        0     2033 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-regional.template.yaml
+-rw-r--r--   0        0        0     9858 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-spoke.template.yaml
+-rw-r--r--   0        0        0    30956 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet.template.yaml
+-rw-r--r--   0        0        0        0 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/__init__.py
+-rw-r--r--   0        0        0    38479 2021-03-18 09:20:06.610500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/bootstrap.py
+-rw-r--r--   0        0        0     3158 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/bootstrap_region.py
+-rw-r--r--   0        0        0        0 2021-03-18 09:19:01.622500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/bootstrap_region_unit_test.py
+-rw-r--r--   0        0        0     1045 2021-03-18 09:20:05.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/bootstrap_unit_test.py
+-rw-r--r--   0        0        0      598 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/associations.template.yaml.j2
+-rw-r--r--   0        0        0      903 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/launch_role_constraints.template.yaml.j2
+-rw-r--r--   0        0        0     4198 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/policies.template.yaml.j2
+-rw-r--r--   0        0        0      560 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/product.template.yaml.j2
+-rw-r--r--   0        0        0       72 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/unittest_utils.py
+-rw-r--r--   0        0        0      202 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/utils.py
+-rw-r--r--   0        0        0        0 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/__init__.py
+-rw-r--r--   0        0        0     1342 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/general.py
+-rw-r--r--   0        0        0     1164 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/general_c_unit_test.py
+-rw-r--r--   0        0        0    10264 2021-03-18 09:19:01.626500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/generate.py
+-rw-r--r--   0        0        0     4419 2021-03-18 09:19:01.630500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/generate_c_unit_test.py
+-rw-r--r--   0        0        0    13548 2021-03-18 09:19:01.630500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/lambda_invocations.py
+-rw-r--r--   0        0        0     4265 2021-03-18 09:19:01.630500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/launch.py
+-rw-r--r--   0        0        0     1309 2021-03-18 09:19:01.630500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/launch_c_unit_test.py
+-rw-r--r--   0        0        0     1101 2021-03-18 09:19:01.630500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/management.py
+-rw-r--r--   0        0        0      934 2021-03-18 09:19:01.630500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/management_c_unit_test.py
+-rw-r--r--   0        0        0     1279 2021-03-18 09:19:01.630500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/manifest.py
+-rw-r--r--   0        0        0    71959 2021-03-18 09:19:01.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/portfoliomanagement.py
+-rw-r--r--   0        0        0    19386 2021-03-18 09:19:01.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/portfoliomanagement_c_unit_test.py
+-rw-r--r--   0        0        0    67296 2021-03-18 09:19:01.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/provisioning.py
+-rw-r--r--   0        0        0    14997 2021-03-18 09:19:01.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/provisioning_c_unit_test.py
+-rw-r--r--   0        0        0    14546 2021-03-18 09:19:01.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/runner.py
+-rw-r--r--   0        0        0     2429 2021-03-18 09:19:01.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/spoke_local_portfolios.py
+-rw-r--r--   0        0        0      584 2021-03-18 09:19:01.634500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/spoke_local_portfolios_c_unit_test.py
+-rw-r--r--   0        0        0     8177 2021-03-18 09:19:01.638500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/tasks.py
+-rw-r--r--   0        0        0      885 2021-03-18 09:19:01.638500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/tasks_c_unit_test.py
+-rw-r--r--   0        0        0     1934 2021-03-18 09:19:01.638500 aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/tasks_unit_tests.py
+-rw-r--r--   0        0        0     3675 2021-03-18 09:22:15.502710 aws-service-catalog-puppet-0.99.2/setup.py
+-rw-r--r--   0        0        0     3657 2021-03-18 09:22:15.503077 aws-service-catalog-puppet-0.99.2/PKG-INFO
```

### Comparing `aws-service-catalog-puppet-0.99.1/LICENSE` & `aws-service-catalog-puppet-0.99.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/README.md` & `aws-service-catalog-puppet-0.99.2/README.md`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/pyproject.toml` & `aws-service-catalog-puppet-0.99.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "aws-service-catalog-puppet"
-version = "0.99.1"
+version = "0.99.2"
 description = "Making it easier to deploy ServiceCatalog products"
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Natural Language :: English"]
 homepage = "https://service-catalog-tools-workshop.com/"
 readme = "README.md"
 repository = "https://github.com/awslabs/aws-service-catalog-puppet-framework"
 authors = ["Eamonn Faherty <aws-service-catalog-tools@amazon.com>"]
 packages = [
```

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/asset_helpers_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/asset_helpers_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/aws.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/aws.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/cli.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/cli.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/config.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/config.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/config_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/config_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/constants.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/constants.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/core.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,27 +501,14 @@
                 s3.put_object(
                     Bucket=f"sc-puppet-parameterised-runs-{puppet_account_id}",
                     Key="parameters.zip",
                     Body=buff.getvalue(),
                 )
 
     click.echo("Finished creating {}.".format(constants.BOOTSTRAP_STACK_NAME))
-    if source_provider == "CodeCommit":
-        with betterboto_client.ClientContextManager("codecommit") as codecommit:
-            response = codecommit.get_repository(repositoryName=repo)
-            clone_url = response.get("repositoryMetadata").get("cloneUrlHttp")
-            clone_command = (
-                "git clone --config 'credential.helper=!aws codecommit credential-helper $@' "
-                "--config 'credential.UseHttpPath=true' {}".format(clone_url)
-            )
-            click.echo(
-                "You need to clone your newly created repo now and will then need to seed it: \n{}".format(
-                    clone_command
-                )
-            )
 
 
 def bootstrap_spoke(
     puppet_account_id, permission_boundary, puppet_role_name, puppet_role_path
 ):
     with betterboto_client.ClientContextManager("cloudformation") as cloudformation:
         _do_bootstrap_spoke(
```

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/all-tasks-for-launch-b.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/all-tasks-for-launch-b.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/all-tasks.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/all-tasks.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/deployment-map.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/deployment-map.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-a.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-a.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-b.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-b.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-c.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-c.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/launch-details-for-launch-b.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/launch-details-for-launch-b.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/manifest-tasks.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/manifest-tasks.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/manifest.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/manifest.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/account-vending/manifest_with_numbers.json` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/account-vending/manifest_with_numbers.json`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_all_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_empty_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_lists_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/accounts/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_all_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_default_region_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_empty_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_enabled_regions_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_lists_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_regions_enabled_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/tags/test_convert_manifest_into_task_defs_handles_unsupported_string.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks_expected.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_handles_depends_on_without-leaks_expected.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248_1.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils/test_convert_manifest_into_task_defs_issue_248_1.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/data/manifest_utils_for_spoke_local_portfolios/simple.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/data/manifest_utils_for_spoke_local_portfolios/simple.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_for_explode_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_for_explode_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_for_launches.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_for_launches.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_for_spoke_local_portfolios.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_for_spoke_local_portfolios.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifest_utils_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifest_utils_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifests/manifest-quickstart.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifests/manifest-quickstart.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/manifests/manifest-simple.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/manifests/manifest-simple.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/puppet_schema_extensions.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/puppet_schema_extensions.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/schema.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/schema.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/sdk.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/sdk.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-initialiser.template.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-initialiser.template.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,16 @@
     Description: For Github.com, GitHub Enterprise and BitBucket Cloud support use CodeStarSourceConnection
     Default: CodeCommit
   SCMRepositoryName:
     Type: String
     Default: ServiceCatalogPuppet
   SCMBranchName:
     Type: String
-    Default: master
+    Default: main
+    Description: The branch name to use for the service-catalog-puppet-pipeline
   SCMConnectionArn:
     Type: String
     Description: The Arn of the CodeStar Connection already created in the account
   SCMFullRepositoryId:
     Type: String
     Description: The full repository id for the git repo to use.  This varies based on which git provider you use
   SCMBucketName:
```

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-org-master.template.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-org-master.template.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-regional.template.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-regional.template.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet-spoke.template.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet-spoke.template.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/servicecatalog-puppet.template.yaml` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/servicecatalog-puppet.template.yaml`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/bootstrap.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -655,70 +655,70 @@
         )
     )
 
     if is_manual_approvals:
         deploy_stage = codepipeline.Stages(
             Name="Deploy",
             Actions=[
-                {
-                    "InputArtifacts": [
+                codepipeline.Actions(
+                    InputArtifacts=[
                         codepipeline.InputArtifacts(Name="Source"),
                         codepipeline.InputArtifacts(Name="ParameterisedSource"),
                     ],
-                    "Name": "DryRun",
-                    "ActionTypeId": codepipeline.ActionTypeId(
+                    Name="DryRun",
+                    ActionTypeId=codepipeline.ActionTypeId(
                         Category="Build",
                         Owner="AWS",
                         Version="1",
                         Provider="CodeBuild",
                     ),
-                    "OutputArtifacts": [
+                    OutputArtifacts=[
                         codepipeline.OutputArtifacts(Name="DryRunProject")
                     ],
-                    "Configuration": {
+                    Configuration={
                         "ProjectName": t.Ref("DryRunProject"),
                         "PrimarySource": "Source",
                     },
-                    "RunOrder": 1,
-                },
-                {
-                    "ActionTypeId": codepipeline.ActionTypeId(
+                    RunOrder=1,
+                ),
+                codepipeline.Actions(
+                    ActionTypeId=codepipeline.ActionTypeId(
                         Category="Approval",
                         Owner="AWS",
                         Version="1",
                         Provider="Manual",
                     ),
-                    "Configuration": {
+                    Configuration={
                         "NotificationArn": t.Ref("DryRunNotificationTopic"),
                         "CustomData": "Approve when you are happy with the dry run.",
                     },
-                    "Name": "DryRunApproval",
-                    "RunOrder": 2,
-                },
-                {
-                    "InputArtifacts": [
+                    Name="DryRunApproval",
+                    RunOrder=2,
+                ),
+                codepipeline.Actions(
+                    InputArtifacts=[
                         codepipeline.InputArtifacts(Name="Source"),
                         codepipeline.InputArtifacts(Name="ParameterisedSource"),
                     ],
-                    "Name": "Deploy",
-                    "ActionTypeId": codepipeline.ActionTypeId(
+                    Name="Deploy",
+                    ActionTypeId=codepipeline.ActionTypeId(
                         Category="Build",
                         Owner="AWS",
                         Version="1",
                         Provider="CodeBuild",
                     ),
-                    "OutputArtifacts": [
+                    OutputArtifacts=[
                         codepipeline.OutputArtifacts(Name="DeployProject")
                     ],
-                    "Configuration": {
+                    Configuration={
                         "ProjectName": t.Ref("DeployProject"),
                         "PrimarySource": "Source",
                     },
-                    "RunOrder": 3,
-                },
+                    RunOrder=3,
+                ),
             ],
         )
     else:
         deploy_stage = codepipeline.Stages(
             Name="Deploy",
             Actions=[
                 codepipeline.Actions(
```

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/bootstrap_region.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/bootstrap_region.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/template_builder/hub/bootstrap_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/template_builder/hub/bootstrap_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/associations.template.yaml.j2` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/associations.template.yaml.j2`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/launch_role_constraints.template.yaml.j2` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/launch_role_constraints.template.yaml.j2`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/policies.template.yaml.j2` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/policies.template.yaml.j2`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/templates/product.template.yaml.j2` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/templates/product.template.yaml.j2`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/general.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/general.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/general_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/general_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/generate.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/generate.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/generate_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/generate_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/lambda_invocations.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/lambda_invocations.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/launch.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/launch.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/launch_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/launch_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/management.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/management.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/management_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/management_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/manifest.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/manifest.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/portfoliomanagement.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/portfoliomanagement.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/portfoliomanagement_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/portfoliomanagement_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/provisioning.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/provisioning.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/provisioning_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/provisioning_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/runner.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/runner.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/spoke_local_portfolios.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/spoke_local_portfolios.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/spoke_local_portfolios_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/spoke_local_portfolios_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/tasks.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/tasks_c_unit_test.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/tasks_c_unit_test.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/servicecatalog_puppet/workflow/tasks_unit_tests.py` & `aws-service-catalog-puppet-0.99.2/servicecatalog_puppet/workflow/tasks_unit_tests.py`

 * *Files identical despite different names*

### Comparing `aws-service-catalog-puppet-0.99.1/setup.py` & `aws-service-catalog-puppet-0.99.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
  'urllib3==1.25.11']
 
 entry_points = \
 {'console_scripts': ['servicecatalog-puppet = servicecatalog_puppet.cli:cli']}
 
 setup_kwargs = {
     'name': 'aws-service-catalog-puppet',
-    'version': '0.99.1',
+    'version': '0.99.2',
     'description': 'Making it easier to deploy ServiceCatalog products',
     'long_description': '# aws-service-catalog-puppet\n\n![logo](./docs/logo.png) \n\n## What is it?\nThis is a python3 framework that makes it easier to share multi region AWS Service Catalog portfolios and makes it \npossible to provision products into accounts declaratively using a metadata based rules engine.\n\nWith this framework you define your accounts in a YAML file.  You give each account a set of tags, a default region and \na set of enabled regions.\n\nOnce you have done this you can define portfolios should be shared with each set of accounts using the tags and you \ncan specify which regions the shares occur in.\n\nIn addition to this, you can also define products that should be provisioned into accounts using the same tag based \napproach.  The framework will assume role into the target account and provision the product on your behalf.\n\n\n## Getting started\n\nYou can read the [installation how to](https://service-catalog-tools-workshop.com/30-how-tos/10-installation/30-service-catalog-puppet.html)\nor you can read through the [every day use](https://service-catalog-tools-workshop.com/30-how-tos/50-every-day-use.html)\nguides.\n\nYou can read the [documentation](https://aws-service-catalog-puppet.readthedocs.io/en/latest/) to understand the inner \nworkings. \n\n\n## Going further\n\nThe framework is one of a pair.  The other is [aws-service-catalog-factory](https://github.com/awslabs/aws-service-catalog-factory).\nWith Service Catalog Factory you can create pipelines that deploy multi region portfolios very easily. \n\n## License\n\nThis library is licensed under the Apache 2.0 License. \n \n',
     'author': 'Eamonn Faherty',
     'author_email': 'aws-service-catalog-tools@amazon.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://service-catalog-tools-workshop.com/',
```

### Comparing `aws-service-catalog-puppet-0.99.1/PKG-INFO` & `aws-service-catalog-puppet-0.99.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-service-catalog-puppet
-Version: 0.99.1
+Version: 0.99.2
 Summary: Making it easier to deploy ServiceCatalog products
 Home-page: https://service-catalog-tools-workshop.com/
 Author: Eamonn Faherty
 Author-email: aws-service-catalog-tools@amazon.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

