# Comparing `tmp/drf-user-activity-tracker-mongodb-1.3.6.tar.gz` & `tmp/drf-user-activity-tracker-mongodb-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-user-activity-tracker-mongodb-1.3.6.tar", last modified: Tue Jun  6 11:01:41 2023, max compression
+gzip compressed data, was "dist/drf-user-activity-tracker-mongodb-1.3.7.tar", last modified: Tue Jun  6 12:55:02 2023, max compression
```

## Comparing `drf-user-activity-tracker-mongodb-1.3.6.tar` & `drf-user-activity-tracker-mongodb-1.3.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      780 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/setup.cfg
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       38 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/setup.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       85 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/pyproject.toml
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      382 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/MANIFEST.in
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13240 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/PKG-INFO
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      732 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/permissions.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9686 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1573 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9626 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/commands/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      913 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2743 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/views.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2969 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/serializers.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9201 2023-06-06 09:17:24.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/tests.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  3039173 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  2315687 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     3815 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/admin.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      169 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/apps.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      600 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      786 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/tagger.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2893 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/events.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    11642 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/utils.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      325 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/urls.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      557 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/0001_initial.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      233 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      250 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/models.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2270 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/insert_log_into_database.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        1 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       34 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/top_level.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       30 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/requires.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13240 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1770 2023-06-06 11:01:41.000000 drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    10435 2023-06-06 10:25:20.000000 drf-user-activity-tracker-mongodb-1.3.6/README.md
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1073 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.6/LICENSE
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      780 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/setup.cfg
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       38 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/setup.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       85 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/pyproject.toml
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      382 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/MANIFEST.in
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13240 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/PKG-INFO
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      732 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/permissions.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/admin/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9686 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1573 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9626 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/management/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/management/commands/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      913 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2743 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/views.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2969 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/serializers.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/middleware/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/middleware/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9378 2023-06-06 12:53:34.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/tests.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/geo_databases/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  3039173 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  2315687 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     3815 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/admin.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      169 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/apps.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      600 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templatetags/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      786 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templatetags/tagger.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templatetags/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2893 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/events.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    11642 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/utils.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      325 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/urls.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/migrations/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      557 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/migrations/0001_initial.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/migrations/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      233 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      250 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/models.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2270 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/insert_log_into_database.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        1 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       34 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       30 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13240 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1770 2023-06-06 12:55:02.000000 drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    10435 2023-06-06 12:54:32.000000 drf-user-activity-tracker-mongodb-1.3.7/README.md
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1073 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.3.7/LICENSE
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/setup.cfg` & `drf-user-activity-tracker-mongodb-1.3.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-user-activity-tracker-mongodb
-version = 1.3.6
+version = 1.3.7
 description = A Django app to logs users activities in mongodb database.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bigmo94/drf-user-activity-tracker-mongodb
 author = Mohamad Rezaie
 author_email = m.rezaie94@gmail.com
 license = MIT
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/PKG-INFO` & `drf-user-activity-tracker-mongodb-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: drf-user-activity-tracker-mongodb
-Version: 1.3.6
+Version: 1.3.7
 Summary: A Django app to logs users activities in mongodb database.
 Home-page: https://github.com/bigmo94/drf-user-activity-tracker-mongodb
 Author: Mohamad Rezaie
 Author-email: m.rezaie94@gmail.com
 License: MIT
 Description: # DRF User Activity Tracker Mongodb
         ## _Log All User Activities_
         
-        ![version](https://img.shields.io/badge/version-1.3.6-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.3.7-blue.svg)
         [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
         <a href="https://github.com/bigmo94/drf-user-activity-tracker-mongodb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
         
         An API Logger of User Activity for your Django Rest Framework project.
         
         It logs all the API information for content type "application/json" in mongo database.
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/permissions.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/views.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/views.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/serializers.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         if hasattr(settings, 'DRF_ACTIVITY_TRACKER_SKIP_URL_NAME'):
             if isinstance(settings.DRF_ACTIVITY_TRACKER_SKIP_URL_NAME, (tuple, list)):
                 self.DRF_ACTIVITY_TRACKER_SKIP_URL_NAME.extend(settings.DRF_ACTIVITY_TRACKER_SKIP_URL_NAME)
 
         self.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME = []
         if hasattr(settings, 'DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME'):
             if isinstance(settings.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME, (tuple, list)):
-                self.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME.extend(settings.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME) 
+                self.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME.extend(settings.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME)
 
         self.DRF_ACTIVITY_TRACKER_SKIP_NAMESPACE = []
         if hasattr(settings, 'DRF_ACTIVITY_TRACKER_SKIP_NAMESPACE'):
             if isinstance(settings.DRF_ACTIVITY_TRACKER_SKIP_NAMESPACE, (tuple, list)):
                 self.DRF_ACTIVITY_TRACKER_SKIP_NAMESPACE = settings.DRF_ACTIVITY_TRACKER_SKIP_NAMESPACE
 
         self.DRF_ACTIVITY_TRACKER_METHODS = []
@@ -110,22 +110,28 @@
             header_token = request.META.get("HTTP_AUTHORIZATION")
             algorithm = 'HS256'
             if hasattr(settings, "JWT_ALGORITHM") and isinstance(settings.JWT_ALGORITHM, str):
                 algorithm = settings.JWT_ALGORITHM
 
             payload_data = {}
             if header_token:
-                token = header_token.split()[1]
-                user_token = jwt.decode(jwt=token, key=settings.SECRET_KEY, algorithms=[algorithm])
+                try:
+                    token = header_token.split()[1]
+                    user_token = jwt.decode(jwt=token, key=settings.SECRET_KEY, algorithms=[algorithm])
+                except:
+                    return response
                 for key in self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS:
                     payload_data[key] = user_token.get(key)
 
             elif hasattr(response, 'data') and isinstance(response.data, dict) and response.data.get('access'):
-                user_token = jwt.decode(jwt=response.data.get('access'), key=settings.SECRET_KEY,
-                                        algorithms=[algorithm])
+                try:
+                    user_token = jwt.decode(jwt=response.data.get('access'), key=settings.SECRET_KEY,
+                                            algorithms=[algorithm])
+                except:
+                    return response
                 for key in self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS:
                     payload_data[key] = user_token.get(key)
 
             elif url_name in self.DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME:
                 for key in self.DRF_ACTIVITY_TRACKER_TOKEN_PAYLOAD_KEYS:
                     payload_data[key] = None
             else:
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/admin.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/admin.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/templatetags/tagger.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/templatetags/tagger.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/events.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/events.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/utils.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/migrations/0001_initial.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb/insert_log_into_database.py` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb/insert_log_into_database.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: drf-user-activity-tracker-mongodb
-Version: 1.3.6
+Version: 1.3.7
 Summary: A Django app to logs users activities in mongodb database.
 Home-page: https://github.com/bigmo94/drf-user-activity-tracker-mongodb
 Author: Mohamad Rezaie
 Author-email: m.rezaie94@gmail.com
 License: MIT
 Description: # DRF User Activity Tracker Mongodb
         ## _Log All User Activities_
         
-        ![version](https://img.shields.io/badge/version-1.3.6-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.3.7-blue.svg)
         [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
         <a href="https://github.com/bigmo94/drf-user-activity-tracker-mongodb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
         
         An API Logger of User Activity for your Django Rest Framework project.
         
         It logs all the API information for content type "application/json" in mongo database.
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt` & `drf-user-activity-tracker-mongodb-1.3.7/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/README.md` & `drf-user-activity-tracker-mongodb-1.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # DRF User Activity Tracker Mongodb
 ## _Log All User Activities_
 
-![version](https://img.shields.io/badge/version-1.3.6-blue.svg)
+![version](https://img.shields.io/badge/version-1.3.7-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/bigmo94/drf-user-activity-tracker-mongodb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 An API Logger of User Activity for your Django Rest Framework project.
 
 It logs all the API information for content type "application/json" in mongo database.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # DRF User Activity Tracker Mongodb ## _Log All User Activities_ ![version]
-(https://img.shields.io/badge/version-1.3.6-blue.svg) [![Open Source](https://
+(https://img.shields.io/badge/version-1.3.7-blue.svg) [![Open Source](https://
 badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 [GitHub] An API Logger of User Activity for your Django Rest Framework project.
 It logs all the API information for content type "application/json" in mongo
 database. Note: It logs just API information for registered user. (Anonymous
 User Activities are ignored. But It's possible to log api without user id by
 add their url names in DRF_ACTIVITY_TRACKER_DONT_SKIP_URL_NAME attribute in
 settings.py) 1. User_ID 2. URL_PATH 3. URL_NAME 4. Request Body 5. Request
```

### Comparing `drf-user-activity-tracker-mongodb-1.3.6/LICENSE` & `drf-user-activity-tracker-mongodb-1.3.7/LICENSE`

 * *Files identical despite different names*

