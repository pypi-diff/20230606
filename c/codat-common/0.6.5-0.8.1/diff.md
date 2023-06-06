# Comparing `tmp/codat-common-0.6.5.tar.gz` & `tmp/codat-common-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-common-0.6.5.tar", last modified: Wed Apr  5 09:29:09 2023, max compression
+gzip compressed data, was "codat-common-0.8.1.tar", last modified: Tue Apr 18 08:14:26 2023, max compression
```

## Comparing `codat-common-0.6.5.tar` & `codat-common-0.8.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.318545 codat-common-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-05 09:29:09.318545 codat-common-0.6.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-04-05 09:28:59.000000 codat-common-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:29:09.318545 codat-common-0.6.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-05 09:28:59.000000 codat-common-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.306545 codat-common-0.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.306545 codat-common-0.6.5/src/codat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7122 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9326 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4764 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/data_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.306545 codat-common-0.6.5/src/codat/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.310545 codat-common-0.6.5/src/codat/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2709 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/create_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/create_data_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/create_pull_operation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/create_rule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/delete_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/delete_company_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_company_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2035 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_company_data_history.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_company_data_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1811 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_company_push_history.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_create_update_model_options_by_data_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_integrations_branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_profile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_profile_syncsettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_pull_operation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_push_operation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/get_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1822 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/list_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/list_company_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/list_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1794 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/list_rules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/refresh_company_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/unlink_company_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/update_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/update_connection_authorization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/update_profile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/operations/update_sync_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.314545 codat-common-0.6.5/src/codat/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/brandingbutton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/brandingimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/brandinglogo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1161 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4159 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/companydataconnectionstatuschangedwebhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/companyrequestbody.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5232 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/connectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1996 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/dataconnectionhistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2347 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/datasetdatachangedwebhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2612 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/datasetstatuschangederrorwebhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/datastatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/datasynccompletedwebhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/datatype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      968 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/datatypefeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/errormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/featurestate_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/featuretype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/href.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/imagereference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1606 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/newcompanysynchronizedwebhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1758 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/profile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3298 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pulloperation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushchangetype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      809 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushfieldvalidation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1223 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushhistoryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5502 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoperation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoperationchange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoperationref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      318 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoperationstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2585 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoperationstatuschangedwebhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5260 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoperationsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoperationtimedoutwebhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1904 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoption.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoptionchoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoptionproperty.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushoptiontype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/pushvalidationinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/rule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1145 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/rules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/sourcetype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/supportedfeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4827 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/syncsetting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/syncsettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/validation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/shared/validationitem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.318545 codat-common-0.6.5/src/codat/models/webhooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/company_data_connection_status_changed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/data_sync_completed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/dataset_data_changed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/dataset_status_has_changed_to_an_error_state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      441 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/new_company_synchronized.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/push_operation_has_timed_out.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      448 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/models/webhooks/push_operation_status_has_changed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5144 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/push_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/refresh_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5000 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5745 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.318545 codat-common-0.6.5/src/codat/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4518 2023-04-05 09:28:59.000000 codat-common-0.6.5/src/codat/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:09.318545 codat-common-0.6.5/src/codat_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-05 09:29:09.000000 codat-common-0.6.5/src/codat_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-05 09:29:09.000000 codat-common-0.6.5/src/codat_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:29:09.000000 codat-common-0.6.5/src/codat_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 09:29:09.000000 codat-common-0.6.5/src/codat_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:29:09.000000 codat-common-0.6.5/src/codat_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.127254 codat-common-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-18 08:14:26.127254 codat-common-0.8.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2224 2023-04-18 08:14:16.000000 codat-common-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:14:26.127254 codat-common-0.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-18 08:14:16.000000 codat-common-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.115254 codat-common-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.115254 codat-common-0.8.1/src/codat_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-18 08:14:26.000000 codat-common-0.8.1/src/codat_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-18 08:14:26.000000 codat-common-0.8.1/src/codat_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:14:26.000000 codat-common-0.8.1/src/codat_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-18 08:14:26.000000 codat-common-0.8.1/src/codat_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 08:14:26.000000 codat-common-0.8.1/src/codat_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.115254 codat-common-0.8.1/src/codatcommon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9348 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11996 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6102 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/data_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5611 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.115254 codat-common-0.8.1/src/codatcommon/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.119254 codat-common-0.8.1/src/codatcommon/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2709 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/create_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1677 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/create_data_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/create_pull_operation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/create_rule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/delete_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/delete_company_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_company_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2035 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_company_data_history.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_company_data_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1811 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_company_push_history.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_create_update_model_options_by_data_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_integrations_branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_profile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_profile_syncsettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_pull_operation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_push_operation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/get_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1822 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/list_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/list_company_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/list_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1794 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/list_rules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/refresh_company_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/unlink_company_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/update_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/update_connection_authorization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/update_profile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/operations/update_sync_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.123254 codat-common-0.8.1/src/codatcommon/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/brandingbutton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      639 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/brandingimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/brandinglogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4165 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3377 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/companydataconnectionstatuschangedwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      803 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/companyrequestbody.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5238 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/connectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2002 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/dataconnectionhistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2353 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/datasetdatachangedwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2618 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/datasetstatuschangederrorwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2137 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/datastatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3060 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/datasynccompletedwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/datatype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/datatypefeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/errormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/featurestate_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/featuretype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/href.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/imagereference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3220 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1612 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/newcompanysynchronizedwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/profile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pulloperation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushchangetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushfieldvalidation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1229 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushhistoryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5508 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoperation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoperationchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      816 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoperationref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      318 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoperationstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2591 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoperationstatuschangedwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5266 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoperationsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2363 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoperationtimedoutwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1910 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoptionchoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1753 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoptionproperty.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushoptiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/pushvalidationinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/rule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/rules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/sourcetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/supportedfeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4833 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/syncsetting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/syncsettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      890 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/shared/validationitem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.123254 codat-common-0.8.1/src/codatcommon/models/webhooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/company_data_connection_status_changed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/data_sync_completed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/dataset_data_changed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/dataset_status_has_changed_to_an_error_state.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      441 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/new_company_synchronized.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/push_operation_has_timed_out.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      448 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/models/webhooks/push_operation_status_has_changed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6482 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/push_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4291 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/refresh_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5012 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7527 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:26.127254 codat-common-0.8.1/src/codatcommon/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5856 2023-04-18 08:14:16.000000 codat-common-0.8.1/src/codatcommon/webhooks.py
```

### Comparing `codat-common-0.6.5/PKG-INFO` & `codat-common-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-common
-Version: 0.6.5
+Version: 0.8.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -18,27 +18,27 @@
 pip install codat-common
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
-import codat
-from codat.models import operations, shared
+import codatcommon
+from codatcommon.models import operations, shared
 
-s = codat.Codat(
+s = codatcommon.CodatCommon(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = shared.CompanyRequestBody(
     description="corrupti",
-    name="provident",
+    name="Kelvin Sporer",
 )
     
 res = s.companies.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
```

### Comparing `codat-common-0.6.5/README.md` & `codat-common-0.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 pip install codat-common
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
-import codat
-from codat.models import operations, shared
+import codatcommon
+from codatcommon.models import operations, shared
 
-s = codat.Codat(
+s = codatcommon.CodatCommon(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = shared.CompanyRequestBody(
     description="corrupti",
-    name="provident",
+    name="Kelvin Sporer",
 )
     
 res = s.companies.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
```

### Comparing `codat-common-0.6.5/setup.py` & `codat-common-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-common",
-    version="0.6.5",
+    version="0.8.1",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `codat-common-0.6.5/src/codat/companies.py` & `codat-common-0.8.1/src/codatcommon/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations, shared
+from codatcommon.models import operations, shared
 from typing import Optional
 
-class Companies:
-    r"""Create and manage your Codat companies."""
+class Settings:
+    r"""Manage your Codat instance."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,150 +18,173 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def create_company(self, request: shared.CompanyRequestBody) -> operations.CreateCompanyResponse:
-        r"""Create company
-        Create a new company
+    def get_profile(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetProfileResponse:
+        r"""Get profile
+        Fetch your Codat profile.
         """
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/companies'
+        url = base_url.removesuffix('/') + '/profile'
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.CreateCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetProfileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
-                res.company = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Profile])
+                res.profile = out
         elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def delete_company(self, request: operations.DeleteCompanyRequest) -> operations.DeleteCompanyResponse:
-        r"""Delete a company
-        Delete the given company from Codat.
-        This operation is not reversible.
+    def get_profile_sync_settings(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetProfileSyncSettingsResponse:
+        r"""Get sync settings
+        Retrieve the sync settings for your client. This includes how often data types should be queued to be updated, and how much history should be fetched.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.DeleteCompanyRequest, base_url, '/companies/{companyId}', request)
+        url = base_url.removesuffix('/') + '/profile/syncSettings'
         
         
         client = self._security_client
         
-        http_res = client.request('DELETE', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 204:
-            pass
-        elif http_res.status_code == 401:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
-                res.error_message = out
-
-        return res
-
-    def get_company(self, request: operations.GetCompanyRequest) -> operations.GetCompanyResponse:
-        r"""Get company
-        Get metadata for a single company
-        """
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetCompanyRequest, base_url, '/companies/{companyId}', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetProfileSyncSettingsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
-                res.company = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.SyncSettings])
+                res.sync_settings = out
         elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def list_companies(self, request: operations.ListCompaniesRequest) -> operations.ListCompaniesResponse:
-        r"""List companies
-        List all companies that you have created in Codat.
+    def update_profile(self, request: shared.Profile, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateProfileResponse:
+        r"""Update profile
+        Update your Codat profile
         """
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/companies'
+        url = base_url.removesuffix('/') + '/profile'
         
-        query_params = utils.get_query_params(operations.ListCompaniesRequest, request)
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PUT', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCompaniesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateProfileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Companies])
-                res.companies = out
-        elif http_res.status_code in [400, 401]:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Profile])
+                res.profile = out
+        elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def update_company(self, request: operations.UpdateCompanyRequest) -> operations.UpdateCompanyResponse:
-        r"""Update company
-        Updates the given company with a new name and description
+    def update_sync_settings(self, request: operations.UpdateSyncSettingsRequestBody, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateSyncSettingsResponse:
+        r"""Update all sync settings
+        Update sync settings for all data types.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.UpdateCompanyRequest, base_url, '/companies/{companyId}', request)
+        url = base_url.removesuffix('/') + '/profile/syncSettings'
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "company_request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('PUT', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.UpdateCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateSyncSettingsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
-                res.company = out
+        if http_res.status_code == 204:
+            pass
         elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
```

### Comparing `codat-common-0.6.5/src/codat/connections.py` & `codat-common-0.8.1/src/codatcommon/companies.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations, shared
+from codatcommon.models import operations, shared
 from typing import Optional
 
-class Connections:
-    r"""Manage your companies' data connections."""
+class Companies:
+    r"""Create and manage your Codat companies."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,178 +18,216 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def create_data_connection(self, request: operations.CreateDataConnectionRequest) -> operations.CreateDataConnectionResponse:
-        r"""Create a data connection
-        Create a data connection for a company
+    def create_company(self, request: shared.CompanyRequestBody, retries: Optional[utils.RetryConfig] = None) -> operations.CreateCompanyResponse:
+        r"""Create company
+        Create a new company
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.CreateDataConnectionRequest, base_url, '/companies/{companyId}/connections', request)
+        url = base_url.removesuffix('/') + '/companies'
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.CreateDataConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
-        elif http_res.status_code == 404:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
+                res.company = out
+        elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def delete_company_connection(self, request: operations.DeleteCompanyConnectionRequest) -> operations.DeleteCompanyConnectionResponse:
-        r"""Delete connection
-        Revoke and remove a connection from a company.
-        This operation is not reversible - the end user would need to reauthorize a new data connection if you wish to view new data for this company.
+    def delete_company(self, request: operations.DeleteCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteCompanyResponse:
+        r"""Delete a company
+        Delete the given company from Codat.
+        This operation is not reversible.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.DeleteCompanyConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
+        url = utils.generate_url(operations.DeleteCompanyRequest, base_url, '/companies/{companyId}', request)
         
         
         client = self._security_client
         
-        http_res = client.request('DELETE', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('DELETE', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteCompanyConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
+        if http_res.status_code == 204:
             pass
-        elif http_res.status_code in [401, 404]:
+        elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def get_company_connection(self, request: operations.GetCompanyConnectionRequest) -> operations.GetCompanyConnectionResponse:
-        r"""Get connection
-        Get a single connection for a company
+    def get_company(self, request: operations.GetCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyResponse:
+        r"""Get company
+        Get metadata for a single company
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetCompanyConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
+        url = utils.generate_url(operations.GetCompanyRequest, base_url, '/companies/{companyId}', request)
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetCompanyConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
-        elif http_res.status_code in [401, 404]:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
+                res.company = out
+        elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def list_company_connections(self, request: operations.ListCompanyConnectionsRequest) -> operations.ListCompanyConnectionsResponse:
-        r"""List connections
-        List the connections for a company
+    def list_companies(self, request: operations.ListCompaniesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListCompaniesResponse:
+        r"""List companies
+        List all companies that you have created in Codat.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCompanyConnectionsRequest, base_url, '/companies/{companyId}/connections', request)
+        url = base_url.removesuffix('/') + '/companies'
         
-        query_params = utils.get_query_params(operations.ListCompanyConnectionsRequest, request)
+        query_params = utils.get_query_params(operations.ListCompaniesRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCompanyConnectionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListCompaniesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connections])
-                res.connections = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Companies])
+                res.companies = out
         elif http_res.status_code in [400, 401]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def unlink_company_connection(self, request: operations.UnlinkCompanyConnectionRequest) -> operations.UnlinkCompanyConnectionResponse:
-        r"""Unlink connection
-        This allows you to deauthorize a connection, without deleting it from Codat. This means you can still view any data that has previously been pulled into Codat, and also lets you re-authorize in future if your customer wishes to resume sharing their data.
+    def update_company(self, request: operations.UpdateCompanyRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateCompanyResponse:
+        r"""Update company
+        Updates the given company with a new name and description
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.UnlinkCompanyConnectionRequest, base_url, '/companies/{companyId}/connections/{connectionId}', request)
+        url = utils.generate_url(operations.UpdateCompanyRequest, base_url, '/companies/{companyId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "company_request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PUT', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.UnlinkCompanyConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
-        elif http_res.status_code in [400, 401, 404]:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
+                res.company = out
+        elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def update_connection_authorization(self, request: operations.UpdateConnectionAuthorizationRequest) -> operations.UpdateConnectionAuthorizationResponse:
-        r"""Update authorization
-        Update data connection's authorization.
-        """
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.UpdateConnectionAuthorizationRequest, base_url, '/companies/{companyId}/connections/{connectionId}/authorization', request)
-        
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        
-        client = self._security_client
-        
-        http_res = client.request('PUT', url, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.UpdateConnectionAuthorizationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
-                res.connection = out
-
-        return res
-
```

### Comparing `codat-common-0.6.5/src/codat/data_status.py` & `codat-common-0.8.1/src/codatcommon/refresh_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations, shared
+from codatcommon.models import operations, shared
 from typing import Optional
 
-class DataStatus:
-    r"""Understand the state of data within Codat."""
+class RefreshData:
+    r"""Queue pull operations to refresh data in Codat."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,89 +18,88 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_company_data_history(self, request: operations.GetCompanyDataHistoryRequest) -> operations.GetCompanyDataHistoryResponse:
-        r"""Get pull operations
-        Gets the pull operation history (datasets) for a given company.
-        """
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetCompanyDataHistoryRequest, base_url, '/companies/{companyId}/data/history', request)
-        
-        query_params = utils.get_query_params(operations.GetCompanyDataHistoryRequest, request)
-        
-        client = self._security_client
+    def create_pull_operation(self, request: operations.CreatePullOperationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreatePullOperationResponse:
+        r"""Queue pull operation
+        Queue a single pull operation for the given company and data type.
         
-        http_res = client.request('GET', url, params=query_params)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetCompanyDataHistoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.DataConnectionHistory])
-                res.data_connection_history = out
-        elif http_res.status_code in [400, 401, 404]:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
-                res.error_message = out
-
-        return res
-
-    def get_company_data_status(self, request: operations.GetCompanyDataStatusRequest) -> operations.GetCompanyDataStatusResponse:
-        r"""Get data status
-        Get the state of each data type for a company
+        This will bring updated data into Codat from the linked integration for you to view.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetCompanyDataStatusRequest, base_url, '/companies/{companyId}/dataStatus', request)
+        url = utils.generate_url(operations.CreatePullOperationRequest, base_url, '/companies/{companyId}/data/queue/{dataType}', request)
         
+        query_params = utils.get_query_params(operations.CreatePullOperationRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetCompanyDataStatusResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreatePullOperationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[dict[str, shared.DataStatus]])
-                res.data_status_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperation])
+                res.pull_operation = out
         elif http_res.status_code in [401, 404]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def get_pull_operation(self, request: operations.GetPullOperationRequest) -> operations.GetPullOperationResponse:
-        r"""Get pull operation
-        Retrieve information about a single dataset or pull operation.
+    def refresh_company_data(self, request: operations.RefreshCompanyDataRequest, retries: Optional[utils.RetryConfig] = None) -> operations.RefreshCompanyDataResponse:
+        r"""Queue pull operations
+        Refreshes all data types marked Fetch on first link.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetPullOperationRequest, base_url, '/companies/{companyId}/data/history/{datasetId}', request)
+        url = utils.generate_url(operations.RefreshCompanyDataRequest, base_url, '/companies/{companyId}/data/all', request)
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetPullOperationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.RefreshCompanyDataResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PullOperation])
-                res.pull_operation = out
+        if http_res.status_code == 204:
+            pass
         elif http_res.status_code in [401, 404]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
```

### Comparing `codat-common-0.6.5/src/codat/integrations.py` & `codat-common-0.8.1/src/codatcommon/integrations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations, shared
+from codatcommon.models import operations, shared
 from typing import Optional
 
 class Integrations:
     r"""View and manage your available integrations in Codat."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
@@ -18,26 +18,39 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_integration(self, request: operations.GetIntegrationRequest) -> operations.GetIntegrationResponse:
+    def get_integration(self, request: operations.GetIntegrationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetIntegrationResponse:
         r"""Get integration
         Get single integration, by platformKey
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetIntegrationRequest, base_url, '/integrations/{platformKey}', request)
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetIntegrationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Integration])
@@ -45,50 +58,76 @@
         elif http_res.status_code in [401, 404]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def get_integrations_branding(self, request: operations.GetIntegrationsBrandingRequest) -> operations.GetIntegrationsBrandingResponse:
+    def get_integrations_branding(self, request: operations.GetIntegrationsBrandingRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetIntegrationsBrandingResponse:
         r"""Get branding
         Get branding for platform.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetIntegrationsBrandingRequest, base_url, '/integrations/{platformKey}/branding', request)
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetIntegrationsBrandingResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Branding])
                 res.branding = out
 
         return res
 
-    def list_integrations(self, request: operations.ListIntegrationsRequest) -> operations.ListIntegrationsResponse:
+    def list_integrations(self, request: operations.ListIntegrationsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListIntegrationsResponse:
         r"""List integrations
         List your available integrations
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/integrations'
         
         query_params = utils.get_query_params(operations.ListIntegrationsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListIntegrationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Integrations])
```

### Comparing `codat-common-0.6.5/src/codat/models/operations/__init__.py` & `codat-common-0.8.1/src/codatcommon/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/create_company.py` & `codat-common-0.8.1/src/codatcommon/models/operations/create_company.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/create_data_connection.py` & `codat-common-0.8.1/src/codatcommon/models/operations/create_data_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connection as shared_connection
 from ..shared import errormessage as shared_errormessage
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateDataConnectionRequestBody:
```

### Comparing `codat-common-0.6.5/src/codat/models/operations/create_pull_operation.py` & `codat-common-0.8.1/src/codatcommon/models/operations/create_pull_operation.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/create_rule.py` & `codat-common-0.8.1/src/codatcommon/models/operations/create_rule.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/delete_company.py` & `codat-common-0.8.1/src/codatcommon/models/operations/delete_company.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/delete_company_connection.py` & `codat-common-0.8.1/src/codatcommon/models/operations/delete_company_connection.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_company.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_company.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_company_connection.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_company_connection.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_company_data_history.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_company_data_history.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_company_data_status.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_company_data_status.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_company_push_history.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_company_push_history.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_create_update_model_options_by_data_type.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_create_update_model_options_by_data_type.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_integration.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_integration.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_integrations_branding.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_integrations_branding.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_profile.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_profile.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_profile_syncsettings.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_profile_syncsettings.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_pull_operation.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_pull_operation.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_push_operation.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_push_operation.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/get_webhook.py` & `codat-common-0.8.1/src/codatcommon/models/operations/get_webhook.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/list_companies.py` & `codat-common-0.8.1/src/codatcommon/models/operations/list_companies.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/list_company_connections.py` & `codat-common-0.8.1/src/codatcommon/models/operations/list_company_connections.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/list_integrations.py` & `codat-common-0.8.1/src/codatcommon/models/operations/list_integrations.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/list_rules.py` & `codat-common-0.8.1/src/codatcommon/models/operations/list_rules.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/refresh_company_data.py` & `codat-common-0.8.1/src/codatcommon/models/operations/refresh_company_data.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/unlink_company_connection.py` & `codat-common-0.8.1/src/codatcommon/models/operations/unlink_company_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connection as shared_connection
 from ..shared import errormessage as shared_errormessage
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UnlinkCompanyConnectionRequestBody:
```

### Comparing `codat-common-0.6.5/src/codat/models/operations/update_company.py` & `codat-common-0.8.1/src/codatcommon/models/operations/update_company.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/update_connection_authorization.py` & `codat-common-0.8.1/src/codatcommon/models/operations/update_connection_authorization.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/update_profile.py` & `codat-common-0.8.1/src/codatcommon/models/operations/update_profile.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/operations/update_sync_settings.py` & `codat-common-0.8.1/src/codatcommon/models/operations/update_sync_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errormessage as shared_errormessage
 from ..shared import syncsetting as shared_syncsetting
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UpdateSyncSettingsRequestBody:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/__init__.py` & `codat-common-0.8.1/src/codatcommon/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/shared/branding.py` & `codat-common-0.8.1/src/codatcommon/models/shared/branding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import brandingbutton as shared_brandingbutton
 from ..shared import brandinglogo as shared_brandinglogo
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Branding:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/brandingbutton.py` & `codat-common-0.8.1/src/codatcommon/models/shared/brandingbutton.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import brandingimage as shared_brandingimage
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingButton:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/brandingimage.py` & `codat-common-0.8.1/src/codatcommon/models/shared/brandingimage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import imagereference as shared_imagereference
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingImage:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/brandinglogo.py` & `codat-common-0.8.1/src/codatcommon/models/shared/brandinglogo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import brandingimage as shared_brandingimage
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingLogo:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/companies.py` & `codat-common-0.8.1/src/codatcommon/models/shared/companies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import company as shared_company
 from ..shared import links as shared_links
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Companies:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/company.py` & `codat-common-0.8.1/src/codatcommon/models/shared/company.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import connection as shared_connection
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Company:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/companydataconnectionstatuschangedwebhook.py` & `codat-common-0.8.1/src/codatcommon/models/shared/companydataconnectionstatuschangedwebhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import connectionstatus_enum as shared_connectionstatus_enum
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompanyDataConnectionStatusChangedWebhookData:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/companyrequestbody.py` & `codat-common-0.8.1/src/codatcommon/models/shared/companyrequestbody.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompanyRequestBody:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/connection.py` & `codat-common-0.8.1/src/codatcommon/models/shared/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import dataconnectionerror as shared_dataconnectionerror
 from ..shared import dataconnectionstatus_enum as shared_dataconnectionstatus_enum
 from ..shared import sourcetype_enum as shared_sourcetype_enum
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Connection:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/connections.py` & `codat-common-0.8.1/src/codatcommon/models/shared/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import connection as shared_connection
 from ..shared import links as shared_links
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Connections:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/dataconnectionerror.py` & `codat-common-0.8.1/src/codatcommon/models/shared/dataconnectionerror.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataConnectionError:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/dataconnectionhistory.py` & `codat-common-0.8.1/src/codatcommon/models/shared/dataconnectionhistory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import links as shared_links
 from ..shared import pulloperation as shared_pulloperation
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataConnectionHistory:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/datasetdatachangedwebhook.py` & `codat-common-0.8.1/src/codatcommon/models/shared/datasetdatachangedwebhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DatasetDataChangedWebhookData:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/datasetstatuschangederrorwebhook.py` & `codat-common-0.8.1/src/codatcommon/models/shared/datasetstatuschangederrorwebhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DatasetStatusChangedErrorWebhookData:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/datastatus.py` & `codat-common-0.8.1/src/codatcommon/models/shared/datastatus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataStatus:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/datasynccompletedwebhook.py` & `codat-common-0.8.1/src/codatcommon/models/shared/datasynccompletedwebhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataSyncCompletedWebhookData:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/datatype_enum.py` & `codat-common-0.8.1/src/codatcommon/models/shared/datatype_enum.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/models/shared/datatypefeature.py` & `codat-common-0.8.1/src/codatcommon/models/shared/datatypefeature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import datatype_enum as shared_datatype_enum
 from ..shared import supportedfeature as shared_supportedfeature
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataTypeFeature:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/errormessage.py` & `codat-common-0.8.1/src/codatcommon/models/shared/errormessage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ErrorMessage:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/imagereference.py` & `codat-common-0.8.1/src/codatcommon/models/shared/imagereference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ImageReference:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/integration.py` & `codat-common-0.8.1/src/codatcommon/models/shared/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import datatypefeature as shared_datatypefeature
 from ..shared import sourcetype_enum as shared_sourcetype_enum
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Integration:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/integrations.py` & `codat-common-0.8.1/src/codatcommon/models/shared/integrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import integration as shared_integration
 from ..shared import links as shared_links
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Integrations:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/links.py` & `codat-common-0.8.1/src/codatcommon/models/shared/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import href as shared_href
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Links:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/newcompanysynchronizedwebhook.py` & `codat-common-0.8.1/src/codatcommon/models/shared/newcompanysynchronizedwebhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class NewCompanySynchronizedWebhook:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/profile.py` & `codat-common-0.8.1/src/codatcommon/models/shared/profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Profile:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pulloperation.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pulloperation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
 class PullOperationStatusEnum(str, Enum):
     INITIAL = 'Initial'
     QUEUED = 'Queued'
     FETCHING = 'Fetching'
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushfieldvalidation.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushfieldvalidation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushFieldValidation:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushhistoryresponse.py` & `codat-common-0.8.1/src/codatcommon/models/shared/rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import links as shared_links
-from ..shared import pushoperationsummary as shared_pushoperationsummary
-from codat import utils
+from ..shared import rule as shared_rule
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PushHistoryResponse:
+class Rules:
     r"""OK"""
     
     links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
     page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
     total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
-    results: Optional[list[shared_pushoperationsummary.PushOperationSummary]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})  
+    results: Optional[list[shared_rule.Rule]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoperation.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoperation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from ..shared import datatype_enum as shared_datatype_enum
 from ..shared import pushoperationchange as shared_pushoperationchange
 from ..shared import pushoperationstatus_enum as shared_pushoperationstatus_enum
 from ..shared import validation as shared_validation
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOperation:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoperationchange.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoperationchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import pushchangetype_enum as shared_pushchangetype_enum
 from ..shared import pushoperationref as shared_pushoperationref
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOperationChange:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoperationref.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoperationref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import datatype_enum as shared_datatype_enum
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOperationRef:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoperationstatuschangedwebhook.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoperationstatuschangedwebhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOperationStatusChangedWebhookData:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoperationsummary.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoperationsummary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from ..shared import datatype_enum as shared_datatype_enum
 from ..shared import pushoperationchange as shared_pushoperationchange
 from ..shared import pushoperationstatus_enum as shared_pushoperationstatus_enum
 from ..shared import validation as shared_validation
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOperationSummary:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoperationtimedoutwebhook.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoperationtimedoutwebhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOperationTimedOutWebhookData:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoption.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoption.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from ..shared import pushoptionchoice as shared_pushoptionchoice
 from ..shared import pushoptionproperty as shared_pushoptionproperty
 from ..shared import pushoptiontype_enum as shared_pushoptiontype_enum
 from ..shared import pushvalidationinfo as shared_pushvalidationinfo
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOption:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoptionchoice.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoptionchoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import pushoptiontype_enum as shared_pushoptiontype_enum
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOptionChoice:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushoptionproperty.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushoptionproperty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import pushoptionchoice as shared_pushoptionchoice
 from ..shared import pushoptiontype_enum as shared_pushoptiontype_enum
 from ..shared import pushvalidationinfo as shared_pushvalidationinfo
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushOptionProperty:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/pushvalidationinfo.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushvalidationinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import pushfieldvalidation as shared_pushfieldvalidation
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PushValidationInfo:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/rule.py` & `codat-common-0.8.1/src/codatcommon/models/shared/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class RuleNotifiers:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/rules.py` & `codat-common-0.8.1/src/codatcommon/models/shared/pushhistoryresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import links as shared_links
-from ..shared import rule as shared_rule
-from codat import utils
+from ..shared import pushoperationsummary as shared_pushoperationsummary
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Rules:
+class PushHistoryResponse:
     r"""OK"""
     
     links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
     page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
     total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
-    results: Optional[list[shared_rule.Rule]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})  
+    results: Optional[list[shared_pushoperationsummary.PushOperationSummary]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/supportedfeature.py` & `codat-common-0.8.1/src/codatcommon/models/shared/supportedfeature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import featurestate_enum as shared_featurestate_enum
 from ..shared import featuretype_enum as shared_featuretype_enum
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SupportedFeature:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/syncsetting.py` & `codat-common-0.8.1/src/codatcommon/models/shared/syncsetting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
 class SyncSettingDataTypeEnum(str, Enum):
     r"""Available Data types"""
     ACCOUNT_TRANSACTIONS = 'accountTransactions'
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/syncsettings.py` & `codat-common-0.8.1/src/codatcommon/models/shared/validationitem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import syncsetting as shared_syncsetting
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SyncSettings:
-    r"""OK"""
+class ValidationItem:
     
-    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clientId'), 'exclude': lambda f: f is None }})  
-    overrides_defaults: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overridesDefaults'), 'exclude': lambda f: f is None }})  
-    settings: Optional[list[shared_syncsetting.SyncSetting]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('settings'), 'exclude': lambda f: f is None }})  
+    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})  
+    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})  
+    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/validation.py` & `codat-common-0.8.1/src/codatcommon/models/shared/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import validationitem as shared_validationitem
-from codat import utils
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Validation:
```

### Comparing `codat-common-0.6.5/src/codat/models/shared/validationitem.py` & `codat-common-0.8.1/src/codatcommon/models/shared/syncsettings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from codat import utils
+from ..shared import syncsetting as shared_syncsetting
+from codatcommon import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ValidationItem:
+class SyncSettings:
+    r"""OK"""
     
-    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})  
-    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})  
-    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})  
+    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clientId'), 'exclude': lambda f: f is None }})  
+    overrides_defaults: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overridesDefaults'), 'exclude': lambda f: f is None }})  
+    settings: Optional[list[shared_syncsetting.SyncSetting]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('settings'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-common-0.6.5/src/codat/models/webhooks/__init__.py` & `codat-common-0.8.1/src/codatcommon/models/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/sdk.py` & `codat-common-0.8.1/src/codatcommon/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from .connections import Connections
 from .data_status import DataStatus
 from .integrations import Integrations
 from .push_data import PushData
 from .refresh_data import RefreshData
 from .settings import Settings
 from .webhooks import Webhooks
-from codat.models import shared
+from codatcommon.models import shared
 
 SERVERS = [
     "https://api.codat.io",
     r"""Production"""
 ]
 """Contains the list of servers available to the SDK"""
 
-class Codat:
+class CodatCommon:
     r"""Common API
     An API for the common components of all of Codat's products.
     
     These end points cover creating and managing your companies, data connections, and integrations.
     
     [Read about the building blocks of Codat...](https://docs.codat.io/core-concepts/companies)
     
@@ -45,16 +45,16 @@
     webhooks: Webhooks
     r"""Manage webhooks, rules and alerts."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.6.5"
-    _gen_version: str = "2.16.7"
+    _sdk_version: str = "0.8.1"
+    _gen_version: str = "2.18.1"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-common-0.6.5/src/codat/settings.py` & `codat-common-0.8.1/src/codatcommon/webhooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations, shared
+from codatcommon.models import operations, shared
 from typing import Optional
 
-class Settings:
-    r"""Manage your Codat instance."""
+class Webhooks:
+    r"""Manage webhooks, rules and alerts."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,122 +18,133 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_profile(self) -> operations.GetProfileResponse:
-        r"""Get profile
-        Fetch your Codat profile.
+    def create_rule(self, request: shared.Rule, retries: Optional[utils.RetryConfig] = None) -> operations.CreateRuleResponse:
+        r"""Create webhook
+        Create a new webhook configuration
         """
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/profile'
+        url = base_url.removesuffix('/') + '/rules'
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetProfileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateRuleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Profile])
-                res.profile = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Rule])
+                res.rule = out
         elif http_res.status_code == 401:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def get_profile_sync_settings(self) -> operations.GetProfileSyncSettingsResponse:
-        r"""Get sync settings
-        Retrieve the sync settings for your client. This includes how often data types should be queued to be updated, and how much history should be fetched.
+    def get_webhook(self, request: operations.GetWebhookRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetWebhookResponse:
+        r"""Get webhook
+        Get a single webhook
         """
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/profile/syncSettings'
+        url = utils.generate_url(operations.GetWebhookRequest, base_url, '/rules/{ruleId}', request)
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetProfileSyncSettingsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.SyncSettings])
-                res.sync_settings = out
-        elif http_res.status_code == 401:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Rule])
+                res.rule = out
+        elif http_res.status_code in [401, 404]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
 
-    def update_profile(self, request: shared.Profile) -> operations.UpdateProfileResponse:
-        r"""Update profile
-        Update your Codat profile
+    def list_rules(self, request: operations.ListRulesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListRulesResponse:
+        r"""List webhooks
+        List webhooks that you are subscribed to.
         """
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/profile'
+        url = base_url.removesuffix('/') + '/rules'
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        query_params = utils.get_query_params(operations.ListRulesRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('PUT', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '408',
+            '429',
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.UpdateProfileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListRulesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Profile])
-                res.profile = out
-        elif http_res.status_code == 401:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
-                res.error_message = out
-
-        return res
-
-    def update_sync_settings(self, request: operations.UpdateSyncSettingsRequestBody) -> operations.UpdateSyncSettingsResponse:
-        r"""Update all sync settings
-        Update sync settings for all data types.
-        """
-        base_url = self._server_url
-        
-        url = base_url.removesuffix('/') + '/profile/syncSettings'
-        
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        
-        client = self._security_client
-        
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.UpdateSyncSettingsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 204:
-            pass
-        elif http_res.status_code == 401:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Rules])
+                res.rules = out
+        elif http_res.status_code in [400, 401]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ErrorMessage])
                 res.error_message = out
 
         return res
```

### Comparing `codat-common-0.6.5/src/codat/utils/retries.py` & `codat-common-0.8.1/src/codatcommon/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-common-0.6.5/src/codat/utils/utils.py` & `codat-common-0.8.1/src/codatcommon/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,70 +148,79 @@
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
 
-        if param_metadata.get('style', 'simple') == 'simple':
-            param = getattr(
-                path_params, field.name) if path_params is not None else None
-            param = _populate_from_globals(
-                field.name, param, 'pathParam', gbls)
-
-            if param is None:
-                continue
-
-            if isinstance(param, list):
-                pp_vals: list[str] = []
-                for pp_val in param:
-                    if pp_val is None:
-                        continue
-                    pp_vals.append(_val_to_string(pp_val))
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif isinstance(param, dict):
-                pp_vals: list[str] = []
-                for pp_key in param:
-                    if param[pp_key] is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{pp_key}={_val_to_string(param[pp_key])}")
-                    else:
-                        pp_vals.append(
-                            f"{pp_key},{_val_to_string(param[pp_key])}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif not isinstance(param, (str, int, float, complex, bool)):
-                pp_vals: list[str] = []
-                param_fields: Tuple[Field, ...] = fields(param)
-                for param_field in param_fields:
-                    param_value_metadata = param_field.metadata.get(
-                        'path_param')
-                    if not param_value_metadata:
-                        continue
-
-                    parm_name = param_value_metadata.get(
-                        'field_name', field.name)
-
-                    param_field_val = getattr(param, param_field.name)
-                    if param_field_val is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{parm_name}={_val_to_string(param_field_val)}")
-                    else:
-                        pp_vals.append(
-                            f"{parm_name},{_val_to_string(param_field_val)}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            else:
+        param = getattr(
+            path_params, field.name) if path_params is not None else None
+        param = _populate_from_globals(
+            field.name, param, 'pathParam', gbls)
+
+        if param is None:
+            continue
+
+        f_name = param_metadata.get("field_name", field.name)
+        serialization = param_metadata.get('serialization', '')
+        if serialization != '':
+            serialized_params = _get_serialized_params(
+                param_metadata, f_name, param)
+            for key, value in serialized_params.items():
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + key + '}', value, 1)
+        else:
+            if param_metadata.get('style', 'simple') == 'simple':
+                if isinstance(param, list):
+                    pp_vals: list[str] = []
+                    for pp_val in param:
+                        if pp_val is None:
+                            continue
+                        pp_vals.append(_val_to_string(pp_val))
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif isinstance(param, dict):
+                    pp_vals: list[str] = []
+                    for pp_key in param:
+                        if param[pp_key] is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        else:
+                            pp_vals.append(
+                                f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif not isinstance(param, (str, int, float, complex, bool)):
+                    pp_vals: list[str] = []
+                    param_fields: Tuple[Field, ...] = fields(param)
+                    for param_field in param_fields:
+                        param_value_metadata = param_field.metadata.get(
+                            'path_param')
+                        if not param_value_metadata:
+                            continue
+
+                        parm_name = param_value_metadata.get(
+                            'field_name', field.name)
+
+                        param_field_val = getattr(param, param_field.name)
+                        if param_field_val is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{parm_name}={_val_to_string(param_field_val)}")
+                        else:
+                            pp_vals.append(
+                                f"{parm_name},{_val_to_string(param_field_val)}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                else:
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -242,16 +251,20 @@
             query_params, param_name) if query_params is not None else None
 
         value = _populate_from_globals(param_name, value, 'queryParam', gbls)
 
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            params = params | _get_serialized_query_params(
-                metadata, f_name, value)
+            serialized_parms = _get_serialized_params(metadata, f_name, value)
+            for key, value in serialized_parms.items():
+                if key in params:
+                    params[key].extend(value)
+                else:
+                    params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
                 params = params | _get_form_query_params(
@@ -278,16 +291,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    params: dict[str, list[str]] = {}
+def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
+    params: dict[str, str] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
```

### Comparing `codat-common-0.6.5/src/codat_common.egg-info/PKG-INFO` & `codat-common-0.8.1/src/codat_common.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-common
-Version: 0.6.5
+Version: 0.8.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -18,27 +18,27 @@
 pip install codat-common
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
-import codat
-from codat.models import operations, shared
+import codatcommon
+from codatcommon.models import operations, shared
 
-s = codat.Codat(
+s = codatcommon.CodatCommon(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = shared.CompanyRequestBody(
     description="corrupti",
-    name="provident",
+    name="Kelvin Sporer",
 )
     
 res = s.companies.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
```

