# Comparing `tmp/fern_vitruvi-0.0.4.tar.gz` & `tmp/fern_vitruvi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_vitruvi-0.0.4.tar", max compression
+gzip compressed data, was "fern_vitruvi-0.0.5.tar", max compression
```

## Comparing `fern_vitruvi-0.0.4.tar` & `fern_vitruvi-0.0.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1294 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/README.md
--rw-r--r--   0        0        0      374 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3438 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/__init__.py
--rw-r--r--   0        0        0     1480 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/client.py
--rw-r--r--   0        0        0      348 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      203 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/errors/not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/py.typed
--rw-r--r--   0        0        0      188 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/auth/__init__.py
--rw-r--r--   0        0        0    32434 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/global_configuration/__init__.py
--rw-r--r--   0        0        0    24463 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/global_configuration/client.py
--rw-r--r--   0        0        0       65 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/jobs/__init__.py
--rw-r--r--   0        0        0     2661 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/reporting/__init__.py
--rw-r--r--   0        0        0    86362 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/resources/reporting/client.py
--rw-r--r--   0        0        0     4984 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/__init__.py
--rw-r--r--   0        0        0      915 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/account.py
--rw-r--r--   0        0        0     1653 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/accounts_payable_item_export.py
--rw-r--r--   0        0        0     1656 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/accounts_receivable_item_export.py
--rw-r--r--   0        0        0      746 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/async_api_result.py
--rw-r--r--   0        0        0     2197 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/company.py
--rw-r--r--   0        0        0      627 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/company_type_enum.py
--rw-r--r--   0        0        0      861 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/crew_export.py
--rw-r--r--   0        0        0      814 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/crew_member_export.py
--rw-r--r--   0        0        0     1105 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/custom_field_settings_export.py
--rw-r--r--   0        0        0     1343 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/design_element_export.py
--rw-r--r--   0        0        0      920 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/design_export.py
--rw-r--r--   0        0        0      749 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/error_message.py
--rw-r--r--   0        0        0      804 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/full_crew_person_role.py
--rw-r--r--   0        0        0      680 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/global_configuration_list_v_1_companies_request_type.py
--rw-r--r--   0        0        0     1415 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/invoice_export.py
--rw-r--r--   0        0        0      993 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_accounts_payable_item_export_list.py
--rw-r--r--   0        0        0     1005 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py
--rw-r--r--   0        0        0      918 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_company_list.py
--rw-r--r--   0        0        0      931 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_crew_export_list.py
--rw-r--r--   0        0        0      956 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_crew_member_export_list.py
--rw-r--r--   0        0        0      993 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_custom_field_settings_export_list.py
--rw-r--r--   0        0        0      968 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_design_element_export_list.py
--rw-r--r--   0        0        0      939 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_design_export_list.py
--rw-r--r--   0        0        0      943 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_invoice_export_list.py
--rw-r--r--   0        0        0      930 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_permission_list.py
--rw-r--r--   0        0        0      980 2023-06-06 17:38:30.940180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_production_report_export_list.py
--rw-r--r--   0        0        0      997 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_production_report_line_export_list.py
--rw-r--r--   0        0        0     1013 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_production_report_quantity_export_list.py
--rw-r--r--   0        0        0      943 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_profile_export_list.py
--rw-r--r--   0        0        0      939 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_region_export_list.py
--rw-r--r--   0        0        0      906 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_results.py
--rw-r--r--   0        0        0      906 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_role_list.py
--rw-r--r--   0        0        0      935 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_scope_export_list.py
--rw-r--r--   0        0        0      948 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_item_export_list.py
--rw-r--r--   0        0        0      981 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_item_quantity_export_list.py
--rw-r--r--   0        0        0      952 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_order_export_list.py
--rw-r--r--   0        0        0      960 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_package_export_list.py
--rw-r--r--   0        0        0      774 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/permission.py
--rw-r--r--   0        0        0     1211 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/production_report_export.py
--rw-r--r--   0        0        0     1094 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/production_report_line_export.py
--rw-r--r--   0        0        0     1218 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/production_report_quantity_export.py
--rw-r--r--   0        0        0     2423 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/profile.py
--rw-r--r--   0        0        0      992 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/profile_export.py
--rw-r--r--   0        0        0      793 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/refresh_token.py
--rw-r--r--   0        0        0     1000 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/region_export.py
--rw-r--r--   0        0        0      801 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/role.py
--rw-r--r--   0        0        0      876 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/scope_export.py
--rw-r--r--   0        0        0      863 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/user_info.py
--rw-r--r--   0        0        0     1312 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/user_tier_enum.py
--rw-r--r--   0        0        0      813 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/verify_json_web_token.py
--rw-r--r--   0        0        0      987 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/web_token.py
--rw-r--r--   0        0        0     1294 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/work_item_export.py
--rw-r--r--   0        0        0     1101 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/work_item_quantity_export.py
--rw-r--r--   0        0        0     1375 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/work_order_export.py
--rw-r--r--   0        0        0     1329 2023-06-06 17:38:30.944180 fern_vitruvi-0.0.4/src/vitruvi/types/work_package_export.py
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 fern_vitruvi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2300 2023-06-06 17:53:56.533512 fern_vitruvi-0.0.5/README.md
+-rw-r--r--   0        0        0      374 2023-06-06 17:53:56.533512 fern_vitruvi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3438 2023-06-06 17:53:56.533512 fern_vitruvi-0.0.5/src/vitruvi/__init__.py
+-rw-r--r--   0        0        0     1451 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/client.py
+-rw-r--r--   0        0        0      348 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      203 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/errors/not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/py.typed
+-rw-r--r--   0        0        0      188 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/auth/__init__.py
+-rw-r--r--   0        0        0    29772 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/global_configuration/__init__.py
+-rw-r--r--   0        0        0    23277 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/global_configuration/client.py
+-rw-r--r--   0        0        0       65 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     2459 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-06-06 17:53:56.537512 fern_vitruvi-0.0.5/src/vitruvi/resources/reporting/__init__.py
+-rw-r--r--   0        0        0    80912 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/resources/reporting/client.py
+-rw-r--r--   0        0        0     4984 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/__init__.py
+-rw-r--r--   0        0        0      915 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/account.py
+-rw-r--r--   0        0        0     1653 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/accounts_payable_item_export.py
+-rw-r--r--   0        0        0     1656 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/accounts_receivable_item_export.py
+-rw-r--r--   0        0        0      746 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/async_api_result.py
+-rw-r--r--   0        0        0     2197 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/company.py
+-rw-r--r--   0        0        0      627 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/company_type_enum.py
+-rw-r--r--   0        0        0      861 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/crew_export.py
+-rw-r--r--   0        0        0      814 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/crew_member_export.py
+-rw-r--r--   0        0        0     1105 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/custom_field_settings_export.py
+-rw-r--r--   0        0        0     1343 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/design_element_export.py
+-rw-r--r--   0        0        0      920 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/design_export.py
+-rw-r--r--   0        0        0      749 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/error_message.py
+-rw-r--r--   0        0        0      804 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/full_crew_person_role.py
+-rw-r--r--   0        0        0      680 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/global_configuration_list_v_1_companies_request_type.py
+-rw-r--r--   0        0        0     1415 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/invoice_export.py
+-rw-r--r--   0        0        0      993 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_accounts_payable_item_export_list.py
+-rw-r--r--   0        0        0     1005 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py
+-rw-r--r--   0        0        0      918 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_company_list.py
+-rw-r--r--   0        0        0      931 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_crew_export_list.py
+-rw-r--r--   0        0        0      956 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_crew_member_export_list.py
+-rw-r--r--   0        0        0      993 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_custom_field_settings_export_list.py
+-rw-r--r--   0        0        0      968 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_design_element_export_list.py
+-rw-r--r--   0        0        0      939 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_design_export_list.py
+-rw-r--r--   0        0        0      943 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_invoice_export_list.py
+-rw-r--r--   0        0        0      930 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_permission_list.py
+-rw-r--r--   0        0        0      980 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_production_report_export_list.py
+-rw-r--r--   0        0        0      997 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_production_report_line_export_list.py
+-rw-r--r--   0        0        0     1013 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_production_report_quantity_export_list.py
+-rw-r--r--   0        0        0      943 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_profile_export_list.py
+-rw-r--r--   0        0        0      939 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_region_export_list.py
+-rw-r--r--   0        0        0      906 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_results.py
+-rw-r--r--   0        0        0      906 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_role_list.py
+-rw-r--r--   0        0        0      935 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_scope_export_list.py
+-rw-r--r--   0        0        0      948 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_item_export_list.py
+-rw-r--r--   0        0        0      981 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_item_quantity_export_list.py
+-rw-r--r--   0        0        0      952 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_order_export_list.py
+-rw-r--r--   0        0        0      960 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_package_export_list.py
+-rw-r--r--   0        0        0      774 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/permission.py
+-rw-r--r--   0        0        0     1211 2023-06-06 17:53:56.541512 fern_vitruvi-0.0.5/src/vitruvi/types/production_report_export.py
+-rw-r--r--   0        0        0     1094 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/production_report_line_export.py
+-rw-r--r--   0        0        0     1218 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/production_report_quantity_export.py
+-rw-r--r--   0        0        0     2423 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/profile.py
+-rw-r--r--   0        0        0      992 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/profile_export.py
+-rw-r--r--   0        0        0      793 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/refresh_token.py
+-rw-r--r--   0        0        0     1000 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/region_export.py
+-rw-r--r--   0        0        0      801 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/role.py
+-rw-r--r--   0        0        0      876 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/scope_export.py
+-rw-r--r--   0        0        0      863 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/user_info.py
+-rw-r--r--   0        0        0     1312 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/user_tier_enum.py
+-rw-r--r--   0        0        0      813 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/verify_json_web_token.py
+-rw-r--r--   0        0        0      987 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/web_token.py
+-rw-r--r--   0        0        0     1294 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/work_item_export.py
+-rw-r--r--   0        0        0     1101 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/work_item_quantity_export.py
+-rw-r--r--   0        0        0     1375 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/work_order_export.py
+-rw-r--r--   0        0        0     1329 2023-06-06 17:53:56.545512 fern_vitruvi-0.0.5/src/vitruvi/types/work_package_export.py
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 fern_vitruvi-0.0.5/PKG-INFO
```

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/__init__.py` & `fern_vitruvi-0.0.5/src/vitruvi/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/core/datetime_utils.py` & `fern_vitruvi-0.0.5/src/vitruvi/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/core/jsonable_encoder.py` & `fern_vitruvi-0.0.5/src/vitruvi/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/resources/auth/client.py` & `fern_vitruvi-0.0.5/src/vitruvi/resources/auth/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from ...types.web_token import WebToken
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AuthClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     def list_auth_permissions(
         self,
         *,
         codename: typing.Optional[str] = None,
         group: typing.Union[typing.Optional[int], typing.List[int]],
         limit: typing.Optional[int] = None,
@@ -45,17 +45,15 @@
                 "codename": codename,
                 "group": group,
                 "limit": limit,
                 "offset": offset,
                 "ordering": ordering,
                 "search": search,
             },
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedPermissionList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -63,34 +61,30 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_auth_permissions(self, *, request: Permission) -> Permission:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "auth/permissions"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_auth_permissions(self, id: int) -> Permission:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -98,17 +92,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_auth_permissions(self, id: int, *, request: Permission) -> Permission:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -130,34 +122,30 @@
             _request["name"] = name
         if codename is not OMIT:
             _request["codename"] = codename
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_auth_permissions(self, id: int) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -179,17 +167,15 @@
             params={
                 "limit": limit,
                 "offset": offset,
                 "ordering": ordering,
                 "permissions": permissions,
                 "search": search,
             },
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRoleList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -197,34 +183,30 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_auth_security_groups(self, *, request: Role) -> Role:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "auth/security_groups"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_auth_security_groups(self, id: int) -> Role:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -232,17 +214,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_auth_security_groups(self, id: int, *, request: Role) -> Role:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -264,34 +244,30 @@
             _request["name"] = name
         if permissions is not OMIT:
             _request["permissions"] = permissions
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_auth_security_groups(self, id: int) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -299,17 +275,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def obtain_token(self, *, request: WebToken) -> WebToken:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "auth/token/obtain"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -317,17 +291,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def refresh_token(self, *, request: RefreshToken) -> RefreshToken:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "auth/token/refresh"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RefreshToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -335,49 +307,45 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def verify_token(self, *, request: VerifyJsonWebToken) -> VerifyJsonWebToken:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "auth/token/verify"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(VerifyJsonWebToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def user_info(self) -> UserInfo:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "auth/user_info"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserInfo, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAuthClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     async def list_auth_permissions(
         self,
         *,
         codename: typing.Optional[str] = None,
         group: typing.Union[typing.Optional[int], typing.List[int]],
         limit: typing.Optional[int] = None,
@@ -393,17 +361,15 @@
                     "codename": codename,
                     "group": group,
                     "limit": limit,
                     "offset": offset,
                     "ordering": ordering,
                     "search": search,
                 },
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedPermissionList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -412,17 +378,15 @@
 
     async def create_auth_permissions(self, *, request: Permission) -> Permission:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "auth/permissions"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -430,17 +394,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_auth_permissions(self, id: int) -> Permission:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -449,17 +411,15 @@
 
     async def update_auth_permissions(self, id: int, *, request: Permission) -> Permission:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -482,17 +442,15 @@
         if codename is not OMIT:
             _request["codename"] = codename
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Permission, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -500,17 +458,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_auth_permissions(self, id: int) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/permissions/{id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -533,17 +489,15 @@
                 params={
                     "limit": limit,
                     "offset": offset,
                     "ordering": ordering,
                     "permissions": permissions,
                     "search": search,
                 },
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRoleList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -552,17 +506,15 @@
 
     async def create_auth_security_groups(self, *, request: Role) -> Role:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "auth/security_groups"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -570,17 +522,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_auth_security_groups(self, id: int) -> Role:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -589,17 +539,15 @@
 
     async def update_auth_security_groups(self, id: int, *, request: Role) -> Role:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -622,17 +570,15 @@
         if permissions is not OMIT:
             _request["permissions"] = permissions
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Role, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -640,17 +586,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_auth_security_groups(self, id: int) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"auth/security_groups/{id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -659,17 +603,15 @@
 
     async def obtain_token(self, *, request: WebToken) -> WebToken:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "auth/token/obtain"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(WebToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -678,17 +620,15 @@
 
     async def refresh_token(self, *, request: RefreshToken) -> RefreshToken:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "auth/token/refresh"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RefreshToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -697,17 +637,15 @@
 
     async def verify_token(self, *, request: VerifyJsonWebToken) -> VerifyJsonWebToken:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "auth/token/verify"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(VerifyJsonWebToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -715,17 +653,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def user_info(self) -> UserInfo:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "auth/user_info"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserInfo, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/resources/global_configuration/client.py` & `fern_vitruvi-0.0.5/src/vitruvi/resources/global_configuration/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from ...types.user_tier_enum import UserTierEnum
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class GlobalConfigurationClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     def list_v_1_companies(
         self,
         *,
         code: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         is_active: typing.Optional[bool] = None,
@@ -50,17 +50,15 @@
                 "offset": offset,
                 "ordering": ordering,
                 "search": search,
                 "type": type,
                 "with_no_subcontract": with_no_subcontract,
                 "with_subcontract_or_epc": with_subcontract_or_epc,
             },
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCompanyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -68,34 +66,30 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_v_1_companies(self, *, request: Company) -> Company:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/companies"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_v_1_companies(self, id: int) -> Company:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -103,17 +97,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_v_1_companies(self, id: int, *, request: Company) -> Company:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -225,66 +217,60 @@
             _request["admin_permission"] = admin_permission
         if denied_permission is not OMIT:
             _request["denied_permission"] = denied_permission
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_v_1_companies(self, id: int) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_company_logo(self, id: int) -> Company:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}/download_logo"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncGlobalConfigurationClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     async def list_v_1_companies(
         self,
         *,
         code: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         is_active: typing.Optional[bool] = None,
@@ -308,17 +294,15 @@
                     "offset": offset,
                     "ordering": ordering,
                     "search": search,
                     "type": type,
                     "with_no_subcontract": with_no_subcontract,
                     "with_subcontract_or_epc": with_subcontract_or_epc,
                 },
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCompanyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -327,17 +311,15 @@
 
     async def create_v_1_companies(self, *, request: Company) -> Company:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/companies"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -345,17 +327,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_v_1_companies(self, id: int) -> Company:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -364,17 +344,15 @@
 
     async def update_v_1_companies(self, id: int, *, request: Company) -> Company:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -487,17 +465,15 @@
         if denied_permission is not OMIT:
             _request["denied_permission"] = denied_permission
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -505,17 +481,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_v_1_companies(self, id: int) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -523,17 +497,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_company_logo(self, id: int) -> Company:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}/download_logo"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/resources/jobs/client.py` & `fern_vitruvi-0.0.5/src/vitruvi/resources/jobs/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,51 +10,47 @@
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.not_found_error import NotFoundError
 from ...types.async_api_result import AsyncApiResult
 
 
 class JobsClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     def job_status(self, id: str) -> AsyncApiResult:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/job_status/{id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AsyncApiResult, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncJobsClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     async def job_status(self, id: str) -> AsyncApiResult:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/job_status/{id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AsyncApiResult, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/resources/reporting/client.py` & `fern_vitruvi-0.0.5/src/vitruvi/resources/reporting/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,34 +29,32 @@
 from ...types.paginated_work_item_export_list import PaginatedWorkItemExportList
 from ...types.paginated_work_item_quantity_export_list import PaginatedWorkItemQuantityExportList
 from ...types.paginated_work_order_export_list import PaginatedWorkOrderExportList
 from ...types.paginated_work_package_export_list import PaginatedWorkPackageExportList
 
 
 class ReportingClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     def design_elements_query(
         self,
         *,
         filter: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         ids: typing.Union[typing.Optional[int], typing.List[int]],
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/engineering/design_elements_query"),
             params={"$filter": filter, "fields": fields, "ids": ids, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -73,17 +71,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/engineering/design_elements_work_items_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -101,17 +97,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/engineering/limited_design_elements_query"),
             params={"$filter": filter, "fields": fields, "ids": ids, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -128,17 +122,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/invoicing/invoice_items_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -155,17 +147,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/invoicing/invoices_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -182,17 +172,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/production/production_report_grid_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -209,17 +197,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/production/production_reports_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -237,17 +223,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/raw/{app_label}/{model_name}"),
             params={"fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
@@ -267,17 +251,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedAccountsPayableItemExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/accounts_payable_items_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountsPayableItemExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -293,17 +275,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedAccountsReceivableItemExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/accounts_receivable_items_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountsReceivableItemExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -319,17 +299,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedCrewMemberExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/crew_members_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCrewMemberExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -345,17 +323,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedCrewExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/crews_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCrewExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -371,17 +347,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedCustomFieldSettingsExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/custom_field_settings_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCustomFieldSettingsExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -397,17 +371,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedDesignElementExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/design_elements_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedDesignElementExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -423,17 +395,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedDesignExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/designs_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedDesignExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -449,17 +419,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedInvoiceExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/invoices_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedInvoiceExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -475,17 +443,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedProductionReportLineExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/production_report_lines_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProductionReportLineExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -501,17 +467,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedProductionReportQuantityExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/production_report_quantities_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProductionReportQuantityExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -527,17 +491,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedProductionReportExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/production_reports_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProductionReportExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -553,17 +515,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedProfileExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/profiles_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProfileExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -579,17 +539,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedRegionExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/regions_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRegionExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -605,17 +563,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedScopeExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/scopes_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedScopeExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -631,17 +587,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkItemQuantityExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_item_quantities_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkItemQuantityExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -657,17 +611,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkItemExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_items_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkItemExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -683,17 +635,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkOrderExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_orders_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkOrderExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -709,17 +659,15 @@
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkPackageExportList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_packages_export"),
             params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkPackageExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -734,17 +682,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/ticketing/tickets_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -761,17 +707,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/time_keeping/timesheet_lines_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -788,17 +732,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/time_keeping/timesheets_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -815,17 +757,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_item_quantities_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -842,17 +782,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_items_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -869,17 +807,15 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_orders_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -896,34 +832,32 @@
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_packages_query"),
             params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncReportingClient:
-    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
+    def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
-        self._token = token
+        self.api_key = api_key
 
     async def design_elements_query(
         self,
         *,
         filter: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         ids: typing.Union[typing.Optional[int], typing.List[int]],
@@ -931,17 +865,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/engineering/design_elements_query"),
                 params={"$filter": filter, "fields": fields, "ids": ids, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -959,17 +891,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/engineering/design_elements_work_items_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -988,17 +918,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/engineering/limited_design_elements_query"),
                 params={"$filter": filter, "fields": fields, "ids": ids, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1016,17 +944,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/invoicing/invoice_items_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1044,17 +970,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/invoicing/invoices_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1072,17 +996,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/production/production_report_grid_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1100,17 +1022,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/production/production_reports_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1129,17 +1049,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/raw/{app_label}/{model_name}"),
                 params={"fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
@@ -1160,17 +1078,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedAccountsPayableItemExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/accounts_payable_items_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountsPayableItemExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1187,17 +1103,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedAccountsReceivableItemExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/accounts_receivable_items_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountsReceivableItemExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1214,17 +1128,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedCrewMemberExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/crew_members_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCrewMemberExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1241,17 +1153,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedCrewExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/crews_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCrewExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1268,17 +1178,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedCustomFieldSettingsExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/custom_field_settings_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCustomFieldSettingsExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1295,17 +1203,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedDesignElementExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/design_elements_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedDesignElementExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1322,17 +1228,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedDesignExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/designs_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedDesignExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1349,17 +1253,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedInvoiceExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/invoices_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedInvoiceExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1376,17 +1278,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedProductionReportLineExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/production_report_lines_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProductionReportLineExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1403,17 +1303,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedProductionReportQuantityExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/production_report_quantities_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProductionReportQuantityExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1430,17 +1328,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedProductionReportExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/production_reports_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProductionReportExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1457,17 +1353,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedProfileExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/profiles_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedProfileExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1484,17 +1378,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedRegionExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/regions_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRegionExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1511,17 +1403,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedScopeExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/scopes_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedScopeExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1538,17 +1428,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkItemQuantityExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_item_quantities_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkItemQuantityExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1565,17 +1453,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkItemExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_items_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkItemExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1592,17 +1478,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkOrderExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_orders_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkOrderExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1619,17 +1503,15 @@
         search: typing.Optional[str] = None,
     ) -> PaginatedWorkPackageExportList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/reporting/work_packages_export"),
                 params={"fields": fields, "limit": limit, "offset": offset, "ordering": ordering, "search": search},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedWorkPackageExportList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -1645,17 +1527,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/ticketing/tickets_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1673,17 +1553,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/time_keeping/timesheet_lines_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1701,17 +1579,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/time_keeping/timesheets_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1729,17 +1605,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_item_quantities_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1757,17 +1631,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_items_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1785,17 +1657,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_orders_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -1813,17 +1683,15 @@
         offset: typing.Optional[int] = None,
     ) -> PaginatedResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/wbs/work_packages_query"),
                 params={"$filter": filter, "fields": fields, "limit": limit, "offset": offset},
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedResults, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/__init__.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/account.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/account.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/accounts_payable_item_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/accounts_payable_item_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/accounts_receivable_item_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/accounts_receivable_item_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/async_api_result.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/async_api_result.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/company.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/company.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/company_type_enum.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/company_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/crew_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/crew_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/crew_member_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/crew_member_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/custom_field_settings_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/custom_field_settings_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/design_element_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/design_element_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/design_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/design_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/error_message.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/error_message.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/full_crew_person_role.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/full_crew_person_role.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/global_configuration_list_v_1_companies_request_type.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/global_configuration_list_v_1_companies_request_type.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/invoice_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/invoice_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_accounts_payable_item_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_accounts_payable_item_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_company_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_crew_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_crew_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_crew_member_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_crew_member_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_custom_field_settings_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_custom_field_settings_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_design_element_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_design_element_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_design_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_design_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_invoice_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_invoice_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_permission_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_production_report_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_production_report_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_production_report_line_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_production_report_line_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_production_report_quantity_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_production_report_quantity_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_profile_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_profile_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_region_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_region_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_results.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_results.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_role_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_scope_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_scope_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_item_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_item_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_item_quantity_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_item_quantity_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_order_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_order_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/paginated_work_package_export_list.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/paginated_work_package_export_list.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/permission.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/permission.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/production_report_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/production_report_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/production_report_line_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/production_report_line_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/production_report_quantity_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/production_report_quantity_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/profile.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/profile.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/profile_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/profile_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/refresh_token.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/refresh_token.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/region_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/region_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/role.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/role.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/scope_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/scope_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/user_info.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/user_info.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/user_tier_enum.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/user_tier_enum.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/verify_json_web_token.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/verify_json_web_token.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/web_token.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/web_token.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/work_item_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/work_item_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/work_item_quantity_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/work_item_quantity_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/work_order_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/work_order_export.py`

 * *Files identical despite different names*

### Comparing `fern_vitruvi-0.0.4/src/vitruvi/types/work_package_export.py` & `fern_vitruvi-0.0.5/src/vitruvi/types/work_package_export.py`

 * *Files identical despite different names*

