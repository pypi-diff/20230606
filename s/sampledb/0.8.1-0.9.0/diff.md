# Comparing `tmp/sampledb-0.8.1.tar.gz` & `tmp/sampledb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sampledb-0.8.1.tar", last modified: Tue Dec 10 12:36:48 2019, max compression
+gzip compressed data, was "dist/sampledb-0.9.0.tar", last modified: Wed Jun 17 11:59:20 2020, max compression
```

## Comparing `sampledb-0.8.1.tar` & `sampledb-0.9.0.tar`

### file list

```diff
@@ -1,371 +1,577 @@
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/
--rw-r--r--   0 rhiem    (20243) staff       (20)       25 2019-12-10 12:35:01.000000 sampledb-0.8.1/MANIFEST.in
--rw-r--r--   0 rhiem    (20243) staff       (20)     3864 2019-12-10 12:36:48.000000 sampledb-0.8.1/PKG-INFO
--rw-r--r--   0 rhiem    (20243) staff       (20)     2769 2019-12-10 12:35:01.000000 sampledb-0.8.1/README.md
--rw-r--r--   0 rhiem    (20243) staff       (20)     1397 2019-12-10 12:35:01.000000 sampledb-0.8.1/requirements.txt
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/
--rw-r--r--   0 rhiem    (20243) staff       (20)     1665 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      724 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/__main__.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/api/
--rw-r--r--   0 rhiem    (20243) staff       (20)       97 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/api/__init__.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/api/server/
--rw-r--r--   0 rhiem    (20243) staff       (20)     3275 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/api/server/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1677 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/api/server/actions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1066 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/api/server/authentication.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     5845 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/api/server/files.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1179 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/api/server/instruments.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2910 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/api/server/locations.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     7583 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/api/server/object_permissions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     7969 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/api/server/objects.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      963 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/api/server/users.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     5339 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/config.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/
--rw-r--r--   0 rhiem    (20243) staff       (20)      827 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/frontend/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    14438 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/actions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2031 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/authentication_forms.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      686 2019-12-09 10:09:31.000000 sampledb-0.8.1/sampledb/frontend/errors.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      200 2017-03-13 15:18:06.000000 sampledb-0.8.1/sampledb/frontend/index.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1592 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/instruments.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    10580 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/labels.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     8403 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/locations.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    10748 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/object_form_parser.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    61692 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/objects.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3068 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/objects_forms.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    22671 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/pdfexport.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    25224 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/projects.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2306 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/projects_forms.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      537 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/status.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      329 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/frontend/tags.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/actions/
--rw-r--r--   0 rhiem    (20243) staff       (20)     2469 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/actions/action.html
--rw-r--r--   0 rhiem    (20243) staff       (20)    18469 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/actions/action_form.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     2429 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/actions/actions.html
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/errors/
--rw-r--r--   0 rhiem    (20243) staff       (20)      158 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/errors/403.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      168 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/errors/404.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      182 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/errors/500.html
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/instruments/
--rw-r--r--   0 rhiem    (20243) staff       (20)     1289 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/instruments/instrument.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      349 2019-02-20 08:41:54.000000 sampledb-0.8.1/sampledb/frontend/templates/instruments/instrument_scientists.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1132 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/instruments/instruments.html
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/locations/
--rw-r--r--   0 rhiem    (20243) staff       (20)     1160 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/locations/location.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     2631 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/locations/location_form.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      779 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/locations/locations.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      602 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/locations/locations_tree.html
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/
--rw-r--r--   0 rhiem    (20243) staff       (20)     4410 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/account_recovery.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     3754 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/account_recovery.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)     2003 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/base.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      325 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/base.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)      884 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/email_confirmation.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      245 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/email_confirmation.txt
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/
--rw-r--r--   0 rhiem    (20243) staff       (20)      201 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/announcement.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      103 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/announcement.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)     1134 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/assigned_as_responsible_user.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      423 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/assigned_as_responsible_user.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)      476 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/base.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      316 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/base.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)     1222 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/invited_to_group.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      416 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/invited_to_group.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)     1238 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/invited_to_project.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      424 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/invited_to_project.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)      111 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/other.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      103 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/other.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)     1156 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/received_object_permissions_request.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      425 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/received_object_permissions_request.txt
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/
--rw-r--r--   0 rhiem    (20243) staff       (20)      975 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_any.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     8227 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_array.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     2482 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_base.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1012 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_bool.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1568 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_create.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1087 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_datetime.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      906 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_edit.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     3287 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_hazards.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1918 2018-10-15 06:20:01.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_object.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1810 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_quantity.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1496 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_sample.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1639 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_select.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      622 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_any.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      814 2018-02-09 11:35:04.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_datetime.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1472 2018-02-09 11:35:04.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_quantity.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1229 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_select.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      761 2018-05-25 10:04:12.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_text.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      805 2018-09-19 13:29:03.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_tags.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1229 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_text.html
--rw-r--r--   0 rhiem    (20243) staff       (20)    22415 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/object_permissions.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      766 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/object_versions.html
--rw-r--r--   0 rhiem    (20243) staff       (20)    11520 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/objects.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      641 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/restore_object_version.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      583 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/unauthorized.html
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/
--rw-r--r--   0 rhiem    (20243) staff       (20)      913 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/any.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     7702 2019-09-10 12:09:52.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/array.html
--rw-r--r--   0 rhiem    (20243) staff       (20)    56253 2019-11-22 10:03:26.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/base.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1030 2018-10-19 06:16:51.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/bool.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      628 2018-10-19 06:16:51.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/datetime.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      829 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/hazards.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     2135 2018-10-19 06:16:51.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/object.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     1249 2018-10-19 06:16:51.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/quantity.html
--rw-r--r--   0 rhiem    (20243) staff       (20)     2931 2019-02-01 15:12:00.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/related_objects.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      765 2018-11-30 15:39:06.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/related_objects_tree_toggle.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      774 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/sample.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      944 2018-10-19 06:16:51.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/select.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      659 2018-09-25 07:46:31.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/table_any.html
--rw-r--r--   0 rhiem    (20243) staff       (20)       80 2018-02-09 11:35:04.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/table_datetime.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      282 2018-09-19 13:29:03.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/table_quantity.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      194 2017-04-24 06:40:30.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/table_sample.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      241 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/table_tags.html
--rw-r--r--   0 rhiem    (20243) staff       (20)       15 2017-03-14 14:33:42.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/table_text.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      515 2018-10-19 06:16:51.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/tags.html
--rw-r--r--   0 rhiem    (20243) staff       (20)      888 2018-10-19 06:16:51.000000 sampledb-0.8.1/sampledb/frontend/templates/objects/view/text.html
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/frontend/users/
--rw-r--r--   0 rhiem    (20243) staff       (20)      412 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      457 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users/activity.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1861 2019-07-08 13:47:12.000000 sampledb-0.8.1/sampledb/frontend/users/authentication.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2427 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users/favorites.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      957 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/users/forms.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    10162 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/users/groups.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3693 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users/invitation.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      306 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users/list.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     6309 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/frontend/users/notifications.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    27448 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users/preferences.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      600 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users/profile.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1698 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/users_forms.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2055 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/frontend/utils.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/logic/
--rw-r--r--   0 rhiem    (20243) staff       (20)     1428 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    14784 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/action_permissions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     4418 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/actions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     9134 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/logic/authentication.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1881 2019-01-07 11:31:20.000000 sampledb-0.8.1/sampledb/logic/comments.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     9623 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/datatypes.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2985 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/logic/errors.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3907 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/logic/favorites.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    14000 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/files.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     9547 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/groups.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     5038 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/instruments.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     5108 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/logic/ldap.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    13070 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/logic/locations.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    18927 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/logic/notifications.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     5062 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/object_log.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    18929 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/logic/object_permissions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     4935 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/object_relationships.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    39260 2019-11-07 07:45:47.000000 sampledb-0.8.1/sampledb/logic/object_search.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    17309 2019-11-07 07:44:48.000000 sampledb-0.8.1/sampledb/logic/object_search_parser.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3725 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/object_sorting.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    12676 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/objects.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    30380 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/projects.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3711 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/publications.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/logic/schemas/
--rw-r--r--   0 rhiem    (20243) staff       (20)      612 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/schemas/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3435 2019-01-07 09:21:12.000000 sampledb-0.8.1/sampledb/logic/schemas/convert_to_schema.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     6368 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/schemas/generate_placeholder.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      733 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/schemas/utils.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    16733 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/logic/schemas/validate.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    20552 2019-10-30 13:45:34.000000 sampledb-0.8.1/sampledb/logic/schemas/validate_schema.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      512 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/security_tokens.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3366 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/settings.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2311 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/tags.py
--rw-r--r--   0 rhiem    (20243) staff       (20)       35 2018-09-18 13:30:50.000000 sampledb-0.8.1/sampledb/logic/unit_definitions.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)      658 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/logic/units.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     6037 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/user_log.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1308 2019-12-10 12:35:01.000000 sampledb-0.8.1/sampledb/logic/users.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3246 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/logic/utils.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     5578 2019-11-07 07:49:05.000000 sampledb-0.8.1/sampledb/logic/where_filters.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/models/
--rw-r--r--   0 rhiem    (20243) staff       (20)     2708 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1749 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/action_permissions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1598 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/actions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      913 2019-01-07 09:21:12.000000 sampledb-0.8.1/sampledb/models/authentication.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1074 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/comments.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      591 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/favorites.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1463 2018-02-09 11:35:04.000000 sampledb-0.8.1/sampledb/models/file_log.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1142 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/files.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      572 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/groups.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1149 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/instruments.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2423 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/models/locations.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/models/migrations/
--rw-r--r--   0 rhiem    (20243) staff       (20)      760 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      696 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/actions_add_user_id.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      775 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/create_migration_index.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2941 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/create_user_object_permissions_by_all_view.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1360 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/files_add_data.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1033 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/models/migrations/object_location_assignments_add_confirmed.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      971 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/object_location_assignments_add_responsible_user_id.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      819 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/object_log_entry_type_add_assign_location.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      823 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/object_log_entry_type_add_link_publication.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      813 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_assign_location.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      813 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_create_location.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      816 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_link_publication.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      813 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_update_location.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2882 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/migrations/utils.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2138 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/notifications.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1503 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/object_log.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     3389 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/object_permissions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      412 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/object_publications.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      543 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/objects.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      872 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/permissions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1818 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/projects.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      909 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/settings.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      265 2018-09-19 13:29:03.000000 sampledb-0.8.1/sampledb/models/tags.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1407 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/user_log.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1017 2019-01-07 09:21:12.000000 sampledb-0.8.1/sampledb/models/users.py
--rw-r--r--   0 rhiem    (20243) staff       (20)    17748 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/models/versioned_json_object_tables.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/scripts/
--rw-r--r--   0 rhiem    (20243) staff       (20)     1001 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/scripts/__init__.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2165 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/scripts/create_action.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      837 2017-04-24 11:24:16.000000 sampledb-0.8.1/sampledb/scripts/create_instrument.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      960 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/scripts/create_other_user.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1068 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/scripts/export_action_schema.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      436 2017-05-16 12:31:28.000000 sampledb-0.8.1/sampledb/scripts/list_actions.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      472 2017-04-24 11:29:26.000000 sampledb-0.8.1/sampledb/scripts/list_instruments.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      918 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/scripts/run.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      690 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/scripts/send_announcement.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1256 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/scripts/set_administrator.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     1447 2017-05-16 12:31:28.000000 sampledb-0.8.1/sampledb/scripts/update_action.py
--rw-r--r--   0 rhiem    (20243) staff       (20)      995 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/scripts/update_instrument.py
--rw-r--r--   0 rhiem    (20243) staff       (20)     2250 2017-05-16 12:31:28.000000 sampledb-0.8.1/sampledb/scripts/update_instrument_responsible_users.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/static/
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/static/css/
--rw-r--r--   0 rhiem    (20243) staff       (20)    10963 2019-10-15 07:16:32.000000 sampledb-0.8.1/sampledb/static/css/base.css
--rw-r--r--   0 rhiem    (20243) staff       (20)     7785 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-datetimepicker.min.css
--rwxr-xr-x   0 rhiem    (20243) staff       (20)     7761 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-select.css
--rwxr-xr-x   0 rhiem    (20243) staff       (20)    16645 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-select.css.map
--rwxr-xr-x   0 rhiem    (20243) staff       (20)     6650 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-select.min.css
--rwxr-xr-x   0 rhiem    (20243) staff       (20)     1359 2018-09-19 13:29:03.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-tagsinput.css
--rw-r--r--   0 rhiem    (20243) staff       (20)    26132 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-theme.css
--rw-r--r--   0 rhiem    (20243) staff       (20)    47706 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-theme.css.map
--rw-r--r--   0 rhiem    (20243) staff       (20)    23409 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-theme.min.css
--rw-r--r--   0 rhiem    (20243) staff       (20)    25648 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-theme.min.css.map
--rw-r--r--   0 rhiem    (20243) staff       (20)     1590 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-toggle.min.css
--rwxr-xr-x   0 rhiem    (20243) staff       (20)      204 2018-02-09 11:35:04.000000 sampledb-0.8.1/sampledb/static/css/bootstrap-treeview.min.css
--rw-r--r--   0 rhiem    (20243) staff       (20)   146010 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap.css
--rw-r--r--   0 rhiem    (20243) staff       (20)   389287 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap.css.map
--rw-r--r--   0 rhiem    (20243) staff       (20)   121200 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap.min.css
--rw-r--r--   0 rhiem    (20243) staff       (20)   542194 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/bootstrap.min.css.map
--rw-r--r--   0 rhiem    (20243) staff       (20)    37414 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/font-awesome.css
--rw-r--r--   0 rhiem    (20243) staff       (20)    31000 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/css/font-awesome.min.css
--rw-r--r--   0 rhiem    (20243) staff       (20)     4600 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/static/css/pygments.css
--rw-r--r--   0 rhiem    (20243) staff       (20)     2017 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/static/css/schema_editor.css
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/static/fonts/
--rw-r--r--   0 rhiem    (20243) staff       (20)   134808 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/FontAwesome.otf
--rw-r--r--   0 rhiem    (20243) staff       (20)   165742 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 rhiem    (20243) staff       (20)   444379 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 rhiem    (20243) staff       (20)   165548 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 rhiem    (20243) staff       (20)    98024 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 rhiem    (20243) staff       (20)    77160 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 rhiem    (20243) staff       (20)    20127 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 rhiem    (20243) staff       (20)   108738 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 rhiem    (20243) staff       (20)    45404 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 rhiem    (20243) staff       (20)    23424 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 rhiem    (20243) staff       (20)    18028 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/static/img/
--rw-r--r--   0 rhiem    (20243) staff       (20)     2621 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs00.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     9952 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs01.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     6028 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs02.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     6593 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs03.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     2625 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs04.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     7357 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs05.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     8581 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs06.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     2667 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs07.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     7267 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs08.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     7275 2018-11-30 08:35:46.000000 sampledb-0.8.1/sampledb/static/img/ghs09.png
--rw-r--r--   0 rhiem    (20243) staff       (20)      771 2019-08-30 14:46:52.000000 sampledb-0.8.1/sampledb/static/img/jupyter-40.png
--rw-r--r--   0 rhiem    (20243) staff       (20)     5428 2019-10-30 12:38:38.000000 sampledb-0.8.1/sampledb/static/img/logo.png
--rw-r--r--   0 rhiem    (20243) staff       (20)      837 2019-10-30 12:37:48.000000 sampledb-0.8.1/sampledb/static/img/logo.svg
--rw-r--r--   0 rhiem    (20243) staff       (20)     1606 2019-10-30 13:02:22.000000 sampledb-0.8.1/sampledb/static/img/logo64.png
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/static/js/
--rw-r--r--   0 rhiem    (20243) staff       (20)    38510 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/bootstrap-datetimepicker.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)    69851 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/bootstrap-select.js
--rw-r--r--   0 rhiem    (20243) staff       (20)    39003 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/bootstrap-select.js.map
--rw-r--r--   0 rhiem    (20243) staff       (20)    33963 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/bootstrap-select.min.js
--rwxr-xr-x   0 rhiem    (20243) staff       (20)     9464 2018-09-19 13:29:03.000000 sampledb-0.8.1/sampledb/static/js/bootstrap-tagsinput.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     4129 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/static/js/bootstrap-toggle.min.js
--rwxr-xr-x   0 rhiem    (20243) staff       (20)    16735 2018-02-09 11:35:04.000000 sampledb-0.8.1/sampledb/static/js/bootstrap-treeview.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)    69707 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/bootstrap.js
--rw-r--r--   0 rhiem    (20243) staff       (20)    37045 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/bootstrap.min.js
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb/static/js/i18n/
--rw-r--r--   0 rhiem    (20243) staff       (20)     1852 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ar_AR.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1308 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ar_AR.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1730 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-bg_BG.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1186 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-bg_BG.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1521 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-cro_CRO.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      977 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-cro_CRO.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1137 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-cs_CZ.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      735 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-cs_CZ.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1459 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-da_DK.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      897 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-da_DK.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1496 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-de_DE.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      952 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-de_DE.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1444 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-en_US.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      900 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-en_US.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1221 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_CL.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      807 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_CL.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1221 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_ES.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      807 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_ES.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1139 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-eu.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      737 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-eu.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1339 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-fa_IR.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      895 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-fa_IR.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1471 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-fi_FI.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      828 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-fi_FI.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1521 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-fr_FR.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      976 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-fr_FR.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1297 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-hu_HU.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      798 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-hu_HU.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1169 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-id_ID.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      757 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-id_ID.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1324 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-it_IT.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      860 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-it_IT.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1358 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ko_KR.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      859 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ko_KR.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1539 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-lt_LT.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      995 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-lt_LT.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1465 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-nb_NO.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      834 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-nb_NO.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1138 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-nl_NL.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      736 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-nl_NL.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1219 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-pl_PL.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      805 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-pl_PL.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1138 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_BR.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      736 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_BR.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1129 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_PT.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      751 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_PT.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1153 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ro_RO.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      751 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ro_RO.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1371 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ru_RU.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      947 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ru_RU.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1244 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-sk_SK.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      830 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-sk_SK.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1312 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-sl_SI.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      814 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-sl_SI.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1362 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-sv_SE.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      846 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-sv_SE.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1521 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-tr_TR.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      892 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-tr_TR.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1220 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ua_UA.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      818 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-ua_UA.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1115 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_CN.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      715 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_CN.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     1190 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_TW.js
--rw-r--r--   0 rhiem    (20243) staff       (20)      778 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_TW.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)    97163 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/jquery-1.12.4.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     3873 2017-05-10 07:15:44.000000 sampledb-0.8.1/sampledb/static/js/js.cookie.js
--rw-r--r--   0 rhiem    (20243) staff       (20)   452020 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/moment-with-locales.js
--rw-r--r--   0 rhiem    (20243) staff       (20)   249778 2017-05-08 07:45:54.000000 sampledb-0.8.1/sampledb/static/js/moment-with-locales.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)    55477 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/static/js/schema_editor.js
--rw-r--r--   0 rhiem    (20243) staff       (20)    39749 2018-09-19 13:29:03.000000 sampledb-0.8.1/sampledb/static/js/typeahead.bundle.min.js
--rw-r--r--   0 rhiem    (20243) staff       (20)     3331 2019-08-30 14:44:21.000000 sampledb-0.8.1/sampledb/utils.py
-drwxr-xr-x   0 rhiem    (20243) staff       (20)        0 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb.egg-info/
--rw-r--r--   0 rhiem    (20243) staff       (20)     3864 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb.egg-info/PKG-INFO
--rw-r--r--   0 rhiem    (20243) staff       (20)    14584 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb.egg-info/SOURCES.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)        1 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb.egg-info/dependency_links.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)     1397 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb.egg-info/requires.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)        9 2019-12-10 12:36:48.000000 sampledb-0.8.1/sampledb.egg-info/top_level.txt
--rw-r--r--   0 rhiem    (20243) staff       (20)       38 2019-12-10 12:36:48.000000 sampledb-0.8.1/setup.cfg
--rw-r--r--   0 rhiem    (20243) staff       (20)     1468 2019-12-10 12:35:01.000000 sampledb-0.8.1/setup.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      113 2020-06-17 11:59:04.000000 sampledb-0.9.0/.gitignore
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3585 2020-06-17 11:59:11.000000 sampledb-0.9.0/.gitlab-ci.yml
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3207 2020-06-17 11:59:04.000000 sampledb-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1140 2020-06-17 11:59:04.000000 sampledb-0.9.0/Dockerfile
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1089 2020-06-17 11:59:04.000000 sampledb-0.9.0/LICENSE
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       25 2020-06-17 11:59:04.000000 sampledb-0.9.0/MANIFEST.in
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3833 2020-06-17 11:59:20.000000 sampledb-0.9.0/PKG-INFO
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2738 2020-06-17 11:59:11.000000 sampledb-0.9.0/README.md
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)      959 2020-06-17 11:59:04.000000 sampledb-0.9.0/demo.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2155 2020-06-17 11:59:11.000000 sampledb-0.9.0/docs/changelog.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3848 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/conf.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/developer_guide/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    32277 2020-06-17 11:59:11.000000 sampledb-0.9.0/docs/developer_guide/api.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2691 2020-06-17 11:59:11.000000 sampledb-0.9.0/docs/developer_guide/configuration.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      730 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/index.rst
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/publications/
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/publications/joss/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      736 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/publications/joss/paper.bib
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      708 2020-06-17 11:59:11.000000 sampledb-0.9.0/docs/publications/joss/paper.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3852 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/publications/joss/paper.md
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/static/
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/static/css/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3265 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/css/custom.css
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/static/fonts/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2936 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-bold-italic-latin-ext.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    14812 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-bold-italic-latin.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2832 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-bold-latin-ext.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    14076 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-bold-latin.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2864 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-italic-latin-ext.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    14824 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-italic-latin.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2824 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-regular-latin-ext.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    13944 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/fonts/lato-regular-latin.woff2
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/static/img/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1606 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/static/img/logo64.png
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/user_guide/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     9015 2020-06-17 11:59:11.000000 sampledb-0.9.0/docs/user_guide/actions.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      747 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/user_guide/citations.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      658 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/user_guide/groups.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      849 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/user_guide/instruments.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11631 2020-06-17 11:59:11.000000 sampledb-0.9.0/docs/user_guide/objects.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      873 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/user_guide/projects.rst
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3782 2020-06-17 11:59:11.000000 sampledb-0.9.0/docs/user_guide/users.rst
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/docs/utils/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    20740 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/utils/generate_images.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    10279 2020-06-17 11:59:04.000000 sampledb-0.9.0/docs/utils/photo.jpg
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/example_data/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    14036 2020-06-17 11:59:11.000000 sampledb-0.9.0/example_data/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7460 2020-06-17 11:59:04.000000 sampledb-0.9.0/example_data/ombe-1.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1397 2020-06-17 11:59:11.000000 sampledb-0.9.0/requirements.txt
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1664 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      724 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/__main__.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/api/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       97 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/__init__.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/api/server/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3275 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1662 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1391 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/authentication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5845 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/files.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1164 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2885 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/locations.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7583 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/object_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     8094 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/api/server/objects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      943 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/api/server/users.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5339 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/config.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      827 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    14924 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2031 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/authentication_forms.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      884 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/errors.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      200 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/index.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4794 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    10580 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/labels.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     8543 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/locations.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11634 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/object_form_parser.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    64021 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/objects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3068 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/objects_forms.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    22923 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/pdfexport.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    25779 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/projects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2306 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/projects_forms.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      537 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/status.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      329 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/tags.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/actions/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2697 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/actions/action.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    18914 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/actions/action_form.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2615 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/actions/actions.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      886 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/api_log.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    15358 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/base.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2425 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/create_other_user.html
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/errors/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      158 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/errors/403.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      168 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/errors/404.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      182 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/errors/500.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      422 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/errors/user_is_readonly.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7333 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/group.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3160 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/groups.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3819 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/index.html
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/instruments/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1745 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/instruments/instrument.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2860 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/instruments/instrument_form.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      349 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/instruments/instrument_scientists.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1305 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/instruments/instruments.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1250 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/invitation.html
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/locations/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1214 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/locations/location.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2631 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/locations/location_form.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      837 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/locations/locations.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      602 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/locations/locations_tree.html
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4410 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/account_recovery.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3754 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/account_recovery.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2003 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/base.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      325 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/base.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      884 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/email_confirmation.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      245 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/email_confirmation.txt
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      201 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/announcement.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      103 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/announcement.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1134 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/assigned_as_responsible_user.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      423 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/assigned_as_responsible_user.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      476 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/base.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      316 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/base.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1222 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/invited_to_group.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      416 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/invited_to_group.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1238 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/invited_to_project.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      424 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/invited_to_project.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      111 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/other.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      103 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/other.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1156 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/received_object_permissions_request.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      425 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/received_object_permissions_request.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1351 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mobile_upload.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      568 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/mobile_upload_success.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     8851 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/notifications.html
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1072 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_any.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     8227 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_array.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2482 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_base.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1012 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_bool.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1568 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_create.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1087 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_datetime.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      906 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_edit.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3287 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_hazards.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1501 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_measurement.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1918 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_object.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1810 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_quantity.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1496 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_sample.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1639 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_select.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      818 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_any.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      814 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_datetime.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1501 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_measurement.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1472 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_quantity.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1496 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_sample.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1229 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_select.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      761 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_text.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      805 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_tags.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1229 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_text.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    22415 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/object_permissions.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      766 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/object_versions.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11520 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/objects.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      641 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/restore_object_version.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      620 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/unauthorized.html
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1001 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/any.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7702 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/array.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    56404 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/base.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1030 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/bool.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      628 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/datetime.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      829 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/hazards.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      779 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/measurement.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2135 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/object.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1249 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/quantity.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2931 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/related_objects.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      765 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/related_objects_tree_toggle.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      774 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/sample.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      944 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/select.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      756 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_any.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       80 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_datetime.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      561 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_measurement.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      282 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_quantity.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      556 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_sample.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      241 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_tags.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       15 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_text.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      515 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/tags.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      888 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/objects/view/text.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1262 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/password.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    34687 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/preferences.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2518 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/profile.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    17145 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/project.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11563 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/project_permissions.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3530 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/projects.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      657 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/recovery_email_send.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2582 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/registration.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1127 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/reset_password_by_email.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1919 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/search.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1960 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/templates/sign_in.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      499 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/sign_out.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      672 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/tags.html
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1567 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/templates/users.html
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/frontend/users/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      506 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      457 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/activity.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1218 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/api_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3683 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/users/authentication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1961 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/create_other_user.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2564 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/favorites.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1078 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/forms.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    10458 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/groups.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3693 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/invitation.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      358 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/list.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     6309 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/notifications.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    31325 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/preferences.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2544 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/frontend/users/profile.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1698 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/users_forms.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2246 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/frontend/utils.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/logic/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1465 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    15261 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/action_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4418 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/logic/actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1019 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/api_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11605 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/authentication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1881 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/comments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     9623 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/datatypes.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3034 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/errors.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3907 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/favorites.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    14000 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/files.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     9547 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/groups.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5882 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/logic/instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5108 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/ldap.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    13070 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/locations.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    18927 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/notifications.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5062 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/object_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    19785 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/object_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4935 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/object_relationships.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    39260 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/object_search.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    17309 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/logic/object_search_parser.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3725 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/object_sorting.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    12718 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/objects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    30380 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/projects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3711 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/publications.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/logic/schemas/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      612 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/schemas/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3465 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/schemas/convert_to_schema.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     6815 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/schemas/generate_placeholder.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      733 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/schemas/utils.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    18369 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/schemas/validate.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    21541 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/schemas/validate_schema.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      512 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/security_tokens.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3366 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/settings.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2311 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/tags.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       35 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/unit_definitions.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      658 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/units.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     6037 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/user_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2412 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/logic/users.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3246 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/utils.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5578 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/logic/where_filters.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/models/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2805 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1749 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/action_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1598 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/models/actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1260 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/api_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      931 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/authentication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1074 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/comments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      591 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/favorites.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1463 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/file_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1142 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/files.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      572 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/groups.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1149 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/models/instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2423 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/models/locations.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/models/migrations/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      760 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      696 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/actions_add_user_id.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      802 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/authentication_type_add_api_token.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      775 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/create_migration_index.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2941 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/create_user_object_permissions_by_all_view.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1360 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/files_add_data.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1033 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/object_location_assignments_add_confirmed.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      971 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/object_location_assignments_add_responsible_user_id.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      819 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/object_log_entry_type_add_assign_location.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      823 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/object_log_entry_type_add_link_publication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      603 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/user_add_is_hidden.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      609 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/user_add_is_readonly.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      813 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_assign_location.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      813 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_create_location.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      816 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_link_publication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      813 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_update_location.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2882 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/migrations/utils.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2138 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/notifications.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1503 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/object_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3389 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/object_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      412 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/object_publications.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      543 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/objects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      872 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1818 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/projects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      909 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/settings.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      265 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/tags.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1407 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/user_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1270 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/users.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    17748 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/models/versioned_json_object_tables.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/schemas/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1098 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/action.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      809 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/instrument.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      198 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/minimal.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1073 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/object.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3857 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/ombe_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3915 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/ombe_measurement_batch.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      410 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/searchable_quantity.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1481 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/schemas/xrr_measurement.sampledb.json
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/scripts/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1157 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2165 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/create_action.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      837 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/create_instrument.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      960 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/create_other_user.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1068 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/export_action_schema.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      436 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/list_actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      472 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/list_instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      918 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/run.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      690 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/send_announcement.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1255 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/scripts/set_administrator.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1200 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/set_user_hidden.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1225 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/set_user_readonly.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1447 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/update_action.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      995 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/update_instrument.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2250 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/scripts/update_instrument_responsible_users.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/static/
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/static/css/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    10963 2020-06-17 11:59:11.000000 sampledb-0.9.0/sampledb/static/css/base.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7785 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-datetimepicker.min.css
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)     7761 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-select.css
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)    16645 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-select.css.map
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)     6650 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-select.min.css
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)     1359 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-tagsinput.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    26132 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-theme.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    47706 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-theme.css.map
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    23409 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-theme.min.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    25648 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1590 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-toggle.min.css
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)      204 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap-treeview.min.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   146010 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   389287 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap.css.map
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   121200 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap.min.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   542194 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/bootstrap.min.css.map
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    37414 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/font-awesome.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    31000 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/font-awesome.min.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4600 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/pygments.css
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2017 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/css/schema_editor.css
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/static/fonts/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   134808 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/FontAwesome.otf
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   165742 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   444379 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   165548 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    98024 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    77160 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    20127 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   108738 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    45404 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    23424 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    18028 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/static/img/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2621 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs00.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     9952 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs01.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     6028 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs02.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     6593 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs03.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2625 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs04.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7357 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs05.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     8581 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs06.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2667 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs07.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7267 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs08.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7275 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/ghs09.png
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      771 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/img/jupyter-40.png
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/static/js/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    38510 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap-datetimepicker.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    69851 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap-select.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    39003 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap-select.js.map
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    33963 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap-select.min.js
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)     9464 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap-tagsinput.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4129 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap-toggle.min.js
+-rwxr-xr-x   0 rhiem    (20243) wheel        (0)    16735 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap-treeview.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    69707 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    37045 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/bootstrap.min.js
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb/static/js/i18n/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1852 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ar_AR.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1308 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ar_AR.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1730 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-bg_BG.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1186 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-bg_BG.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1521 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-cro_CRO.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      977 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-cro_CRO.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1137 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-cs_CZ.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      735 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-cs_CZ.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1459 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-da_DK.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      897 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-da_DK.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1496 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-de_DE.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      952 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-de_DE.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1444 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-en_US.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      900 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-en_US.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1221 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_CL.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      807 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_CL.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1221 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_ES.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      807 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_ES.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1139 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-eu.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      737 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-eu.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1339 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-fa_IR.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      895 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-fa_IR.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1471 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-fi_FI.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      828 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-fi_FI.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1521 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-fr_FR.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      976 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-fr_FR.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1297 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-hu_HU.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      798 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-hu_HU.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1169 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-id_ID.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      757 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-id_ID.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1324 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-it_IT.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      860 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-it_IT.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1358 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ko_KR.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      859 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ko_KR.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1539 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-lt_LT.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      995 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-lt_LT.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1465 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-nb_NO.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      834 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-nb_NO.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1138 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-nl_NL.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      736 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-nl_NL.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1219 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-pl_PL.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      805 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-pl_PL.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1138 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_BR.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      736 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_BR.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1129 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_PT.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      751 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_PT.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1153 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ro_RO.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      751 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ro_RO.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1371 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ru_RU.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      947 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ru_RU.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1244 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-sk_SK.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      830 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-sk_SK.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1312 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-sl_SI.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      814 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-sl_SI.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1362 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-sv_SE.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      846 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-sv_SE.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1521 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-tr_TR.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      892 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-tr_TR.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1220 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ua_UA.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      818 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-ua_UA.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1115 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_CN.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      715 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_CN.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1190 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_TW.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      778 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_TW.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    97163 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/jquery-1.12.4.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3873 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/js.cookie.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   452020 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/moment-with-locales.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   249778 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/moment-with-locales.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    56405 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/schema_editor.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    39749 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/static/js/typeahead.bundle.min.js
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3531 2020-06-17 11:59:04.000000 sampledb-0.9.0/sampledb/utils.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/sampledb.egg-info/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3833 2020-06-17 11:59:19.000000 sampledb-0.9.0/sampledb.egg-info/PKG-INFO
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    21471 2020-06-17 11:59:19.000000 sampledb-0.9.0/sampledb.egg-info/SOURCES.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)        1 2020-06-17 11:59:19.000000 sampledb-0.9.0/sampledb.egg-info/dependency_links.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1397 2020-06-17 11:59:19.000000 sampledb-0.9.0/sampledb.egg-info/requires.txt
+-rw-r--r--   0 rhiem    (20243) wheel        (0)        9 2020-06-17 11:59:19.000000 sampledb-0.9.0/sampledb.egg-info/top_level.txt
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/server_schemas/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      978 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/cad_simulation.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      978 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/cfd_simulation.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2586 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/crystal_growing_sample.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      978 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/fem_simulation.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1887 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/galaxi_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1597 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/mbe_aes_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1483 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/mbe_leed_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1309 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/mbe_rheed_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      976 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/mc_simulation.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     8747 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/ombe_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      811 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/other_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      753 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/other_sample.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      848 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/other_sample_batch.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      843 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/other_simulation.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2492 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/powder_diffractometer_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2908 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/powder_preparation_sample.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1234 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/simulation.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2592 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/single_crystal_diffractometer_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3252 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/squid_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3603 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/xrd_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3437 2020-06-17 11:59:04.000000 sampledb-0.9.0/server_schemas/xrr_measurement.sampledb.json
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       38 2020-06-17 11:59:20.000000 sampledb-0.9.0/setup.cfg
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1468 2020-06-17 11:59:11.000000 sampledb-0.9.0/setup.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/__init__.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/api/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       79 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/__init__.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/api/server/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       79 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3377 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2215 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_authentication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11088 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_files.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2495 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     6243 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_locations.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2922 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    23553 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_object_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    19219 2020-06-17 11:59:11.000000 sampledb-0.9.0/tests/api/server/test_objects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2114 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/api/server/test_users.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      819 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/conftest.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/frontend/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       79 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    10088 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_authentication.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4077 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_comments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7214 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_favorites.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7283 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_files.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11052 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_groups.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     8753 2020-06-17 11:59:11.000000 sampledb-0.9.0/tests/frontend/test_invitation.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1727 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_labels.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3660 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_object_pagination.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2566 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_object_sorting.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   128479 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_objects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4130 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_password.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3015 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_pdfexport.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    41361 2020-06-17 11:59:11.000000 sampledb-0.9.0/tests/frontend/test_preferences.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    34021 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_projects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1908 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/frontend/test_user_log.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/logic/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       79 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/__init__.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/logic/schemas/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       79 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/schemas/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5521 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/schemas/test_convert_to_schema.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     6944 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/schemas/test_generate_placeholder.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    31888 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/schemas/test_validate.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    42363 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/schemas/test_validate_schema.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    18633 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_action_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4478 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1564 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_add_user.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2539 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_build_recovery_url.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2301 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_comments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11101 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_datatypes.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3402 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_favorites.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     9548 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_files.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      979 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_get_user.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    22771 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_groups.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4329 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1803 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_ldap.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    12728 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_locations.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     7955 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_login.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5971 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_notifications.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3576 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_object_pagination.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    28507 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_object_permissions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5794 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_object_relationships.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    12807 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_object_sorting.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    15496 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_objects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    65185 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_projects.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3709 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_publications.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)   118371 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_search.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1780 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_send_confirmation_email.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     5020 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_send_recovery_email.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1925 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_settings.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2984 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_tags.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1125 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_token.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      878 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_units.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     3670 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_user_log.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1734 2020-06-17 11:59:11.000000 sampledb-0.9.0/tests/logic/test_users.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2416 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_validate_user.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    11381 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/logic/test_where_filters.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/models/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)    10998 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/models/test_objects.py
+drwxr-xr-x   0 rhiem    (20243) wheel        (0)        0 2020-06-17 11:59:20.000000 sampledb-0.9.0/tests/scripts/
+-rw-r--r--   0 rhiem    (20243) wheel        (0)       79 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/__init__.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4977 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_create_action.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1568 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_create_instrument.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1906 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_create_other_user.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2523 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_export_action_schema.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1411 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_list_actions.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)      921 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_list_instruments.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     1120 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_send_announcement.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2843 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_set_administrator.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2788 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_set_user_hidden.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2832 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_set_user_readonly.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4103 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_update_action.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2565 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_update_instrument.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     4455 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/scripts/test_update_instrument_responsible_users.py
+-rw-r--r--   0 rhiem    (20243) wheel        (0)     2422 2020-06-17 11:59:04.000000 sampledb-0.9.0/tests/test_utils.py
```

### Comparing `sampledb-0.8.1/PKG-INFO` & `sampledb-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampledb
-Version: 0.8.1
+Version: 0.9.0
 Summary: A sample and measurement metadata database
 Home-page: https://github.com/sciapp/sampledb
 Author: Florian Rhiem
 Author-email: f.rhiem@fz-juelich.de
 License: MIT
 Description: # SampleDB
         
@@ -42,15 +42,15 @@
             -e SAMPLEDB_CONTACT_EMAIL=sampledb@example.com \
             -e SAMPLEDB_SQLALCHEMY_DATABASE_URI=postgresql+psycopg2://postgres:@sampledb-postgres:5432/postgres \
             -e SAMPLEDB_FILE_STORAGE_PATH=/home/sampledb/files/ \
             -v `pwd`/files:/home/sampledb/files:rw \
             --restart=always \
             --name sampledb \
             -p 8000:8000 \
-            docker.pkg.github.com/sciapp/sampledb/sampledb:0.8.1
+            sciapp/sampledb:0.9.0
         ```
         
         This will start a basic SampleDB instance at `http://localhost:8000`.
         
         To use the administration scripts, run:
         
         ```bash
```

### Comparing `sampledb-0.8.1/README.md` & `sampledb-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     -e SAMPLEDB_CONTACT_EMAIL=sampledb@example.com \
     -e SAMPLEDB_SQLALCHEMY_DATABASE_URI=postgresql+psycopg2://postgres:@sampledb-postgres:5432/postgres \
     -e SAMPLEDB_FILE_STORAGE_PATH=/home/sampledb/files/ \
     -v `pwd`/files:/home/sampledb/files:rw \
     --restart=always \
     --name sampledb \
     -p 8000:8000 \
-    docker.pkg.github.com/sciapp/sampledb/sampledb:0.8.1
+    sciapp/sampledb:0.9.0
 ```
 
 This will start a basic SampleDB instance at `http://localhost:8000`.
 
 To use the administration scripts, run:
 
 ```bash
```

### Comparing `sampledb-0.8.1/requirements.txt` & `sampledb-0.9.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 beautifulsoup4==4.8.1
 blinker==1.4
 certifi==2019.9.11
 cffi==1.13.2
 chardet==3.0.4
 cheroot==8.2.1
 CherryPy==18.4.0
-chromedriver-binary==77.0.3865.40.0
+chromedriver-binary==79.0.3945.36.0
 Click==7.0
 coverage==4.5.4
 docutils==0.15.2
 Flask==1.1.1
 Flask-HTTPAuth==3.3.0
 Flask-Login==0.4.1
 Flask-Mail==0.9.1
```

### Comparing `sampledb-0.8.1/sampledb/__init__.py` & `sampledb-0.9.0/sampledb/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import flask
 from werkzeug.middleware.proxy_fix import ProxyFix
 from flask_login import LoginManager
 from flask_mail import Mail
 from flask_sqlalchemy import SQLAlchemy
 
 login_manager = LoginManager()
-login_manager.session_protection = 'strong'
+login_manager.session_protection = 'basic'
 
 mail = Mail()
 db = SQLAlchemy()
 
 import sampledb.frontend
 import sampledb.api
 import sampledb.logic
```

### Comparing `sampledb-0.8.1/sampledb/__main__.py` & `sampledb-0.9.0/sampledb/__main__.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/api/server/__init__.py` & `sampledb-0.9.0/sampledb/api/server/__init__.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/api/server/actions.py` & `sampledb-0.9.0/sampledb/api/server/actions.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 RESTful API for iffSamples
 """
 
 import flask
 from flask_restful import Resource
 
-from .authentication import http_basic_auth
+from .authentication import multi_auth
 from ...logic.actions import get_action, ActionType
 from ...logic.action_permissions import get_user_action_permissions, get_actions_with_permissions, Permissions
 from ...logic import errors
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 
@@ -26,15 +26,15 @@
         'name': action.name,
         'description': action.description,
         'schema': action.schema
     }
 
 
 class Action(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self, action_id: int):
         try:
             action = get_action(action_id=action_id)
         except errors.ActionDoesNotExistError:
             return {
                 "message": "action {} does not exist".format(action_id)
             }, 404
@@ -42,11 +42,11 @@
             return {
                 "message": "insufficient permissions to access action {}".format(action_id)
             }, 403
         return action_to_json(action)
 
 
 class Actions(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self):
         actions = get_actions_with_permissions(user_id=flask.g.user.id, permissions=Permissions.READ)
         return [action_to_json(action) for action in actions]
```

### Comparing `sampledb-0.8.1/sampledb/api/server/authentication.py` & `sampledb-0.9.0/sampledb/api/server/authentication.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # coding: utf-8
 """
 Authentication functions for the iffSamples RESTful API.
 """
 
 import flask
 
-from flask_httpauth import HTTPBasicAuth
+from flask_httpauth import HTTPBasicAuth, HTTPTokenAuth, MultiAuth
 
-from sampledb.logic.authentication import login
+from sampledb.logic.authentication import login, login_via_api_token
 from sampledb.logic.object_permissions import Permissions
 from sampledb.utils import object_permissions_required as object_permissions_required_generic
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 http_basic_auth = HTTPBasicAuth()
+http_token_auth = HTTPTokenAuth(scheme='Bearer')
+multi_auth = MultiAuth(http_basic_auth, http_token_auth)
+
+
+@http_token_auth.verify_token
+def verify_token(api_token):
+    if not api_token:
+        return None
+    flask.g.user = login_via_api_token(api_token)
+    return flask.g.user
 
 
 @http_basic_auth.verify_password
 def verify_password(username, password):
     if not username:
         return None
     flask.g.user = login(username, password)
@@ -29,8 +39,8 @@
     Only allow access to a route it the user has the required permissions.
 
     Wrapper around the more generic sampledb.utils.object_permissions_required
     for use with the http_basic_auth object from this module.
 
     :param permissions: the required object permissions
     """
-    return object_permissions_required_generic(permissions, http_basic_auth, lambda: flask.g.user.id)
+    return object_permissions_required_generic(permissions, multi_auth, lambda: flask.g.user.id)
```

### Comparing `sampledb-0.8.1/sampledb/api/server/files.py` & `sampledb-0.9.0/sampledb/api/server/files.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/api/server/instruments.py` & `sampledb-0.9.0/sampledb/api/server/instruments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 """
 RESTful API for iffSamples
 """
 
 from flask_restful import Resource
 
-from sampledb.api.server.authentication import http_basic_auth
+from sampledb.api.server.authentication import multi_auth
 from sampledb.logic.instruments import get_instrument, get_instruments
 from sampledb.logic import errors
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 
 def instrument_to_json(instrument):
@@ -18,23 +18,23 @@
         'name': instrument.name,
         'description': instrument.description,
         'instrument_scientists': [user.id for user in instrument.responsible_users]
     }
 
 
 class Instrument(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self, instrument_id: int):
         try:
             instrument = get_instrument(instrument_id=instrument_id)
         except errors.InstrumentDoesNotExistError:
             return {
                 "message": "instrument {} does not exist".format(instrument_id)
             }, 404
         return instrument_to_json(instrument)
 
 
 class Instruments(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self):
         instruments = get_instruments()
         return [instrument_to_json(instrument) for instrument in instruments]
```

### Comparing `sampledb-0.8.1/sampledb/api/server/locations.py` & `sampledb-0.9.0/sampledb/api/server/locations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 """
 RESTful API for iffSamples
 """
 
 from flask_restful import Resource
 
-from .authentication import http_basic_auth
+from .authentication import multi_auth
 from ...logic import errors, locations
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 
 def location_to_json(location: locations.Location):
     return {
@@ -28,33 +28,33 @@
         'user_id': object_location_assignment.user_id,
         'description': object_location_assignment.description,
         'utc_datetime': object_location_assignment.utc_datetime.strftime('%Y-%m-%d %H:%M:%S')
     }
 
 
 class Location(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self, location_id: int):
         try:
             location = locations.get_location(location_id=location_id)
         except errors.LocationDoesNotExistError:
             return {
                 "message": "location {} does not exist".format(location_id)
             }, 404
         return location_to_json(location)
 
 
 class Locations(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self):
         return [location_to_json(location) for location in locations.get_locations()]
 
 
 class ObjectLocationAssignment(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self, object_id: id, object_location_assignment_index: int):
         try:
             object_location_assignments = locations.get_object_location_assignments(object_id=object_id)
         except errors.ObjectDoesNotExistError:
             return {
                 "message": "object {} does not exist".format(object_id)
             }, 404
@@ -62,15 +62,15 @@
             return {
                 "message": "location assignment {} for object {} does not exist".format(object_location_assignment_index, object_id)
             }, 404
         return object_location_assignment_to_json(object_location_assignments[object_location_assignment_index])
 
 
 class ObjectLocationAssignments(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self, object_id: int):
         try:
             return [
                 object_location_assignment_to_json(object_location_assignment)
                 for object_location_assignment in locations.get_object_location_assignments(object_id)
             ]
         except errors.ObjectDoesNotExistError:
```

### Comparing `sampledb-0.8.1/sampledb/api/server/object_permissions.py` & `sampledb-0.9.0/sampledb/api/server/object_permissions.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/api/server/objects.py` & `sampledb-0.9.0/sampledb/api/server/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import json
 import flask
 
 from flask_restful import Resource
 
-from sampledb.api.server.authentication import http_basic_auth, object_permissions_required, Permissions
+from sampledb.api.server.authentication import multi_auth, object_permissions_required, Permissions
 from sampledb.logic.actions import get_action
 from sampledb.logic.objects import get_object, update_object, create_object
 from sampledb.logic.object_permissions import get_objects_with_permissions
 from sampledb.logic import errors
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
@@ -111,15 +111,15 @@
             object_id=object.object_id,
             version_id=object.version_id
         )
         return flask.redirect(object_version_url, code=302)
 
 
 class Objects(Resource):
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def get(self):
         # TODO: implement filters
         def filter_func(data):
             return True
         action_id = None
         action_type = None
         project_id = None
@@ -144,16 +144,20 @@
                 'action_id': object.action_id,
                 'schema': object.schema,
                 'data': object.data
             }
             for object in objects
         ]
 
-    @http_basic_auth.login_required
+    @multi_auth.login_required
     def post(self):
+        if flask.g.user.is_readonly:
+            return {
+                'message': 'user has been marked as read only'
+            }, 400
         request_json = flask.request.get_json(force=True)
         if not isinstance(request_json, dict):
             return {
                 "message": "JSON object body required"
             }, 400
         for key in request_json:
             if key not in {'object_id', 'version_id', 'action_id', 'schema', 'data'}:
```

### Comparing `sampledb-0.8.1/sampledb/config.py` & `sampledb-0.9.0/sampledb/config.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/__init__.py` & `sampledb-0.9.0/sampledb/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/actions.py` & `sampledb-0.9.0/sampledb/frontend/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from ..logic.action_permissions import Permissions, action_is_public, get_user_action_permissions, set_action_public
 from ..logic.favorites import get_user_favorite_action_ids
 from ..logic.instruments import get_instrument, get_user_instruments
 from ..logic import errors, users
 from ..logic.schemas.validate_schema import validate_schema
 from ..logic.settings import get_user_settings
 from .users.forms import ToggleFavoriteActionForm
+from .utils import check_current_user_is_not_readonly
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 
 class ActionForm(FlaskForm):
     name = StringField(validators=[Length(min=1, max=100)])
     description = StringField()
@@ -35,14 +36,15 @@
         ('sample', 'Sample Creation'),
         ('measurement', 'Measurement'),
         ('simulation', 'Simulation')
     ])
     instrument = SelectField()
     schema = StringField(validators=[InputRequired()])
     is_public = BooleanField()
+    is_user_specific = BooleanField(default=True)
 
 
 @frontend.route('/actions/')
 @flask_login.login_required
 def actions():
     action_type = flask.request.args.get('t', None)
     action_type = {
@@ -99,14 +101,15 @@
         return flask.abort(404)
     permissions = get_user_action_permissions(action_id, flask_login.current_user.id)
     if Permissions.READ not in permissions:
         return flask.abort(403)
     may_edit = Permissions.WRITE in permissions
     mode = flask.request.args.get('mode', None)
     if mode == 'edit':
+        check_current_user_is_not_readonly()
         if not may_edit:
             return flask.abort(403)
         return show_action_form(action)
     return flask.render_template(
         'actions/action.html',
         action=action,
         ActionType=ActionType,
@@ -114,14 +117,15 @@
         is_public=action_is_public(action_id)
     )
 
 
 @frontend.route('/actions/new/', methods=['GET', 'POST'])
 @flask_login.login_required
 def new_action():
+    check_current_user_is_not_readonly()
     previous_action = None
     previous_action_id = flask.request.args.get('previous_action_id', None)
     if previous_action_id is not None:
         try:
             previous_action_id = int(previous_action_id)
         except ValueError:
             previous_action_id = None
@@ -203,14 +207,15 @@
                     'type': 'text'
                 }
             },
             'required': ['name']
         }, indent=2)
         submit_text = "Create"
     may_change_public = action is None or action.user_id is not None
+    may_set_user_specific = action is None and flask_login.current_user.is_admin
     schema = None
     pygments_output = None
     error_message = None
     action_form = ActionForm()
     if action is not None:
         if action.instrument_id:
             action_form.instrument.choices = [
@@ -327,15 +332,19 @@
         try:
             instrument_id = int(instrument_id)
         except ValueError:
             instrument_id = None
         if instrument_id < 0:
             instrument_id = None
         if action is None:
-            action = create_action(action_type, name, description, schema, instrument_id, flask_login.current_user.id)
+            if action_form.is_user_specific.data or not may_set_user_specific:
+                user_id = flask_login.current_user.id
+            else:
+                user_id = None
+            action = create_action(action_type, name, description, schema, instrument_id, user_id)
             flask.flash('The action was created successfully.', 'success')
             if may_change_public and is_public:
                 set_action_public(action.id, True)
         else:
             update_action(action.id, name, description, schema)
             flask.flash('The action was updated successfully.', 'success')
             if may_change_public and is_public is not None:
@@ -348,9 +357,10 @@
         pygments_output=pygments_output,
         error_message=error_message,
         schema_json=schema_json,
         submit_text=submit_text,
         use_schema_editor=use_schema_editor,
         may_change_type=action is None,
         may_change_instrument=action is None,
+        may_set_user_specific=may_set_user_specific,
         may_change_public=may_change_public
     )
```

### Comparing `sampledb-0.8.1/sampledb/frontend/authentication_forms.py` & `sampledb-0.9.0/sampledb/frontend/authentication_forms.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/labels.py` & `sampledb-0.9.0/sampledb/frontend/labels.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/locations.py` & `sampledb-0.9.0/sampledb/frontend/locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import typing
 
 from . import frontend
 from ..logic import errors
 from ..logic.locations import Location, create_location, get_location, get_locations_tree, update_location, get_object_location_assignment, confirm_object_responsibility
 from ..logic.security_tokens import verify_token
 from ..logic.notifications import mark_notification_for_being_assigned_as_responsible_user_as_read
+from .utils import check_current_user_is_not_readonly
 
 
 class LocationForm(FlaskForm):
     name = StringField(validators=[Length(min=1, max=100)])
     description = StringField()
     parent_location = SelectField()
 
@@ -39,14 +40,15 @@
 def location(location_id):
     try:
         location = get_location(location_id)
     except errors.LocationDoesNotExistError:
         return flask.abort(404)
     mode = flask.request.args.get('mode', None)
     if mode == 'edit':
+        check_current_user_is_not_readonly()
         return _show_location_form(location, None)
     locations_map, locations_tree = get_locations_tree()
     ancestors = []
     parent_location = location
     while parent_location.parent_location_id is not None:
         parent_location = get_location(parent_location.parent_location_id)
         ancestors.insert(0, (parent_location.id, parent_location.name))
@@ -60,14 +62,15 @@
         sort_location_ids_by_name=_sort_location_ids_by_name
     )
 
 
 @frontend.route('/locations/new/', methods=['GET', 'POST'])
 @flask_login.login_required
 def new_location():
+    check_current_user_is_not_readonly()
     parent_location = None
     parent_location_id = flask.request.args.get('parent_location_id', None)
     if parent_location_id is not None:
         try:
             parent_location_id = int(parent_location_id)
         except ValueError:
             parent_location_id = None
```

### Comparing `sampledb-0.8.1/sampledb/frontend/object_form_parser.py` & `sampledb-0.9.0/sampledb/frontend/object_form_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         return parse_object_form_data(form_data, schema, id_prefix, errors, required=required)
     elif schema.get('type') == 'array':
         return parse_array_form_data(form_data, schema, id_prefix, errors, required=required)
     elif schema.get('type') == 'text':
         return parse_text_form_data(form_data, schema, id_prefix, errors, required=required)
     elif schema.get('type') == 'sample':
         return parse_sample_form_data(form_data, schema, id_prefix, errors, required=required)
+    elif schema.get('type') == 'measurement':
+        return parse_measurement_form_data(form_data, schema, id_prefix, errors, required=required)
     elif schema.get('type') == 'datetime':
         return parse_datetime_form_data(form_data, schema, id_prefix, errors, required=required)
     elif schema.get('type') == 'bool':
         return parse_boolean_form_data(form_data, schema, id_prefix, errors, required=required)
     elif schema.get('type') == 'quantity':
         return parse_quantity_form_data(form_data, schema, id_prefix, errors, required=required)
     elif schema.get('type') == 'tags':
@@ -146,14 +148,37 @@
         'object_id': object_id
     }
     schemas.validate(data, schema)
     return data
 
 
 @form_data_parser
+def parse_measurement_form_data(form_data, schema, id_prefix, errors, required=False):
+    keys = [key for key in form_data.keys() if key.startswith(id_prefix + '__')]
+    if keys != [id_prefix + '__oid']:
+        raise ValueError('invalid measurement form data')
+    object_id = form_data.get(id_prefix + '__oid', [''])[0]
+    if not object_id:
+        if not required:
+            return None
+        else:
+            raise ValueError('Please select a measurement.')
+    try:
+        object_id = int(object_id)
+    except ValueError:
+        raise ValueError('object_id must be int')
+    data = {
+        '_type': 'measurement',
+        'object_id': object_id
+    }
+    schemas.validate(data, schema)
+    return data
+
+
+@form_data_parser
 def parse_quantity_form_data(form_data, schema, id_prefix, errors, required=False):
     keys = [key for key in form_data.keys() if key.startswith(id_prefix + '__')]
     # TODO: validate schema?
     if set(keys) != {id_prefix + '__magnitude', id_prefix + '__units'} and keys != [id_prefix + '__magnitude']:
         raise ValueError('invalid quantity form data')
     magnitude = form_data[id_prefix + '__magnitude'][0].strip()
     if not magnitude:
```

### Comparing `sampledb-0.8.1/sampledb/frontend/objects.py` & `sampledb-0.9.0/sampledb/frontend/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,27 @@
 from ..logic.errors import GroupDoesNotExistError, ObjectDoesNotExistError, UserDoesNotExistError, ActionDoesNotExistError, ValidationError, ProjectDoesNotExistError, LocationDoesNotExistError
 from .objects_forms import ObjectPermissionsForm, ObjectForm, ObjectVersionRestoreForm, ObjectUserPermissionsForm, CommentForm, ObjectGroupPermissionsForm, ObjectProjectPermissionsForm, FileForm, FileInformationForm, FileHidingForm, ObjectLocationAssignmentForm, ExternalLinkForm, ObjectPublicationForm
 from ..utils import object_permissions_required
 from .utils import jinja_filter, generate_qrcode
 from .object_form_parser import parse_form_data
 from .labels import create_labels
 from .pdfexport import create_pdfexport
+from .utils import check_current_user_is_not_readonly
 
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 
 def on_unauthorized(object_id):
-    return flask.render_template('objects/unauthorized.html', object_id=object_id), 403
+    permissions_by_user = get_object_permissions_for_users(object_id)
+    has_grant_user = any(
+        Permissions.GRANT in permissions
+        for permissions in permissions_by_user.values()
+    )
+    return flask.render_template('objects/unauthorized.html', object_id=object_id, has_grant_user=has_grant_user), 403
 
 
 @frontend.route('/objects/')
 @flask_login.login_required
 def objects():
     object_ids = flask.request.args.get('ids', '')
     objects = []
@@ -311,33 +317,40 @@
             'display_properties': {}
         }
 
     # TODO: select display_properties? nested display_properties? find common properties? use searched for properties?
     display_properties = []
     display_property_titles = {}
     sample_ids = set()
+    measurement_ids = set()
     if action is not None:
         action_schema = action.schema
         display_properties = action_schema.get('displayProperties', [])
         for property_name in display_properties:
             display_property_titles[property_name] = action_schema['properties'][property_name]['title']
 
     for obj in objects:
         for property_name in display_properties:
             if property_name not in obj['data'] or '_type' not in obj['data'][property_name] or property_name not in obj['schema']['properties']:
                 obj['display_properties'][property_name] = None
                 continue
             obj['display_properties'][property_name] = (obj['data'][property_name], obj['schema']['properties'][property_name])
             if obj['schema']['properties'][property_name]['type'] == 'sample':
                 sample_ids.add(obj['data'][property_name]['object_id'])
+            elif obj['schema']['properties'][property_name]['type'] == 'measurement':
+                measurement_ids.add(obj['data'][property_name]['object_id'])
 
     samples = {
         sample_id: get_object(object_id=sample_id)
         for sample_id in sample_ids
     }
+    measurements = {
+        measurement_id: get_object(object_id=measurement_id)
+        for measurement_id in measurement_ids
+    }
     if action_id is None:
         show_action = True
     else:
         show_action = False
 
     def build_modified_url(**kwargs):
         return flask.url_for(
@@ -359,14 +372,15 @@
         project_id=project_id,
         location_id=location_id,
         location=location,
         user_id=user_id,
         user=user,
         doi=doi,
         samples=samples,
+        measurements=measurements,
         build_modified_url=build_modified_url,
         sorting_property=sorting_property_name,
         sorting_order=sorting_order_name,
         limit=limit,
         offset=offset,
         pagination_enabled=pagination_enabled,
         num_objects_found=num_objects_found,
@@ -607,20 +621,66 @@
 
     # TODO: make this search more narrow
     samples = get_objects_with_permissions(
         user_id=flask_login.current_user.id,
         permissions=Permissions.READ,
         action_type=ActionType.SAMPLE_CREATION
     )
+    measurements = get_objects_with_permissions(
+        user_id=flask_login.current_user.id,
+        permissions=Permissions.READ,
+        action_type=ActionType.MEASUREMENT
+    )
+    if object is not None:
+        samples = [
+            sample
+            for sample in samples
+            if sample.object_id != object.object_id
+        ]
+        measurements = [
+            measurement
+            for measurement in measurements
+            if measurement.object_id != object.object_id
+        ]
 
     tags = [{'name': tag.name, 'uses': tag.uses} for tag in logic.tags.get_tags()]
     if object is None:
-        return flask.render_template('objects/forms/form_create.html', action_id=action_id, schema=schema, data=data, errors=errors, object_errors=object_errors, form_data=form_data, previous_actions=serializer.dumps(previous_actions), form=form, samples=samples, datetime=datetime, tags=tags, previous_object_id=previous_object_id)
+        return flask.render_template(
+            'objects/forms/form_create.html',
+            action_id=action_id,
+            schema=schema,
+            data=data,
+            errors=errors,
+            object_errors=object_errors,
+            form_data=form_data,
+            previous_actions=serializer.dumps(previous_actions),
+            form=form,
+            samples=samples,
+            measurements=measurements,
+            datetime=datetime,
+            tags=tags,
+            previous_object_id=previous_object_id
+        )
     else:
-        return flask.render_template('objects/forms/form_edit.html', schema=schema, data=data, object_id=object.object_id, errors=errors, object_errors=object_errors, form_data=form_data, previous_actions=serializer.dumps(previous_actions), form=form, samples=samples, datetime=datetime, tags=tags, mode=mode)
+        return flask.render_template(
+            'objects/forms/form_edit.html',
+            schema=schema,
+            data=data,
+            object_id=object.object_id,
+            errors=errors,
+            object_errors=object_errors,
+            form_data=form_data,
+            previous_actions=serializer.dumps(previous_actions),
+            form=form,
+            samples=samples,
+            measurements=measurements,
+            datetime=datetime,
+            tags=tags,
+            mode=mode
+        )
 
 
 @frontend.route('/objects/<int:object_id>', methods=['GET', 'POST'])
 @object_permissions_required(Permissions.READ, on_unauthorized=on_unauthorized)
 def object(object_id):
     object = get_object(object_id=object_id)
     related_objects_tree = logic.object_relationships.build_related_objects_tree(object_id, flask_login.current_user.id)
@@ -640,14 +700,19 @@
     if flask.request.method == 'GET' and flask.request.args.get('mode', '') not in ('edit', 'upgrade'):
         # TODO: make this search more narrow
         samples = get_objects_with_permissions(
             user_id=flask_login.current_user.id,
             permissions=Permissions.READ,
             action_type=ActionType.SAMPLE_CREATION
         )
+        measurements = get_objects_with_permissions(
+            user_id=flask_login.current_user.id,
+            permissions=Permissions.READ,
+            action_type=ActionType.MEASUREMENT
+        )
         instrument = action.instrument
         object_type = {
             ActionType.SAMPLE_CREATION: "Sample",
             ActionType.MEASUREMENT: "Measurement",
             ActionType.SIMULATION: "Simulation"
         }.get(action.type, "Object")
         object_log_entries = object_log.get_object_log_entries(object_id=object_id, user_id=flask_login.current_user.id)
@@ -673,15 +738,15 @@
             location = locations_map[location_id]
             locations.append((str(location_id), '{}{} (#{})'.format(prefix, location.name, location.id)))
             for location_id in sorted(subtree, key=lambda location_id: locations_map[location_id].name, reverse=True):
                 unvisited_location_ids_prefixes_and_subtrees.insert(0, (location_id, '{}{} / '.format(prefix, location.name), subtree[location_id]))
 
         location_form.location.choices = locations
         possible_responsible_users = [('-1', '—')]
-        for user in logic.users.get_users():
+        for user in logic.users.get_users(exclude_hidden=True):
             possible_responsible_users.append((str(user.id), '{} (#{})'.format(user.name, user.id)))
         location_form.responsible_user.choices = possible_responsible_users
 
         measurement_actions = logic.actions.get_actions(logic.actions.ActionType.MEASUREMENT)
         favorite_action_ids = logic.favorites.get_user_favorite_action_ids(flask_login.current_user.id)
         favorite_measurement_actions = [
             action
@@ -757,14 +822,15 @@
             notebook_templates=notebook_templates,
             object_qrcode=object_qrcode,
             object_url=object_url,
             restore_form=None,
             version_id=object.version_id,
             user_may_grant=user_may_grant,
             samples=samples,
+            measurements=measurements,
             favorite_measurement_actions=favorite_measurement_actions,
             FileLogEntryType=FileLogEntryType,
             file_information_form=FileInformationForm(),
             file_hiding_form=FileHidingForm(),
             new_schema_available=new_schema_available,
             related_objects_tree=related_objects_tree,
             object_publications=object_publications,
@@ -775,14 +841,15 @@
             get_user=get_user,
             get_location=get_location,
             object_location_assignments=get_object_location_assignments(object_id),
             build_object_location_assignment_confirmation_url=build_object_location_assignment_confirmation_url,
             user_may_assign_location=user_may_edit,
             location_form=location_form
         )
+    check_current_user_is_not_readonly()
     if flask.request.args.get('mode', '') == 'upgrade':
         should_upgrade_schema = True
     else:
         should_upgrade_schema = False
     return show_object_form(object, action=get_action(object.action_id), should_upgrade_schema=should_upgrade_schema)
 
 
@@ -827,14 +894,15 @@
         cache_timeout=-1
     )
 
 
 @frontend.route('/objects/<int:object_id>/comments/', methods=['POST'])
 @object_permissions_required(Permissions.WRITE)
 def post_object_comments(object_id):
+    check_current_user_is_not_readonly()
     comment_form = CommentForm()
     if comment_form.validate_on_submit():
         content = comment_form.content.data
         comments.create_comment(object_id=object_id, user_id=flask_login.current_user.id, content=content)
         flask.flash('Successfully posted a comment.', 'success')
     else:
         flask.flash('Please enter a comment text.', 'error')
@@ -858,21 +926,22 @@
     flask.flash('Your request for permissions has been sent.', 'success')
     return flask.redirect(flask.url_for('.objects'))
 
 
 @frontend.route('/objects/<int:object_id>/locations/', methods=['POST'])
 @object_permissions_required(Permissions.WRITE)
 def post_object_location(object_id):
+    check_current_user_is_not_readonly()
     location_form = ObjectLocationAssignmentForm()
     location_form.location.choices = [('-1', '—')] + [
         (str(location.id), '{} (#{})'.format(location.name, location.id))
         for location in get_locations()
     ]
     possible_responsible_users = [('-1', '—')]
-    for user in logic.users.get_users():
+    for user in logic.users.get_users(exclude_hidden=True):
         possible_responsible_users.append((str(user.id), '{} (#{})'.format(user.name, user.id)))
     location_form.responsible_user.choices = possible_responsible_users
     if location_form.validate_on_submit():
         location_id = int(location_form.location.data)
         if location_id < 0:
             location_id = None
         responsible_user_id = int(location_form.responsible_user.data)
@@ -888,14 +957,15 @@
         flask.flash('Please select a location or a responsible user.', 'error')
     return flask.redirect(flask.url_for('.object', object_id=object_id))
 
 
 @frontend.route('/objects/<int:object_id>/publications/', methods=['POST'])
 @object_permissions_required(Permissions.WRITE)
 def post_object_publication(object_id):
+    check_current_user_is_not_readonly()
     publication_form = ObjectPublicationForm()
     if publication_form.validate_on_submit():
         doi = publication_form.doi.data
         title = publication_form.title.data
         if not title:
             title = None
         existing_publication = ([
@@ -957,14 +1027,15 @@
     # TODO: better error handling
     return flask.abort(404)
 
 
 @frontend.route('/objects/<int:object_id>/files/<int:file_id>', methods=['POST'])
 @object_permissions_required(Permissions.WRITE)
 def update_file_information(object_id, file_id):
+    check_current_user_is_not_readonly()
     form = FileInformationForm()
     if not form.validate_on_submit():
         return flask.abort(400)
     title = form.title.data
     description = form.description.data
     try:
         logic.files.update_file_information(
@@ -978,14 +1049,15 @@
         return flask.abort(404)
     return flask.redirect(flask.url_for('.object', object_id=object_id, _anchor='file-{}'.format(file_id)))
 
 
 @frontend.route('/objects/<int:object_id>/files/<int:file_id>/hide', methods=['POST'])
 @object_permissions_required(Permissions.WRITE)
 def hide_file(object_id, file_id):
+    check_current_user_is_not_readonly()
     form = FileHidingForm()
     if not form.validate_on_submit():
         return flask.abort(400)
     reason = form.reason.data
     try:
         logic.files.hide_file(
             object_id=object_id,
@@ -997,24 +1069,26 @@
         return flask.abort(404)
     flask.flash('The file was hidden successfully.', 'success')
     return flask.redirect(flask.url_for('.object', object_id=object_id, _anchor='file-{}'.format(file_id)))
 
 
 @frontend.route('/objects/<int:object_id>/files/mobile_upload/<token>', methods=['GET'])
 def mobile_file_upload(object_id: int, token: str):
+    check_current_user_is_not_readonly()
     serializer = itsdangerous.URLSafeTimedSerializer(flask.current_app.config['SECRET_KEY'], salt='mobile-upload')
     try:
         user_id, object_id = serializer.loads(token, max_age=15 * 60)
     except itsdangerous.BadSignature:
         return flask.abort(400)
     return flask.render_template('mobile_upload.html', user_id=logic.users.get_user(user_id), object=logic.objects.get_object(object_id))
 
 
 @frontend.route('/objects/<int:object_id>/files/mobile_upload/<token>', methods=['POST'])
 def post_mobile_file_upload(object_id: int, token: str):
+    check_current_user_is_not_readonly()
     serializer = itsdangerous.URLSafeTimedSerializer(flask.current_app.config['SECRET_KEY'], salt='mobile-upload')
     try:
         user_id, object_id = serializer.loads(token, max_age=15 * 60)
     except itsdangerous.BadSignature:
         return flask.abort(400)
     files = flask.request.files.getlist('file_input')
     for file_storage in files:
@@ -1022,14 +1096,15 @@
         logic.files.create_local_file(object_id, user_id, file_name, lambda stream: file_storage.save(dst=stream))
     return flask.render_template('mobile_upload_success.html', num_files=len(files))
 
 
 @frontend.route('/objects/<int:object_id>/files/', methods=['POST'])
 @object_permissions_required(Permissions.WRITE)
 def post_object_files(object_id):
+    check_current_user_is_not_readonly()
     external_link_form = ExternalLinkForm()
     file_form = FileForm()
     if file_form.validate_on_submit():
         file_source = file_form.file_source.data
         if file_source == 'local':
             files = flask.request.files.getlist(file_form.local_files.name)
             for file_storage in files:
@@ -1049,14 +1124,15 @@
         flask.flash('Failed to upload files.', 'error')
     return flask.redirect(flask.url_for('.object', object_id=object_id))
 
 
 @frontend.route('/objects/new', methods=['GET', 'POST'])
 @flask_login.login_required
 def new_object():
+    check_current_user_is_not_readonly()
     action_id = flask.request.args.get('action_id', None)
     previous_object_id = flask.request.args.get('previous_object_id', None)
     if not action_id and not previous_object_id:
         # TODO: handle error
         return flask.abort(404)
 
     sample_id = flask.request.args.get('sample_id', None)
@@ -1166,18 +1242,19 @@
         return flask.redirect(flask.url_for('.object', object_id=object_id))
     return flask.render_template('objects/restore_object_version.html', object_id=object_id, version_id=version_id, restore_form=form)
 
 
 @frontend.route('/objects/<int:object_id>/permissions')
 @object_permissions_required(Permissions.READ, on_unauthorized=on_unauthorized)
 def object_permissions(object_id):
+    check_current_user_is_not_readonly()
     object = get_object(object_id)
     action = get_action(object.action_id)
     instrument = action.instrument
-    user_permissions = get_object_permissions_for_users(object_id=object_id, include_instrument_responsible_users=False, include_groups=False, include_projects=False)
+    user_permissions = get_object_permissions_for_users(object_id=object_id, include_instrument_responsible_users=False, include_groups=False, include_projects=False, include_readonly=False)
     group_permissions = get_object_permissions_for_groups(object_id=object_id, include_projects=False)
     project_permissions = get_object_permissions_for_projects(object_id=object_id)
     public_permissions = Permissions.READ if object_is_public(object_id) else Permissions.NONE
     suggested_user_id = flask.request.args.get('add_user_id', '')
     try:
         suggested_user_id = int(suggested_user_id)
     except ValueError:
@@ -1195,15 +1272,15 @@
             group_permission_form_data.append({'group_id': group_id, 'permissions': permissions.name.lower()})
         project_permission_form_data = []
         for project_id, permissions in project_permissions.items():
             if project_id is None:
                 continue
             project_permission_form_data.append({'project_id': project_id, 'permissions': permissions.name.lower()})
         edit_user_permissions_form = ObjectPermissionsForm(public_permissions=public_permissions.name.lower(), user_permissions=user_permission_form_data, group_permissions=group_permission_form_data, project_permissions=project_permission_form_data)
-        users = get_users()
+        users = get_users(exclude_hidden=True)
         users = [user for user in users if user.id not in user_permissions]
         add_user_permissions_form = ObjectUserPermissionsForm()
         groups = get_user_groups(flask_login.current_user.id)
         groups = [group for group in groups if group.id not in group_permissions]
         add_group_permissions_form = ObjectGroupPermissionsForm()
         projects = get_user_projects(flask_login.current_user.id, include_groups=True)
         projects = [project for project in projects if project.id not in project_permissions]
```

### Comparing `sampledb-0.8.1/sampledb/frontend/objects_forms.py` & `sampledb-0.9.0/sampledb/frontend/objects_forms.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/pdfexport.py` & `sampledb-0.9.0/sampledb/frontend/pdfexport.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,16 @@
         _handle_text(data, schema, path, canvas)
     elif schema['type'] == 'bool':
         _handle_bool(data, schema, path, canvas)
     elif schema['type'] == 'quantity':
         _handle_quantity(data, schema, path, canvas)
     elif schema['type'] == 'sample':
         _handle_sample(data, schema, path, canvas)
+    elif schema['type'] == 'measurement':
+        _handle_measurement(data, schema, path, canvas)
     elif schema['type'] == 'tags':
         _handle_tags(data, schema, path, canvas)
     elif schema['type'] == 'datetime':
         _handle_datetime(data, schema, path, canvas)
     elif schema['type'] == 'hazards':
         _handle_hazards(data, schema, path, canvas)
     else:
@@ -197,14 +199,19 @@
 
 
 def _handle_sample(data, schema, path, canvas):
     text = '• {}: #{}'.format(schema['title'], data['object_id'])
     _append_text(canvas, text)
 
 
+def _handle_measurement(data, schema, path, canvas):
+    text = '• {}: #{}'.format(schema['title'], data['object_id'])
+    _append_text(canvas, text)
+
+
 def _handle_datetime(data, schema, path, canvas):
     text = '• {}: {}'.format(schema['title'], data['utc_datetime'])
     _append_text(canvas, text)
 
 
 def _handle_tags(data, schema, path, canvas):
     text = '• {}: {}'.format(schema['title'], ', '.join(data['tags']))
```

### Comparing `sampledb-0.8.1/sampledb/frontend/projects.py` & `sampledb-0.9.0/sampledb/frontend/projects.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import flask_login
 
 from . import frontend
 from .. import logic
 from ..logic.object_permissions import Permissions
 from ..logic.security_tokens import verify_token
 from .projects_forms import CreateProjectForm, EditProjectForm, LeaveProjectForm, InviteUserToProjectForm, InviteGroupToProjectForm, ProjectPermissionsForm, AddSubprojectForm, RemoveSubprojectForm, DeleteProjectForm, RemoveProjectMemberForm, RemoveProjectGroupForm
+from .utils import check_current_user_is_not_readonly
 
 
 @frontend.route('/projects/<int:project_id>', methods=['GET', 'POST'])
 @flask_login.login_required
 def project(project_id):
     if 'token' in flask.request.args:
         token = flask.request.args.get('token')
@@ -71,15 +72,15 @@
     project_member_user_ids.sort(key=lambda user_id: logic.users.get_user(user_id).name.lower())
 
     project_member_group_ids = list(project_member_group_ids_and_permissions.keys())
     project_member_group_ids.sort(key=lambda group_id: logic.groups.get_group(group_id).name.lower())
 
     if Permissions.GRANT in user_permissions:
         invitable_user_list = []
-        for user in logic.users.get_users():
+        for user in logic.users.get_users(exclude_hidden=True):
             if user.id not in project_member_user_ids_and_permissions:
                 invitable_user_list.append(user)
         parent_projects_with_add_permissions = logic.projects.get_ancestor_project_ids(project_id, only_if_child_can_add_users_to_ancestor=True)
     else:
         invitable_user_list = []
         parent_projects_with_add_permissions = []
     if invitable_user_list:
@@ -145,24 +146,26 @@
                 flask.flash('You cannot leave this project, because your are the only user with GRANT permissions.', 'error')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
             else:
                 flask.flash('You have successfully left the project.', 'success')
                 return flask.redirect(flask.url_for('.projects'))
     if 'delete' in flask.request.form and Permissions.GRANT in user_permissions:
         if delete_project_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             try:
                 logic.projects.delete_project(project_id=project_id)
             except logic.errors.ProjectDoesNotExistError:
                 flask.flash('This project has already been deleted.', 'success')
                 return flask.redirect(flask.url_for('.projects'))
             else:
                 flask.flash('You have successfully deleted the project.', 'success')
                 return flask.redirect(flask.url_for('.projects'))
     if 'remove_member' in flask.request.form and Permissions.GRANT in user_permissions:
         if remove_project_member_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             member_id_str = flask.request.form['remove_member']
             try:
                 member_id = int(member_id_str)
             except ValueError:
                 flask.flash('The member ID was invalid. Please contact an administrator.', 'error')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
             if member_id == flask_login.current_user.id:
@@ -183,14 +186,15 @@
                 flask.flash('You cannot remove this users from this project, because they are the only user with GRANT permissions.', 'error')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
             else:
                 flask.flash('You have successfully removed this user from the project.', 'success')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
     if 'remove_group' in flask.request.form and Permissions.GRANT in user_permissions:
         if remove_project_group_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             group_id_str = flask.request.form['remove_group']
             try:
                 group_id = int(group_id_str)
             except ValueError:
                 flask.flash('The group ID was invalid. Please contact an administrator.', 'error')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
             try:
@@ -209,28 +213,30 @@
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
             else:
                 flask.flash('You have successfully removed this group from the project.', 'success')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
     if 'edit' in flask.request.form and Permissions.WRITE in user_permissions:
         show_edit_form = True
         if edit_project_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             try:
                 logic.projects.update_project(project_id, edit_project_form.name.data, edit_project_form.description.data)
             except logic.errors.ProjectDoesNotExistError:
                 flask.flash('This project does not exist.', 'error')
                 return flask.redirect(flask.url_for('.projects'))
             except logic.errors.ProjectAlreadyExistsError:
                 edit_project_form.name.errors.append('A project with this name already exists.')
             except logic.errors.InvalidProjectNameError:
                 edit_project_form.name.errors.append('This project name is invalid.')
             else:
                 flask.flash('Project information updated successfully.', 'success')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
     if 'add_user' in flask.request.form and Permissions.GRANT in user_permissions:
         if invite_user_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             if not any(user.id == invite_user_form.user_id.data for user in invitable_user_list):
                 flask.flash('You cannot add this user.', 'error')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
             try:
                 other_project_ids = []
                 for other_project_id_form in invite_user_form.other_project_ids:
                     try:
@@ -247,14 +253,15 @@
             except logic.errors.UserAlreadyMemberOfProjectError:
                 flask.flash('This user is already a member of this project.', 'error')
             else:
                 flask.flash('The user was successfully invited to the project.', 'success')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
     if 'add_group' in flask.request.form and Permissions.GRANT in user_permissions:
         if invite_group_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             if not any(group.id == invite_group_form.group_id.data for group in invitable_group_list):
                 flask.flash('You cannot add this group.', 'error')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
             try:
                 logic.projects.add_group_to_project(project_id, invite_group_form.group_id.data, permissions=Permissions.READ)
             except logic.errors.ProjectDoesNotExistError:
                 flask.flash('This project does not exist.', 'error')
@@ -264,23 +271,25 @@
             except logic.errors.GroupAlreadyMemberOfProjectError:
                 flask.flash('This group is already a member of this project.', 'error')
             else:
                 flask.flash('The group was successfully added to the project.', 'success')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
     if 'remove_subproject' in flask.request.form and Permissions.GRANT in user_permissions:
         if remove_subproject_form is not None and remove_subproject_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             child_project_id = remove_subproject_form.child_project_id.data
             if child_project_id not in child_project_ids:
                 flask.flash('Project #{} is not a subproject of this project.'.format(int(child_project_id)), 'error')
             else:
                 logic.projects.delete_subproject_relationship(project_id, child_project_id)
                 flask.flash('The subproject was successfully removed from this project.', 'success')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
     if 'add_subproject' in flask.request.form and Permissions.GRANT in user_permissions:
         if add_subproject_form is not None and add_subproject_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             child_project_id = add_subproject_form.child_project_id.data
             if child_project_id not in addable_project_ids:
                 flask.flash('Project #{} cannot become a subproject of this project.'.format(int(child_project_id)), 'error')
             else:
                 logic.projects.create_subproject_relationship(project_id, child_project_id, child_can_add_users_to_parent=add_subproject_form.child_can_add_users_to_parent.data)
                 flask.flash('The subproject was successfully added to this project.', 'success')
                 return flask.redirect(flask.url_for('.project', project_id=project_id))
@@ -337,14 +346,15 @@
         create_project_form.name.data = ''
     if create_project_form.description.data is None:
         create_project_form.description.data = ''
     show_create_form = False
     if 'create' in flask.request.form:
         show_create_form = True
         if create_project_form.validate_on_submit():
+            check_current_user_is_not_readonly()
             try:
                 project_id = logic.projects.create_project(create_project_form.name.data, create_project_form.description.data, flask_login.current_user.id).id
             except logic.errors.ProjectAlreadyExistsError:
                 create_project_form.name.errors.append('A project with this name already exists.')
             except logic.errors.InvalidProjectNameError:
                 create_project_form.name.errors.append('This project name is invalid.')
             else:
@@ -379,14 +389,15 @@
         edit_user_permissions_form = None
     return flask.render_template('project_permissions.html', project=project, user_permissions=user_permissions, group_permissions=group_permissions, project_permissions=project_permissions, get_user=logic.users.get_user, get_group=logic.groups.get_group, Permissions=Permissions, form=edit_user_permissions_form)
 
 
 @frontend.route('/projects/<int:project_id>/permissions', methods=['POST'])
 @flask_login.login_required
 def update_project_permissions(project_id):
+    check_current_user_is_not_readonly()
     try:
         if Permissions.GRANT not in logic.projects.get_user_project_permissions(project_id, flask_login.current_user.id, include_groups=True):
             return flask.abort(403)
     except logic.errors.ProjectDoesNotExistError:
         return flask.abort(404)
 
     edit_user_permissions_form = ProjectPermissionsForm()
```

### Comparing `sampledb-0.8.1/sampledb/frontend/projects_forms.py` & `sampledb-0.9.0/sampledb/frontend/projects_forms.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/status.py` & `sampledb-0.9.0/sampledb/frontend/status.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/actions/action.html` & `sampledb-0.9.0/sampledb/frontend/templates/actions/action.html`

 * *Files 9% similar despite different names*

```diff
@@ -17,26 +17,34 @@
   {% endif %}
   <p>{{ action.description }}</p>
   {% with instrument = action.instrument %}
     {% include "instruments/instrument_scientists.html" %}
   {% endwith %}
   {% if action.type == ActionType.MEASUREMENT %}
     <a href="{{ url_for('.objects', action=action.id) }}" class="btn btn-default">View Measurements</a>
+    {% if not current_user.is_readonly %}
     <a href="{{ url_for('.new_object', action_id=action.id) }}" class="btn btn-primary">Perform Measurement</a>
+    {% endif %}
   {% elif action.type == ActionType.SIMULATION %}
     <a href="{{ url_for('.objects', action=action.id) }}" class="btn btn-default">View Simulations</a>
+    {% if not current_user.is_readonly %}
     <a href="{{ url_for('.new_object', action_id=action.id) }}" class="btn btn-primary">Perform Simulation</a>
+    {% endif %}
   {% else %}
     <a href="{{ url_for('.objects', action=action.id) }}" class="btn btn-default">View Samples</a>
+    {% if not current_user.is_readonly %}
     <a href="{{ url_for('.new_object', action_id=action.id) }}" class="btn btn-primary">Create Sample</a>
+    {% endif %}
   {% endif %}
+  {% if not current_user.is_readonly %}
   {% if may_edit %}
     <a href="{{ url_for('.action', action_id=action.id, mode='edit') }}" class="btn btn-default" data-toggle="tooltip" data-placement="top" title="Modify the settings for this action.">Edit Action</a>
   {% endif %}
   <a href="{{ url_for('.new_action', previous_action_id=action.id) }}" class="btn btn-default" data-toggle="tooltip" data-placement="top" title="Create a new custom action based on the settings for this action.">Use as Template</a>
+  {% endif %}
 {% endblock %}
 
 {% block scripts %}
 {{ super() }}
 <script>
 $(function () {
   $('[data-toggle="tooltip"]').tooltip()
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/actions/action_form.html` & `sampledb-0.9.0/sampledb/frontend/templates/actions/action_form.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,21 @@
   <form method="post">
   {{ action_form.hidden_tag() }}
     <div class="col-md-12">
       <div class="form-group {% if action_form.name.name in action_form.errors %}has-error{% endif %}">
         <label for="input-name" class="control-label">Name</label>
          <input type="text" class="form-control" id="input-name" placeholder="Name" name="{{ action_form.name.name }}" value="{{ action_form.name.data or '' }}">
       </div>
+      {% if may_set_user_specific %}
+      <div class="checkbox">
+        <label for="input-is_user_specific" style="font-weight:700">
+          <input type="checkbox" id="input-is_user_specific" name="{{ action_form.is_user_specific.name }}" {% if action_form.is_user_specific.data %}checked="checked"{% endif %}> User specific action
+        </label>
+      </div>
+      {% endif %}
       <div class="checkbox {% if action_form.description.name in action_form.errors %}has-error{% endif %}">
         <label for="input-public" style="font-weight:700">
           <input type="checkbox" id="input-public" name="{{ action_form.is_public.name }}" {% if action_form.is_public.data %}checked="checked"{% endif %} {% if not may_change_public %}disabled="disabled"{% endif %}> Public
         </label>
       </div>
       <div class="form-group {% if action_form.type.name in action_form.errors %}has-error{% endif %}">
         <label for="input-type" class="control-label">Type</label>
@@ -150,14 +157,15 @@
             <option value="text">Text (Simple)</option>
             <option value="multiline">Text (Multiline)</option>
             <option value="choice">Text (Choice)</option>
             <option value="quantity">Quantity</option>
             <option value="bool">Boolean</option>
             <option value="datetime">Datetime</option>
             <option value="sample">Sample</option>
+            <option value="measurement">Measurement</option>
           </select>
         </div>
         <div class="schema-editor-form-group">
           <label class="control-label schema-editor-generic-property-required-label">Required</label>
           <div class="checkbox">
             <label>
               <input type="checkbox" data-onstyle="default" data-width="176" data-on="Yes" data-off="No" class="schema-editor-generic-property-required-input">
```

#### html2text {}

```diff
@@ -6,14 +6,19 @@
  {% endif %} {% endblock %} {% block scripts %} {{ super() }}
  {% if use_schema_editor %}
  {% endif %} {% endblock %} {% block content %}
 Warning: Custom Actions are an advanced feature that most users of {
 { service_name }} will not need. See the User_Guide for more information.
 {{ action_form.hidden_tag() }}
 Name [{{ action_form.name.data or '' }}]
+{% if may_set_user_specific %}
+
+% if action_form.is_user_specific.data %}checked="checked"{% endif %}> User
+specific action
+{% endif %}
 
 % if action_form.is_public.data %}checked="checked"{% endif %} {% if not
 may_change_public %}disabled="disabled"{% endif %}> Public
 Type
 % if not may_change_type %}disabled="disabled"{% endif %}>
 % if action_form.type.data == 'sample' %}selected="selected"{% endif %}>Sample
 Creation
@@ -47,15 +52,15 @@
 Hazards
  ⁰ Hazards
 Properties
 
 Name  [                    ]
 Title  [                    ]
 Type [One of: Text (Simple)/Text (Multiline)/Text (Choice)/Quantity/Boolean/
-Datetime/Sample]
+Datetime/Sample/Measurement]
 Required
  ⁰ Required
 ⁰Note  [                    ]
 ⁰Default [                    ]
 ⁰Pattern  [                    ]
 ⁰Minimum Length [                    ]
 ⁰Maximum Length [                    ]
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/actions/actions.html` & `sampledb-0.9.0/sampledb/frontend/templates/actions/actions.html`

 * *Files 9% similar despite different names*

```diff
@@ -23,18 +23,24 @@
     <p>{{ action.description }}</p>
     {% with instrument = action.instrument %}
       {% include "instruments/instrument_scientists.html" %}
     {% endwith %}
     <p>
     {% if action.type == ActionType.MEASUREMENT %}
       <a href="{{ url_for('.objects', action=action.id) }}" class="btn btn-default">View Measurements</a>
+      {% if not current_user.is_readonly %}
       <a href="{{ url_for('.new_object', action_id=action.id, sample_id=request.args.get('sample_id', None)) }}" class="btn btn-primary">Perform Measurement</a>
+      {% endif %}
     {% elif action.type == ActionType.SIMULATION %}
       <a href="{{ url_for('.objects', action=action.id) }}" class="btn btn-default">View Simulations</a>
+      {% if not current_user.is_readonly %}
       <a href="{{ url_for('.new_object', action_id=action.id) }}" class="btn btn-primary">Perform Simulation</a>
+      {% endif %}
     {% else %}
       <a href="{{ url_for('.objects', action=action.id) }}" class="btn btn-default">View Samples</a>
+      {% if not current_user.is_readonly %}
       <a href="{{ url_for('.new_object', action_id=action.id) }}" class="btn btn-primary">Create Sample</a>
+      {% endif %}
     {% endif %}
     </p>
   {% endfor %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -7,11 +7,13 @@
  {{ toggle_favorite_action_form.csrf_token() }}
 ***** {% if action.user is not none %} {{_action.user.name_}} / {% endif %} {%
 if action.instrument is not none %} {{_action.instrument.name_}} — {% endif %}
 {{_action.name_}}  *****
 {{ action.description }}
 {% with instrument = action.instrument %} {% include "instruments/
 instrument_scientists.html" %} {% endwith %}
-{% if action.type == ActionType.MEASUREMENT %} View_Measurements Perform
-Measurement {% elif action.type == ActionType.SIMULATION %} View_Simulations
-Perform_Simulation {% else %} View_Samples Create_Sample {% endif %}
+{% if action.type == ActionType.MEASUREMENT %} View_Measurements {% if not
+current_user.is_readonly %} Perform_Measurement {% endif %} {% elif action.type
+== ActionType.SIMULATION %} View_Simulations {% if not current_user.is_readonly
+%} Perform_Simulation {% endif %} {% else %} View_Samples {% if not
+current_user.is_readonly %} Create_Sample {% endif %} {% endif %}
 {% endfor %} {% endblock %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/instruments/instruments.html` & `sampledb-0.9.0/sampledb/frontend/templates/instruments/instruments.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 {% extends "base.html" %}
 
 {% block title %}Instruments — {{ service_name }}{% endblock %}
 
 {% block content %}
   <h1>Instruments</h1>
   <p class="text-muted">Instruments in {{ service_name }} map real instruments in Jülich or at other facilities to <a href="{{ url_for('.actions') }}">actions</a> performed with them. <a href="https://scientific-it-systems.iffgit.fz-juelich.de/SampleDB/user_guide/instruments.html">Read more.</a></p>
+  {% if current_user.is_admin and not current_user.is_readonly %}
+    <a href="{{ url_for('.new_instrument') }}" class="btn btn-default">Create Instrument</a>
+  {% endif %}
   {% for instrument in instruments %}
     <form action="{{ url_for('.toggle_favorite_instrument') }}" method="post">
     <input type="hidden" name="instrument_id" value="{{ instrument.id }}">
     {{ toggle_favorite_instrument_form.csrf_token() }}
     <h2>
       <a href="{{ url_for('.instrument', instrument_id=instrument.id) }}" title="{{ instrument.name }}">{{ instrument.name }}</a>
       <button type="submit" class="fa {% if instrument.id in user_favorite_instrument_ids %}fav-star-on{% else %}fav-star-off{% endif %}" value=""></button>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends "base.html" %} {% block title %}Instruments â {{ service_name }}{%
 endblock %} {% block content %}
 ****** Instruments ******
 Instruments in {{ service_name }} map real instruments in JÃ¼lich or at other
 facilities to actions performed with them. Read_more.
-{% for instrument in instruments %}
+{% if current_user.is_admin and not current_user.is_readonly %} Create
+Instrument {% endif %} {% for instrument in instruments %}
  {{ toggle_favorite_instrument_form.csrf_token() }}
 ***** {{_instrument.name_}}  *****
 {{ instrument.description }}
 {% include "instruments/instrument_scientists.html" %} {% endfor %} {% endblock
 %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/locations/location.html` & `sampledb-0.9.0/sampledb/frontend/templates/locations/location.html`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,18 @@
     {% for ancestor_id, ancestor_name in ancestors %}
       <a href="{{ url_for('.location', location_id=ancestor_id) }}">{{ ancestor_name }}</a> /
     {% endfor %}
     {{ location.name }}
   </h1>
   <pre style="font-family: sans-serif; background-color: transparent; border: 0; padding: 0;">{{ location.description }}</pre>
   <a href="{{ url_for('.objects', location=location.id) }}" class="btn btn-default">View Objects</a>
+  {% if not current_user.is_readonly %}
   <a href="{{ url_for('.location', location_id=location.id, mode='edit') }}" class="btn btn-default">Edit Location</a>
   <a href="{{ url_for('.new_location', parent_location_id=location.id) }}" class="btn btn-default">Create Sub-Location</a>
+  {% endif %}
   {% if locations_tree %}
     <h2>Sub-Locations</h2>
     <ul>
     {% set location_ids_sorted_by_name = sort_location_ids_by_name(locations_tree.keys(), locations_map) %}
     {% for location_id in location_ids_sorted_by_name %}
       {% include "locations/locations_tree.html" %}
     {% endfor %}
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {% extends "base.html" %} {% block title %}Location #{{ location.id }}: {
 { location.name }} â {{ service_name }}{% endblock %} {% block content %}
 ****** {% for ancestor_id, ancestor_name in ancestors %} {{_ancestor_name_}} /
 {% endfor %} {{ location.name }} ******
 {{ location.description }}
-View_Objects Edit_Location Create_Sub-Location {% if locations_tree %}
+View_Objects {% if not current_user.is_readonly %} Edit_Location Create_Sub-
+Location {% endif %} {% if locations_tree %}
 ***** Sub-Locations *****
     * {% set location_ids_sorted_by_name = sort_location_ids_by_name
       (locations_tree.keys(), locations_map) %} {% for location_id in
       location_ids_sorted_by_name %} {% include "locations/locations_tree.html"
       %} {% endfor %}
 {% endif %} {% endblock %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/locations/location_form.html` & `sampledb-0.9.0/sampledb/frontend/templates/locations/location_form.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/locations/locations.html` & `sampledb-0.9.0/sampledb/frontend/templates/locations/locations.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 {% block title %}Locations — {{ service_name }}{% endblock %}
 
 {% block content %}
   <h1>Locations</h1>
   <p class="text-muted">Locations allow users to track where an object can be found. <a href="https://scientific-it-systems.iffgit.fz-juelich.de/SampleDB/user_guide/objects.html#location">Read more.</a></p>
   <p>
+    {% if not current_user.is_readonly %}
     <a href="{{ url_for('.new_location') }}" class="btn btn-default" style="margin-bottom: 10px;">Create Location</a>
+    {% endif %}
   </p>
   {% if locations_tree %}
     <ul>
     {% set location_ids_sorted_by_name = sort_location_ids_by_name(locations_tree.keys(), locations_map) %}
     {% for location_id in location_ids_sorted_by_name %}
       {% include "locations/locations_tree.html" %}
     {% endfor %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends "base.html" %} {% block title %}Locations â {{ service_name }}{%
 endblock %} {% block content %}
 ****** Locations ******
 Locations allow users to track where an object can be found. Read_more.
-Create_Location
+{% if not current_user.is_readonly %} Create_Location {% endif %}
 {% if locations_tree %}
     * {% set location_ids_sorted_by_name = sort_location_ids_by_name
       (locations_tree.keys(), locations_map) %} {% for location_id in
       location_ids_sorted_by_name %} {% include "locations/locations_tree.html"
       %} {% endfor %}
 {% endif %} {% endblock %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/locations/locations_tree.html` & `sampledb-0.9.0/sampledb/frontend/templates/locations/locations_tree.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/account_recovery.html` & `sampledb-0.9.0/sampledb/frontend/templates/mails/account_recovery.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/account_recovery.txt` & `sampledb-0.9.0/sampledb/frontend/templates/mails/account_recovery.txt`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/base.html` & `sampledb-0.9.0/sampledb/frontend/templates/mails/base.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/email_confirmation.html` & `sampledb-0.9.0/sampledb/frontend/templates/mails/email_confirmation.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/assigned_as_responsible_user.html` & `sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/assigned_as_responsible_user.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/invited_to_group.html` & `sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/invited_to_group.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/invited_to_project.html` & `sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/invited_to_project.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/mails/notifications/received_object_permissions_request.html` & `sampledb-0.9.0/sampledb/frontend/templates/mails/notifications/received_object_permissions_request.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_any.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_any.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 {% if schema['type'] == 'text' and 'choices' not in schema  %}
   {% include "objects/forms/form_text.html" %}
 {% elif schema['type'] == 'text' and 'choices' in schema %}
   {% include "objects/forms/form_select.html" %}
 {% elif schema['type'] == 'sample' %}
   {% include "objects/forms/form_sample.html" %}
+{% elif schema['type'] == 'measurement' %}
+  {% include "objects/forms/form_measurement.html" %}
 {% elif schema['type'] == 'datetime' %}
   {% include "objects/forms/form_datetime.html" %}
 {% elif schema['type'] == 'bool' %}
   {% include "objects/forms/form_bool.html" %}
 {% elif schema['type'] == 'quantity' %}
   {% include "objects/forms/form_quantity.html" %}
 {% elif schema.type == 'object' %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_array.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_array.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_base.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_base.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_bool.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_bool.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_create.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_create.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_datetime.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_datetime.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_edit.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_edit.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_hazards.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_hazards.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_object.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_object.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_quantity.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_quantity.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_sample.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_sample.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_select.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_select.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_any.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_any.html`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,18 @@
   {% include "objects/forms/form_table_select.html" %}
 {% elif schema['type'] == 'text' %}
   {% include "objects/forms/form_table_text.html" %}
 {% elif schema['type'] == 'datetime' %}
   {% include "objects/forms/form_table_datetime.html" %}
 {% elif schema['type'] == 'quantity' %}
   {% include "objects/forms/form_table_quantity.html" %}
+{% elif schema['type'] == 'sample' %}
+  {% include "objects/forms/form_table_sample.html" %}
+{% elif schema['type'] == 'measurement' %}
+  {% include "objects/forms/form_table_measurement.html" %}
 {#{% elif schema.type == 'object' %}#}
 {#  {% include "form_object.html" %}#}
 {#{% elif schema.type == 'array' %}#}
 {#  {% include "form_array.html" %}#}
 {% else %}
   {{ name }}{{ schema.type }}{{ schema['type'] }}
 {% endif %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_datetime.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_datetime.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_quantity.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_quantity.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_select.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_select.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_table_text.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_table_text.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_tags.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_tags.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/forms/form_text.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/forms/form_text.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/object_permissions.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/object_permissions.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/object_versions.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/object_versions.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/objects.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/objects.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/restore_object_version.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/restore_object_version.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/unauthorized.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/unauthorized.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends "base.html" %}
 
 {% block title %}Insufficient Permissions — {{ service_name }}{% endblock %}
 
 {% block content %}
   <h1>Insufficient Permissions</h1>
-  <p>You do not have sufficient <a href="https://scientific-it-systems.iffgit.fz-juelich.de/SampleDB/user_guide/objects.html#permissions">permissions</a> to access this object. Would you like to request read permissions?</p>
+  <p>You do not have sufficient <a href="https://scientific-it-systems.iffgit.fz-juelich.de/SampleDB/user_guide/objects.html#permissions">permissions</a> to access this object. {% if has_grant_user %}Would you like to request read permissions?</p>
   <form action="{{ url_for('.object_permissions_request', object_id=object_id) }}" method="post">
     <button type="submit" class="btn btn-primary">Send Request</button>
   </form>
+  {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% extends "base.html" %} {% block title %}Insufficient Permissions â {
 { service_name }}{% endblock %} {% block content %}
 ****** Insufficient Permissions ******
-You do not have sufficient permissions to access this object. Would you like to
-request read permissions?
+You do not have sufficient permissions to access this object. {% if
+has_grant_user %}Would you like to request read permissions?
 Send Request
-{% endblock %}
+{% endif %} {% endblock %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/any.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/any.html`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
   {% include "objects/view/datetime.html" %}
 {% elif schema['type'] == 'bool' %}
   {% include "objects/view/bool.html" %}
 {% elif schema['type'] == 'quantity' %}
   {% include "objects/view/quantity.html" %}
 {% elif schema.type == 'sample' %}
   {% include "objects/view/sample.html" %}
+{% elif schema.type == 'measurement' %}
+  {% include "objects/view/measurement.html" %}
 {% elif schema.type == 'object' %}
   {% include "objects/view/object.html" %}
 {% elif schema.type == 'array' %}
   {% include "objects/view/array.html" %}
 {% elif schema.type == 'tags' %}
   {% include "objects/view/tags.html" %}
 {% elif schema.type == 'hazards' %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/array.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/array.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/base.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   <div class="row" style="padding-right:0.75em">
     <label class="col-md-3" style="text-align: right">Action <a href="{{ url_for('.objects', action=action.id) }}" class="search-helper"><i class="fa fa-search" aria-hidden="true"></i></a></label>
     <div class="col-md-9"><a href="{{ url_for('frontend.action', action_id=action.id) }}">{{ action.name }}</a></div>
   </div>
   {% include "objects/view/any.html" %}
   <div class="object-button-bar">
   {% if not is_archived %}
+    {% if not current_user.is_readonly %}
     {% if user_may_edit %}
     <div class="form-group">
       <a href="{{ url_for('.object', object_id=object_id, mode='edit') }}" class="btn btn-primary" data-toggle="tooltip" data-placement="top" title="Create a new version of the information for this object."><i class="fa fa-pencil" aria-hidden="true"></i> Edit Object</a>
     </div>
     {% endif %}
     {% if user_may_edit and new_schema_available %}
     <div class="form-group">
@@ -75,14 +76,15 @@
           {% endif %}
           <li role="separator" class="divider"></li>
           <li><a href="{{ url_for('.actions', t='measurements', sample_id=object_id) }}">See other Measurement Actions...</a></li>
         </ul>
       </div>
     </div>
     {% endif %}
+    {% endif %}
     <div class="form-group">
       <a href="{{ url_for('.print_object_label', object_id=object_id) }}" class="btn btn-primary" data-toggle="tooltip" data-placement="top" title="Show a PDF containing labels for this object."><i class="fa fa-tag" aria-hidden="true"></i> Show Labels</a>
     </div>
     <div class="form-group">
       <button type="button" class="btn btn-primary" id="button-show-object-qrcode-modal" data-toggle="tooltip" data-placement="top" title="Show a QR code for a link to this object."><i class="fa fa-qrcode" aria-hidden="true"></i> Show QR Code</button>
     </div>
     <div class="form-group">
@@ -587,26 +589,26 @@
             <td class="text-right">
               {% if 'version_id' in object_log_entry.data %}
                 <a href="{{ url_for('.object_version', object_id=object_id, version_id=object_log_entry.data['version_id']) }}">View</a>
               {% endif %}
             </td>
           {% elif object_log_entry.type == ObjectLogEntryType.USE_OBJECT_IN_MEASUREMENT %}
             {% if object_log_entry.data['measurement_id'] %}
-            <td><a href="{{ url_for('.user_profile', user_id=object_log_entry.user.id) }}">{{ object_log_entry.user.name }}</a> used the object in measurement <a href="{{ url_for('.object', object_id=object_log_entry.data['measurement_id']) }}">{{ object_log_entry.data['measurement'].data['name']['text'] }}</a>.</td>
+            <td><a href="{{ url_for('.user_profile', user_id=object_log_entry.user.id) }}">{{ object_log_entry.user.name }}</a> used the object in measurement <a href="{{ url_for('.object', object_id=object_log_entry.data['measurement_id']) }}">{{ object_log_entry.data['measurement'].data['name']['text'] }} (#{{ object_log_entry.data['measurement_id'] }})</a>.</td>
             <td class="text-right">
               <a href="{{ url_for('.object', object_id=object_log_entry.data['measurement_id']) }}">View</a>
             </td>
             {% else %}
             <td><a href="{{ url_for('.user_profile', user_id=object_log_entry.user.id) }}">{{ object_log_entry.user.name }}</a> used the object in a measurement.</td>
             <td class="text-right">
             </td>
             {% endif %}
           {% elif object_log_entry.type == ObjectLogEntryType.USE_OBJECT_IN_SAMPLE_CREATION %}
             {% if object_log_entry.data['sample_id'] %}
-            <td><a href="{{ url_for('.user_profile', user_id=object_log_entry.user.id) }}">{{ object_log_entry.user.name }}</a> used the object to create the sample <a href="{{ url_for('.object', object_id=object_log_entry.data['sample_id']) }}">{{ object_log_entry.data['sample'].data['name']['text'] }}</a>.</td>
+            <td><a href="{{ url_for('.user_profile', user_id=object_log_entry.user.id) }}">{{ object_log_entry.user.name }}</a> used the object to create the sample <a href="{{ url_for('.object', object_id=object_log_entry.data['sample_id']) }}">{{ object_log_entry.data['sample'].data['name']['text'] }} (#{{ object_log_entry.data['sample_id'] }})</a>.</td>
             <td class="text-right">
               <a href="{{ url_for('.object', object_id=object_log_entry.data['sample_id']) }}">View</a>
             </td>
             {% else %}
             <td><a href="{{ url_for('.user_profile', user_id=object_log_entry.user.id) }}">{{ object_log_entry.user.name }}</a> used the object to create a sample.</td>
             <td class="text-right">
             </td>
```

#### html2text {}

```diff
@@ -10,15 +10,16 @@
 **** {{ object_type }} #{{ object_id }}: {{ data['name']['text'] }} ****
 *** Information ***
 Instrument
 {% if instrument is not none %}{{_instrument.name_}}{% else %}—{% endif %}
 Action
 {{_action.name_}}
 {% include "objects/view/any.html" %}
-{% if not is_archived %} {% if user_may_edit %}
+{% if not is_archived %} {% if not current_user.is_readonly %} {% if
+user_may_edit %}
  Edit_Object
 {% endif %} {% if user_may_edit and new_schema_available %}
  Update_Schema
 {% endif %} {% if user_may_grant %}
  Edit_Permissions
 {% endif %}
  Use_as_Template
@@ -30,15 +31,15 @@
     * {%_if_action.user_is_not_none_%}_{{_action.user.name_}}_/_{%_endif_%}_{%
       if_action.instrument_is_not_none_%}_{{_action.instrument.name_}}_—_{%
       endif_%}_{{_action.name_}}
     * {% endfor %} {% else %}
     * —
     * {% endif %}
     * See_other_Measurement_Actions...
-{% endif %}
+{% endif %} {% endif %}
  Show_Labels
  Show QR Code
  Export to PDF
 {% if notebook_templates and jupyterhub_url %}
 
 , filename="img/jupyter-40.png") }}" style="height:1.3em; margin-top:-0.2em;
 margin-right: -0.2em;" alt=""/> Create Notebook
@@ -190,24 +191,24 @@
  Post Comment
 {% endif %} {% endif %} {% if object_log_entries %}
 *** Activity Log ***
 Datetime
                                                                                                                                                                                                                                                                                                                                                                                   {
                                                                                                                                                                                                                                                                                                                                                                                   {
                                                                                                                                                                                                                                                                                                                                                                                   object_log_entry.user.name
-                                       {                                                                                                                                                                                                                                                                                                                                          }} {% for file in files %}
+                                       {                                                                                                                                                                 {                                                           {                                                                                                            }} {% for file in files %}
                                        {                                                                                                                {                                                {                                                           {                                                                                                            {% if file.id ==
-                                       object_log_entry.user.name      {                                                                                {                                                {                               {                           {                               {                           {                                                object_log_entry.data                            {{_object_log_entry.user.name_}} assigned this object                                                                                                      {
-{                                      }} created the object{% if      {                               {                          {% if 'version_id' in object_log_entry.user.name {% if 'version_id' in object_log_entry.user.name      {                           object_log_entry.user.name      {                           {                          {% if 'comment_id' in ['file_id'] %}{% if        {% if 'file_id' in    to location {{_get_location                           {{_object_log_entry.user.name_}} assigned     {{_object_log_entry.user.name_}} assigned this object  {
-{                                      'previous_object_id' in    View object_log_entry.user.name View {                          object_log_entry.data }} restored object version object_log_entry.data }} used the object in      View object_log_entry.user.name  }} used the object to      View object_log_entry.user.name  object_log_entry.user.name object_log_entry.data file.storage == 'local'    object_log_entry.data (object_location_assignment.location_id).name_}} and  this object to location {{_get_location       to user {{_get_user                                    object_log_entry.user.name View Unknown
-object_log_entry.utc_datetime.strftime object_log_entry.data %}        }} created the object as        object_log_entry.user.name %} View {% endif %}   #{{_object_log_entry.data  %} View {% endif %}   measurement {                   }} used the object in a     create the sample {             }} used the object to       }} posted a comment for    %} View {% endif %}   %}uploaded {               %} View {% endif %}   user {{_get_user                                      (object_location_assignment.location_id).name (object_location_assignment.responsible_user_id).name  }} linked publication {         event
-('%Y-%m-%d %H:%M:%S') }}               using data from Object_{        part of a batch.                }} edited the object.                            ['restored_version_id']                          {_object_log_entry.data         measurement.                {_object_log_entry.data         create a sample.            this object.                                     {_file.original_file_name                        (object_location_assignment.responsible_user_id).name }}.                                           }}.                                                    {_object_log_entry.data
-                                       {_object_log_entry.data                                                                                          }}.                                              ['measurement'].data                                        ['sample'].data['name']                                                                                      }}{% elif file.storage ==                        }}.                                                                                                                                                        ['doi']_}} to this object.
-                                       ['previous_object_id']_}}                                                                                                                                         ['name']['text']_}}.                                        ['text']_}}.                                                                                                 'url' %}linked {
-                                       {% endif %}.                                                                                                                                                                                                                                                                                                                               {_file.data.url_}}{% else
+                                       object_log_entry.user.name      {                                                                                {                                                object_log_entry.user.name      {                           object_log_entry.user.name      {                           {                                                object_log_entry.data                            {{_object_log_entry.user.name_}} assigned this object                                                                                                      {
+{                                      }} created the object{% if      {                               {                          {% if 'version_id' in object_log_entry.user.name {% if 'version_id' in }} used the object in           {                           }} used the object to           {                           {                          {% if 'comment_id' in ['file_id'] %}{% if        {% if 'file_id' in    to location {{_get_location                           {{_object_log_entry.user.name_}} assigned     {{_object_log_entry.user.name_}} assigned this object  {
+{                                      'previous_object_id' in    View object_log_entry.user.name View {                          object_log_entry.data }} restored object version object_log_entry.data measurement {              View object_log_entry.user.name  create the sample {        View object_log_entry.user.name  object_log_entry.user.name object_log_entry.data file.storage == 'local'    object_log_entry.data (object_location_assignment.location_id).name_}} and  this object to location {{_get_location       to user {{_get_user                                    object_log_entry.user.name View Unknown
+object_log_entry.utc_datetime.strftime object_log_entry.data %}        }} created the object as        object_log_entry.user.name %} View {% endif %}   #{{_object_log_entry.data  %} View {% endif %}   {_object_log_entry.data         }} used the object in a     {_object_log_entry.data         }} used the object to       }} posted a comment for    %} View {% endif %}   %}uploaded {               %} View {% endif %}   user {{_get_user                                      (object_location_assignment.location_id).name (object_location_assignment.responsible_user_id).name  }} linked publication {         event
+('%Y-%m-%d %H:%M:%S') }}               using data from Object_{        part of a batch.                }} edited the object.                            ['restored_version_id']                          ['measurement'].data            measurement.                ['sample'].data['name']         create a sample.            this object.                                     {_file.original_file_name                        (object_location_assignment.responsible_user_id).name }}.                                           }}.                                                    {_object_log_entry.data
+                                       {_object_log_entry.data                                                                                          }}.                                              ['name']['text']_}}_(#{                                     ['text']_}}_(#{                                                                                              }}{% elif file.storage ==                        }}.                                                                                                                                                        ['doi']_}} to this object.
+                                       ['previous_object_id']_}}                                                                                                                                         {_object_log_entry.data                                     {_object_log_entry.data                                                                                      'url' %}linked {
+                                       {% endif %}.                                                                                                                                                      ['measurement_id']_}}).                                     ['sample_id']_}}).                                                                                           {_file.data.url_}}{% else
                                                                                                                                                                                                                                                                                                                                                                                   %}posted file_#{{_file.id
                                                                                                                                                                                                                                                                                                                                                                                   }}{% endif %}{% endif %}{%
                                                                                                                                                                                                                                                                                                                                                                                   endfor %}.
 {% endif %} {% if related_objects_tree %}
 *** Related Objects ***
 {% set in_export_pdf_model = False %} {% include "objects/view/
 related_objects_tree_toggle.html" %}{% include "objects/view/
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/bool.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/bool.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/datetime.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/datetime.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/hazards.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/hazards.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/object.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/object.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/quantity.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/quantity.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/related_objects.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/related_objects.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/related_objects_tree_toggle.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/related_objects_tree_toggle.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/sample.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/sample.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/select.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/select.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/table_any.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/table_any.html`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
   {% include "objects/view/table_datetime.html" %}
 {% elif schema['type'] == 'tags' %}
   {% include "objects/view/table_tags.html" %}
 {% elif schema['type'] == 'quantity' %}
   {% include "objects/view/table_quantity.html" %}
 {% elif schema['type'] == 'sample' %}
   {% include "objects/view/table_sample.html" %}
+{% elif schema['type'] == 'measurement' %}
+  {% include "objects/view/table_measurement.html" %}
 {#{% elif schema.type == 'object' %}#}
 {#  {% include "form_object.html" %}#}
 {#{% elif schema.type == 'array' %}#}
 {#  {% include "form_array.html" %}#}
 {% else %}
   {{ name }}{{ schema.type }}{{ schema['type'] }}
 {% endif %}
```

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/tags.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/tags.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/templates/objects/view/text.html` & `sampledb-0.9.0/sampledb/frontend/templates/objects/view/text.html`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/users/favorites.py` & `sampledb-0.9.0/sampledb/frontend/users/favorites.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 import flask
 import flask_login
 
 from .. import frontend
 from .forms import ToggleFavoriteActionForm, ToggleFavoriteInstrumentForm
 from ...logic.favorites import add_favorite_action, remove_favorite_action, get_user_favorite_action_ids, add_favorite_instrument, remove_favorite_instrument, get_user_favorite_instrument_ids
+from ..utils import check_current_user_is_not_readonly
 
 
 @frontend.route('/users/me/favorite_actions/', methods=['POST'])
 @flask_login.login_required
 def toggle_favorite_action():
+    check_current_user_is_not_readonly()
     toggle_favorite_action_form = ToggleFavoriteActionForm()
     if toggle_favorite_action_form.validate():
         action_id = toggle_favorite_action_form.action_id.data
         user_id = flask_login.current_user.id
         if action_id not in get_user_favorite_action_ids(user_id=user_id):
             add_favorite_action(action_id=action_id, user_id=user_id)
             flask.flash('The action has been added to your favorites.', 'success')
@@ -32,14 +34,15 @@
         t=flask.request.args.get('t', None)
     ))
 
 
 @frontend.route('/users/me/favorite_instruments/', methods=['POST'])
 @flask_login.login_required
 def toggle_favorite_instrument():
+    check_current_user_is_not_readonly()
     toggle_favorite_instrument_form = ToggleFavoriteInstrumentForm()
     if toggle_favorite_instrument_form.validate():
         instrument_id = toggle_favorite_instrument_form.instrument_id.data
         user_id = flask_login.current_user.id
         if instrument_id not in get_user_favorite_instrument_ids(user_id=user_id):
             add_favorite_instrument(instrument_id=instrument_id, user_id=user_id)
             flask.flash('The instrument has been added to your favorites.', 'success')
```

### Comparing `sampledb-0.8.1/sampledb/frontend/users/forms.py` & `sampledb-0.9.0/sampledb/frontend/users/forms.py`

 * *Files 22% similar despite different names*

```diff
@@ -45,7 +45,11 @@
 
 class NotificationModeForm(FlaskForm):
     pass
 
 
 class OtherSettingsForm(FlaskForm):
     pass
+
+
+class CreateAPITokenForm(FlaskForm):
+    description = StringField('description', validators=[Length(min=1, max=100)])
```

### Comparing `sampledb-0.8.1/sampledb/frontend/users/groups.py` & `sampledb-0.9.0/sampledb/frontend/users/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import flask
 import flask_login
 
 from .. import frontend
 from ... import logic
 from .forms import InviteUserForm, EditGroupForm, LeaveGroupForm, CreateGroupForm, DeleteGroupForm, RemoveGroupMemberForm
 from ...logic.security_tokens import verify_token
+from ..utils import check_current_user_is_not_readonly
 
 
 @frontend.route('/groups/', methods=['GET', 'POST'])
 @flask_login.login_required
 def groups():
     user_id = None
     if 'user_id' in flask.request.args:
@@ -32,14 +33,15 @@
     create_group_form = CreateGroupForm()
     if create_group_form.name.data is None:
         create_group_form.name.data = ''
     if create_group_form.description.data is None:
         create_group_form.description.data = ''
     show_create_form = False
     if 'create' in flask.request.form:
+        check_current_user_is_not_readonly()
         show_create_form = True
         if create_group_form.validate_on_submit():
             try:
                 group_id = logic.groups.create_group(create_group_form.name.data, create_group_form.description.data, flask_login.current_user.id).id
             except logic.errors.GroupAlreadyExistsError:
                 create_group_form.name.errors.append('A group with this name already exists.')
             except logic.errors.InvalidGroupNameError:
@@ -99,14 +101,15 @@
         remove_group_member_form = RemoveGroupMemberForm()
         if edit_group_form.name.data is None:
             edit_group_form.name.data = group.name
         if edit_group_form.description.data is None:
             edit_group_form.description.data = group.description
 
         if 'edit' in flask.request.form:
+            check_current_user_is_not_readonly()
             show_edit_form = True
             if edit_group_form.validate_on_submit():
                 try:
                     logic.groups.update_group(group_id, edit_group_form.name.data, edit_group_form.description.data)
                 except logic.errors.GroupDoesNotExistError:
                     flask.flash('This group does not exist.', 'error')
                     return flask.redirect(flask.url_for('.groups'))
@@ -114,14 +117,15 @@
                     edit_group_form.name.errors.append('A group with this name already exists.')
                 except logic.errors.InvalidGroupNameError:
                     edit_group_form.name.errors.append('This group name is invalid.')
                 else:
                     flask.flash('Group information updated successfully.', 'success')
                     return flask.redirect(flask.url_for('.group', group_id=group_id))
         elif 'add_user' in flask.request.form:
+            check_current_user_is_not_readonly()
             if invite_user_form.validate_on_submit():
                 try:
                     logic.groups.invite_user_to_group(group_id, invite_user_form.user_id.data, flask_login.current_user.id)
                 except logic.errors.GroupDoesNotExistError:
                     flask.flash('This group does not exist.', 'error')
                     return flask.redirect(flask.url_for('.groups'))
                 except logic.errors.UserDoesNotExistError:
@@ -143,24 +147,26 @@
                 except logic.errors.UserNotMemberOfGroupError:
                     flask.flash('You have already left the group.', 'error')
                     return flask.redirect(flask.url_for('.groups'))
                 else:
                     flask.flash('You have successfully left the group.', 'success')
                     return flask.redirect(flask.url_for('.groups'))
         elif 'delete' in flask.request.form:
+            check_current_user_is_not_readonly()
             if delete_group_form.validate_on_submit():
                 try:
                     logic.groups.delete_group(group_id)
                 except logic.errors.GroupDoesNotExistError:
                     flask.flash('This group has already been deleted.', 'success')
                     return flask.redirect(flask.url_for('.groups'))
                 else:
                     flask.flash('You have successfully deleted the group.', 'success')
                     return flask.redirect(flask.url_for('.groups'))
         elif 'remove_member' in flask.request.form:
+            check_current_user_is_not_readonly()
             if remove_group_member_form.validate_on_submit():
                 member_id_str = flask.request.form['remove_member']
                 try:
                     member_id = int(member_id_str)
                 except ValueError:
                     flask.flash('The member ID was invalid. Please contact an administrator.', 'error')
                     return flask.redirect(flask.url_for('.group', group_id=group_id))
```

### Comparing `sampledb-0.8.1/sampledb/frontend/users/invitation.py` & `sampledb-0.9.0/sampledb/frontend/users/invitation.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/users/notifications.py` & `sampledb-0.9.0/sampledb/frontend/users/notifications.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/users/preferences.py` & `sampledb-0.9.0/sampledb/frontend/users/preferences.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # coding: utf-8
 """
 
 """
 
+import secrets
+
 import flask
 import flask_login
 import sqlalchemy.sql.expression
 
 from ... import db
 
 from .. import frontend
 from ..authentication_forms import ChangeUserForm, AuthenticationForm, AuthenticationMethodForm
 from ..users_forms import RequestPasswordResetForm, PasswordForm, AuthenticationPasswordForm
 from ..objects_forms import ObjectPermissionsForm, ObjectUserPermissionsForm, ObjectGroupPermissionsForm, ObjectProjectPermissionsForm
-from .forms import NotificationModeForm, OtherSettingsForm
+from .forms import NotificationModeForm, OtherSettingsForm, CreateAPITokenForm
 
 from ...logic import user_log
-from ...logic.authentication import add_authentication_method, remove_authentication_method, change_password_in_authentication_method
+from ...logic.authentication import add_authentication_method, remove_authentication_method, change_password_in_authentication_method, add_api_token
 from ...logic.users import get_user, get_users
 from ...logic.utils import send_confirm_email, send_recovery_email
 from ...logic.security_tokens import verify_token
 from ...logic.object_permissions import Permissions, get_default_permissions_for_users, set_default_permissions_for_user, get_default_permissions_for_groups, set_default_permissions_for_group, get_default_permissions_for_projects, set_default_permissions_for_project, default_is_public, set_default_public
 from ...logic.projects import get_user_projects, get_project
 from ...logic.groups import get_user_groups, get_group
 from ...logic.errors import GroupDoesNotExistError, UserDoesNotExistError, ProjectDoesNotExistError
@@ -47,30 +49,37 @@
         else:
             # es ist egal, ob eingeloggt oder nicht
             return confirm_email()
     elif flask_login.current_user.is_authenticated:
         if user_id != flask_login.current_user.id:
             return flask.abort(403)
         else:
+            if not flask_login.login_fresh():
+                # ensure only fresh sessions can edit preferences including passwords and api tokens
+                return flask.redirect(flask.url_for('.refresh_sign_in', next=flask.url_for('.user_preferences', user_id=flask_login.current_user.id)))
             # user eingeloggt, change preferences möglich
             user = flask_login.current_user
             return change_preferences(user, user_id)
     else:
         return flask.current_app.login_manager.unauthorized()
 
 
 def change_preferences(user, user_id):
-    authentication_methods = Authentication.query.filter(Authentication.user_id == user_id).all()
+    api_tokens = Authentication.query.filter(Authentication.user_id == user_id, Authentication.type == AuthenticationType.API_TOKEN).all()
+    authentication_methods = Authentication.query.filter(Authentication.user_id == user_id, Authentication.type != AuthenticationType.API_TOKEN).all()
     authentication_method_ids = [authentication_method.id for authentication_method in authentication_methods]
-    confirmed_authentication_methods = Authentication.query.filter(Authentication.user_id == user_id, Authentication.confirmed == sqlalchemy.sql.expression.true()).count()
+    confirmed_authentication_methods = Authentication.query.filter(Authentication.user_id == user_id, Authentication.confirmed == sqlalchemy.sql.expression.true(), Authentication.type != AuthenticationType.API_TOKEN).count()
     change_user_form = ChangeUserForm()
     authentication_form = AuthenticationForm()
     authentication_method_form = AuthenticationMethodForm()
     authentication_password_form = AuthenticationPasswordForm()
 
+    created_api_token = None
+    create_api_token_form = CreateAPITokenForm()
+
     add_user_permissions_form = ObjectUserPermissionsForm()
     add_group_permissions_form = ObjectGroupPermissionsForm()
     add_project_permissions_form = ObjectProjectPermissionsForm()
 
     notification_mode_form = NotificationModeForm()
 
     other_settings_form = OtherSettingsForm()
@@ -93,15 +102,15 @@
     project_permission_form_data = []
     for project_id, permissions in project_permissions.items():
         if project_id is None:
             continue
         project_permission_form_data.append({'project_id': project_id, 'permissions': permissions.name.lower()})
     default_permissions_form = ObjectPermissionsForm(public_permissions=public_permissions.name.lower(), user_permissions=user_permission_form_data, group_permissions=group_permission_form_data, project_permissions=project_permission_form_data)
 
-    users = get_users()
+    users = get_users(exclude_hidden=True)
     users = [user for user in users if user.id not in user_permissions]
     groups = get_user_groups(flask_login.current_user.id)
     groups = [group for group in groups if group.id not in group_permissions]
     projects = get_user_projects(flask_login.current_user.id)
     projects = [project for project in projects if project.id not in project_permissions]
 
     if 'change' not in flask.request.form:
@@ -135,16 +144,17 @@
                                              groups=groups,
                                              get_group=get_group,
                                              user_permissions=user_permissions,
                                              group_permissions=group_permissions,
                                              public_permissions=public_permissions,
                                              authentication_method_form=authentication_method_form,
                                              authentication_form=authentication_form,
+                                             create_api_token_form=create_api_token_form,
                                              confirmed_authentication_methods=confirmed_authentication_methods,
-                                             authentications=authentication_methods, error=str(e))
+                                             authentications=authentication_methods, error=str(e), api_tokens=api_tokens)
             user_log.edit_user_preferences(user_id=user_id)
             return flask.redirect(flask.url_for('frontend.user_me_preferences'))
         else:
             flask.flash("Failed to change the password.", 'error')
     if 'change' in flask.request.form and flask.request.form['change'] == 'Change':
         if change_user_form.validate_on_submit():
             if change_user_form.name.data != user.name:
@@ -184,16 +194,17 @@
                                              groups=groups,
                                              get_group=get_group,
                                              user_permissions=user_permissions,
                                              group_permissions=group_permissions,
                                              public_permissions=public_permissions,
                                              authentication_method_form=authentication_method_form,
                                              authentication_form=authentication_form,
+                                             create_api_token_form=create_api_token_form,
                                              confirmed_authentication_methods=confirmed_authentication_methods,
-                                             authentications=authentication_methods, error=str(e))
+                                             authentications=authentication_methods, error=str(e), api_tokens=api_tokens)
             user_log.edit_user_preferences(user_id=user_id)
             return flask.redirect(flask.url_for('frontend.user_me_preferences'))
     if 'add' in flask.request.form and flask.request.form['add'] == 'Add':
         if authentication_form.validate_on_submit():
             # check, if login already exists
             all_authentication_methods = {
                 'E': AuthenticationType.EMAIL,
@@ -227,19 +238,52 @@
                                              groups=groups,
                                              get_group=get_group,
                                              user_permissions=user_permissions,
                                              group_permissions=group_permissions,
                                              public_permissions=public_permissions,
                                              authentication_method_form=authentication_method_form,
                                              authentication_form=authentication_form,
+                                             create_api_token_form=create_api_token_form,
                                              confirmed_authentication_methods=confirmed_authentication_methods,
-                                             authentications=authentication_methods, error_add=str(e))
-            authentication_methods = Authentication.query.filter(Authentication.user_id == user_id).all()
+                                             authentications=authentication_methods, error_add=str(e), api_tokens=api_tokens)
+            authentication_methods = Authentication.query.filter(Authentication.user_id == user_id, Authentication.type != AuthenticationType.API_TOKEN).all()
         else:
             flask.flash("Failed to add an authentication method.", 'error')
+    if 'create_api_token' in flask.request.form and create_api_token_form.validate_on_submit():
+        created_api_token = secrets.token_hex(32)
+        description = create_api_token_form.description.data
+        try:
+            add_api_token(flask_login.current_user.id, created_api_token, description)
+            api_tokens = Authentication.query.filter(Authentication.user_id == user_id, Authentication.type == AuthenticationType.API_TOKEN).all()
+        except Exception as e:
+            flask.flash("Failed to add an API token.", 'error')
+            return flask.render_template('preferences.html', user=user, change_user_form=change_user_form,
+                                         authentication_password_form=authentication_password_form,
+                                         default_permissions_form=default_permissions_form,
+                                         add_user_permissions_form=add_user_permissions_form,
+                                         add_group_permissions_form=add_group_permissions_form,
+                                         notification_mode_form=notification_mode_form,
+                                         Permissions=Permissions,
+                                         NotificationMode=NotificationMode,
+                                         NotificationType=NotificationType,
+                                         notification_modes=get_notification_modes(flask_login.current_user.id),
+                                         user_settings=user_settings,
+                                         other_settings_form=other_settings_form,
+                                         get_user=get_user,
+                                         users=users,
+                                         groups=groups,
+                                         get_group=get_group,
+                                         user_permissions=user_permissions,
+                                         group_permissions=group_permissions,
+                                         public_permissions=public_permissions,
+                                         authentication_method_form=authentication_method_form,
+                                         authentication_form=authentication_form,
+                                         create_api_token_form=create_api_token_form,
+                                         confirmed_authentication_methods=confirmed_authentication_methods,
+                                         authentications=authentication_methods, error_add=str(e), api_tokens=api_tokens)
     if 'edit_user_permissions' in flask.request.form and default_permissions_form.validate_on_submit():
         set_default_public(creator_id=flask_login.current_user.id, is_public=(default_permissions_form.public_permissions.data == 'read'))
         for user_permissions_data in default_permissions_form.user_permissions.data:
             user_id = user_permissions_data['user_id']
             try:
                 get_user(user_id)
             except UserDoesNotExistError:
@@ -297,15 +341,15 @@
                 notification_mode_text = flask.request.form.get('notification_mode_for_type_' + notification_type.name.lower())
                 for notification_mode in [NotificationMode.IGNORE, NotificationMode.WEBAPP, NotificationMode.EMAIL]:
                     if notification_mode_text == notification_mode.name.lower():
                         set_notification_mode_for_type(notification_type, flask_login.current_user.id, notification_mode)
                         break
         flask.flash("Successfully updated your notification settings.", 'success')
         return flask.redirect(flask.url_for('.user_preferences', user_id=flask_login.current_user.id))
-    confirmed_authentication_methods = Authentication.query.filter(Authentication.user_id == user_id, Authentication.confirmed == sqlalchemy.sql.expression.true()).count()
+    confirmed_authentication_methods = Authentication.query.filter(Authentication.user_id == user_id, Authentication.confirmed == sqlalchemy.sql.expression.true(), Authentication.type != AuthenticationType.API_TOKEN).count()
     if 'edit_other_settings' in flask.request.form and other_settings_form.validate_on_submit():
         use_schema_editor = flask.request.form.get('input-use-schema-editor', 'yes') != 'no'
         modified_settings = {
             'USE_SCHEMA_EDITOR': use_schema_editor
         }
 
         objects_per_page = flask.request.form.get('input-objects-per-page', '')
@@ -341,16 +385,18 @@
                                  get_project=get_project,
                                  user_permissions=user_permissions,
                                  group_permissions=group_permissions,
                                  project_permissions=project_permissions,
                                  public_permissions=public_permissions,
                                  authentication_method_form=authentication_method_form,
                                  authentication_form=authentication_form,
+                                 create_api_token_form=create_api_token_form,
+                                 created_api_token=created_api_token,
                                  confirmed_authentication_methods=confirmed_authentication_methods,
-                                 authentications=authentication_methods)
+                                 authentications=authentication_methods, api_tokens=api_tokens)
 
 
 def confirm_email():
     token = flask.request.args.get('token')
     data1 = verify_token(token, salt='edit_profile', secret_key=flask.current_app.config['SECRET_KEY'])
     data2 = verify_token(token, salt='add_login', secret_key=flask.current_app.config['SECRET_KEY'])
     if data1 is None and data2 is None:
```

### Comparing `sampledb-0.8.1/sampledb/frontend/users_forms.py` & `sampledb-0.9.0/sampledb/frontend/users_forms.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/frontend/utils.py` & `sampledb-0.9.0/sampledb/frontend/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 import base64
 from io import BytesIO
 import os
 from urllib.parse import quote_plus
 
 import flask
+import flask_login
 import qrcode
 import qrcode.image.svg
 
+from ..logic.errors import UserIsReadonlyError
 from ..logic.units import prettify_units
 from ..logic.notifications import get_num_notifications
 
 
 def jinja_filter(func):
     global _jinja_filters
     _jinja_filters[func.__name__] = func
@@ -65,12 +67,17 @@
     return flask.current_app.config.get('MIME_TYPES', {}).get(file_extension, '').startswith('image/')
 
 
 def get_num_unread_notifications(user):
     return get_num_notifications(user.id, unread_only=True)
 
 
+def check_current_user_is_not_readonly():
+    if flask_login.current_user.is_readonly:
+        raise UserIsReadonlyError()
+
+
 _jinja_filters['prettify_units'] = prettify_units
 _jinja_filters['has_preview'] = has_preview
 _jinja_filters['is_image'] = is_image
 _jinja_filters['get_num_unread_notifications'] = get_num_unread_notifications
 _jinja_filters['urlencode'] = quote_plus
```

### Comparing `sampledb-0.8.1/sampledb/logic/__init__.py` & `sampledb-0.9.0/sampledb/logic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding: utf-8
 """
 
 """
 
 from . import actions
+from . import api_log
 from . import authentication
 from . import comments
 from . import datatypes
 from . import errors
 from . import favorites
 from . import files
 from . import groups
@@ -36,14 +37,15 @@
 from ..models.objects import Objects
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 
 __all__ = [
     'actions',
+    'api_log',
     'authentication',
     'comments',
     'datatypes',
     'errors',
     'favorites',
     'files',
     'groups',
```

### Comparing `sampledb-0.8.1/sampledb/logic/action_permissions.py` & `sampledb-0.9.0/sampledb/logic/action_permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,18 @@
         for project_action_permissions in ProjectActionPermissions.query.filter_by(action_id=action_id).all():
             for user_id, permissions in projects.get_project_member_user_ids_and_permissions(project_action_permissions.project_id, include_groups=include_groups).items():
                 permissions = min(permissions, project_action_permissions.permissions)
                 previous_permissions = action_permissions.get(user_id, Permissions.NONE)
                 action_permissions[user_id] = max(previous_permissions, permissions)
     if action.user_id is not None:
         action_permissions[action.user_id] = Permissions.GRANT
+    for user_id in action_permissions:
+        user = users.get_user(user_id)
+        if user.is_readonly:
+            action_permissions[user_id] = min(action_permissions[user_id], Permissions.READ)
     return action_permissions
 
 
 def _get_action_responsible_user_ids(action_id: int) -> typing.List[int]:
     try:
         action = actions.get_action(action_id)
     except errors.ActionDoesNotExistError:
@@ -157,51 +161,56 @@
         exists
     """
     # ensure that the action can be found
     action = actions.get_action(action_id)
     # ensure that the user can be found
     user = users.get_user(user_id)
 
+    if user.is_readonly:
+        max_permissions = Permissions.READ
+    else:
+        max_permissions = Permissions.GRANT
+
     # administrators always have GRANT permissions
     if user.is_admin:
-        return Permissions.GRANT
+        return min(Permissions.GRANT, max_permissions)
     # action owners always have GRANT permissions
     if action.user_id == user_id:
-        return Permissions.GRANT
+        return min(Permissions.GRANT, max_permissions)
     if include_instrument_responsible_users:
         # instrument responsible users always have GRANT permissions for an action
         if user_id in _get_action_responsible_user_ids(action_id):
-            return Permissions.GRANT
+            return min(Permissions.GRANT, max_permissions)
     # other users might have been granted permissions, either individually or as group or project members
     user_action_permissions = UserActionPermissions.query.filter_by(action_id=action_id, user_id=user_id).first()
     if user_action_permissions is None:
         permissions = Permissions.NONE
     else:
         permissions = user_action_permissions.permissions
     if Permissions.GRANT in permissions:
-        return permissions
+        return min(permissions, max_permissions)
     if include_groups:
         for group in groups.get_user_groups(user_id):
             group_action_permissions = GroupActionPermissions.query.filter_by(action_id=action_id, group_id=group.id).first()
             if group_action_permissions is not None and permissions in group_action_permissions.permissions:
                 permissions = group_action_permissions.permissions
     if Permissions.GRANT in permissions:
-        return permissions
+        return min(permissions, max_permissions)
     if include_projects:
         for user_project in projects.get_user_projects(user_id, include_groups=include_groups):
             user_project_permissions = projects.get_user_project_permissions(user_project.id, user_id, include_groups=include_groups)
             if user_project_permissions not in permissions:
                 project_action_permissions = ProjectActionPermissions.query.filter_by(action_id=action_id, project_id=user_project.id).first()
                 if project_action_permissions is not None:
                     permissions = min(user_project_permissions, project_action_permissions.permissions)
     if Permissions.READ in permissions:
-        return permissions
+        return min(permissions, max_permissions)
     # lastly, the action may be public, so all users have READ permissions
     if action_is_public(action_id):
-        return Permissions.READ
+        return min(Permissions.READ, max_permissions)
     # otherwise the user has no permissions for this action
     return Permissions.NONE
 
 
 def set_user_action_permissions(action_id: int, user_id: int, permissions: Permissions):
     """
     Set the action permissions for a user.
```

### Comparing `sampledb-0.8.1/sampledb/logic/actions.py` & `sampledb-0.9.0/sampledb/logic/actions.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/authentication.py` & `sampledb-0.9.0/sampledb/logic/authentication.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import bcrypt
 import typing
-
+import flask
 
 from .. import logic, db
 from .ldap import validate_user, create_user_from_ldap, is_ldap_configured
 from ..models import Authentication, AuthenticationType, User
-from . import errors
+from . import errors, api_log
 
 
 def _hash_password(password: str) -> str:
     return bcrypt.hashpw(password.encode('utf-8'), bcrypt.gensalt()).decode('utf-8')
 
 
 def _validate_password_hash(password: str, password_hash: str) -> bool:
@@ -85,14 +85,41 @@
         confirmed=confirmed,
         user_id=user_id
     )
     db.session.add(authentication)
     db.session.commit()
 
 
+def add_api_token(user_id: int, api_token: str, description: str) -> None:
+    """
+    Add an API token as an authentication method for a given user.
+
+    :param user_id: the ID of an existing user
+    :param api_token: the api token as a 64 character string
+    :param description: a description for the token
+    """
+
+    assert len(api_token) == 64
+    api_token = api_token.lower()
+    # split into a short part (8 hex digits / 4 bytes) for identification and a long part for authentication
+    login, password = api_token[:8], api_token[8:]
+    authentication = Authentication(
+        login={
+            'login': login,
+            'bcrypt_hash': _hash_password(password),
+            'description': description
+        },
+        authentication_type=AuthenticationType.API_TOKEN,
+        confirmed=True,
+        user_id=user_id
+    )
+    db.session.add(authentication)
+    db.session.commit()
+
+
 def login(login: str, password: str) -> typing.Optional[User]:
     """
     Authenticate a user and create an LDAP based user if necessary.
 
     :param login: the name, email or LDAP uid to use during authentication
     :param password: the password
     :return: the user or None
@@ -135,14 +162,38 @@
         except errors.AuthenticationMethodAlreadyExists:
             # user might have been created in the background already due to concurrent, duplicate requests
             pass
         return user
     return None
 
 
+def login_via_api_token(api_token: str) -> typing.Optional[User]:
+    """
+    Authenticate a user using an API token.
+
+    :param api_token: the API token to use during authentication
+    :return: the user or None
+    """
+    # convert to lower case to enforce case insensitivity
+    api_token = api_token.lower().strip()
+    username, password = api_token[:8], api_token[8:]
+    authentication_methods = Authentication.query.filter(
+        db.and_(Authentication.login['login'].astext == username,
+                Authentication.type == AuthenticationType.API_TOKEN)
+    ).all()
+
+    for authentication_method in authentication_methods:
+        if not authentication_method.confirmed:
+            continue
+        if _validate_password_authentication(authentication_method, password):
+            api_log.create_log_entry(authentication_method.id, getattr(api_log.HTTPMethod, flask.request.method, api_log.HTTPMethod.OTHER), flask.request.path)
+            return authentication_method.user
+    return None
+
+
 def add_authentication_method(user_id: int, login: str, password: str, authentication_type: AuthenticationType) -> bool:
     """
     Add an authentication method for a user.
 
     :param user_id: the ID of an existing user
     :param login: the name, email or LDAP uid to use
     :param password: the password
@@ -175,17 +226,18 @@
 
     :param authentication_method_id: the ID of an existing authentication method
     :return:
     """
     authentication_method = Authentication.query.filter(Authentication.id == authentication_method_id).first()
     if authentication_method is None:
         return False
-    authentication_methods_count = Authentication.query.filter(Authentication.user_id == authentication_method.user_id).count()
-    if authentication_methods_count <= 1:
-        raise errors.OnlyOneAuthenticationMethod('one authentication-method must at least exist, delete not possible')
+    if authentication_method.type != AuthenticationType.API_TOKEN:
+        authentication_methods_count = Authentication.query.filter(Authentication.user_id == authentication_method.user_id, Authentication.type != AuthenticationType.API_TOKEN).count()
+        if authentication_methods_count <= 1:
+            raise errors.OnlyOneAuthenticationMethod('one authentication-method must at least exist, delete not possible')
     db.session.delete(authentication_method)
     db.session.commit()
     return True
 
 
 def change_password_in_authentication_method(authentication_method_id: int, password: str) -> bool:
     """
@@ -204,7 +256,19 @@
         return False
     if authentication_method.type not in {AuthenticationType.EMAIL, AuthenticationType.OTHER}:
         return False
     authentication_method.login = {'login': authentication_method.login['login'], 'bcrypt_hash': _hash_password(password)}
     db.session.add(authentication_method)
     db.session.commit()
     return True
+
+
+def is_login_available(login: str) -> bool:
+    """
+    Return whether or not a login is still available for use.
+
+    For password-based authentication, the login can only be used once.
+
+    :param login: the login for which to check availability
+    :return: whether the login is available
+    """
+    return Authentication.query.filter(Authentication.login['login'].astext == login).first() is None
```

### Comparing `sampledb-0.8.1/sampledb/logic/comments.py` & `sampledb-0.9.0/sampledb/logic/comments.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/datatypes.py` & `sampledb-0.9.0/sampledb/logic/datatypes.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/errors.py` & `sampledb-0.9.0/sampledb/logic/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,7 +180,11 @@
 
 class InvalidDOIError(Exception):
     pass
 
 
 class LDAPNotConfiguredError(Exception):
     pass
+
+
+class UserIsReadonlyError(Exception):
+    pass
```

### Comparing `sampledb-0.8.1/sampledb/logic/favorites.py` & `sampledb-0.9.0/sampledb/logic/favorites.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/files.py` & `sampledb-0.9.0/sampledb/logic/files.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/groups.py` & `sampledb-0.9.0/sampledb/logic/groups.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/instruments.py` & `sampledb-0.9.0/sampledb/logic/instruments.py`

 * *Files 9% similar despite different names*

```diff
@@ -124,14 +124,36 @@
     if user not in instrument.responsible_users:
         raise errors.UserNotResponsibleForInstrumentError()
     instrument.responsible_users.remove(user)
     db.session.add(instrument)
     db.session.commit()
 
 
+def set_instrument_responsible_users(instrument_id: int, user_ids: typing.List[int]) -> None:
+    """
+    Set the list of instrument responsible users for a an instrument.
+
+    :param instrument_id: the ID of an existing instrument
+    :param user_ids: the IDs of existing users
+    :raise errors.InstrumentDoesNotExistError: when no instrument with the
+        given instrument ID exists
+    :raise errors.UserDoesNotExistError: when no user with one of the given
+        user IDs exists
+    """
+    instrument = Instrument.query.get(instrument_id)
+    if instrument is None:
+        raise errors.InstrumentDoesNotExistError()
+    instrument.responsible_users.clear()
+    for user_id in user_ids:
+        user = users.get_user(user_id)
+        instrument.responsible_users.append(user)
+    db.session.add(instrument)
+    db.session.commit()
+
+
 def get_user_instruments(user_id: int) -> typing.List[int]:
     """
     Get a list of instruments a user with a given user ID is responsible for.
 
     :param user_id: the ID of an existing user
     :return: a list of instrument IDs
     :raise errors.UserDoesNotExistError: when no user with the given user ID
```

### Comparing `sampledb-0.8.1/sampledb/logic/ldap.py` & `sampledb-0.9.0/sampledb/logic/ldap.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/locations.py` & `sampledb-0.9.0/sampledb/logic/locations.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/notifications.py` & `sampledb-0.9.0/sampledb/logic/notifications.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/object_log.py` & `sampledb-0.9.0/sampledb/logic/object_log.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/object_permissions.py` & `sampledb-0.9.0/sampledb/logic/object_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from . import actions
 from .groups import get_user_groups, get_group_member_ids
 from .instruments import get_instrument
 from .notifications import create_notification_for_having_received_an_objects_permissions_request
 from . import objects
 from ..models import Permissions, UserObjectPermissions, GroupObjectPermissions, ProjectObjectPermissions, PublicObjects, ActionType, Action, Object, DefaultUserPermissions, DefaultGroupPermissions, DefaultProjectPermissions, DefaultPublicPermissions
 from . import projects
+from .users import get_user
 
 
 __author__ = 'Florian Rhiem <f.rhiem@fz-juelich.de>'
 
 
 def object_is_public(object_id: int):
     return PublicObjects.query.filter_by(object_id=object_id).first() is not None
@@ -42,15 +43,15 @@
     if not is_public:
         PublicObjects.query.filter_by(object_id=object_id).delete()
     elif not object_is_public(object_id):
         db.session.add(PublicObjects(object_id=object_id))
     db.session.commit()
 
 
-def get_object_permissions_for_users(object_id: int, include_instrument_responsible_users: bool = True, include_groups: bool = True, include_projects: bool = True):
+def get_object_permissions_for_users(object_id: int, include_instrument_responsible_users: bool = True, include_groups: bool = True, include_projects: bool = True, include_readonly: bool = True):
     object_permissions = {}
     for user_object_permissions in UserObjectPermissions.query.filter_by(object_id=object_id).all():
         object_permissions[user_object_permissions.user_id] = user_object_permissions.permissions
     if include_instrument_responsible_users:
         for user_id in _get_object_responsible_user_ids(object_id):
             object_permissions[user_id] = Permissions.GRANT
     if include_groups:
@@ -60,14 +61,18 @@
                     object_permissions[user_id] = group_object_permissions.permissions
     if include_projects:
         for project_object_permissions in ProjectObjectPermissions.query.filter_by(object_id=object_id).all():
             for user_id, permissions in projects.get_project_member_user_ids_and_permissions(project_object_permissions.project_id, include_groups=include_groups).items():
                 permissions = min(permissions, project_object_permissions.permissions)
                 previous_permissions = object_permissions.get(user_id, Permissions.NONE)
                 object_permissions[user_id] = max(previous_permissions, permissions)
+    if include_readonly:
+        for user_id in object_permissions:
+            if get_user(user_id).is_readonly:
+                object_permissions[user_id] = min(object_permissions[user_id], Permissions.READ)
     return object_permissions
 
 
 def get_object_permissions_for_groups(object_id: int, include_projects: bool = False) -> typing.Dict[int, Permissions]:
     object_permissions = {}
     for group_object_permissions in GroupObjectPermissions.query.filter_by(object_id=object_id).all():
         if group_object_permissions.permissions != Permissions.NONE:
@@ -97,63 +102,73 @@
         return []
     if action.instrument_id is None:
         return []
     instrument = get_instrument(action.instrument_id)
     return [user.id for user in instrument.responsible_users]
 
 
-def get_user_object_permissions(object_id: int, user_id: int, include_instrument_responsible_users: bool = True, include_groups: bool = True, include_projects: bool = True):
-    assert user_id is not None
+def get_user_object_permissions(object_id: int, user_id: int, include_instrument_responsible_users: bool = True, include_groups: bool = True, include_projects: bool = True, include_readonly: bool = True):
+    user = get_user(user_id)
 
     if include_instrument_responsible_users and include_groups and include_projects:
         stmt = db.text("""
         SELECT
         MAX(permissions_int)
         FROM user_object_permissions_by_all
         WHERE (user_id = :user_id OR user_id IS NULL) AND object_id = :object_id
         """)
         permissions_int = db.engine.execute(stmt, {
             'user_id': user_id,
             'object_id': object_id
         }).fetchone()[0]
         if permissions_int is None or permissions_int <= 0:
             return Permissions.NONE
+        elif include_readonly and user.is_readonly and permissions_int in (1, 2, 3):
+            return Permissions.READ
         elif permissions_int == 1:
             return Permissions.READ
         elif permissions_int == 2:
             return Permissions.WRITE
         elif permissions_int >= 3:
             return Permissions.GRANT
 
     if include_instrument_responsible_users:
         # instrument responsible users always have GRANT permissions for an object
         if user_id in _get_object_responsible_user_ids(object_id):
+            if include_readonly and user.is_readonly:
+                return Permissions.READ
             return Permissions.GRANT
     # other users might have been granted permissions, either individually or as group or project members
     user_object_permissions = UserObjectPermissions.query.filter_by(object_id=object_id, user_id=user_id).first()
     if user_object_permissions is None:
         permissions = Permissions.NONE
     else:
         permissions = user_object_permissions.permissions
+    if include_readonly and user.is_readonly and Permissions.READ in permissions:
+        return Permissions.READ
     if Permissions.GRANT in permissions:
         return permissions
     if include_groups:
         for group in get_user_groups(user_id):
             group_object_permissions = GroupObjectPermissions.query.filter_by(object_id=object_id, group_id=group.id).first()
             if group_object_permissions is not None and permissions in group_object_permissions.permissions:
                 permissions = group_object_permissions.permissions
+    if include_readonly and user.is_readonly and Permissions.READ in permissions:
+        return Permissions.READ
     if Permissions.GRANT in permissions:
         return permissions
     if include_projects:
         for user_project in projects.get_user_projects(user_id, include_groups=include_groups):
             user_project_permissions = projects.get_user_project_permissions(user_project.id, user_id, include_groups=include_groups)
             if user_project_permissions not in permissions:
                 project_object_permissions = ProjectObjectPermissions.query.filter_by(object_id=object_id, project_id=user_project.id).first()
                 if project_object_permissions is not None:
                     permissions = min(user_project_permissions, project_object_permissions.permissions)
+    if include_readonly and user.is_readonly and Permissions.READ in permissions:
+        return Permissions.READ
     if Permissions.READ in permissions:
         return permissions
     # lastly, the object may be public, so all users have READ permissions
     if object_is_public(object_id):
         return Permissions.READ
     # otherwise the user has no permissions for this object
     return Permissions.NONE
```

### Comparing `sampledb-0.8.1/sampledb/logic/object_relationships.py` & `sampledb-0.9.0/sampledb/logic/object_relationships.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/object_search.py` & `sampledb-0.9.0/sampledb/logic/object_search.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/object_search_parser.py` & `sampledb-0.9.0/sampledb/logic/object_search_parser.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/object_sorting.py` & `sampledb-0.9.0/sampledb/logic/object_sorting.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/objects.py` & `sampledb-0.9.0/sampledb/logic/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
     :param object: the updated (or newly created) object
     :param find_previous_referenced_object_ids: whether or not to find
         previous referenced object ids
     """
     referenced_object_ids = []
     for path, schema, data in _get_object_properties(object):
-        if schema['type'] == 'sample' and data is not None and data['object_id'] is not None:
+        if schema['type'] in ('sample', 'measurement') and data is not None and data['object_id'] is not None:
             referenced_object_id = data['object_id']
             previous_referenced_object_id = None
             if find_previous_referenced_object_ids and object.version_id > 0:
                 previous_object_version = get_object(object.object_id, object.version_id - 1)
                 previous_data = previous_object_version.data
                 try:
                     for path_element in path:
@@ -251,17 +251,17 @@
     return referenced_object_ids
 
 
 def _update_object_references(object: Object, user_id: int) -> None:
     """
     Searches for references to other objects and updates these accordingly.
 
-    At this time, only measurements or samples referencing samples will be
-    handled, adding an entry to the sample's object log about being used in a
-    measurement.
+    At this time, only measurements or samples referencing other measurements
+    or samples will be handled, adding an entry to the object's log about
+    being used in a sample or measurement.
 
     :param object: the updated (or newly created) object
     :param user_id: the user who caused the object update or creation
     """
     action_type = actions.get_action(object.action_id).type
     for referenced_object_id, previous_referenced_object_id in find_object_references(object):
         if referenced_object_id != previous_referenced_object_id:
```

### Comparing `sampledb-0.8.1/sampledb/logic/projects.py` & `sampledb-0.9.0/sampledb/logic/projects.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/publications.py` & `sampledb-0.9.0/sampledb/logic/publications.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/schemas/__init__.py` & `sampledb-0.9.0/sampledb/logic/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/schemas/convert_to_schema.py` & `sampledb-0.9.0/sampledb/logic/schemas/convert_to_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Convert data from one schema to another.
 
     :param data: the sampledb object data
     :param previous_schema: the sampledb object schema for the given data
     :param new_schema: the target sampledb object schema
     :return: the converted data and a list of conversion warnings/notes
     """
-    if new_schema == previous_schema and new_schema['type'] in ('bool', 'text', 'datetime', 'tags', 'sample', 'quantity', 'array', 'objects', 'hazards'):
+    if new_schema == previous_schema and new_schema['type'] in ('bool', 'text', 'datetime', 'tags', 'sample', 'measurement', 'quantity', 'array', 'objects', 'hazards'):
         return data, []
 
     if new_schema['type'] == 'tags' and previous_schema['type'] == 'text':
         tags = []
         for tag in data['text'].split(','):
             tag = tag.strip().lower()
             if tag not in tags:
@@ -29,15 +29,15 @@
         new_data = {
             '_type': 'tags',
             'tags': tags
         }
         return new_data, []
     if previous_schema['type'] != new_schema['type']:
         return generate_placeholder(new_schema), ["Unable to convert property '{}' from type '{}' to type '{}'.".format(new_schema['title'], previous_schema['type'], new_schema['type'])]
-    if new_schema['type'] in ('bool', 'text', 'datetime', 'tags', 'sample', 'hazards'):
+    if new_schema['type'] in ('bool', 'text', 'datetime', 'tags', 'sample', 'measurement', 'hazards'):
         return data, []
     if new_schema['type'] == 'quantity':
         previous_dimensionality = get_dimensionality_for_units(previous_schema['units'])
         new_dimensionality = get_dimensionality_for_units(new_schema['units'])
         if new_dimensionality == previous_dimensionality:
             return data, []
         return generate_placeholder(new_schema), ["Unable to convert quantity '{}' to different dimensionality: {} -> {}".format(new_schema['title'], previous_dimensionality, new_dimensionality)]
```

### Comparing `sampledb-0.8.1/sampledb/logic/schemas/generate_placeholder.py` & `sampledb-0.9.0/sampledb/logic/schemas/generate_placeholder.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
         return _generate_datetime_placeholder(schema, path)
     elif schema['type'] == 'bool':
         return _generate_bool_placeholder(schema, path)
     elif schema['type'] == 'quantity':
         return _generate_quantity_placeholder(schema, path)
     elif schema['type'] == 'sample':
         return _generate_sample_placeholder(schema, path)
+    elif schema['type'] == 'measurement':
+        return _generate_measurement_placeholder(schema, path)
     elif schema['type'] == 'tags':
         return _generate_tags_placeholder(schema, path)
     elif schema['type'] == 'hazards':
         return _generate_hazards_placeholder(schema, path)
     else:
         raise SchemaError('invalid type', path)
 
@@ -196,7 +198,18 @@
     Generates a placeholder sample object based on an object schema.
 
     :param schema: the sampledb object schema
     :param path: the path to this subschema
     :return: None, as there can be no default sample
     """
     return None
+
+
+def _generate_measurement_placeholder(schema: dict, path: typing.List[str]) -> None:
+    """
+    Generates a placeholder measurement object based on an object schema.
+
+    :param schema: the sampledb object schema
+    :param path: the path to this subschema
+    :return: None, as there can be no default measurement
+    """
+    return None
```

### Comparing `sampledb-0.8.1/sampledb/logic/schemas/utils.py` & `sampledb-0.9.0/sampledb/logic/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/schemas/validate.py` & `sampledb-0.9.0/sampledb/logic/schemas/validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         return _validate_datetime(instance, schema, path)
     elif schema['type'] == 'bool':
         return _validate_bool(instance, schema, path)
     elif schema['type'] == 'quantity':
         return _validate_quantity(instance, schema, path)
     elif schema['type'] == 'sample':
         return _validate_sample(instance, schema, path)
+    elif schema['type'] == 'measurement':
+        return _validate_measurement(instance, schema, path)
     elif schema['type'] == 'tags':
         return _validate_tags(instance, schema, path)
     elif schema['type'] == 'hazards':
         return _validate_hazards(instance, schema, path)
     else:
         raise ValidationError('invalid type', path)
 
@@ -359,7 +361,40 @@
     try:
         sample = objects.get_object(object_id=instance['object_id'])
     except ObjectDoesNotExistError:
         raise ValidationError('object does not exist', path)
     action = actions.get_action(sample.action_id)
     if action.type != actions.ActionType.SAMPLE_CREATION:
         raise ValidationError('object must be sample', path)
+
+
+def _validate_measurement(instance: dict, schema: dict, path: typing.List[str]) -> None:
+    """
+    Validates the given instance using the given measurement object schema and raises a ValidationError if it is invalid.
+
+    :param instance: the sampledb object
+    :param schema: the valid sampledb object schema
+    :param path: the path to this subinstance / subschema
+    :raise ValidationError: if the schema is invalid.
+    """
+    if not isinstance(instance, dict):
+        raise ValidationError('instance must be dict', path)
+    valid_keys = {'_type', 'object_id'}
+    required_keys = valid_keys
+    schema_keys = set(instance.keys())
+    invalid_keys = schema_keys - valid_keys
+    if invalid_keys:
+        raise ValidationError('unexpected keys in schema: {}'.format(invalid_keys), path)
+    missing_keys = required_keys - schema_keys
+    if missing_keys:
+        raise ValidationError('missing keys in schema: {}'.format(missing_keys), path)
+    if instance['_type'] != 'measurement':
+        raise ValidationError('expected _type "measurement"', path)
+    if not isinstance(instance['object_id'], int):
+        raise ValidationError('object_id must be int', path)
+    try:
+        measurement = objects.get_object(object_id=instance['object_id'])
+    except ObjectDoesNotExistError:
+        raise ValidationError('object does not exist', path)
+    action = actions.get_action(measurement.action_id)
+    if action.type != actions.ActionType.MEASUREMENT:
+        raise ValidationError('object must be measurement', path)
```

### Comparing `sampledb-0.8.1/sampledb/logic/schemas/validate_schema.py` & `sampledb-0.9.0/sampledb/logic/schemas/validate_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         return _validate_datetime_schema(schema, path)
     elif schema['type'] == 'bool':
         return _validate_bool_schema(schema, path)
     elif schema['type'] == 'quantity':
         return _validate_quantity_schema(schema, path)
     elif schema['type'] == 'sample':
         return _validate_sample_schema(schema, path)
+    elif schema['type'] == 'measurement':
+        return _validate_measurement_schema(schema, path)
     elif schema['type'] == 'tags':
         return _validate_tags_schema(schema, path)
     elif schema['type'] == 'hazards':
         return _validate_hazards_schema(schema, path)
     else:
         raise ValidationError('invalid type', path)
 
@@ -371,14 +373,35 @@
 
     :param schema: the sampledb object schema
     :param path: the path to this subschema
     :raise ValidationError: if the schema is invalid.
     """
     valid_keys = {'type', 'title', 'note'}
     required_keys = {'type', 'title'}
+    schema_keys = set(schema.keys())
+    invalid_keys = schema_keys - valid_keys
+    if invalid_keys:
+        raise ValidationError('unexpected keys in schema: {}'.format(invalid_keys), path)
+    missing_keys = required_keys - schema_keys
+    if missing_keys:
+        raise ValidationError('missing keys in schema: {}'.format(missing_keys), path)
+    if 'note' in schema and not isinstance(schema['note'], str):
+        raise ValidationError('note must be str', path)
+
+
+def _validate_measurement_schema(schema: dict, path: typing.List[str]) -> None:
+    """
+    Validates the given measurement object schema and raises a ValidationError if it is invalid.
+
+    :param schema: the sampledb object schema
+    :param path: the path to this subschema
+    :raise ValidationError: if the schema is invalid.
+    """
+    valid_keys = {'type', 'title', 'note'}
+    required_keys = {'type', 'title'}
     schema_keys = set(schema.keys())
     invalid_keys = schema_keys - valid_keys
     if invalid_keys:
         raise ValidationError('unexpected keys in schema: {}'.format(invalid_keys), path)
     missing_keys = required_keys - schema_keys
     if missing_keys:
         raise ValidationError('missing keys in schema: {}'.format(missing_keys), path)
```

### Comparing `sampledb-0.8.1/sampledb/logic/security_tokens.py` & `sampledb-0.9.0/sampledb/logic/security_tokens.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/settings.py` & `sampledb-0.9.0/sampledb/logic/settings.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/tags.py` & `sampledb-0.9.0/sampledb/logic/tags.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/units.py` & `sampledb-0.9.0/sampledb/logic/units.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/user_log.py` & `sampledb-0.9.0/sampledb/logic/user_log.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/utils.py` & `sampledb-0.9.0/sampledb/logic/utils.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/logic/where_filters.py` & `sampledb-0.9.0/sampledb/logic/where_filters.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/__init__.py` & `sampledb-0.9.0/sampledb/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from . import object_permissions
 from . import projects
 from . import settings
 from . import users
 
 from .actions import Action, ActionType
 from .action_permissions import UserActionPermissions, GroupActionPermissions, ProjectActionPermissions, PublicActions
+from .api_log import APILogEntry, HTTPMethod
 from .authentication import Authentication, AuthenticationType
 from .comments import Comment
 from .favorites import FavoriteAction, FavoriteInstrument
 from .files import File
 from .groups import Group
 from .instruments import Instrument
 from .locations import Location, ObjectLocationAssignment
@@ -34,14 +35,15 @@
 from .settings import Settings
 from .tags import Tag
 from .users import User, UserType
 from .user_log import UserLogEntry, UserLogEntryType
 
 
 __all__ = [
+    'api_log',
     'authentication',
     'favorites',
     'files',
     'groups',
     'instruments',
     'locations',
     'objects',
@@ -51,21 +53,23 @@
     'users',
     'Action',
     'ActionType',
     'UserActionPermissions',
     'GroupActionPermissions',
     'ProjectActionPermissions',
     'PublicActions',
+    'APILogEntry',
     'Authentication',
     'AuthenticationType',
     'Comment',
     'FavoriteAction',
     'FavoriteInstrument',
     'File',
     'Group',
+    'HTTPMethod',
     'Instrument',
     'Location',
     'ObjectLocationAssignment',
     'Notification',
     'NotificationType',
     'NotificationMode',
     'NotificationModeForType',
```

### Comparing `sampledb-0.8.1/sampledb/models/action_permissions.py` & `sampledb-0.9.0/sampledb/models/action_permissions.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/actions.py` & `sampledb-0.9.0/sampledb/models/actions.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/authentication.py` & `sampledb-0.9.0/sampledb/models/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 @enum.unique
 class AuthenticationType(enum.Enum):
     LDAP = 1
     EMAIL = 2
     OTHER = 3
+    API_TOKEN = 4
 
 
 class Authentication(db.Model):
     __tablename__ = "authentications"
 
     id = db.Column(db.Integer, primary_key=True)
     user_id = db.Column(db.Integer, db.ForeignKey('users.id'))
```

### Comparing `sampledb-0.8.1/sampledb/models/comments.py` & `sampledb-0.9.0/sampledb/models/comments.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/favorites.py` & `sampledb-0.9.0/sampledb/models/favorites.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/file_log.py` & `sampledb-0.9.0/sampledb/models/file_log.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/files.py` & `sampledb-0.9.0/sampledb/models/files.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/groups.py` & `sampledb-0.9.0/sampledb/models/groups.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/instruments.py` & `sampledb-0.9.0/sampledb/models/instruments.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/locations.py` & `sampledb-0.9.0/sampledb/models/locations.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/__init__.py` & `sampledb-0.9.0/sampledb/models/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/actions_add_user_id.py` & `sampledb-0.9.0/sampledb/models/migrations/actions_add_user_id.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/create_migration_index.py` & `sampledb-0.9.0/sampledb/models/migrations/create_migration_index.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/create_user_object_permissions_by_all_view.py` & `sampledb-0.9.0/sampledb/models/migrations/create_user_object_permissions_by_all_view.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/files_add_data.py` & `sampledb-0.9.0/sampledb/models/migrations/files_add_data.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/object_location_assignments_add_confirmed.py` & `sampledb-0.9.0/sampledb/models/migrations/object_location_assignments_add_confirmed.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/object_location_assignments_add_responsible_user_id.py` & `sampledb-0.9.0/sampledb/models/migrations/object_location_assignments_add_responsible_user_id.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/object_log_entry_type_add_assign_location.py` & `sampledb-0.9.0/sampledb/models/migrations/object_log_entry_type_add_assign_location.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/object_log_entry_type_add_link_publication.py` & `sampledb-0.9.0/sampledb/models/migrations/object_log_entry_type_add_link_publication.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_assign_location.py` & `sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_assign_location.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_create_location.py` & `sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_create_location.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_link_publication.py` & `sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_link_publication.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/user_log_entry_type_add_update_location.py` & `sampledb-0.9.0/sampledb/models/migrations/user_log_entry_type_add_update_location.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/migrations/utils.py` & `sampledb-0.9.0/sampledb/models/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/notifications.py` & `sampledb-0.9.0/sampledb/models/notifications.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/object_log.py` & `sampledb-0.9.0/sampledb/models/object_log.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/object_permissions.py` & `sampledb-0.9.0/sampledb/models/object_permissions.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/objects.py` & `sampledb-0.9.0/sampledb/models/objects.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/permissions.py` & `sampledb-0.9.0/sampledb/models/permissions.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/projects.py` & `sampledb-0.9.0/sampledb/models/projects.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/settings.py` & `sampledb-0.9.0/sampledb/models/settings.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/user_log.py` & `sampledb-0.9.0/sampledb/models/user_log.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/models/users.py` & `sampledb-0.9.0/sampledb/models/users.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,26 +18,31 @@
     __tablename__ = 'users'
 
     id = db.Column(db.Integer, primary_key=True)
     name = db.Column(db.String, nullable=False)
     email = db.Column(db.String, nullable=False)
     type = db.Column(db.Enum(UserType), nullable=False)
     is_admin = db.Column(db.Boolean, default=False, nullable=False)
+    is_readonly = db.Column(db.Boolean, default=False, nullable=False)
+    is_hidden = db.Column(db.Boolean, default=False, nullable=False)
 
     def __init__(self, name, email, type):
         self.name = name
         self.email = email
         self.type = type
 
     def __eq__(self, other):
         return (
             self.id == other.id and
             self.name == other.name and
             self.email == other.email and
             self.type == other.type and
-            self.is_admin == other.is_admin)
+            self.is_admin == other.is_admin and
+            self.is_readonly == other.is_readonly and
+            self.is_hidden == other.is_hidden
+        )
 
     def get_id(self):
         return self.id
 
     def __repr__(self):
         return '<{0}(id={1.id}, name={1.name})>'.format(type(self).__name__, self)
```

### Comparing `sampledb-0.8.1/sampledb/models/versioned_json_object_tables.py` & `sampledb-0.9.0/sampledb/models/versioned_json_object_tables.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/__init__.py` & `sampledb-0.9.0/sampledb/scripts/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from . import create_action
 from . import update_action
 from . import list_actions
 from . import export_action_schema
 from . import create_other_user
 from . import send_announcement
 from . import set_administrator
+from . import set_user_readonly
+from . import set_user_hidden
 from . import run
 
 
 script_functions = {
     'create_instrument': create_instrument.main,
     'update_instrument': update_instrument.main,
     'list_instruments': list_instruments.main,
@@ -25,9 +27,11 @@
     'create_action': create_action.main,
     'update_action': update_action.main,
     'list_actions': list_actions.main,
     'export_action_schema': export_action_schema.main,
     'create_other_user': create_other_user.main,
     'send_announcement': send_announcement.main,
     'set_administrator': set_administrator.main,
+    'set_user_readonly': set_user_readonly.main,
+    'set_user_hidden': set_user_hidden.main,
     'run': run.main
 }
```

### Comparing `sampledb-0.8.1/sampledb/scripts/create_action.py` & `sampledb-0.9.0/sampledb/scripts/create_action.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/create_instrument.py` & `sampledb-0.9.0/sampledb/scripts/create_instrument.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/create_other_user.py` & `sampledb-0.9.0/sampledb/scripts/create_other_user.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/export_action_schema.py` & `sampledb-0.9.0/sampledb/scripts/export_action_schema.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/run.py` & `sampledb-0.9.0/sampledb/scripts/run.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/send_announcement.py` & `sampledb-0.9.0/sampledb/scripts/send_announcement.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/set_administrator.py` & `sampledb-0.9.0/sampledb/scripts/set_administrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def main(arguments):
     if len(arguments) != 2 or not all(arguments) or arguments[1] not in ('yes', 'no'):
         print(__doc__)
         exit(1)
     user_id, yes_or_no = arguments
     try:
-        user_id == int(user_id)
+        user_id = int(user_id)
     except ValueError:
         print("Error: user_id must be an integer", file=sys.stderr)
         exit(1)
     is_admin = yes_or_no == 'yes'
     app = create_app()
     with app.app_context():
         try:
```

### Comparing `sampledb-0.8.1/sampledb/scripts/update_action.py` & `sampledb-0.9.0/sampledb/scripts/update_action.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/update_instrument.py` & `sampledb-0.9.0/sampledb/scripts/update_instrument.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/scripts/update_instrument_responsible_users.py` & `sampledb-0.9.0/sampledb/scripts/update_instrument_responsible_users.py`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/base.css` & `sampledb-0.9.0/sampledb/static/css/base.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-datetimepicker.min.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-select.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap-select.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-select.css.map` & `sampledb-0.9.0/sampledb/static/css/bootstrap-select.css.map`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-select.min.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-tagsinput.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap-tagsinput.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-theme.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-theme.css.map` & `sampledb-0.9.0/sampledb/static/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-theme.min.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-theme.min.css.map` & `sampledb-0.9.0/sampledb/static/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap-toggle.min.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap.css.map` & `sampledb-0.9.0/sampledb/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap.min.css` & `sampledb-0.9.0/sampledb/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/bootstrap.min.css.map` & `sampledb-0.9.0/sampledb/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/font-awesome.css` & `sampledb-0.9.0/sampledb/static/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/font-awesome.min.css` & `sampledb-0.9.0/sampledb/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/pygments.css` & `sampledb-0.9.0/sampledb/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/css/schema_editor.css` & `sampledb-0.9.0/sampledb/static/css/schema_editor.css`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/FontAwesome.otf` & `sampledb-0.9.0/sampledb/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.eot` & `sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.svg` & `sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.ttf` & `sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.woff` & `sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/fontawesome-webfont.woff2` & `sampledb-0.9.0/sampledb/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.eot` & `sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.svg` & `sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.ttf` & `sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.woff` & `sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/fonts/glyphicons-halflings-regular.woff2` & `sampledb-0.9.0/sampledb/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs00.png` & `sampledb-0.9.0/sampledb/static/img/ghs00.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs01.png` & `sampledb-0.9.0/sampledb/static/img/ghs01.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs02.png` & `sampledb-0.9.0/sampledb/static/img/ghs02.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs03.png` & `sampledb-0.9.0/sampledb/static/img/ghs03.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs04.png` & `sampledb-0.9.0/sampledb/static/img/ghs04.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs05.png` & `sampledb-0.9.0/sampledb/static/img/ghs05.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs06.png` & `sampledb-0.9.0/sampledb/static/img/ghs06.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs07.png` & `sampledb-0.9.0/sampledb/static/img/ghs07.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs08.png` & `sampledb-0.9.0/sampledb/static/img/ghs08.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/ghs09.png` & `sampledb-0.9.0/sampledb/static/img/ghs09.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/jupyter-40.png` & `sampledb-0.9.0/sampledb/static/img/jupyter-40.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/img/logo64.png` & `sampledb-0.9.0/docs/static/img/logo64.png`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap-datetimepicker.min.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap-select.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap-select.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap-select.js.map` & `sampledb-0.9.0/sampledb/static/js/bootstrap-select.js.map`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap-select.min.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap-tagsinput.min.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap-tagsinput.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap-toggle.min.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap-treeview.min.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap-treeview.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/bootstrap.min.js` & `sampledb-0.9.0/sampledb/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ar_AR.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ar_AR.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ar_AR.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ar_AR.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-bg_BG.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-bg_BG.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-bg_BG.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-bg_BG.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-cro_CRO.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-cro_CRO.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-cro_CRO.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-cro_CRO.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-cs_CZ.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-cs_CZ.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-cs_CZ.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-cs_CZ.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-da_DK.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-da_DK.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-da_DK.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-da_DK.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-de_DE.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-de_DE.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-de_DE.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-de_DE.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-en_US.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-en_US.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-en_US.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-en_US.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_CL.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_CL.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_CL.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_CL.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_ES.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_ES.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-es_ES.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-es_ES.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-eu.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-eu.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-eu.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-eu.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-fa_IR.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-fa_IR.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-fa_IR.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-fa_IR.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-fi_FI.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-fi_FI.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-fi_FI.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-fi_FI.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-fr_FR.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-fr_FR.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-fr_FR.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-fr_FR.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-hu_HU.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-hu_HU.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-hu_HU.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-hu_HU.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-id_ID.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-id_ID.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-id_ID.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-id_ID.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-it_IT.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-it_IT.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-it_IT.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-it_IT.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ko_KR.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ko_KR.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ko_KR.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ko_KR.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-lt_LT.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-lt_LT.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-lt_LT.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-lt_LT.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-nb_NO.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-nb_NO.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-nb_NO.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-nb_NO.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-nl_NL.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-nl_NL.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-nl_NL.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-nl_NL.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-pl_PL.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-pl_PL.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-pl_PL.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-pl_PL.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_BR.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_BR.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_BR.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_BR.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_PT.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_PT.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-pt_PT.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-pt_PT.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ro_RO.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ro_RO.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ro_RO.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ro_RO.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ru_RU.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ru_RU.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ru_RU.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ru_RU.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-sk_SK.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-sk_SK.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-sk_SK.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-sk_SK.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-sl_SI.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-sl_SI.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-sl_SI.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-sl_SI.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-sv_SE.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-sv_SE.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-sv_SE.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-sv_SE.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-tr_TR.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-tr_TR.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-tr_TR.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-tr_TR.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ua_UA.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ua_UA.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-ua_UA.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-ua_UA.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_CN.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_CN.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_CN.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_CN.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_TW.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_TW.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/i18n/defaults-zh_TW.min.js` & `sampledb-0.9.0/sampledb/static/js/i18n/defaults-zh_TW.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/jquery-1.12.4.min.js` & `sampledb-0.9.0/sampledb/static/js/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/js.cookie.js` & `sampledb-0.9.0/sampledb/static/js/js.cookie.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/moment-with-locales.js` & `sampledb-0.9.0/sampledb/static/js/moment-with-locales.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/moment-with-locales.min.js` & `sampledb-0.9.0/sampledb/static/js/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/static/js/schema_editor.js` & `sampledb-0.9.0/sampledb/static/js/schema_editor.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -292,14 +292,16 @@
             } else if ('multiline' in schema && schema['multiline']) {
                 type = "multiline";
             } else {
                 type = "text";
             }
         } else if (schema['type'] === 'sample') {
             type = "sample";
+        } else if (schema['type'] === 'measurement') {
+            type = "measurement";
         } else if (schema['type'] === 'bool') {
             type = "bool";
         } else if (schema['type'] === 'quantity') {
             type = "quantity";
         } else if (schema['type'] === 'datetime') {
             type = "datetime";
         } else if (schema['type'] === 'tags') {
@@ -326,14 +328,16 @@
                 updateChoiceProperty(path, real_path);
             } else if (type === "multiline") {
                 updateMultilineProperty(path, real_path);
             } else if (type === "bool") {
                 updateBoolProperty(path, real_path);
             } else if (type === "sample") {
                 updateSampleProperty(path, real_path);
+            } else if (type === "measurement") {
+                updateMeasurementProperty(path, real_path);
             } else if (type === "quantity") {
                 updateQuantityProperty(path, real_path);
             } else if (type === "datetime") {
                 updateDatetimeProperty(path, real_path);
             }
             globallyValidateSchema();
         }
@@ -838,14 +842,32 @@
 
             schema['properties'][real_path[real_path.length - 1]] = property_schema;
 
             input_schema.text(JSON.stringify(schema, null, 4));
 
             window.schema_editor_errors[path.join('__') + '__specific'] = true;
             if (!has_error) {
+                delete window.schema_editor_errors[path.join('__') + '__specific'];
+            }
+            $('button[name="action_submit"]').prop('disabled', (JSON.stringify(window.schema_editor_errors) !== '{}'));
+        }
+
+        function updateMeasurementProperty(path, real_path) {
+            var has_error = false;
+            updateGenericProperty(path, real_path);
+            var schema = JSON.parse(input_schema.text());
+            var property_schema = schema['properties'][real_path[real_path.length - 1]];
+            property_schema["type"] = "measurement";
+
+            schema['properties'][real_path[real_path.length - 1]] = property_schema;
+
+            input_schema.text(JSON.stringify(schema, null, 4));
+
+            window.schema_editor_errors[path.join('__') + '__specific'] = true;
+            if (!has_error) {
                 delete window.schema_editor_errors[path.join('__') + '__specific'];
             }
             $('button[name="action_submit"]').prop('disabled', (JSON.stringify(window.schema_editor_errors) !== '{}'));
         }
 
         function updateDatetimeProperty(path, real_path) {
             var has_error = false;
```

### Comparing `sampledb-0.8.1/sampledb/static/js/typeahead.bundle.min.js` & `sampledb-0.9.0/sampledb/static/js/typeahead.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sampledb-0.8.1/sampledb/utils.py` & `sampledb-0.9.0/sampledb/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,17 @@
             object_id = kwargs['object_id']
             try:
                 logic.objects.get_object(object_id)
             except logic.errors.ObjectDoesNotExistError:
                 return flask.abort(404)
             if not (logic.object_permissions.object_is_public(object_id) and required_object_permissions in Permissions.READ):
                 user_id = user_id_callable()
+                user = logic.users.get_user(user_id)
+                if user.is_readonly and required_object_permissions not in Permissions.READ:
+                    return on_unauthorized(object_id)
                 user_object_permissions = logic.object_permissions.get_user_object_permissions(object_id=object_id, user_id=user_id)
                 if required_object_permissions not in user_object_permissions:
                     return on_unauthorized(object_id)
             return func(*args, **kwargs)
         return wrapper
     return decorator
```

### Comparing `sampledb-0.8.1/sampledb.egg-info/PKG-INFO` & `sampledb-0.9.0/sampledb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampledb
-Version: 0.8.1
+Version: 0.9.0
 Summary: A sample and measurement metadata database
 Home-page: https://github.com/sciapp/sampledb
 Author: Florian Rhiem
 Author-email: f.rhiem@fz-juelich.de
 License: MIT
 Description: # SampleDB
         
@@ -42,15 +42,15 @@
             -e SAMPLEDB_CONTACT_EMAIL=sampledb@example.com \
             -e SAMPLEDB_SQLALCHEMY_DATABASE_URI=postgresql+psycopg2://postgres:@sampledb-postgres:5432/postgres \
             -e SAMPLEDB_FILE_STORAGE_PATH=/home/sampledb/files/ \
             -v `pwd`/files:/home/sampledb/files:rw \
             --restart=always \
             --name sampledb \
             -p 8000:8000 \
-            docker.pkg.github.com/sciapp/sampledb/sampledb:0.8.1
+            sciapp/sampledb:0.9.0
         ```
         
         This will start a basic SampleDB instance at `http://localhost:8000`.
         
         To use the administration scripts, run:
         
         ```bash
```

### Comparing `sampledb-0.8.1/sampledb.egg-info/requires.txt` & `sampledb-0.9.0/sampledb.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 beautifulsoup4==4.8.1
 blinker==1.4
 certifi==2019.9.11
 cffi==1.13.2
 chardet==3.0.4
 cheroot==8.2.1
 CherryPy==18.4.0
-chromedriver-binary==77.0.3865.40.0
+chromedriver-binary==79.0.3945.36.0
 Click==7.0
 coverage==4.5.4
 docutils==0.15.2
 Flask==1.1.1
 Flask-HTTPAuth==3.3.0
 Flask-Login==0.4.1
 Flask-Mail==0.9.1
```

### Comparing `sampledb-0.8.1/setup.py` & `sampledb-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = readme_file.read()
 
 with open(os.path.join(setup_directory, 'requirements.txt')) as requirements_file:
     requirements = requirements_file.readlines()
 
 setup(
     name='sampledb',
-    version='0.8.1',
+    version='0.9.0',
     description='A sample and measurement metadata database',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sciapp/sampledb',
     author='Florian Rhiem',
     author_email='f.rhiem@fz-juelich.de',
     license='MIT',
```

