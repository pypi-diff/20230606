# Comparing `tmp/perseus_restful_api_framework-1.26.8.tar.gz` & `tmp/perseus_restful_api_framework-1.26.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perseus_restful_api_framework-1.26.8.tar", max compression
+gzip compressed data, was "perseus_restful_api_framework-1.26.9.tar", max compression
```

## Comparing `perseus_restful_api_framework-1.26.8.tar` & `perseus_restful_api_framework-1.26.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0     9192 2023-03-09 11:04:14.646040 perseus_restful_api_framework-1.26.8/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.26.8/LICENSE
--rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.26.8/README.md
--rw-r--r--   0        0        0     1140 2023-03-09 11:04:32.345435 perseus_restful_api_framework-1.26.8/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.26.8/src/majormode/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.26.8/src/majormode/perseus/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.26.8/src/majormode/perseus/agent/__init__.py
--rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.26.8/src/majormode/perseus/agent/email_address_verification_agent.py
--rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.26.8/src/majormode/perseus/agent/email_sender_agent.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.26.8/src/majormode/perseus/bootstrap/__init__.py
--rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.26.8/src/majormode/perseus/bootstrap/tornado_handler.py
--rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_currency_dataset.sql
--rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_exception_function.sql
--rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_geometry_function.sql
--rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_label_type.sql
--rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_locale_function.sql
--rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_object_constant.sql
--rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_object_table.sql
--rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_visibility_constant.sql
--rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.26.8/src/majormode/perseus/manage.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/__init__.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/__init__.py
--rwxr-xr-x   0        0        0   155440 2023-03-09 11:02:47.482326 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/account_service.py
--rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/contact_service.py
--rwxr-xr-x   0        0        0     3551 2023-03-03 01:25:29.385031 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_constraint.sql
--rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_function.sql
--rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_index.sql
--rwxr-xr-x   0        0        0    19483 2023-02-15 11:46:09.587868 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_table.sql
--rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_constraint.sql
--rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_function.sql
--rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_index.sql
--rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_table.sql
--rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
--rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
--rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
--rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
--rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
--rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
--rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
--rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
--rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
--rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
--rw-r--r--   0        0        0     2739 2023-03-03 01:36:14.949292 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
--rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/oauth_service.py
--rwxr-xr-x   0        0        0    15044 2023-02-09 01:22:31.540928 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/session_service.py
--rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
--rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/test/__init__.py
--rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/test/account_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/__init__.py
--rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/application_service.py
--rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/db/create_application_constraint.sql
--rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/db/create_application_index.sql
--rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/db/create_application_table.sql
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/test/__init__.py
--rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/test/application_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/__init__.py
--rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/area_service.py
--rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/data/vietnam/area2sql.py
--rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
--rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
--rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_constraint.sql
--rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_dataset.sql
--rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_function.sql
--rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_index.sql
--rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_table.sql
--rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_type.sql
--rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
--rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_geoip_index.sql
--rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_geoip_table.sql
--rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
--rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
--rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_rir_table.sql
--rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
--rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/script/_geolite_importer.py
--rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/script/_rir_importer.py
--rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/script/geoip2sql.py
--rw-r--r--   0        0        0    64863 2023-01-30 02:07:47.788329 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_http_handler.py
--rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_job_service.py
--rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_rdbms_service.py
--rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_service.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/__init__.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/agent/__init__.py
--rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/agent/push_notification.py
--rw-r--r--   0        0        0      899 2022-11-23 10:31:53.449426 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
--rw-r--r--   0        0        0     1167 2022-11-23 10:31:53.449636 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/db/create_notification_index.sql
--rw-r--r--   0        0        0    10511 2022-11-23 10:31:53.449859 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/db/create_notification_table.sql
--rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/gcm.py
--rw-r--r--   0        0        0    65115 2023-02-09 01:22:31.540956 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/notification_service.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/__init__.py
--rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/doc/api/get_ping.rst
--rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/doc/api/get_status.rst
--rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/doc/api/index.rst
--rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/status_service.py
--rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/status_service_http_handler.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/__init__.py
--rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/agent/team_invite.py
--rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_constraint.sql
--rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_function.sql
--rw-r--r--   0        0        0      907 2022-11-23 10:31:53.453841 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_index.sql
--rw-r--r--   0        0        0     9062 2022-11-23 10:31:53.454053 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_table.sql
--rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/migrate_20190501.sql
--rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
--rwxr-xr-x   0        0        0   121781 2023-02-09 01:23:15.435624 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/team_service.py
--rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/template/default_invite_email.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/test/__init__.py
--rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/test/team_service_unittest.py
--rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/__init__.py
--rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/doc/api/get_version.rst
--rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/doc/api/index.rst
--rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/test/__init__.py
--rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/test/version_service_unittest.py
--rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/version_service.py
--rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/version_service_http_handler.py
--rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.26.8/setup.py
--rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.26.8/PKG-INFO
+-rw-r--r--   0        0        0     9313 2023-05-23 03:25:01.596563 perseus_restful_api_framework-1.26.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.26.9/LICENSE
+-rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.26.9/README.md
+-rw-r--r--   0        0        0     1140 2023-05-23 03:29:53.383254 perseus_restful_api_framework-1.26.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.26.9/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.26.9/src/majormode/perseus/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/__init__.py
+-rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_address_verification_agent.py
+-rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_sender_agent.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/__init__.py
+-rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/tornado_handler.py
+-rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_currency_dataset.sql
+-rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_exception_function.sql
+-rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_geometry_function.sql
+-rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_label_type.sql
+-rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_locale_function.sql
+-rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_constant.sql
+-rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_table.sql
+-rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_visibility_constant.sql
+-rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.26.9/src/majormode/perseus/manage.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/__init__.py
+-rwxr-xr-x   0        0        0   155565 2023-05-23 03:24:04.575726 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/account_service.py
+-rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/contact_service.py
+-rwxr-xr-x   0        0        0     3551 2023-03-03 01:25:29.385031 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_constraint.sql
+-rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_function.sql
+-rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_index.sql
+-rwxr-xr-x   0        0        0    19425 2023-05-19 10:16:08.747757 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_table.sql
+-rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_constraint.sql
+-rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_function.sql
+-rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_index.sql
+-rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_table.sql
+-rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
+-rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
+-rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
+-rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
+-rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
+-rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
+-rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
+-rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
+-rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
+-rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
+-rw-r--r--   0        0        0     3165 2023-03-10 00:12:11.857881 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
+-rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/oauth_service.py
+-rwxr-xr-x   0        0        0    15044 2023-02-09 01:22:31.540928 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/session_service.py
+-rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
+-rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/__init__.py
+-rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/account_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/__init__.py
+-rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/application_service.py
+-rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_constraint.sql
+-rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_index.sql
+-rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_table.sql
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/__init__.py
+-rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/application_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/__init__.py
+-rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/area_service.py
+-rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area2sql.py
+-rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
+-rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
+-rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_constraint.sql
+-rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_dataset.sql
+-rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_function.sql
+-rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_index.sql
+-rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_table.sql
+-rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_type.sql
+-rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
+-rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_index.sql
+-rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_table.sql
+-rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
+-rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
+-rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_rir_table.sql
+-rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
+-rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_geolite_importer.py
+-rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_rir_importer.py
+-rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/geoip2sql.py
+-rw-r--r--   0        0        0    64863 2023-01-30 02:07:47.788329 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_http_handler.py
+-rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_job_service.py
+-rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_rdbms_service.py
+-rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_service.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/__init__.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/__init__.py
+-rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/push_notification.py
+-rw-r--r--   0        0        0      899 2022-11-23 10:31:53.449426 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
+-rw-r--r--   0        0        0     1167 2022-11-23 10:31:53.449636 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_index.sql
+-rw-r--r--   0        0        0    10511 2022-11-23 10:31:53.449859 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_table.sql
+-rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/gcm.py
+-rw-r--r--   0        0        0    65115 2023-02-09 01:22:31.540956 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/notification_service.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/__init__.py
+-rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_ping.rst
+-rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_status.rst
+-rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/index.rst
+-rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service.py
+-rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service_http_handler.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/__init__.py
+-rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/agent/team_invite.py
+-rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_constraint.sql
+-rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_function.sql
+-rw-r--r--   0        0        0      968 2023-05-19 09:03:02.094015 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_index.sql
+-rw-r--r--   0        0        0     9034 2023-05-19 09:32:28.819485 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_table.sql
+-rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/migrate_20190501.sql
+-rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
+-rwxr-xr-x   0        0        0   121781 2023-02-09 01:23:15.435624 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/team_service.py
+-rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/template/default_invite_email.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/__init__.py
+-rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/team_service_unittest.py
+-rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/__init__.py
+-rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/get_version.rst
+-rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/index.rst
+-rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/__init__.py
+-rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/version_service_unittest.py
+-rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service.py
+-rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service_http_handler.py
+-rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.26.9/setup.py
+-rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.26.9/PKG-INFO
```

### Comparing `perseus_restful_api_framework-1.26.8/CHANGELOG.md` & `perseus_restful_api_framework-1.26.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [1.26.9] - 2023-05-23
+# Changed
+- The method Account Service's `sign_up` allows passing a single contact information
+
 ## [1.26.8] - 2023-03-08
 # Changed
 - Remove the column `picture_time` from the table `account`
 
 ## [1.26.7] - 2023-02-15
 # Fixed
 - An issue that occurs when searching a picture that doesn't exist
```

### Comparing `perseus_restful_api_framework-1.26.8/LICENSE` & `perseus_restful_api_framework-1.26.9/LICENSE`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/README.md` & `perseus_restful_api_framework-1.26.9/README.md`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/pyproject.toml` & `perseus_restful_api_framework-1.26.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["perseus", "resful", "api", "server", "framework"]
 license = "Proprietary"
 name = "perseus-restful-api-framework"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/perseus-restful-api-server-framework"
-version = "1.26.8"
+version = "1.26.9"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psutil = "^5.9.4"
 tornado = "^6.2"
 perseus-core-library = "^1.18.24"
 pillow = "^9.4.0"
```

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/agent/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/agent/email_address_verification_agent.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_address_verification_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/agent/email_sender_agent.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_sender_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/bootstrap/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/bootstrap/tornado_handler.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/tornado_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_currency_dataset.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_currency_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_exception_function.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_exception_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_geometry_function.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_geometry_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_label_type.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_label_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_locale_function.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_locale_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_object_constant.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_object_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/db/create_visibility_constant.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_visibility_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/manage.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/manage.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/account_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/account_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,46 +165,46 @@
             team_id: uuid.UUID = None):
         """
         Add a new picture to a user account.
 
         The function stores the image file in the NFS storage.
 
 
-        @param app_id: The identification of the client application such as a
+        :param app_id: The identification of the client application such as a
             Web, a desktop, or a mobile application, that accesses the service.
 
-        @param account_id: The identification of the account of the user who
+        :param account_id: The identification of the account of the user who
             is associated to this picture.
 
-        @param submitter_account_id: The identification of the account of the
+        :param submitter_account_id: The identification of the account of the
             user who submitted this picture.
 
-        @param capture_time: The time when the photo was capture.  The
+        :param capture_time: The time when the photo was capture.  The
             function registers the current time if the provided capture time
             is in the future.
 
-        @param image: The image of the user's photo.
+        :param image: The image of the user's photo.
 
-        @param image_file_checksum: Message digest of the binary data of the
+        :param image_file_checksum: Message digest of the binary data of the
             user's original photo image file.
 
-        @param image_file_size: Size in bytes of the user's original photo
+        :param image_file_size: Size in bytes of the user's original photo
             image file.
 
-        @param connection: An object `RdbmsConnection` with auto-commit.
+        :param connection: An object `RdbmsConnection` with auto-commit.
 
-        @param is_review_required: Indicate whether the picture needs to be
+        :param is_review_required: Indicate whether the picture needs to be
             reviewed by someone who has authority on the online service used
             by the end users.
 
-        @param team_id: The identification of the organization of the user who
+        :param team_id: The identification of the organization of the user who
             submitted this picture.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id: uuid.UUID` (required): The identification of the account
               of the user this picture is associated with.
 
             - `picture_id: uuid.UUID` (required): The identification of the picture.
 
             - `object_status: ObjectStatus` (required): The current status of the
@@ -280,21 +280,21 @@
 
     @classmethod
     def __adjust_photo_capture_time(cls, capture_time):
         """
         Adjust the capture time of a photo when this time is not in the future.
 
 
-        @param capture_time: The time when a photo was captured.
+        :param capture_time: The time when a photo was captured.
 
 
-        @return: The adjusted capture time of the photo.
+        :return: The adjusted capture time of the photo.
 
 
-        @raise InvalidArgumentException: If the capture time is way in the
+        :raise InvalidArgumentException: If the capture time is way in the
             future.
         """
         if capture_time is None:
             return None
 
         current_time = ISO8601DateTime.now()
         if capture_time <= current_time:
@@ -313,18 +313,18 @@
     def __cleanse_keywords(keywords):
         """
         Remove any punctuation character from the specified list of keywords,
         remove any double or more space character and represent Unicode
         characters in ASCII.
 
 
-        @param keywords: a list of keywords strip out any punctuation characters.
+        :param keywords: a list of keywords strip out any punctuation characters.
 
 
-        @return: the set of keywords cleansed from any special Unicode
+        :return: the set of keywords cleansed from any special Unicode
             accentuated character, punctuation character, and double space
             character.
         """
         if not isinstance(keywords, (list, set, tuple)):
             keywords = [keywords]
 
         # Normalize the given keywords and split them into sub-keywords if
@@ -357,21 +357,21 @@
 
     @classmethod
     def __convert_uploaded_photo_file_to_image(cls, uploaded_file):
         """
         Convert an uploaded photo file to an image
 
 
-        @param uploaded_file: An object `HttpRequest.HttpRequestUploadedFile`.
+        :param uploaded_file: An object `HttpRequest.HttpRequestUploadedFile`.
 
 
-        @return: An object `PIL.Image`.
+        :return: An object `PIL.Image`.
 
 
-        @raise InvalidOperationException: If the uploaded file has not a
+        :raise InvalidOperationException: If the uploaded file has not a
             supported format.
         """
         # Retrieve the pixel resolution of the photo image, and check whether
         # it respects the minimal size required.  If not, ignore this photo.
         try:
             string_io_stream = io.BytesIO(uploaded_file.data)
             image = image_util.convert_image_to_rgb_mode(
@@ -385,53 +385,53 @@
 
     @classmethod
     def __encrypt_password(cls, password):
         """
         Return the encrypted version of a password.
 
 
-        @param password: A password.
+        :param password: A password.
 
 
-        @return: The encrypted password.
+        :return: The encrypted password.
         """
         password = password.strip()
         encrypted_password = hashlib.md5(password.encode()).hexdigest()
         return encrypted_password
 
     @staticmethod
     def __generate_nonce(digit_count):
         """
         Generate a string composed of the requested number of digits
 
 
-        @param digit_count: Number of digit to generate.
+        :param digit_count: Number of digit to generate.
 
 
-        @return: A string composed of the request number of digits.
+        :return: A string composed of the request number of digits.
         """
         return ''.join([
             str(random.randint(0, 9))
             for _ in range(digit_count)
         ])
 
     @classmethod
     def __generate_password(cls, length=8, are_symbols_allowed=False):
         """
         Generate a password
 
 
-        @param length: Number of characters that composes the password to be
+        :param length: Number of characters that composes the password to be
             generated.
 
-        @param are_symbols_allowed: Indicate whether the password can
+        :param are_symbols_allowed: Indicate whether the password can
             contain punctuation characters.
 
 
-        @return: A string representing a password randomly generated.
+        :return: A string representing a password randomly generated.
         """
         alphabet = string.ascii_letters + string.digits
         if are_symbols_allowed:
             alphabet += cls.PASSWORD_ALLOWED_SPECIAL_CHARACTERS_LIST
 
         password = ''.join(secrets.choice(alphabet) for _ in range(length))
         return password
@@ -444,40 +444,40 @@
             contact=None,
             nonce=None,
             request_id=None):
         """
         Return extended information about a password reset request
 
 
-        @param app_id: Identification of the client application such as a Web,
+        :param app_id: Identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param check_app: indicate whether the function must check if the
+        :param check_app: indicate whether the function must check if the
             client application on behalf of which the function is called is
             the same than the client application that requested the password
             reset of the user's account.
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...`.
 
-        @param contact: An object `Contact` corresponding to an email address
+        :param contact: An object `Contact` corresponding to an email address
             or a mobile phone number where a random number (nonce) has been
             sent to for verifying the password reset request.  The argument
             `nonce` is also required.
 
-        @param nonce: "Number used once", a pseudo-random number issued when
+        :param nonce: "Number used once", a pseudo-random number issued when
             generating the request to allow the user to change his password
             through a mobile application.  The argument `account_id` is
             required.
 
-        @param request_id: Identification of the request of the user to reset
+        :param request_id: Identification of the request of the user to reset
              his forgotten password (cf. function `request_password_reset`).
 
 
-        @return: An instance containing the following members:
+        :return: An instance containing the following members:
 
             - `account_id` (required): identification of the user's account
               which the user has requested to reset his password.
 
             - `app_id` (required): identification of the client application that
               submitted on behalf of the user the request to reset the password
               of his account.
@@ -496,27 +496,27 @@
               request.
 
             - `update_time` (required): the most recent time when the platform
               sent an email to the user with an embedded link to let this user
               reset his password.
 
 
-        @raise `DeletedObjectException`: if the specified password reset
+        :raise `DeletedObjectException`: if the specified password reset
             request has been cancelled by the user or if this request has
             expired.
 
-        @raise `DisabledObjectException`: if the specified password reset
+        :raise `DisabledObjectException`: if the specified password reset
             request has been already used by the user to reset the password
             of his account.
 
-        @raise `IllegalAccessException`: if the client application or the
+        :raise `IllegalAccessException`: if the client application or the
             user account, on behalf of this function is called, is not allowed
             to retrieve the information of this password reset request.
 
-        @raise `UndefinedObjectException`: if the specified password reset
+        :raise `UndefinedObjectException`: if the specified password reset
             request has not been registered on the platform.
         """
         if contact is None and request_id is None:
             raise ValueError("A password reset request or a contact information MUST be passed")
 
         if contact and nonce is None:
             raise ValueError("A nonce MUST be passed")
@@ -607,19 +607,19 @@
             full_name,
             connection=None):
         """
         Index the account of a user with the personal name by which this user
         is known.
 
 
-        @param account_id: identification of the account of this child.
+        :param account_id: identification of the account of this child.
 
-        @param full_name: Personal name by which this user is known.
+        :param full_name: Personal name by which this user is known.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
         """
         keywords = self.__string_to_keywords(full_name)
 
         if keywords:
             with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
                 connection.execute(
                     """
@@ -676,39 +676,39 @@
             picture_id,
             status,
             connection=None):
         """
         Set the current status of a picture
 
 
-        @param picture_id: The identification of a picture.
+        :param picture_id: The identification of a picture.
 
-        @param status: An item of the enumeration `ObjectStatus`
+        :param status: An item of the enumeration `ObjectStatus`
             representing the new status of the picture.
 
-        @param connection: An object `RdbmsConnection` with auto-commit.
+        :param connection: An object `RdbmsConnection` with auto-commit.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id` (required): The identification of the account of the user
               this picture is associated with.
 
             - `picture_id` (required): The identification of the new picture.
 
             - `object_status` (required): An item of the enumeration `ObjectStatus`
               representing the current status of the picture.
 
             - `update_time` (required): The time of the most recent modification of
               the picture's status.
 
 
-        @raise DeletedObjectException: If the picture has been deleted.
+        :raise DeletedObjectException: If the picture has been deleted.
 
-        @raise UndefinedObjectException: If the picture doesn't not exist.
+        :raise UndefinedObjectException: If the picture doesn't not exist.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             picture = self.get_picture(picture_id, check_status=False, connection=connection)
             if picture.object_status == status:
                 return
             elif picture.object_status == ObjectStatus.deleted:
                 raise self.DeletedObjectException(f"The picture {picture_id} has been deleted")
@@ -808,21 +808,21 @@
             account_id,
             password,
             connection=None,
             include_contacts=False,
             session_duration=None):
         """
 
-        @param app_id:
-        @param account_id:
-        @param password:
-        @param connection:
-        @param include_contacts:
-        @param session_duration:
-        @return:
+        :param app_id:
+        :param account_id:
+        :param password:
+        :param connection:
+        :param include_contacts:
+        :param session_duration:
+        :return:
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             if not self.__is_password_correct(account_id, password, connection=connection):
                 raise self.AuthenticationFailureException()
 
             account = self.get_account(
                 account_id,
@@ -853,28 +853,28 @@
             image_quality: int = DEFAULT_IMAGE_QUALITY):
         """
         Store the image data of the avatar/photo of an account to the temporary
         directory of the local Network File System (NFS).  This file will be
         read by background tasks for additional processing.
 
 
-        @param picture_id: The identification of the photo of a user account.
+        :param picture_id: The identification of the photo of a user account.
 
-        @param image: An object `PIL.Image`.
+        :param image: An object `PIL.Image`.
 
-        @param image_file_format: Image file format to store the image with
+        :param image_file_format: Image file format to store the image with
             (cf. https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html).
 
-        @param image_quality: The image quality to store locally, on a scale from `1`
+        :param image_quality: The image quality to store locally, on a scale from `1`
             (worst) to `95` (best).  Values above `95` should be avoided; `100`
             disables portions of the JPEG compression algorithm, and results
             in large files with hardly any gain in image quality.
 
 
-        @return: The absolute file path name of the photo image stored in the
+        :return: The absolute file path name of the photo image stored in the
             local Network File System (NFS)
         """
         # Create the path of the folder to store the image file in.
         path = os.path.join(
             settings.CDN_NFS_ROOT_PATH,
             cls.CDN_BUCKET_NAME_PICTURE,
             file_util.build_tree_path_name(str(picture_id)))
@@ -903,21 +903,21 @@
     def __string_to_keywords(s, keyword_minimal_length=1):
         """
         Remove any punctuation character from the specified list of keywords,
         remove any double or more space character and represent Unicode
         characters in ASCII.
 
 
-        @param s: a list of keywords strip out any punctuation characters.
+        :param s: a list of keywords strip out any punctuation characters.
 
-        @param keyword_minimal_length: minimal number of characters of the
+        :param keyword_minimal_length: minimal number of characters of the
             keywords to be returned.
 
 
-        @return: the set of keywords cleansed from any special Unicode
+        :return: the set of keywords cleansed from any special Unicode
             accentuated character, punctuation character, and double space
             character.
         """
         if not s:
             return
 
         # Convert the string to ASCII lower characters.
@@ -936,17 +936,17 @@
         return [keyword for keyword in keywords if len(keyword) > keyword_minimal_length]
 
     def __update_last_login_time(self, account_id, connection=None):
         """
         Update the last login time of a user.
 
 
-        @param account_id: Identification of the user's account.
+        :param account_id: Identification of the user's account.
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...`.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             connection.execute(
                 """
                 UPDATE
                     account
@@ -961,39 +961,39 @@
 
     @classmethod
     def __validate_image_size(cls, image, minimal_size):
         """
         Validate the resolution of a new photo of an account
 
 
-        @param image: An object `PIL.Image`.
+        :param image: An object `PIL.Image`.
 
-        @param minimal_size: A tuple of two integers `(width, height)`
+        :param minimal_size: A tuple of two integers `(width, height)`
             representing the minimal size of the image of a photo.
 
 
-        @raise PictureSizeTooSmallException: If the photo is too small.
+        :raise PictureSizeTooSmallException: If the photo is too small.
         """
         image_width, image_height = image.size
         min_width, min_height = minimal_size
 
         if (image_width < min_width and image_height < min_height) or \
            (image_width < min_height and image_height < min_width):
             raise cls.PictureSizeTooSmallException(f"Image is too small: minimal size is {min_width}x{min_height}")
 
     @classmethod
     def __validate_password_complexity_requirements(cls, password):
         """
         Check whether a new password meets the complexity requirements.
 
 
-        @param password: A password.
+        :param password: A password.
 
 
-        @raise InvalidArgumentException: If the new password doesn't meet
+        :raise InvalidArgumentException: If the new password doesn't meet
             the complexity requirements {@link
             AccountService.REGEX_PASSWORD_COMPLEXITY_REQUIREMENTS}.
         """
         if not cls.REGEX_PASSWORD_COMPLEXITY_REQUIREMENTS.match(password):
             raise cls.InvalidArgumentException("The password doesn't meet complexity requirements")
 
     def assert_password_reset_request_nonce_valid(
@@ -1002,45 +1002,45 @@
             nonce=None,
             connection=None,
             request_id=None):
         """
         Check whether a password reset request exists and has not expired
 
 
-        @param contact: An object `Contact` representing a contact of the user
+        :param contact: An object `Contact` representing a contact of the user
             who is requesting to reset his forgotten password.
 
-        @param nonce: A nonce ("number used once") composed of digits that has
+        :param nonce: A nonce ("number used once") composed of digits that has
             been generated when the user requested to reset his password.
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...:`.
 
-        @param request_id: Identification of a password reset request.
+        :param request_id: Identification of a password reset request.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `expiration_time` (required): The time when this password reset
               request will expire.
 
             - `object_status` required): The current status of this password reset
               request.
 
 
-        @raise DisabledObjectException: If the password reset request has
+        :raise DisabledObjectException: If the password reset request has
             expired.
 
-        @raise IllegalAccessException: If the nonce or the password reset
+        :raise IllegalAccessException: If the nonce or the password reset
             request identification passed to the function is not valid.
 
-        @raise UndefinedObjectException: If the password reset request doesn't
+        :raise UndefinedObjectException: If the password reset request doesn't
             exist.  It may be an expired request that has been deleted.
 
-        @raise ValueError: If both the argument `nonce` and `request_id` have
+        :raise ValueError: If both the argument `nonce` and `request_id` have
             not been passed to this function.
         """
         if not nonce and not request_id:
             raise ValueError("A nonce or request identification MUST be passed")
 
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             cursor = connection.execute(
@@ -1111,18 +1111,18 @@
 
     @classmethod
     def build_picture_url(cls, picture_id):
         """
         Return the Uniform Resource Locator of an account's picture.
 
 
-        @param picture_id: Identification of the picture of an account.
+        :param picture_id: Identification of the picture of an account.
 
 
-        @return: A string representing the Uniform Resource Locator of the
+        :return: A string representing the Uniform Resource Locator of the
             picture.
         """
         return picture_id and os.path.join(
             settings.CDN_URL_HOSTNAME,
             cls.CDN_BUCKET_NAME_PICTURE,
             str(picture_id))
 
@@ -1137,42 +1137,42 @@
         Change the password of a user's account with a new password
 
         The new password must respect the rules of definition of a password.
         It cannot be identical to the old password.  It cannot contains part
         of the email address of the user.
 
 
-        @param app_id: identification of the client application such as a Web,
+        :param app_id: identification of the client application such as a Web,
            a desktop, or a mobile application, that accesses the service.
 
-        @param account_id: identification of the account of the user who is
+        :param account_id: identification of the account of the user who is
            changing his password.
 
-        @param old_password: old password of the user's account.
+        :param old_password: old password of the user's account.
 
-        @param new_password: new password of this user's account.
+        :param new_password: new password of this user's account.
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...`.
 
 
-        @raise DeletedObjectException: If the user's account has been deleted.
+        :raise DeletedObjectException: If the user's account has been deleted.
 
-        @raise DisabledObjectException: If the user's account has been
+        :raise DisabledObjectException: If the user's account has been
             disabled.
 
-        @raise IllegalAccessException: If the old password that is passed to
+        :raise IllegalAccessException: If the old password that is passed to
             the function doesn't match the current password of the user's
             account.
 
-        @raise InvalidArgumentException: If the new password doesn't conform
+        :raise InvalidArgumentException: If the new password doesn't conform
            to the rules of password definition, if the new  password is
            identical to the old password of the user.
 
-        @raise UndefinedObjectException: If the user's account doesn't exist.
+        :raise UndefinedObjectException: If the user's account doesn't exist.
         """
         # Encrypt both the old password and the new password passed to the
         # function.
         encrypted_old_password = self.__encrypt_password(old_password)
         self.__validate_password_complexity_requirements(new_password)
         encrypted_new_password = self.__encrypt_password(new_password)
 
@@ -1228,20 +1228,20 @@
             account_id,
             connection=None,
             hard_delete=False):
         """
         Delete the account of user
 
 
-        @param account_id: Identification of a user account.
+        :param account_id: Identification of a user account.
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...`.
 
-        @param hard_delete: Indicate whether to do a hard-delete of this
+        :param hard_delete: Indicate whether to do a hard-delete of this
             account, i.e, completely removing its record. By default, the
             function performs a soft-delete, marking this account has
             deleted.
         """
         with self.acquire_rdbms_connection(
                 auto_commit=True,
                 connection=connection) as connection:
@@ -1282,35 +1282,35 @@
             connection: RdbmsConnection = None,
             include_image_info: bool = False,
             include_sys_info: bool = False):
         """
         Return a picture corresponding to the specified file size and checksum.
 
 
-        @param image_file_size: The size in bytes of the user's original photo
+        :param image_file_size: The size in bytes of the user's original photo
             image file.
 
-        @param image_file_checksum: The message digest of the binary data of
+        :param image_file_checksum: The message digest of the binary data of
             the user's original photo image file.
 
-        @param check_status: Indicate whether to check the current status of
+        :param check_status: Indicate whether to check the current status of
             the picture.
 
-        @param connection: An existing connection to the user account database.
+        :param connection: An existing connection to the user account database.
 
-        @param include_image_info: Indicate whether to return information
+        :param include_image_info: Indicate whether to return information
             about the image itself, such as its resolution, its file size,
             etc.
 
-        @param include_sys_info: Indicate whether to return system information
+        :param include_sys_info: Indicate whether to return system information
             such as the identification of the client application that uploaded
             this picture, the time when the picture has been registered.
 
 
-        @return: `None` if no picture corresponds to the specified criteria;
+        :return: `None` if no picture corresponds to the specified criteria;
             otherwise, an object containing the following attributes:
 
             - `account_id` (required): The identification of the user account that
               the picture is associated with.
 
             - `image_height` (required): Number of pixel rows of the user's
               original photo image.
@@ -1373,33 +1373,33 @@
             check_status=False,
             connection=None,
             include_contacts=False):
         """
         Return extended information about a user account specified by its
         identification.
 
-        @warning: this function is for internal usage only; it MUST not be
+        :warning: this function is for internal usage only; it MUST not be
             surfaced to client applications.
 
 
-        @param account_id: identification of the user account that is
+        :param account_id: identification of the user account that is
             requested its information.
 
-        @param check_status: indicate whether the function must check the
+        :param check_status: indicate whether the function must check the
             current status of this user account and raise an exception if it
             is not of enabled.
 
-        @param include_contacts: indicate whether to include the contacts
+        :param include_contacts: indicate whether to include the contacts
             information of this user account.
 
-        @param connection: a `RdbmsConnection` instance to be used
+        :param connection: a `RdbmsConnection` instance to be used
             supporting the Python clause `with ...:`.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id: uuid.UUID` (required): The identification of the user
               account.
 
             - `account_type: AccountType` (required(: The type of the user account.
 
             - `contacts: list[Contact]` (optional): A list of contact information
@@ -1428,21 +1428,21 @@
             - `update_time: ISO8601DateTime` (required): The time of the most recent
               modification of one or more attributes of this user account.
 
             - `username: str`: The username of the user to gain access to the
               online service.
 
 
-        @raise DeletedObjectException: If the user account has been deleted
+        :raise DeletedObjectException: If the user account has been deleted
             while the argument `check_status` has been set to `True`.
 
-        @raise DisabledObjectException: If the user account has been disabled
+        :raise DisabledObjectException: If the user account has been disabled
             while the argument `check_status` has been set to `True`.
 
-        @raise UndefinedObjectException: If the specified identification
+        :raise UndefinedObjectException: If the specified identification
             doesn't refer to a user account registered to the platform.
         """
         with self.acquire_rdbms_connection(auto_commit=False, connection=connection) as connection:
             cursor = connection.execute(
                 """
                 SELECT
                     account_id,
@@ -1513,36 +1513,36 @@
         contact information, such as, for instance, an email address, a phone
         number.
 
 
         @note: The provided contact information MUST have been verified in
         order to return a user account.
 
-        @warning: This function is for internal usage only; it MUST not be
+        :warning: This function is for internal usage only; it MUST not be
             surfaced to client applications.
 
 
-        @param contact: An object `Contact`.
+        :param contact: An object `Contact`.
 
-        @param check_status: Indicate whether the function MUST check the
+        :param check_status: Indicate whether the function MUST check the
             current status of this user account and raise an exception if is
             not of enabled.
 
-        @param connection: Am object `RdbmsConnection` to be used supporting
+        :param connection: Am object `RdbmsConnection` to be used supporting
             the Python clause `with ...:`.
 
-        @param include_pending: indicate whether to include pending account
+        :param include_pending: indicate whether to include pending account
             or only enabled account.
 
-        @param is_verified: Indicate whether the function MUST only return a
+        :param is_verified: Indicate whether the function MUST only return a
             user account if the matching contact information has been
             verified.
 
 
-        @return: An object containing the following members:
+        :return: An object containing the following members:
 
             - `account_id`: Identification of the user account.
 
             - `full_name`: Full name of the user.
 
             - `username`: Name of the account of the user, if any defined.
 
@@ -1577,21 +1577,21 @@
               on behalf of whom this function is called is the owner of this
               account or connected with this user.
 
             - `update_time`: Time when the information of this user account has
               been updated for the last time.
 
 
-        @raise DeletedObjectException: If the user account has been deleted,
+        :raise DeletedObjectException: If the user account has been deleted,
             while the argument `check_status` has been set to `True`.
 
-        @raise DisabledObjectException: If the user account has been disabled,
+        :raise DisabledObjectException: If the user account has been disabled,
             while the argument `check_status` has been set to `True`.
 
-        @raise UndefinedObjectException: If the specified contact doesn't
+        :raise UndefinedObjectException: If the specified contact doesn't
             refer to a user account registered against the platform.
         """
         with self.acquire_rdbms_connection(auto_commit=False, connection=connection) as connection:
             cursor = connection.execute(
                 """
                 SELECT 
                     account.account_id,
@@ -1659,32 +1659,32 @@
         Return up to 100 users worth of extended information, specified by
         their identification.
 
         If a requested user is unknown, suspended, or deleted, then that user
         will not be returned in the results list.
 
 
-        @param account_ids: a list of account identifications or email
+        :param account_ids: a list of account identifications or email
                addresses.
 
-        @param connection: An object `RdbmsConnection`.
+        :param connection: An object `RdbmsConnection`.
 
-        @param include_contacts: indicate whether to include the contacts
+        :param include_contacts: indicate whether to include the contacts
             information of these user accounts.
 
-        @param include_hashed_password: Indicate whether to include the hashed
+        :param include_hashed_password: Indicate whether to include the hashed
             password of these accounts.  The called MUST ensure that this
             information will be secretly communicated to a client application
             owned by the organization to which these users belong to.
 
-        @param include_verified_only: Indicate whether to only return accounts
+        :param include_verified_only: Indicate whether to only return accounts
             whose given contact information has been verified.
 
 
-        @return: A list of objects containing the following members:
+        :return: A list of objects containing the following members:
 
                  - `account_id`: identification of the user account.
 
                  - `full_name`: full name of the user.
 
                  - `username`: name of the account of the user,
                    if any defined.
@@ -1702,19 +1702,19 @@
                  - `language`: a `Locale` instance that identifies the
                    preferred language of the user, or English by default.
 
                 - `update_time`: time when the information of this user
                   account has been updated for the last time.
 
 
-        @raise DeletedObjectException: if the user account has been deleted.
+        :raise DeletedObjectException: if the user account has been deleted.
 
-        @raise DisabledObjectException: if the user account has been disabled.
+        :raise DisabledObjectException: if the user account has been disabled.
 
-        @raise UndefinedObjectException: if the specified identification
+        :raise UndefinedObjectException: if the specified identification
                doesn't refer to a user account registered against the
                platform.
         """
         account_ids = set(account_ids)
         if not account_ids:
             return []
 
@@ -1839,15 +1839,15 @@
             verified_only=False,
             ignore_deleted=True):
         """
         Return a list of accounts that match the specified contact
         information.
 
 
-        @param contacts: a list of tuple `(name, value)` where:
+        :param contacts: a list of tuple `(name, value)` where:
 
                - `name`: name of a property, which can be one of a set of
                  pre-defined strings such as:
 
                  - `EMAIL`: e-mail address.
 
                  - `PHONE`: phone number in E.164 numbering plan, an ITU-T
@@ -1855,23 +1855,23 @@
                    telecommunication numbering plan used in the Public
                    Switched Telephone Network (PSTN).
 
               - `value`: value of the property representing by a string,
                 such as `+84.01272170781`, the formatted value for the
                 Telephone Number property.
 
-        @param verified_only: indicate whether the function must only return
+        :param verified_only: indicate whether the function must only return
                accounts that match contact information which has been
                verified.
 
-        @param ignore_deleted: indicate whether the function must ignore
+        :param ignore_deleted: indicate whether the function must ignore
                accounts that are deleted.
 
 
-        @return: a list of instances containing the following members:
+        :return: a list of instances containing the following members:
 
             - `account_id`: identification of the user account.
 
             - `full_name`: full name of the user.
 
             - `username`: name of the account of the user, if any defined.
 
@@ -1958,47 +1958,46 @@
             connection: RdbmsConnection = None,
             include_image_info: bool = False,
             include_sys_info: bool = False) -> any:
         """
         Return the information about a picture.
 
 
-        @param picture_id: The identification of a picture.
+        :param picture_id: The identification of a picture.
 
-        @param check_status: Indicate whether to check the current status of
+        :param check_status: Indicate whether to check the current status of
             the picture.
 
-        @param connection: An existing connection to the account database.
+        :param connection: An existing connection to the account database.
 
-        @param include_image_info: Indicate whether to return information
+        :param include_image_info: Indicate whether to return information
             about the image itself, such as its resolution, its file size,
             etc.
 
-        @param include_sys_info: Indicate whether to return system information
+        :param include_sys_info: Indicate whether to return system information
             such as the identification of the client application that uploaded
             this picture, the time when the picture has been registered.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id: uuid.UUID` (required): The identification of the user
               account that the picture is associated with.
 
             - `app_id: uuid` (optional): The identification of the client
               application that uploaded the picture.  This attribute is returned
               only if the argument `include_sys_info` is passed with the value
               `True`.
 
             - `capture_time: ISO8601DateTime` (required): The time when this picture
-              (a photo) was captured.
+              (a photo) was captured.  This attribute is returned only if the
+              argument `include_sys_info` is passed with the value `True`.
 
             - `creation_time: ISO8601DateTime` (optional): The time when this
-              picture has been registered to the platform.  This attribute is
-              returned only if the argument `include_sys_info` is passed with the
-              value `True`.
+              picture has been registered to the platform.
 
             - `image_file_checksum: str` (required): The message digest of the
               binary data of the user's original image file.  This attribute is
               returned only if the argument `include_image_info` is passed with the
               value `True`.
 
             - `image_file_size: int` (required): The size in bytes of the user's
@@ -2054,18 +2053,18 @@
               is returned only if the argument `include_sys_info` is passed with the
                value `True`.
 
             - `update_time: ISO8601DateTime` (required): The time of the most recent
               modification of the status of this picture.
 
 
-        @raise DeletedObjectException: If the picture has been deleted or
+        :raise DeletedObjectException: If the picture has been deleted or
             rejected.
 
-        @raise UndefinedObjectException: If the picture doesn't exist.
+        :raise UndefinedObjectException: If the picture doesn't exist.
         """
         with self.acquire_rdbms_connection(connection=connection) as connection:
             cursor = connection.execute(
                 """
                 SELECT
                     account_id,
                     app_id,
@@ -2136,22 +2135,22 @@
     def get_sns_data_deletion(self, app_id, request_id):
         """
         Return information about a request sent to the platform to delete the
         data of auser that an application has collected from the given Social
         Networking Service about this user.
 
 
-        @param app_id: identification of the client application such as a Web,
+        :param app_id: identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param request_id: identification of the data deletion request as
+        :param request_id: identification of the data deletion request as
             registered to the platform.
 
 
-        @return: an instance containing the following attributes:
+        :return: an instance containing the following attributes:
 
             - `creation_time` (required): time when the request to delete the data
               of a user has been initiated.
 
             - `object_status` (required): current status of this data deletion
               request.
 
@@ -2216,15 +2215,15 @@
             ```
 
         :todo: This function SHOULD be replaced with the use of another
             technology such as Elasticsearch more suitable for indexing and
             indexing data.
 
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             cursor = connection.execute(
                 """
                 SELECT
                     account_id, 
                     full_name
@@ -2248,41 +2247,41 @@
             contact: Contact = None,
             request_id: uuid.UUID = None,
             verification_code: str = None):
         """
         Indicate whether the specified contact verification request exists.
 
 
-        @param contact: An object `Contact`.
+        :param contact: An object `Contact`.
 
-        @param request_id: The identification of the contact verification request.
+        :param request_id: The identification of the contact verification request.
 
 
-        @return: `True` if the specified identification corresponds to a
+        :return: `True` if the specified identification corresponds to a
             contact verification request registered to the platform;
             `False` otherwise.
         """
         return ContactService().validate_contact_verification_request(
             contact=contact,
             request_id=request_id,
             verification_code=verification_code)
 
     def is_username_available(self, app_id, username):
         """
         Indicate whether the specified username is available or not.
 
 
-        @param app_id: Identification of the client application such as a Web,
+        :param app_id: Identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param username: A username to check whether it is already registered
+        :param username: A username to check whether it is already registered
             by an existing user or not.  A username is unique across the
             platform.  A username is not case sensitive.
 
-        @return: `True` if the username is not registered by any existing
+        :return: `True` if the username is not registered by any existing
             account; `False` otherwise.
         """
         with self.acquire_rdbms_connection() as connection:
             cursor = connection.execute(
                 """
                 SELECT 
                     true
@@ -2326,45 +2325,45 @@
 
         Note: If the user sends consecutively two requests to reset his
         password within the minimal allowed duration of time (cf. the constant
         `MINIMAL_TIME_BETWEEN_PASSWORD_RESET_REQUEST`), the function ignores the
         last request and returns the identification of the first request.
 
 
-        @param app_id: Identification of the client application such as a Web,
+        :param app_id: Identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param contact: An object `Contact` representing a contact of the user
+        :param contact: An object `Contact` representing a contact of the user
             who is requesting to reset his forgotten password.
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...:`.
 
-        @param context: A JSON expression corresponding to the context in
+        :param context: A JSON expression corresponding to the context in
             this contact information has been added and needs to be verified.
 
-        @param lifespan: Duration in seconds the password reset request lives
+        :param lifespan: Duration in seconds the password reset request lives
             before it expires.
 
-        @param language: A `Locale` instance referencing the preferred language
+        :param language: A `Locale` instance referencing the preferred language
             of the user that will be used to generate a message to be sent to
             this user.
 
-        @param nonce_digit_count: Number of digits that composed the nonce, or
+        :param nonce_digit_count: Number of digits that composed the nonce, or
             `0` if the function doesn't need to generate a nonce.
 
 
-        @raise DeletedObjectException: If the user account has been deleted.
+        :raise DeletedObjectException: If the user account has been deleted.
 
-        @raise DisabledObjectException: If the user account has been disabled.
+        :raise DisabledObjectException: If the user account has been disabled.
 
-        @raise InvalidOperationException: If a password reset has already been
+        :raise InvalidOperationException: If a password reset has already been
             requested recently for this email address.
 
-        @raise UndefinedObjectException: If the specified email address
+        :raise UndefinedObjectException: If the specified email address
             doesn't refer to any user account registered against the platform.
         """
         account = self.get_account_by_contact(
             contact,
             check_status=True,
             is_verified=False)
 
@@ -2469,27 +2468,27 @@
     def request_sns_data_deletion(self, app_id, sns_name, sns_app_id, sns_user_id):
         """
         Request the platform to delete the data of the specified user that an
         application has collected from the given Social Networking Service
         about this user.
 
 
-        @param app_id: identification of the client application such as a Web,
+        :param app_id: identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param sns_name: code name of the 3rd party Social Networking Service.
+        :param sns_name: code name of the 3rd party Social Networking Service.
 
-        @param sns_app_id: identification of the application as registered to
+        :param sns_app_id: identification of the application as registered to
             the 3rd party Social Networking Service.
 
-        @param sns_user_id: identification of the user as registered to the
+        :param sns_user_id: identification of the user as registered to the
             3rd party Social Networking Service.
 
 
-        @return: an instance containing the following attributes:
+        :return: an instance containing the following attributes:
 
             - `creation_time` (required): time when this request has been
               registered to the platform.
 
             - `request_id` (required): identification of the data deletion
               request as registered to the platform.
         """
@@ -2548,33 +2547,33 @@
 
 
         :todo: Store this password reset in the history of actions, including
             the account of the administrator who performs this action, for
             security audit purpose.
 
 
-        @param account_id: Identification of the account of the user to reset
+        :param account_id: Identification of the account of the user to reset
             their password.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
 
-        @param is_password_change_required: Indicate whether the user will
+        :param is_password_change_required: Indicate whether the user will
             have to change their password at the next login.
 
-        @param are_symbols_allowed: Indicate whether the password can
+        :param are_symbols_allowed: Indicate whether the password can
             contain punctuation characters.
 
-        @param new_password: New password to be associated to the user's
+        :param new_password: New password to be associated to the user's
             account, or `None` to automatically generate a new password.
 
-        @param password_length: Number of characters that composes the
+        :param password_length: Number of characters that composes the
             password to be generated.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id` (required): Identification of the account of the user
                 whose password has been reset.
 
             - `new_password` (required): Plain text password that has been set for
               this user.
         """
@@ -2625,52 +2624,52 @@
             request_id=None):
         """
         Change the password of the account of a user who forgot his password
         and who requested the platform to reset, as this user cannot login
         into the platform anymore.
 
 
-        @param app_id: Identification of the client application such as a Web,
+        :param app_id: Identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param new_password: New password to be associated to the user's
+        :param new_password: New password to be associated to the user's
             account.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
 
-        @param contact: An object `Contact` corresponding to an email address
+        :param contact: An object `Contact` corresponding to an email address
             or a mobile phone number where a random number (nonce) has been
             sent to for verifying the password reset request.  The argument
             `nonce` is also required.
 
-        @param nonce: "Number used once", a pseudo-random number issued when
+        :param nonce: "Number used once", a pseudo-random number issued when
             generating the request to allow the user to change his password
             through a mobile application.  The argument `contact` is also
             required.
 
-        @param request_id: Identification of the request of the user to reset
+        :param request_id: Identification of the request of the user to reset
              his forgotten password (cf. function `request_password_reset`).
 
 
-        @raise `DeletedObjectException`: if the specified password reset
+        :raise `DeletedObjectException`: if the specified password reset
             request has been cancelled by the user or if this request has
             expired.
 
-        @raise `DisabledObjectException`: if the specified password reset
+        :raise `DisabledObjectException`: if the specified password reset
             request has been already used by the user to reset the password
             of his account.
 
-        @raise `IllegalAccessException`: if the client application or the
+        :raise `IllegalAccessException`: if the client application or the
             user account, on behalf of this function is called, is not allowed
             to reset this password.
 
-        @raise InvalidArgumentException: if the new password doesn't conform
+        :raise InvalidArgumentException: if the new password doesn't conform
             to the rules of password definition.
 
-        @raise `UndefinedObjectException`: if the specified password reset
+        :raise `UndefinedObjectException`: if the specified password reset
             request has not been registered on the platform.
         """
         # Encrypt the new password passed to the function.
         self.__validate_password_complexity_requirements(new_password)
         encrypted_new_password = self.__encrypt_password(new_password)
 
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
@@ -2713,36 +2712,36 @@
     #         limit=BaseRdbmsService.DEFAULT_LIMIT,
     #         offset=0):
     #     """
     #     Search for users providing input text that may correspond to partial
     #     name, or contact information, such as email address or phone number.
     #
     #
-    #     @param full_name: partial or complete personal name by which the child
+    #     :param full_name: partial or complete personal name by which the child
     #         is known.
     #
-    #     @param account_id: identification of the account of the user who is
+    #     :param account_id: identification of the account of the user who is
     #         requesting this search.
     #
-    #     @param connection: a `RdbmsConnection` instance to be used
+    #     :param connection: a `RdbmsConnection` instance to be used
     #         supporting the Python clause `with ...:`.
     #
-    #     @param limit: constrain the number of children to return to the
+    #     :param limit: constrain the number of children to return to the
     #         specified number.  If not specified, the default value is
     #         `BaseService.DEFAULT_RESULT_SET_SIZE`.  The maximum value is
     #         `BaseService.MAXIMUM_RESULT_SET_LIMIT`.
     #
-    #     @param offset: require to skip that many records before beginning to
+    #     :param offset: require to skip that many records before beginning to
     #         return records to the client.  Default value is `0`.  If both
     #         `offset` and `limit` are specified, then `offset` records
     #         are skipped before starting to count the limit records that are
     #         returned.
     #
     #
-    #     @return: an instance containing the following members:
+    #     :return: an instance containing the following members:
     #
     #         - `account_id`: identification of the user account.
     #
     #         - `full_name`: full name of the user.
     #
     #         - `username`: name of the account of the user, if any defined.
     #
@@ -2814,40 +2813,40 @@
     #         return accounts
 
     def set_full_name(self, app_id, account_id, full_name):
         """
         Update the complete full_name of a user.
 
 
-        @param app_id: identification of the client application such as a Web,
+        :param app_id: identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param account_id: identification of the user's account.
+        :param account_id: identification of the user's account.
 
-        @param full_name: complete full name of the user as given by the user
+        :param full_name: complete full name of the user as given by the user
             himself, i.e., untrusted information.
 
 
-        @return: an instance containing the following members:
+        :return: an instance containing the following members:
 
             - `account_id` (required): identification of the user's account.
 
             - `full_name` (required): the new complete full name of the user as
               given by the user himself.
 
             - `update_time` (required): time of the most recent modification of
               the properties of the user's account.
 
 
-        @raise DeletedObjectException: if the user's account has been deleted.
+        :raise DeletedObjectException: if the user's account has been deleted.
 
-        @raise DisabledObjectException: if the user's account has been
+        :raise DisabledObjectException: if the user's account has been
             disabled.
 
-        @raise Undefined ObjectException: if the specified identification
+        :raise Undefined ObjectException: if the specified identification
             doesn't refer to a user account registered to the platform.
         """
         with self.acquire_rdbms_connection(auto_commit=True) as connection:
             cursor = connection.execute(
                 """
                 UPDATE
                     account
@@ -2892,22 +2891,22 @@
             account_id: uuid.UUID,
             language: Locale,
             connection=None):
         """
         Change the preferred language of a user
 
 
-        @param account_id: The identification of user's account.
+        :param account_id: The identification of user's account.
 
-        @param language: An object `Locale`.
+        :param language: An object `Locale`.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id` (required): The identification of the user's account.
 
             - `object_status` (required): An item of the enumeration `ObjectStatus`
               representing the current status of the user's account.
 
             - `update_time` (required): The time of the most recent modification of
@@ -2948,23 +2947,23 @@
             account_id,
             nationality,
             connection=None):
         """
         Change the nationality of a user
 
 
-        @param account_id: The identification of user's account.
+        :param account_id: The identification of user's account.
 
-        @param nationality: A ISO 3166-1 alpha-2 code referencing the
+        :param nationality: A ISO 3166-1 alpha-2 code referencing the
             nationality of the user.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id` (required): The identification of the user's account.
 
             - `object_status` (required): An item of the enumeration `ObjectStatus`
               representing the current status of the user's account.
 
             - `update_time` (required): The time of the most recent modification of
@@ -3006,23 +3005,23 @@
             account_id,
             username,
             connection=None):
         """
         Set the username of a user account.
 
 
-        @param app_id: The identification of the client application that
+        :param app_id: The identification of the client application that
             accesses this service.
 
-        @param account_id: The identification of the user account to set the
+        :param account_id: The identification of the user account to set the
             username.
 
-        @param username: The username to set for the user account.
+        :param username: The username to set for the user account.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
         """
         if not self.is_username_available(app_id, username):
             raise self.UsernameAlreadyUsedException(f'The username "{username}" is already used')
 
         self.get_account(account_id, check_status=True, connection=connection)
 
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
@@ -3067,47 +3066,47 @@
             connection=None,
             include_contacts=False,
             session_duration=None):
         """
         Sign in the user with his account identification
 
 
-        @param app_id: The identification of the client application that
+        :param app_id: The identification of the client application that
             accesses this service.
 
-        @param account_id: The identification of the user account.
+        :param account_id: The identification of the user account.
 
-        @param password: The password of the user account.
+        :param password: The password of the user account.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: An object `RdbmsConnection` with auto commit.
 
-        @param include_contacts: Indicate whether to return the contact
+        :param include_contacts: Indicate whether to return the contact
             information of the user.
 
-        @param session_duration: The login session duration, expressed in
+        :param session_duration: The login session duration, expressed in
             seconds, corresponding to the interval of time between the
             creation of the token and the expiration of this login session.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id`: identification of the account of the user.
 
             - `expiration_time`: time when the login session will expire.
 
             - `session_id`: identification of the login session of the user.
 
 
-        @raise AuthenticationFailureException: If the account identification
+        :raise AuthenticationFailureException: If the account identification
             and/or the password don't match an account registered to the
             server platform.
 
-        @raise DeletedObjectException: If the user account has been deleted.
+        :raise DeletedObjectException: If the user account has been deleted.
 
-        @raise DisabledObjectException: If the user account has been disabled.
+        :raise DisabledObjectException: If the user account has been disabled.
         """
         session = self.__sign_in(
             app_id,
             account_id,
             password,
             connection=connection,
             include_contacts=include_contacts,
@@ -3125,36 +3124,36 @@
             connection: RdbmsConnection = None,
             include_contacts: bool = False,
             session_ttl: int = None):
         """
         Sign-in the user with a contact information and a password.
 
 
-        @param app_id: The identification of the client application that
+        :param app_id: The identification of the client application that
             initiates this call.
 
-        @param contact: The contact information associated with the account of
+        :param contact: The contact information associated with the account of
             a user.
 
-        @param password: The password of the user account.
+        :param password: The password of the user account.
 
-        @param allow_unverified_contact: Indicate whether the user is allowed
+        :param allow_unverified_contact: Indicate whether the user is allowed
             to sign in with a contact not yet verified.
 
-        @param connection: An existing connection to the user database with
+        :param connection: An existing connection to the user database with
             the option `auto_commit` enabled.
 
-        @param include_contacts: Indicate whether to return the contact
+        :param include_contacts: Indicate whether to return the contact
             information of the user.
 
-        @param session_ttl: Login session time-to-live (TTL), expressed in
+        :param session_ttl: Login session time-to-live (TTL), expressed in
             seconds, of the user.
 
 
-        @return: An object containing the following members:
+        :return: An object containing the following members:
 
             - `account_id: uuid.UUID` (required): The identification of the account
               of the user.
 
             - `expiration_time: ISO8601DateTime` (required): The time when the login
               session of the user will expire.
 
@@ -3173,23 +3172,23 @@
             - `session_id: uuid.UUID` (required): The identification of the login
               session of the user.
 
             - `username: str` (optional): The username of the user.  Also known as
               the screen name or the nickname of the user.
 
 
-        @raise AuthenticationFailureException: If the given contact
+        :raise AuthenticationFailureException: If the given contact
             information and/or password don't match any account registered
             against the platform.
 
-        @raise DeletedObjectException: If the user account has been deleted.
+        :raise DeletedObjectException: If the user account has been deleted.
 
-        @raise DisabledObjectException: If the user account has been disabled.
+        :raise DisabledObjectException: If the user account has been disabled.
 
-        @raise UnverifiedContactException: If the contact of this user has not
+        :raise UnverifiedContactException: If the contact of this user has not
             been verified yet, while the parameter `allow_unverified_contact`
             has been passed with the value `False`.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             # Retrieve the identification of the user account corresponding to this
             # contact information, including the hashed version of its password
             # since the method `get_account` doesn't return it for security reason.
@@ -3248,46 +3247,46 @@
             include_contacts: bool = False,
             session_duration: int = None):
         """
         Sign-in the user against the platform providing a username and a
         password.
 
 
-        @param app_id: identification of the client application such as a Web,
+        :param app_id: identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param username: the username of the user account.
+        :param username: the username of the user account.
 
-        @param password: the password of the user account.
+        :param password: the password of the user account.
 
-        @param connection: An object `RdbmsConnection` that supports Python
+        :param connection: An object `RdbmsConnection` that supports Python
             clause `with ...`.
 
-        @param include_contacts: Indicate whether to return the contact
+        :param include_contacts: Indicate whether to return the contact
             information of the user.
 
-        @param session_duration: Login session duration, expressed in
+        :param session_duration: Login session duration, expressed in
             seconds, corresponding to the interval of time between the
             creation of the token and the expiration of this login session.
 
 
-        @return: a session instance containing the following members:
+        :return: a session instance containing the following members:
 
             - `account_id`: identification of the account of the user.
 
             - `expiration_time`: time when the login session will expire.
 
             - `session_id`: identification of the login session of the user.
 
 
-        @raise DeletedObjectException: if the user account has been deleted.
+        :raise DeletedObjectException: if the user account has been deleted.
 
-        @raise DisabledObjectException: if the user account has been disabled.
+        :raise DisabledObjectException: if the user account has been disabled.
 
-        @raise AuthenticationFailureException: if the given username and/or
+        :raise AuthenticationFailureException: if the given username and/or
             password don't match any account registered against the
             platform.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             cursor = connection.execute(
                 """
                 SELECT 
@@ -3324,28 +3323,28 @@
             return session
 
     def sign_out(self, app_id, session):
         """
         Sign out the specified user from his login session.
 
 
-        @param app_id: Identification of the client application such as a Web,
+        :param app_id: Identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param session: An object containing the following attributes:
+        :param session: An object containing the following attributes:
 
             - `account_id` (required): Identification of the account of the a user.
 
             - `session_id` (required): Identification of the user's session.
 
 
-        @raise IllegalAccessException: If the specified login session doesn't
+        :raise IllegalAccessException: If the specified login session doesn't
             belong to the specified user.
 
-        @raise UndefinedObjectException: If the specified identification
+        :raise UndefinedObjectException: If the specified identification
             doesn't refer to any user login session registered against the
             platform.
         """
         SessionService().drop_session(app_id, session)
 
     def sign_up(
             self,
@@ -3390,95 +3389,95 @@
         another user account.
 
         If the specified contact has been already registered but not verified
         yet, the function doesn't create a new account but returns the user
         account which this contact is associated to.
 
 
-        @param app_id: Identification of the client application such as a Web,
+        :param app_id: Identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
-        @param account_type: an item of `AccountType` that
+        :param account_type: an item of `AccountType` that
             describes the context that caused the registration of this user
             account.
 
-        @param action_type: Indicate the type of the action that initiates
+        :param action_type: Indicate the type of the action that initiates
             the request for verifying the specified contact information.
 
-        @param auto_sign_in: Indicate whether the platform is requested to
+        :param auto_sign_in: Indicate whether the platform is requested to
             sign-in this user once the sign-up procedure completes
             successfully.
 
-        @param can_password_be_changed: Indicate whether the user can change
+        :param can_password_be_changed: Indicate whether the user can change
             his password.
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...`.
 
-        @param contacts: An object `Contact` or a list of objects `Contact`.
+        :param contacts: An object `Contact` or a list of objects `Contact`.
 
-        @param context: A JSON expression corresponding to the context in
+        :param context: A JSON expression corresponding to the context in
             which this contact has been added and need to be verified.
 
-        @param inherited_table_name: Name of the table, inheriting from the
+        :param inherited_table_name: Name of the table, inheriting from the
             base table `account`, in which to insert the information of the
             account of the user to create.
 
-        @param does_password_never_expire: Indicate whether the password of
+        :param does_password_never_expire: Indicate whether the password of
             the user never expires.
 
-        @param enable_account: Indicate whether this user account is immediately
+        :param enable_account: Indicate whether this user account is immediately
             enabled, or whether it needs to be flagged as pending until the
             user takes some action, such as, for instance, confirming his
             contact information.
 
-        @param full_name: Complete name of the user.
+        :param full_name: Complete name of the user.
 
-        @param first_name: Forename (also known as *given name*) of the user.
+        :param first_name: Forename (also known as *given name*) of the user.
 
-        @param is_password_change_required: Indicate whether user must change
+        :param is_password_change_required: Indicate whether user must change
             his password at the next login.
 
-        @param last_name: Surname (also known as *family name*) of the user.
+        :param last_name: Surname (also known as *family name*) of the user.
 
-        @param language: An object `Locale` referencing the preferred language
+        :param language: An object `Locale` referencing the preferred language
             of the user.
 
-        @param nationality: A ISO 3166-1 alpha-2 code referencing the
+        :param nationality: A ISO 3166-1 alpha-2 code referencing the
             nationality of the user.
 
-        @param password: Password associated to the user account.  A password
+        :param password: Password associated to the user account.  A password
             is required if the argument `set_enabled` is `True`.
 
-        @param set_pending_if_unverified_contact: Indicate whether to set the
+        :param set_pending_if_unverified_contact: Indicate whether to set the
             account of this user in a pending status if the specified contact
             information has not been verified.
 
-        @param strict_prosoponym: Indicate whether the function must verify
+        :param strict_prosoponym: Indicate whether the function must verify
             if the full name of a user matches the first and the last name of
             this user.
 
-        @param team_id: Identification of the organization that creates this
+        :param team_id: Identification of the organization that creates this
             user account.
 
-        @param to_be_verified: Indicate whether the platform needs to send a
+        :param to_be_verified: Indicate whether the platform needs to send a
             request to the user to verify his contact information.  This
             argument cannot be set to `True` if the argument `has_been_verified`
             has been set to `True`.
 
-        @param username: A name used to gain access to the platform.  The
+        :param username: A name used to gain access to the platform.  The
             username MUST be unique among all the usernames already registered
             by other users to the platform.  This argument is optional if and
             only if contact information has been passed.
 
-        @param validate_password: Indicate whether the format of the password
+        :param validate_password: Indicate whether the format of the password
             needs to be validated.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id` (required): identification of the account of the
               user.
 
             - `creation_time` (required): time when this account has been
               registered.  This information should be stored by the client
               application to manage its cache of accounts.
@@ -3496,45 +3495,46 @@
 
             - `session_id` (optional): identification of the login session of
               the user.  This information is provided if the client application
               requires the platform to automatically sign-in the user (cf.
               parameter `auto_sigin`).
 
 
-        @raise ContactAlreadyUsedException: if one or more contacts are
+        :raise ContactAlreadyUsedException: if one or more contacts are
             already associated and verified for a user account.
 
-        @raise InvalidArgumentException: if one or more arguments are not
+        :raise InvalidArgumentException: if one or more arguments are not
             compliant with their required format, if some required information
             is missing.
 
-        @raise UsernameAlreadyUsedException: if the specified username is
+        :raise UsernameAlreadyUsedException: if the specified username is
             already associated with an existing user account.
         """
         if account_type not in AccountType:
             raise self.InvalidArgumentException(f'Unsupported type "{str(account_type)}" of user account')
 
-        # A user name must be provided when the given contact information has
-        # not be verified.  The reason is if another user provides the same
-        # contact information and he passes the verification challenge, this
+        # A username must be provided when the given contact information has
+        # not been verified.  The reason is if another user provides the same
+        # contact information and it passes the verification challenge, this
         # identification will be reallocated to this second user account,
         # meaning that the first user won't have any more identification to
         # sign-in to the platform.
         if not username and not contacts and account_type not in [
                 AccountType.sns,
                 AccountType.ghost
             ]:
             raise self.InvalidArgumentException(
                 "A username and/or a contact information MUST be provided")
 
         if username:
             username = username.strip().lower()
             if not self.is_username_available(app_id, username):
                 raise self.UsernameAlreadyUsedException(
-                    "This username is already associated with an existing user account")
+                    "This username is already associated with an existing user account"
+                )
 
         generate_password = password is None and enable_account and account_type not in [
                 AccountType.sns,
                 AccountType.ghost,
                 AccountType.botnet
         ]
         if generate_password:
@@ -3577,20 +3577,24 @@
         #   account.
         if recaptcha:
             (recaptcha_private_key, client_ip_address, recaptcha_challenge, recaptcha_response) = recaptcha
             if not recaptcha.verify(recaptcha_private_key, client_ip_address, recaptcha_challenge, recaptcha_response):
                 raise self.IllegalAccessException('Incorrect reCAPTCHA response')
 
         if contacts:
+            if not isinstance(contacts, (list, set, tuple)):
+                contacts = [contacts]
+
             for contact in contacts:
                 print(f"Verifying the contact {contact.property_value} ({contact.property_name})")
                 is_available, is_verified = ContactService().is_contact_available(contact)
                 if not is_available:
                     raise ContactService.ContactAlreadyInUseException(
-                        f"The contact information {contact.property_value} is already in use")
+                        f"The contact information {contact.property_value} is already in use"
+                    )
 
         with self.acquire_rdbms_connection(
                 auto_commit=True,
                 connection=connection) as connection:
 
             # # Register the account with the provided information.
             # account_status = ObjectStatus.enabled if (set_enabled and (not set_pending_if_unverified_contact or verified_contacts)) \
@@ -3693,36 +3697,36 @@
 
                 account_session.creation_time = account.creation_time
                 account_session.language = account.language
                 account_session.object_status = account.object_status
 
                 self.__update_last_login_time(account.account_id, connection)
 
-        # @todo: Remove this ugly hack with a message queue system.
+        # :todo: Remove this ugly hack with a message queue system.
         if generate_password:
             account.password = generated_password
 
         return account_session if auto_sign_in else account
 
     def update_password_reset_request(
             self,
             request_id,
             connection=None,
             object_status=ObjectStatus.deleted):
         """
         Delete a password reset request
 
 
-        @param request_id: Identification of the request of the user to reset
+        :param request_id: Identification of the request of the user to reset
              his forgotten password (cf. function `request_password_reset`).
 
-        @param connection: An object `RdbmsConnection` supporting the Python
+        :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...`.
 
-        @param object_status: An item of the enumeration `ObjectStatus`
+        :param object_status: An item of the enumeration `ObjectStatus`
 
             - `deleted`:  The request has been fulfilled.
 
             - `disabled`: The request has expired.
         """
         if object_status not in [ObjectStatus.deleted, ObjectStatus.disabled]:
             raise ValueError("Wrong value of the argument 'object_status'")
@@ -3754,59 +3758,59 @@
             is_review_required: bool = False,
             picture_minimal_size: tuple[int, int] = None,
             team_id: uuid.UUID = None):
         """
         Upload a user's picture of a user
 
 
-        @param app_id: The identification of the client application such as a
+        :param app_id: The identification of the client application such as a
             Web, a desktop, or a mobile application, that accesses the service.
 
-        @param account_id: The identification of the account of the user who
+        :param account_id: The identification of the account of the user who
             is associated to this picture.
 
-        @param submitter_account_id: The identification of the account of the
+        :param submitter_account_id: The identification of the account of the
             user who submitted this picture.
 
-        @param uploaded_file: An object `HttpRequest.HttpRequestUploadedFile`.
+        :param uploaded_file: An object `HttpRequest.HttpRequestUploadedFile`.
 
-        @param capture_time: The time when the photo was captured.
+        :param capture_time: The time when the photo was captured.
 
-        @param connection: An existing connection to the account database.
+        :param connection: An existing connection to the account database.
 
-        @param is_review_required: Indicate whether the picture needs to be
+        :param is_review_required: Indicate whether the picture needs to be
             reviewed by someone who has authority on the online service used
             by the end users.
 
-        @param picture_minimal_size: A tuple `width, height` specifying the
+        :param picture_minimal_size: A tuple `width, height` specifying the
             minimal width and height of a user's picture.
 
-        @param team_id: The identification of the organization of the user who
+        :param team_id: The identification of the organization of the user who
             submitted this picture.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
             - `account_id: uuid.UUID` (required): The identification of the account
               of the user that the picture is associated with.
 
             - `picture_id: uuid.UUID` (required): The identification of the new
               picture.
 
             - `object_status: ObjectStatus` (required): The current status of the
               picture.
 
             - `update_time: ISO8601DateTime` (required): The time of the most recent
               modification of the picture's status.
 
 
-        @raise IllegalAccessException: If the picture has been already
+        :raise IllegalAccessException: If the picture has been already
             associated to another user.
 
-        @raise PictureSizeTooSmallException: If the size of the picture is too
+        :raise PictureSizeTooSmallException: If the size of the picture is too
             small.
         """
         # Convert the uploaded file to a PIL image and check that the image is
         # of the minimal required size.
         image = self.__convert_uploaded_photo_file_to_image(uploaded_file)
         self.__validate_image_size(image, picture_minimal_size or self.DEFAULT_PICTURE_MINIMAL_SIZE)
 
@@ -3858,20 +3862,20 @@
             connection=None):
         """
         Register the account of a user to allow an account registration agent
         to send an email to the user providing his credentials to connect to
         the service
 
 
-        @todo: Replace this ugly hack with a message queue system.
+        :todo: Replace this ugly hack with a message queue system.
 
-        @param record:
-        @param connection:
-        @param team_id:
-        @return:
+        :param record:
+        :param connection:
+        :param team_id:
+        :return:
         """
         email_address_contact = [
             contact
             for contact in record.contacts
             if contact.property_name == ContactName.EMAIL
         ]
 
@@ -3919,19 +3923,19 @@
             team_id,
             connection=None,
             strict_prosoponym=True):
         """
         Insert a new account or update an existing account depending on
         whether the contact information match
 
-        @todo: The function doesn't support for the moment the update of an
+        :todo: The function doesn't support for the moment the update of an
             existing account.
 
 
-        @param record: An object containing the following attributes:
+        :param record: An object containing the following attributes:
 
             - `account_type` (optional) An item of the enumeration `AccountType`.
               Defaults to `AccountType.standard`.
 
             - `can_password_be_changed` (optional): Indicate whether the user can
               change his password.
 
@@ -3962,25 +3966,25 @@
             - `phone_number` (optional): Mobile phone number of the user.
 
             - `username` (optional): Username to associate with the user account.
               The bulk operation for this user account will fail if this username
               already exists and the attribute `account_id` is not given or if this
               username is associated to another user account.
 
-        @param team_id: Identification of the organization that creates this
+        :param team_id: Identification of the organization that creates this
             user account.
 
-        @param connection: An object `RdbmsObject` with auto commit.
+        :param connection: An object `RdbmsObject` with auto commit.
 
-        @param strict_prosoponym: Indicate whether the function must verify
+        :param strict_prosoponym: Indicate whether the function must verify
             if the full name of a user matches the first and the last name of
             this user.
 
 
-        @return: An object containing information about the account.
+        :return: An object containing information about the account.
         """
         if not record.contacts:
             raise ValueError("Missing contact information of the user")
 
         email_address_contact = [
             contact
             for contact in record.contacts
@@ -3990,15 +3994,15 @@
         if len(email_address_contact) != 1:
             raise ValueError("Zero or multiple email addresses")
 
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             account = ContactService().find_account(email_address_contact[0], connection=connection)
 
             if account:
-                pass  # @todo: Complete this feature.
+                pass  # :todo: Complete this feature.
             else:
                 account = self.sign_up(
                     account_type=AccountType.standard,
                     auto_sign_in=False,
                     connection=connection,
                     contacts=record.contacts,
                     enable_account=True,
@@ -4007,15 +4011,15 @@
                     full_name=record.full_name,
                     last_name=record.last_name,
                     language=record.language,
                     strict_prosoponym=strict_prosoponym,
                     team_id=team_id,
                 )
 
-                # @todo: Remove this ugly hack with a message queue system.
+                # :todo: Remove this ugly hack with a message queue system.
                 record.account_id = account.account_id
                 record.password = account.password
                 self.__register_account(record, team_id, connection=connection)
 
             return account
```

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/contact_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/contact_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_constraint.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_function.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_account_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_table.sql`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  *
  * MAJORMODE MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE SUITABILITY
  * OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
  * TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
  * PURPOSE, OR NON-INFRINGEMENT.  MAJORMODE SHALL NOT BE LIABLE FOR ANY
  * LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING
  * OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
-*/
+ */
 
 --(defconstant +account-type-standard+ 'standard')
 --(defconstant +account-type-sns+ 'sns')
 --(defconstant +account-type-botnet+ 'botnet')
 --(defconstant +account-type-test+ 'test')
 --(defconstant +account-type-administrator+ 'administrator')
 
@@ -29,22 +29,21 @@
  * Email address and password are optional since a user might use an
  * authenticated session of a Social Networking Site (such as Facebook,
  * Twitter, etc.) to sign-in against the online service.  email
  * address and password are more likely defined when a user signs-up
  * against the platform without sign-in against a Social Networking
  * Site (SNS).
  */
-CREATE TABLE account
-(
+CREATE TABLE account (
   -- Identification of this user account.
-  account_id uuid NOT NULL DEFAULT uuid_generate_v1(),
+  account_id uuid NOT NULL DEFAULT uuid_generate_v4(),
 
-  -- Full name by which the user is known.  It is either given by the user
-  -- himself or an administrator, or as determined from the email address
-  -- of this user.
+  -- The personal name by which the user is known.  It is either given by
+  -- the user himself or an administrator, or as determined from the email
+  -- address of this user.
   full_name text NULL,
 
   -- Forename (also known as *given name*) of the user.  The first name can
   -- be used to alphabetically sort a list of users.
   first_name text NULL,
 
   -- Surname (also known as *family name*) of the user.  The last name can
@@ -56,15 +55,15 @@
   -- with others online.  A username should be totally made-up pseudonym,
   -- not reveal the real name of the person.  The username is unique across
   -- the platform.  A username is not case sensitive.
   username text NULL,
 
   -- Describe the context that caused the registration of this user account,
   -- such as `standard`, `botnet`, `ghost`, `sns`.
-  account_type text NOT NULL DEFAULT +account-type-standard+,
+  account_type text NOT NULL DEFAULT 'standard',
 
   -- Encrypted version of the password.
   password text NULL,
 
   -- Indicate whether user must change his password at the next login.
   is_password_change_required boolean NOT NULL DEFAULT false,
 
@@ -90,15 +89,15 @@
 
   -- Time zone of the default location of the user.  It is the difference
   -- between the time at this location and UTC (Universal Time Coordinated).
   -- UTC is also known as GMT or Greenwich Mean Time or Zulu Time.
   timezone smallint NULL,
 
   -- Current status of this user account.
-  object_status text NOT NULL DEFAULT +object-status-enabled+,
+  object_status text NOT NULL DEFAULT 'pending',
 
   -- Time when this user account has been created.
   creation_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
   -- Time of the most recent modification of information of this user
   -- account.
   update_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
@@ -120,16 +119,15 @@
  * A contact information corresponds to e-mail addresses and phone
  * numbers.
  *
  *
  * @note: There can be only a unique property with a given name and a
  *     given value.
  */
-CREATE TABLE account_contact
-(
+CREATE TABLE account_contact (
   -- The identification of a user account.
   account_id uuid NOT NULL,
 
   -- The name (type) of this contact information:
   --
   -- * `EMAIL`: An electronic mail address.
   --
@@ -143,31 +141,31 @@
   -- information.
   property_value text NOT NULL,
 
   -- The property value of a contact information can be further
   -- qualified with a property parameter expression.  The property
   -- parameter expressions are specified as either a single string or
   -- `name=value`, separated with comas.  This information is optional.
-  property_parameter text  NULL,
+  property_parameter text NULL,
 
   -- Indicate whether this contact information is the primary contact
   -- for this type of contact information (cf. {@link
   -- account_contact.property_name}).
   is_primary boolean NOT NULL DEFAULT false,
 
   -- The visibility of this contact information to other users.
-  visibility text NOT NULL DEFAULT +visibility-private+,
+  visibility text NOT NULL DEFAULT 'private',
 
   -- Indicate whether this contact information has been verified, it has
   -- been grabbed from a trusted Social Networking Service (SNS), or
   -- through a challenge/response process.
   is_verified boolean NOT NULL DEFAULT false,
 
   -- The current status of this contact information.
-  object_status text NOT NULL DEFAULT +object-status-enabled+,
+  object_status text NOT NULL DEFAULT 'enabled',
 
   -- The time when this contact information has been created.
   creation_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
   -- The time of the most recent modification of this contact information.
   update_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
@@ -262,16 +260,15 @@
   last_attempt_time timestamptz(3) NULL
 );
 
 
 /**
  * Represent requests to users to verify their contact information.
  */
-CREATE TABLE account_contact_verification
-(
+CREATE TABLE account_contact_verification (
   -- Identification of contact information verification request.
   request_id uuid NOT NULL DEFAULT uuid_generate_v4(),
 
   -- A pseudo-random number (nonce) that was generated and sent to the
   -- user to verify his contact information.
   verification_code text NULL,
 
@@ -316,15 +313,15 @@
   -- verified.
   request_count smallint NOT NULL DEFAULT 0,
 
   -- Number of times the platform sent this request to the user.
   attempt_count smallint NOT NULL DEFAULT 0,
 
   -- The current status of this request.
-  object_status text NOT NULL DEFAULT +object-status-enabled+;
+  object_status text NOT NULL DEFAULT 'enabled',
 
   -- The time when this request has been sent to the user for the first time.
   creation_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
   -- The time of the most recent modification of one attribute of this request.
   update_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
@@ -336,32 +333,30 @@
 );
 
 
 /**
  * Represent the normalized keywords extracted from several attributes
  * of user accounts.
  */
-CREATE TABLE account_index
-(
+CREATE TABLE account_index (
   -- The identification of a user account.
   account_id uuid NOT NULL,
 
 -- A plain ASCII and lowercase representation of a word collected from
 -- the full_name of the account.  Each keyword is at least 2-character
 -- long.
   keyword text NOT NULL
 );
 
 
 /**
  * Represent requests from users who have forgotten their password and
  * who would like to reset their password.
  */
-CREATE TABLE account_password_reset
-(
+CREATE TABLE account_password_reset (
   -- Identification of the password reset request.  This identification
   -- can be used in a link sent to the user to allow him to change his
   -- password through a Web application.
   request_id uuid NOT NULL DEFAULT uuid_generate_v4(),
 
   -- "Number used once", a pseudo-random number issued when generating the
   -- request to allow the user to change his password through a mobile
@@ -433,16 +428,15 @@
   last_attempt_time timestamptz(3) NULL
 );
 
 
 /**
  * Represent the history of the past and current pictures of the user.
  */
-CREATE TABLE account_picture
-(
+CREATE TABLE account_picture (
   -- The identification of the picture.
   picture_id uuid NOT NULL,
 
   -- The identification of the user account that the picture is associated
   -- with.
   --
   -- @note: This column is null when the user account was hard-deleted.  A
```

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_constraint.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_function.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/create_session_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table.718.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table.718.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql`

 * *Files 5% similar despite different names*

```diff
@@ -40,34 +40,37 @@
 
 DELETE FROM account_picture
   WHERE picture_id IN (
     SELECT
         picture_id
       FROM
         account_picture
-      WHERE NOT EXISTS (
-        SELECT
-            true
-          FROM
-            account
-          WHERE
-            account.account_id = account_picture.account_id
-      )
+      WHERE
+        NOT EXISTS (
+          SELECT
+              true
+            FROM
+              account
+            WHERE
+              account.account_id = account_picture.account_id
+        )
   );
 
 UPDATE account_picture
-  SET submitter_account_id = account_id
-  WHERE NOT EXISTS (
-    SELECT
-        true
-      FROM
-        account
-      WHERE
-        account.account_id = account_picture.submitter_account_id
-  );
+  SET
+    submitter_account_id = account_id
+  WHERE
+    NOT EXISTS (
+      SELECT
+          true
+        FROM
+          account
+        WHERE
+          account.account_id = account_picture.submitter_account_id
+    );
 
 ALTER TABLE account_picture
   ADD CONSTRAINT fk_account_picture_team_id
       FOREIGN KEY (team_id)
       REFERENCES team (team_id)
       ON DELETE SET NULL
       ON UPDATE CASCADE;
@@ -84,24 +87,43 @@
         picture_id
     FROM
         account_picture
     WHERE
         object_status = 'enabled'
   ) AS account_picture
   WHERE
-    account.account_id = account_picture.account_id;
+    account.account_id = account_picture.account_id
+    AND account.picture_id != account_picture.picture_id;
+
 
 -- Remove the reference to a picture for accounts which haven't an active
 -- picture.
 UPDATE
     account
   SET
     picture_id = NULL
   WHERE
-    NOT EXISTS (
+    picture_id IS NOT NULL
+    AND NOT EXISTS (
+      SELECT
+          true
+        FROM
+          account_picture
+        WHERE
+          account_picture.account_id = account.account_id
+          AND object_status = 'enabled'
+    );
+
+SELECT DISTINCT
+    picture_id
+  FROM
+    account
+  WHERE
+    picture_id IS NOT NULL
+    AND NOT EXISTS (
       SELECT
           true
         FROM
           account_picture
         WHERE
           account_picture.account_id = account.account_id
           AND object_status = 'enabled'
```

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/oauth_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/oauth_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/session_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/session_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/test/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/account/test/account_service_unittest.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/account_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/application_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/application_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/db/create_application_constraint.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/db/create_application_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/db/create_application_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/test/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/application/test/application_service_unittest.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/application_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/area_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/area_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/data/vietnam/area2sql.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/data/vietnam/area_extractor.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area_extractor.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_constraint.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_dataset.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_function.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_area_type.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_geoip_constraint.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_geoip_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_geoip_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/create_rir_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_rir_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/db/migrate_area_dataset.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/migrate_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/script/_geolite_importer.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_geolite_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/script/_rir_importer.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_rir_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/area/script/geoip2sql.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/geoip2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_http_handler.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_job_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_job_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_rdbms_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_rdbms_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/base_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/agent/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/agent/push_notification.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/push_notification.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/db/create_notification_constraint.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/db/create_notification_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/db/create_notification_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/gcm.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/gcm.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/notification/notification_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/doc/api/get_ping.rst` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_ping.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/doc/api/get_status.rst` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_status.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/doc/api/index.rst` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/status_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/status/status_service_http_handler.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/agent/team_invite.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/agent/team_invite.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_constraint.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_function.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_index.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_index.sql`

 * *Files 6% similar despite different names*

```diff
@@ -11,12 +11,16 @@
  * OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
  * TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
  * PURPOSE, OR NON-INFRINGEMENT.  MAJORMODE SHALL NOT BE LIABLE FOR ANY
  * LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING
  * OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
 */
 
+CREATE UNIQUE INDEX idx_team_name
+  ON team (lower(name));
+
+
 CREATE UNIQUE INDEX idx_team_contact
   ON team_contact (
     lower(property_value),
     property_name
   );
```

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/create_team_table.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_table.sql`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,17 @@
  */
 
 /**
  * Represent a group of people having a common purpose or interest,
  * such as, for instance, an organization, an association, a guild,
  * an institute, a squad. etc.
  */
-CREATE TABLE team
-(
+CREATE TABLE team (
   -- Identification of the team.
-  team_id uuid NOT NULL DEFAULT uuid_generate_v1(),
+  team_id uuid NOT NULL DEFAULT uuid_generate_v4(),
 
   -- The name given to the team.
   name text NOT NULL,
 
   -- A short textual description of the team written in whatever locale.
   description text NULL,
 
@@ -75,15 +74,15 @@
   -- of the total number of administrators, that must revoke a member from
   -- the team so that decisions can be made properly.  If the value is `0.0`,
   -- only the agent of the team can revoke the role of administrator from a
   -- member.
   administrator_revocation_quorum float NULL DEFAULT 0.0,
 
   -- Current status of this team.
-  object_status text NOT NULL DEFAULT +object-status-enabled+,
+  object_status text NOT NULL DEFAULT 'enabled',
 
   -- Time when the team has been registered.
   creation_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
   -- Time of the most recent modification of some information of the team.
   update_time timestamptz(3) NOT NULL DEFAULT current_timestamp
 );
@@ -160,15 +159,15 @@
   -- `account.full_name`) by an administrator of the team.
   full_name text NULL,
 
   -- Role of this user within the team.
   role text NOT NULL,
 
   -- Current status of the member.
-  object_status text NOT NULL DEFAULT +object-status-enabled+,
+  object_status text NOT NULL DEFAULT 'enabled',
 
   -- Time when this user has been added as a member of the team.
   creation_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
   -- Time of the most recent modification of the membership of this user.
   update_time timestamptz(3) NOT NULL DEFAULT current_timestamp
 );
```

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/team_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/team_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/template/default_invite_email.txt` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/template/default_invite_email.txt`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/test/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/team/test/team_service_unittest.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/team_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/doc/api/get_version.rst` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/get_version.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/doc/api/index.rst` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/test/__init__.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/test/version_service_unittest.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/version_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/version_service.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/src/majormode/perseus/service/version/version_service_http_handler.py` & `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.8/setup.py` & `perseus_restful_api_framework-1.26.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  'prosoponym>=1.0.7,<2.0.0',
  'psutil>=5.9.4,<6.0.0',
  'pymemcache>=4.0.0,<5.0.0',
  'tornado>=6.2,<7.0']
 
 setup_kwargs = {
     'name': 'perseus-restful-api-framework',
-    'version': '1.26.8',
+    'version': '1.26.9',
     'description': 'Python server framework for quickly building RESTful APIs with minimal effort',
     'long_description': '# Perseus: RESTful API Server Framework\n\nPerseus is a Python framework for quickly building RESTful API servers with minimal effort.\n\nPerseus provides an initial set of core services that supports the following features:\n\n- Client application registration with API keys generation\n- Client application access control with RESTful request signature\n- Client application and RESTful API server version compatibility check\n- User authentication and session management\n- Team/group management\n- RESTful request logging with data sensitiveness support\n- RESTful service automatic discovery\n- HTTP request query parameters & body JSON message automatically parsing (depending on the HTTP method used) with data type check and conversion\n\nPerseus is based on [Tornado](https://www.tornadoweb.org/) for handling client network connection.\n\n## RESTful API Request Handler\n\n```python\nfrom majormode.perseus.service.base_http_handler import HttpRequest\nfrom majormode.perseus.service.base_http_handler import HttpRequestHandler\nfrom majormode.perseus.service.base_http_handler import http_request\n\nimport AttendantService\n\n\nclass AttendantServiceHttpRequestHandler(HttpRequestHandler):\n    @http_request(r\'^/attendant/session$\',\n                  http_method=HttpRequest.HttpMethod.POST,\n                  authentication_required=False,\n                  sensitive_data=True,\n                  signature_required=False)\n    def sign_in(self, request):\n        email_address = request.get_argument(\n            \'email_address\',\n            data_type=HttpRequest.ArgumentDataType.email_address,\n            is_required=True)\n\n        password = request.get_argument(\n            \'password\',\n            data_type=HttpRequest.ArgumentDataType.string,\n            is_required=True)\n\n        return AttendantService().sign_in(request.app_id, email_address, password)\n```\n\n## Configure the environment variables\n\n```env\n# Copyright (C) 2021 Majormode.  All rights reserved.\n#\n# Permission is hereby granted, free of charge, to any person obtaining\n# a copy of this software and associated documentation files (the\n# "Software"), to deal in the Software without restriction, including\n# without limitation the rights to use, copy, modify, merge, publish,\n# distribute, sublicense, and/or sell copies of the Software, and to\n# permit persons to whom the Software is furnished to do so, subject to\n# the following conditions:\n#\n# The above copyright notice and this permission notice shall be\n# included in all copies or substantial portions of the Software.\n#\n# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,\n# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\n# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\n# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\n# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n# Connection properties of the RESTful API server instances.  Defaults\n# to 127.0.0.1:8081.\nAPI_SERVER_HOSTNAME=127.0.0.1\nAPI_SERVER_PORTS=\n\n# Root path of the Network File System (NFS) -- referring to the\n# distributed file system (not the protocol) -- where the Content\n# Delivery Network (CDN) files are stored into, such as avatars, etc.\nCDN_NFS_ROOT_PATH=\n\n# Hostname of the Content Delivery Network (CDN) server that hosts media\n# files such as avatars, etc.\nCDN_URL_HOSTNAME=\n\n# Environment stage of the API server instances.  Possible values are:\n#\n# - dev\n# - int\n# - staging\n# - prod\n#\n# Defaults to `dev`.\nENVIRONMENT_STAGE=\n\n# Connection properties to a Memcached server (a distributed memory\n# object caching system).  Defaults to 127.0.0.1:11211.\nMEMCACHED_HOSTNAME = \'127.0.0.1\'\nMEMCACHED_PORT = 11211\n\n# Threshold for the logger to level.  Logging messages which are less\n# severe than the specified level will be ignored; logging messages\n# which have this severity level or higher will be emitted.  Possible\n# values are:\n#\n# - debug\n# - info\n# - warning\n# - error\n# - critical\n#\n# Default to \'debug\'.\nLOGGING_LEVEL=\n\n# Environment variables to select default parameter values to connect\n# to PostgreSQL Relational Database Management System.\nPG_HOSTNAME=localhost\nPG_PORT=5432\nPG_DATABASE_NAME=\nPG_USERNAME=\nPG_PASSWORD=\n```\n\n## Run the RESTful API Server Processes\n\n```bash\n$ fab start --port=65180,65181,...\n```\n\nHashtags/Topics: `#perseus` `#restful` `#api` `#server` `#framework` `#python`\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/perseus-restful-api-server-framework',
```

### Comparing `perseus_restful_api_framework-1.26.8/PKG-INFO` & `perseus_restful_api_framework-1.26.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perseus-restful-api-framework
-Version: 1.26.8
+Version: 1.26.9
 Summary: Python server framework for quickly building RESTful APIs with minimal effort
 Home-page: https://github.com/majormode/perseus-restful-api-server-framework
 License: Proprietary
 Keywords: perseus,resful,api,server,framework
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
 Requires-Python: >=3.9,<4.0
```

