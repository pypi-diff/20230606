# Comparing `tmp/drf-user-activity-tracker-mongodb-1.3.5.tar.gz` & `tmp/drf-user-activity-tracker-mongodb-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-user-activity-tracker-mongodb-1.3.5.tar", last modified: Sat Nov 12 07:44:27 2022, max compression
+gzip compressed data, was "dist/drf-user-activity-tracker-mongodb-1.3.6.tar", last modified: Tue Jun  6 11:01:41 2023, max compression
```

## Comparing `drf-user-activity-tracker-mongodb-1.3.5.tar` & `drf-user-activity-tracker-mongodb-1.3.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1770 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       34 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/top_level.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    12547 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        1 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       30 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/requires.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      780 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/setup.cfg
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      382 2022-11-09 12:41:56.000000 drf-user-activity-tracker-mongodb-1.3.5/MANIFEST.in
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1073 2022-04-26 13:01:37.000000 drf-user-activity-tracker-mongodb-1.3.5/LICENSE
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/geo_databases/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  3039173 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  2315687 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     3815 2022-09-18 12:51:09.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/admin.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2743 2022-09-18 11:04:52.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/views.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      233 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      600 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/management/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/management/commands/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      913 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      169 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/apps.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/admin/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9626 2022-09-18 12:55:11.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9686 2022-09-18 12:55:11.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1573 2022-05-30 12:29:10.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2969 2022-09-18 11:02:10.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/serializers.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      325 2022-06-06 06:15:39.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/urls.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      250 2022-09-18 12:52:06.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/models.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/tests.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    11642 2022-11-06 08:00:43.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/utils.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/migrations/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2022-09-19 07:57:09.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/migrations/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      557 2022-11-12 07:43:45.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/migrations/0001_initial.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2270 2022-09-18 11:02:10.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/insert_log_into_database.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      732 2022-09-21 10:34:33.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/permissions.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templatetags/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templatetags/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      786 2022-06-11 05:31:28.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templatetags/tagger.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2893 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/events.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/middleware/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2022-05-16 08:26:05.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/middleware/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     8811 2022-11-06 07:46:03.000000 drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9854 2022-11-12 07:42:59.000000 drf-user-activity-tracker-mongodb-1.3.5/README.md
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    12547 2022-11-12 07:44:27.000000 drf-user-activity-tracker-mongodb-1.3.5/PKG-INFO
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       85 2022-04-27 09:57:04.000000 drf-user-activity-tracker-mongodb-1.3.5/pyproject.toml
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       38 2022-04-27 06:56:06.000000 drf-user-activity-tracker-mongodb-1.3.5/setup.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      780 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/setup.cfg
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       38 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/setup.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       85 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/pyproject.toml
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      382 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/MANIFEST.in
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13240 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/PKG-INFO
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      732 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/permissions.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9686 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1573 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9626 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/commands/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      913 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2743 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/views.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2969 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/serializers.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9201 2023-06-06 09:17:24.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/tests.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  3039173 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  2315687 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     3815 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/admin.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      169 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/apps.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      600 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      786 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/tagger.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2893 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/events.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    11642 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/utils.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      325 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/urls.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      557 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/0001_initial.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      233 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      250 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/models.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2270 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/insert_log_into_database.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        1 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       34 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       30 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13240 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1770 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    10435 2023-06-06 10:25:20.000000 drf-user-activity-tracker-mongodb-1.3.6/README.md
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1073 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/LICENSE
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO` & `drf-user-activity-tracker-mongodb-1.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: drf-user-activity-tracker-mongodb
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Django app to logs users activities in mongodb database.
 Home-page: https://github.com/bigmo94/drf-user-activity-tracker-mongodb
 Author: Mohamad Rezaie
 Author-email: m.rezaie94@gmail.com
 License: MIT
 Description: # DRF User Activity Tracker Mongodb
         ## _Log All User Activities_
         
-        ![version](https://img.shields.io/badge/version-1.3.4-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.3.6-blue.svg)
         [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
         <a href="https://github.com/bigmo94/drf-user-activity-tracker-mongodb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
         
         An API Logger of User Activity for your Django Rest Framework project.
         
         It logs all the API information for content type "application/json" in mongo database.
         
@@ -191,14 +191,30 @@
         
         ### Want to log only selected request methods? (Optional)
         You can log only selected methods by specifying `DRF_ACTIVITY_TRACKER_METHODS` in settings.py.
         ```python
         DRF_ACTIVITY_TRACKER_METHODS = ['GET', 'POST', 'DELETE', 'PUT']  # Default to empty list (Log all the requests).
         ```
         
+        ### Want to log token's payload keys?
+        If you add some keys to payload of token, and you want to log these keys into db, you can do this by setting `DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS` in settings.py.
+        Note: the user_id is logged by default, and you don't need to add this key.
+        ```python
+        # Example
+        token_payload = {
+          "token_type": "access",
+          "exp": 1313131313,
+          "jti": "32b32caa7c4c04d3ab7050175e54680d1",
+          "user_id": 13,
+          "protect_key": "13CC13DSF424FSF",
+          "company_id": "13"
+        }
+        DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS = ['company_id', 'protect_key']
+        ```
+        
         ### Want to see the API information in local timezone? (Optional)
         You can also change the timezone by specifying `DRF_ACTIVITY_TRACKER_TIMEDELTA` in settings.py.
         It won't change the Database timezone. It will still remain UTC or the timezone you have defined.
         ```python
         DRF_ACTIVITY_TRACKER_TIMEDELTA = 330 # UTC + 330 Minutes = IST (5:Hours, 30:Minutes ahead from UTC) 
         # Specify in minutes.
         ```
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/setup.cfg` & `drf-user-activity-tracker-mongodb-1.3.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-user-activity-tracker-mongodb
-version = 1.3.5
+version = 1.3.6
 description = A Django app to logs users activities in mongodb database.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bigmo94/drf-user-activity-tracker-mongodb
 author = Mohamad Rezaie
 author_email = m.rezaie94@gmail.com
 license = MIT
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/LICENSE` & `drf-user-activity-tracker-mongodb-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/admin.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/admin.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/views.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/views.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/serializers.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/utils.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/migrations/0001_initial.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/insert_log_into_database.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/insert_log_into_database.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/permissions.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/templatetags/tagger.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/tagger.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/events.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/events.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,19 @@
                 self.DRF_ACTIVITY_TRACKER_SKIP_NAMESPACE = settings.DRF_ACTIVITY_TRACKER_SKIP_NAMESPACE
 
         self.DRF_ACTIVITY_TRACKER_METHODS = []
         if hasattr(settings, 'DRF_ACTIVITY_TRACKER_METHODS'):
             if isinstance(settings.DRF_ACTIVITY_TRACKER_METHODS, (tuple, list)):
                 self.DRF_ACTIVITY_TRACKER_METHODS = settings.DRF_ACTIVITY_TRACKER_METHODS
 
+        self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS = ['user_id']
+        if hasattr(settings, 'DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS'):
+            if isinstance(settings.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS, (tuple, list)):
+                self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS.extend(settings.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS)
+
     def __call__(self, request):
 
         # Run only if logger is enabled.
         if self.DRF_ACTIVITY_TRACKER_DATABASE or self.DRF_ACTIVITY_TRACKER_SIGNAL:
 
             url_name = resolve(request.path).url_name
             namespace = resolve(request.path).namespace
@@ -103,30 +108,30 @@
             # the view is called.
 
             header_token = request.META.get("HTTP_AUTHORIZATION")
             algorithm = 'HS256'
             if hasattr(settings, "JWT_ALGORITHM") and isinstance(settings.JWT_ALGORITHM, str):
                 algorithm = settings.JWT_ALGORITHM
 
+            payload_data = {}
             if header_token:
-                try:
-                    token = header_token.split()[1]
-                    user_token = jwt.decode(jwt=token, key=settings.SECRET_KEY, algorithms=[algorithm])
-                    user = User.objects.get(id=user_token.get('user_id'))
-                except:
-                    return response
+                token = header_token.split()[1]
+                user_token = jwt.decode(jwt=token, key=settings.SECRET_KEY, algorithms=[algorithm])
+                for key in self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS:
+                    payload_data[key] = user_token.get(key)
+
             elif hasattr(response, 'data') and isinstance(response.data, dict) and response.data.get('access'):
                 user_token = jwt.decode(jwt=response.data.get('access'), key=settings.SECRET_KEY,
                                         algorithms=[algorithm])
-                try:
-                    user = User.objects.get(id=user_token.get('user_id'))
-                except User.DoesNotExist:
-                    return response
+                for key in self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS:
+                    payload_data[key] = user_token.get(key)
+
             elif url_name in self.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME:
-                user = None
+                for key in self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS:
+                    payload_data[key] = None
             else:
                 return response
 
             headers = get_headers(request=request)
             method = request.method
 
             # Log only registered methods if available.
@@ -163,26 +168,26 @@
                             '{}/geo_databases/GeoIPv6.dat'.format(pathlib.Path(__file__).parent.parent),
                             pygeoip.MEMORY_CACHE).country_name_by_addr(ip)
                     except:
                         country_name = ''
                 data = dict(
                     url_name=url_name,
                     url_path=request.path,
-                    user_id=user.id if user else None,
                     api=api,
                     headers=mask_sensitive_data(headers),
                     body=mask_sensitive_data(request_data),
                     method=method,
                     client_ip_address=ip,
                     response=mask_sensitive_data(response_body),
                     status_code=response.status_code,
                     execution_time=time.time() - start_time,
                     created_time=timezone.now(),
                     country=country_name,
                 )
+                data.update(payload_data)
                 if self.DRF_ACTIVITY_TRACKER_DATABASE:
                     if LOGGER_THREAD:
                         LOGGER_THREAD.put_log_data(data=data)
                 if self.DRF_ACTIVITY_TRACKER_SIGNAL:
                     ACTIVITY_TRACKER_SIGNAL.listen(**data)
             else:
                 return response
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/README.md` & `drf-user-activity-tracker-mongodb-1.3.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # DRF User Activity Tracker Mongodb
 ## _Log All User Activities_
 
-![version](https://img.shields.io/badge/version-1.3.4-blue.svg)
+![version](https://img.shields.io/badge/version-1.3.6-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/bigmo94/drf-user-activity-tracker-mongodb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 An API Logger of User Activity for your Django Rest Framework project.
 
 It logs all the API information for content type "application/json" in mongo database.
 
@@ -183,14 +183,30 @@
 
 ### Want to log only selected request methods? (Optional)
 You can log only selected methods by specifying `DRF_ACTIVITY_TRACKER_METHODS` in settings.py.
 ```python
 DRF_ACTIVITY_TRACKER_METHODS = ['GET', 'POST', 'DELETE', 'PUT']  # Default to empty list (Log all the requests).
 ```
 
+### Want to log token's payload keys?
+If you add some keys to payload of token, and you want to log these keys into db, you can do this by setting `DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS` in settings.py.
+Note: the user_id is logged by default, and you don't need to add this key.
+```python
+# Example
+token_payload = {
+  "token_type": "access",
+  "exp": 1313131313,
+  "jti": "32b32caa7c4c04d3ab7050175e54680d1",
+  "user_id": 13,
+  "protect_key": "13CC13DSF424FSF",
+  "company_id": "13"
+}
+DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS = ['company_id', 'protect_key']
+```
+
 ### Want to see the API information in local timezone? (Optional)
 You can also change the timezone by specifying `DRF_ACTIVITY_TRACKER_TIMEDELTA` in settings.py.
 It won't change the Database timezone. It will still remain UTC or the timezone you have defined.
 ```python
 DRF_ACTIVITY_TRACKER_TIMEDELTA = 330 # UTC + 330 Minutes = IST (5:Hours, 30:Minutes ahead from UTC) 
 # Specify in minutes.
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # DRF User Activity Tracker Mongodb ## _Log All User Activities_ ![version]
-(https://img.shields.io/badge/version-1.3.4-blue.svg) [![Open Source](https://
+(https://img.shields.io/badge/version-1.3.6-blue.svg) [![Open Source](https://
 badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 [GitHub] An API Logger of User Activity for your Django Rest Framework project.
 It logs all the API information for content type "application/json" in mongo
 database. Note: It logs just API information for registered user. (Anonymous
 User Activities are ignored. But It's possible to log api without user id by
 add their url names in DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME attribute in
 settings.py) 1. User_ID 2. URL_PATH 3. URL_NAME 4. Request Body 5. Request
@@ -74,36 +74,43 @@
 this by setting `DRF_ACTIVITY_TRACKER_EXCLUDE_KEYS` in settings.py to a list of
 your desired sensitive keys. The default is ```python
 DRF_ACTIVITY_TRACKER_EXCLUDE_KEYS = ['password', 'token', 'access', 'refresh']
 # Sensitive data will be replaced with "***FILTERED***". ``` ### Want to log
 only selected request methods? (Optional) You can log only selected methods by
 specifying `DRF_ACTIVITY_TRACKER_METHODS` in settings.py. ```python
 DRF_ACTIVITY_TRACKER_METHODS = ['GET', 'POST', 'DELETE', 'PUT'] # Default to
-empty list (Log all the requests). ``` ### Want to see the API information in
-local timezone? (Optional) You can also change the timezone by specifying
-`DRF_ACTIVITY_TRACKER_TIMEDELTA` in settings.py. It won't change the Database
-timezone. It will still remain UTC or the timezone you have defined. ```python
-DRF_ACTIVITY_TRACKER_TIMEDELTA = 330 # UTC + 330 Minutes = IST (5:Hours, 30:
-Minutes ahead from UTC) # Specify in minutes. ``` ```python # Yoc can specify
-negative values for the countries behind the UTC timezone.
-DRF_ACTIVITY_TRACKER_TIMEDELTA = -30 # Example ``` ### API with or without Host
-You can specify an endpoint of API should have absolute URI or not by setting
-this variable in DRF settings.py file. ```python DRF_ACTIVITY_TRACKER_PATH_TYPE
-= 'ABSOLUTE' # Default to ABSOLUTE if not specified # Possible values are
-ABSOLUTE, FULL_PATH or RAW_URI ``` Considering we are accessing the following
-URL: http://127.0.0.1:8000/api/v1/?page=123 DRF_ACTIVITY_TRACKER_PATH_TYPE
-possible values are: 1. ABSOLUTE (Default) : Function used
-```request.build_absolute_uri()``` Output: ```http://127.0.0.1:8000/api/v1/
-?page=123``` 2. FULL_PATH Function used ```request.get_full_path()``` Output:
-```/api/v1/?page=123``` 3. RAW_URI Function used ```request.get_raw_uri()```
-Output: ```http://127.0.0.1:8000/api/v1/?page=123``` Note: Similar to ABSOLUTE
-but skip allowed hosts protection, so may return an insecure URI. ### API Call
-For History Of Activities By Users Or Admin Add in your_project_root/
-project_name/urls.py ``` urlpatterns = [ path('service_admin_zone/',
-admin.site.urls), path('activity-logs/', include
+empty list (Log all the requests). ``` ### Want to log token's payload keys? If
+you add some keys to payload of token, and you want to log these keys into db,
+you can do this by setting `DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS` in
+settings.py. Note: the user_id is logged by default, and you don't need to add
+this key. ```python # Example token_payload = { "token_type": "access", "exp":
+1313131313, "jti": "32b32caa7c4c04d3ab7050175e54680d1", "user_id": 13,
+"protect_key": "13CC13DSF424FSF", "company_id": "13" }
+DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS = ['company_id', 'protect_key'] ``` ###
+Want to see the API information in local timezone? (Optional) You can also
+change the timezone by specifying `DRF_ACTIVITY_TRACKER_TIMEDELTA` in
+settings.py. It won't change the Database timezone. It will still remain UTC or
+the timezone you have defined. ```python DRF_ACTIVITY_TRACKER_TIMEDELTA = 330 #
+UTC + 330 Minutes = IST (5:Hours, 30:Minutes ahead from UTC) # Specify in
+minutes. ``` ```python # Yoc can specify negative values for the countries
+behind the UTC timezone. DRF_ACTIVITY_TRACKER_TIMEDELTA = -30 # Example ``` ###
+API with or without Host You can specify an endpoint of API should have
+absolute URI or not by setting this variable in DRF settings.py file. ```python
+DRF_ACTIVITY_TRACKER_PATH_TYPE = 'ABSOLUTE' # Default to ABSOLUTE if not
+specified # Possible values are ABSOLUTE, FULL_PATH or RAW_URI ``` Considering
+we are accessing the following URL: http://127.0.0.1:8000/api/v1/?page=123
+DRF_ACTIVITY_TRACKER_PATH_TYPE possible values are: 1. ABSOLUTE (Default) :
+Function used ```request.build_absolute_uri()``` Output: ```http://127.0.0.1:
+8000/api/v1/?page=123``` 2. FULL_PATH Function used ```request.get_full_path
+()``` Output: ```/api/v1/?page=123``` 3. RAW_URI Function used
+```request.get_raw_uri()``` Output: ```http://127.0.0.1:8000/api/v1/
+?page=123``` Note: Similar to ABSOLUTE but skip allowed hosts protection, so
+may return an insecure URI. ### API Call For History Of Activities By Users Or
+Admin Add in your_project_root/project_name/urls.py ``` urlpatterns = [ path
+('service_admin_zone/', admin.site.urls), path('activity-logs/', include
 ('drf_user_activity_tracker.urls')), ] ``` ##### Access to this API by
 following URL: {{ your_base_url }}/activity-logs/user-history/ {{ your_base_url
 }}/activity-logs/admin-history/ `for calling admin history api; you must have
 'can view avtivity log' permission. or add DRF_ACTIVITY_TRACKER_PERMISSION in
 settings.py and add your permission in a string format.` ```
 DRF_ACTIVITY_TRACKER_PERMISSION = 'customers.can_view_logs' ``` ##### The
 response includes these: 1. id 2. event_name 3. client_ip_address 4.
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.5/PKG-INFO` & `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: drf-user-activity-tracker-mongodb
-Version: 1.3.5
+Version: 1.3.6
 Summary: A Django app to logs users activities in mongodb database.
 Home-page: https://github.com/bigmo94/drf-user-activity-tracker-mongodb
 Author: Mohamad Rezaie
 Author-email: m.rezaie94@gmail.com
 License: MIT
 Description: # DRF User Activity Tracker Mongodb
         ## _Log All User Activities_
         
-        ![version](https://img.shields.io/badge/version-1.3.4-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.3.6-blue.svg)
         [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
         <a href="https://github.com/bigmo94/drf-user-activity-tracker-mongodb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
         
         An API Logger of User Activity for your Django Rest Framework project.
         
         It logs all the API information for content type "application/json" in mongo database.
         
@@ -191,14 +191,30 @@
         
         ### Want to log only selected request methods? (Optional)
         You can log only selected methods by specifying `DRF_ACTIVITY_TRACKER_METHODS` in settings.py.
         ```python
         DRF_ACTIVITY_TRACKER_METHODS = ['GET', 'POST', 'DELETE', 'PUT']  # Default to empty list (Log all the requests).
         ```
         
+        ### Want to log token's payload keys?
+        If you add some keys to payload of token, and you want to log these keys into db, you can do this by setting `DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS` in settings.py.
+        Note: the user_id is logged by default, and you don't need to add this key.
+        ```python
+        # Example
+        token_payload = {
+          "token_type": "access",
+          "exp": 1313131313,
+          "jti": "32b32caa7c4c04d3ab7050175e54680d1",
+          "user_id": 13,
+          "protect_key": "13CC13DSF424FSF",
+          "company_id": "13"
+        }
+        DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS = ['company_id', 'protect_key']
+        ```
+        
         ### Want to see the API information in local timezone? (Optional)
         You can also change the timezone by specifying `DRF_ACTIVITY_TRACKER_TIMEDELTA` in settings.py.
         It won't change the Database timezone. It will still remain UTC or the timezone you have defined.
         ```python
         DRF_ACTIVITY_TRACKER_TIMEDELTA = 330 # UTC + 330 Minutes = IST (5:Hours, 30:Minutes ahead from UTC) 
         # Specify in minutes.
         ```
```

