# Comparing `tmp/celery-5.3.0rc1.tar.gz` & `tmp/celery-5.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-5.3.0rc1.tar", last modified: Thu May 11 12:00:34 2023, max compression
+gzip compressed data, was "celery-5.3.0rc2.tar", last modified: Wed May 31 14:55:48 2023, max compression
```

## Comparing `celery-5.3.0rc1.tar` & `celery-5.3.0rc2.tar`

### file list

```diff
@@ -1,751 +1,749 @@
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.369059 celery-5.3.0rc1/
--rw-r--r--   0 nusnus     (501) staff       (20)     8184 2023-02-01 19:42:55.000000 celery-5.3.0rc1/CONTRIBUTORS.txt
--rw-r--r--   0 nusnus     (501) staff       (20)    11199 2023-05-11 11:48:52.000000 celery-5.3.0rc1/Changelog.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2631 2022-08-03 16:05:58.000000 celery-5.3.0rc1/LICENSE
--rw-r--r--   0 nusnus     (501) staff       (20)      709 2022-08-03 16:05:58.000000 celery-5.3.0rc1/MANIFEST.in
--rw-r--r--   0 nusnus     (501) staff       (20)    18012 2023-05-11 12:00:34.369172 celery-5.3.0rc1/PKG-INFO
--rw-r--r--   0 nusnus     (501) staff       (20)    15861 2023-05-11 11:45:05.000000 celery-5.3.0rc1/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)       84 2022-08-03 16:05:58.000000 celery-5.3.0rc1/TODO
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.254361 celery-5.3.0rc1/celery/
--rw-r--r--   0 nusnus     (501) staff       (20)     5951 2023-05-11 11:45:05.000000 celery-5.3.0rc1/celery/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      409 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/__main__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5029 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/_state.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.258541 celery-5.3.0rc1/celery/app/
--rw-r--r--   0 nusnus     (501) staff       (20)     2430 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    23151 2023-02-01 10:58:20.000000 celery-5.3.0rc1/celery/app/amqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1445 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/annotations.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2489 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/autoretry.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2702 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/backends.py
--rw-r--r--   0 nusnus     (501) staff       (20)    50088 2023-03-24 12:39:07.000000 celery-5.3.0rc1/celery/app/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6673 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/builtins.py
--rw-r--r--   0 nusnus     (501) staff       (20)    29170 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15014 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/app/defaults.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1326 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9067 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2001 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/registry.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4527 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/routes.py
--rw-r--r--   0 nusnus     (501) staff       (20)    43264 2023-03-24 18:03:27.000000 celery-5.3.0rc1/celery/app/task.py
--rw-r--r--   0 nusnus     (501) staff       (20)    28314 2023-03-24 12:39:07.000000 celery-5.3.0rc1/celery/app/trace.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13160 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/app/utils.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.258940 celery-5.3.0rc1/celery/apps/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/celery/apps/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5724 2023-03-11 14:59:39.000000 celery-5.3.0rc1/celery/apps/beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16360 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/apps/multi.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13208 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/apps/worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.261597 celery-5.3.0rc1/celery/backends/
--rw-r--r--   0 nusnus     (501) staff       (20)       23 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7739 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/arangodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10309 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/asynchronous.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5127 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/azureblockblob.py
--rw-r--r--   0 nusnus     (501) staff       (20)    43970 2023-03-11 14:59:39.000000 celery-5.3.0rc1/celery/backends/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4817 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/cache.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9006 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/cassandra.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3816 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/consul.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6777 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/cosmosdbsql.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3393 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/couchbase.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2935 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/couchdb.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.261997 celery-5.3.0rc1/celery/backends/database/
--rw-r--r--   0 nusnus     (501) staff       (20)     7751 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/database/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3351 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/database/models.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3011 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/database/session.py
--rw-r--r--   0 nusnus     (501) staff       (20)    17179 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/dynamodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8319 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/elasticsearch.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3776 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/filesystem.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10666 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/mongodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    26389 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/redis.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12077 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/rpc.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2752 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/backends/s3.py
--rw-r--r--   0 nusnus     (501) staff       (20)    24338 2023-02-01 21:32:36.000000 celery-5.3.0rc1/celery/beat.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.263936 celery-5.3.0rc1/celery/bin/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10023 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/amqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8525 2023-02-08 16:42:25.000000 celery-5.3.0rc1/celery/bin/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2592 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2370 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/call.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7317 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7058 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2794 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5796 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/graph.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1058 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/list.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4267 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/logtool.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2108 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/migrate.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15364 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/multi.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2547 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/purge.py
--rw-r--r--   0 nusnus     (501) staff       (20)      976 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/result.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4778 2023-02-01 17:22:50.000000 celery-5.3.0rc1/celery/bin/shell.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3064 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bin/upgrade.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12884 2023-03-24 12:39:07.000000 celery-5.3.0rc1/celery/bin/worker.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12277 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/bootsteps.py
--rw-r--r--   0 nusnus     (501) staff       (20)    95874 2023-02-15 19:02:20.000000 celery-5.3.0rc1/celery/canvas.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.264837 celery-5.3.0rc1/celery/concurrency/
--rw-r--r--   0 nusnus     (501) staff       (20)     1457 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/concurrency/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    51471 2023-04-09 22:45:48.000000 celery-5.3.0rc1/celery/concurrency/asynpool.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4706 2023-02-01 10:58:20.000000 celery-5.3.0rc1/celery/concurrency/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5126 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/concurrency/eventlet.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3387 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/concurrency/gevent.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5850 2023-02-01 10:58:20.000000 celery-5.3.0rc1/celery/concurrency/prefork.py
--rw-r--r--   0 nusnus     (501) staff       (20)      754 2023-02-01 10:58:20.000000 celery-5.3.0rc1/celery/concurrency/solo.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1920 2023-02-01 10:58:20.000000 celery-5.3.0rc1/celery/concurrency/thread.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.265729 celery-5.3.0rc1/celery/contrib/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/celery/contrib/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5003 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/contrib/abortable.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14361 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/contrib/migrate.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6754 2023-05-03 13:09:34.000000 celery-5.3.0rc1/celery/contrib/pytest.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5005 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/contrib/rdb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3391 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/contrib/sphinx.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.266558 celery-5.3.0rc1/celery/contrib/testing/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/celery/contrib/testing/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3112 2023-02-01 17:22:50.000000 celery-5.3.0rc1/celery/contrib/testing/app.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7739 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/contrib/testing/manager.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4182 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/contrib/testing/mocks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      208 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/contrib/testing/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5792 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/contrib/testing/worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.267728 celery-5.3.0rc1/celery/events/
--rw-r--r--   0 nusnus     (501) staff       (20)      477 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/events/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    17961 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/events/cursesmon.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8987 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/events/dispatcher.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3116 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/events/dumper.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1736 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/events/event.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4998 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/events/receiver.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3294 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/events/snapshot.py
--rw-r--r--   0 nusnus     (501) staff       (20)    25648 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/events/state.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9086 2023-03-24 12:39:07.000000 celery-5.3.0rc1/celery/exceptions.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.268015 celery-5.3.0rc1/celery/fixups/
--rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-08-03 16:05:58.000000 celery-5.3.0rc1/celery/fixups/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7161 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/fixups/django.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.268507 celery-5.3.0rc1/celery/loaders/
--rw-r--r--   0 nusnus     (501) staff       (20)      490 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/loaders/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      199 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/loaders/app.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8825 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/loaders/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1520 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/loaders/default.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16087 2023-02-01 21:21:33.000000 celery-5.3.0rc1/celery/local.py
--rw-r--r--   0 nusnus     (501) staff       (20)    25290 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/platforms.py
--rw-r--r--   0 nusnus     (501) staff       (20)    35282 2023-03-05 11:09:02.000000 celery-5.3.0rc1/celery/result.py
--rw-r--r--   0 nusnus     (501) staff       (20)    32003 2023-03-15 18:36:50.000000 celery-5.3.0rc1/celery/schedules.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.269078 celery-5.3.0rc1/celery/security/
--rw-r--r--   0 nusnus     (501) staff       (20)     2363 2023-02-01 17:22:50.000000 celery-5.3.0rc1/celery/security/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4008 2023-03-05 11:09:02.000000 celery-5.3.0rc1/celery/security/certificate.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1189 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/security/key.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4248 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/security/serialization.py
--rw-r--r--   0 nusnus     (501) staff       (20)      845 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/security/utils.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4384 2023-04-09 22:45:48.000000 celery-5.3.0rc1/celery/signals.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3324 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/states.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.272573 celery-5.3.0rc1/celery/utils/
--rw-r--r--   0 nusnus     (501) staff       (20)      935 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2874 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/abstract.py
--rw-r--r--   0 nusnus     (501) staff       (20)    25427 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/utils/collections.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4709 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/debug.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3620 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/deprecated.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.272846 celery-5.3.0rc1/celery/utils/dispatch/
--rw-r--r--   0 nusnus     (501) staff       (20)       74 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/dispatch/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13603 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/dispatch/signal.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12017 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/functional.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9041 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/graph.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5032 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/imports.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2871 2023-04-09 22:45:48.000000 celery-5.3.0rc1/celery/utils/iso8601.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8757 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/utils/log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2858 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/nodenames.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4215 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/objects.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8945 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/utils/saferepr.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8209 2023-03-24 12:39:07.000000 celery-5.3.0rc1/celery/utils/serialization.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.273099 celery-5.3.0rc1/celery/utils/static/
--rw-r--r--   0 nusnus     (501) staff       (20)      299 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/static/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2556 2022-08-03 16:05:58.000000 celery-5.3.0rc1/celery/utils/static/celery_128.png
--rw-r--r--   0 nusnus     (501) staff       (20)     1085 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/sysinfo.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4532 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/term.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5844 2023-04-09 22:45:48.000000 celery-5.3.0rc1/celery/utils/text.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9552 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/threads.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14987 2023-04-09 22:45:48.000000 celery-5.3.0rc1/celery/utils/time.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4813 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/utils/timer2.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.274500 celery-5.3.0rc1/celery/worker/
--rw-r--r--   0 nusnus     (501) staff       (20)       95 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4593 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/autoscale.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7497 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/components.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.275586 celery-5.3.0rc1/celery/worker/consumer/
--rw-r--r--   0 nusnus     (501) staff       (20)      391 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      525 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/agent.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1026 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/connection.py
--rw-r--r--   0 nusnus     (501) staff       (20)    28320 2023-02-01 19:42:55.000000 celery-5.3.0rc1/celery/worker/consumer/consumer.py
--rw-r--r--   0 nusnus     (501) staff       (20)      946 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2054 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6833 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/gossip.py
--rw-r--r--   0 nusnus     (501) staff       (20)      930 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/heart.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2519 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/mingle.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1960 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/consumer/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)    19460 2023-05-03 10:04:14.000000 celery-5.3.0rc1/celery/worker/control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2107 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/heartbeat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4433 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/loops.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3630 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/pidbox.py
--rw-r--r--   0 nusnus     (501) staff       (20)    27019 2023-05-03 10:04:14.000000 celery-5.3.0rc1/celery/worker/request.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8583 2023-05-03 10:04:14.000000 celery-5.3.0rc1/celery/worker/state.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7349 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/strategy.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14460 2022-12-29 15:36:27.000000 celery-5.3.0rc1/celery/worker/worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.256371 celery-5.3.0rc1/celery.egg-info/
--rw-r--r--   0 nusnus     (501) staff       (20)    18012 2023-05-11 12:00:34.000000 celery-5.3.0rc1/celery.egg-info/PKG-INFO
--rw-r--r--   0 nusnus     (501) staff       (20)    21178 2023-05-11 12:00:34.000000 celery-5.3.0rc1/celery.egg-info/SOURCES.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        1 2023-05-11 12:00:34.000000 celery-5.3.0rc1/celery.egg-info/dependency_links.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       48 2023-05-11 12:00:34.000000 celery-5.3.0rc1/celery.egg-info/entry_points.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        1 2023-02-01 21:51:23.000000 celery-5.3.0rc1/celery.egg-info/not-zip-safe
--rw-r--r--   0 nusnus     (501) staff       (20)     1605 2023-05-11 12:00:34.000000 celery-5.3.0rc1/celery.egg-info/requires.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        7 2023-05-11 12:00:34.000000 celery-5.3.0rc1/celery.egg-info/top_level.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.279370 celery-5.3.0rc1/docs/
--rw-r--r--   0 nusnus     (501) staff       (20)     5293 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/AUTHORS.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     8111 2023-02-01 19:58:41.000000 celery-5.3.0rc1/docs/Makefile
--rw-r--r--   0 nusnus     (501) staff       (20)      494 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/THANKS
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.279651 celery-5.3.0rc1/docs/_ext/
--rw-r--r--   0 nusnus     (501) staff       (20)     5164 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/_ext/celerydocs.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.279913 celery-5.3.0rc1/docs/_static/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/_static/.keep
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.280018 celery-5.3.0rc1/docs/_templates/
--rw-r--r--   0 nusnus     (501) staff       (20)      486 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/_templates/sidebardonations.html
--rw-r--r--   0 nusnus     (501) staff       (20)       30 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/changelog.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      981 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/community.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2597 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/conf.py
--rw-r--r--   0 nusnus     (501) staff       (20)       83 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/configuration.html
--rw-r--r--   0 nusnus     (501) staff       (20)       33 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/contributing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      931 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/copyright.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.280570 celery-5.3.0rc1/docs/django/
--rw-r--r--   0 nusnus     (501) staff       (20)     7886 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/django/first-steps-with-django.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      137 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/django/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    29852 2023-04-09 22:45:48.000000 celery-5.3.0rc1/docs/faq.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.281603 celery-5.3.0rc1/docs/getting-started/
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.282472 celery-5.3.0rc1/docs/getting-started/backends-and-brokers/
--rw-r--r--   0 nusnus     (501) staff       (20)     3903 2023-04-09 22:45:48.000000 celery-5.3.0rc1/docs/getting-started/backends-and-brokers/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5010 2023-02-01 19:42:55.000000 celery-5.3.0rc1/docs/getting-started/backends-and-brokers/rabbitmq.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     7239 2023-02-19 13:53:35.000000 celery-5.3.0rc1/docs/getting-started/backends-and-brokers/redis.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    10843 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/getting-started/backends-and-brokers/sqs.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    14995 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/getting-started/first-steps-with-celery.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/getting-started/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    10903 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/getting-started/introduction.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    22787 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/getting-started/next-steps.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      132 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/getting-started/resources.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     4448 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/glossary.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.287689 celery-5.3.0rc1/docs/history/
--rw-r--r--   0 nusnus     (501) staff       (20)    58104 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-1.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    34009 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-2.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    23550 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-2.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    33558 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-2.2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    11200 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-2.3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    13012 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-2.4.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5414 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-2.5.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    49344 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-3.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    52336 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-3.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     6432 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-4.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8950 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-4.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    13593 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-4.2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    17251 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-4.3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    24332 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-4.4.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5720 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-5.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5592 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/changelog-5.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      675 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    16026 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-2.5.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    30892 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-3.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    44129 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-3.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    76466 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-4.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8244 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-4.1.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    35711 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-4.2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    16865 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-4.3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     6999 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-4.4.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    10957 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-5.0.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    14128 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/history/whatsnew-5.1.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.289699 celery-5.3.0rc1/docs/images/
--rw-r--r--   0 nusnus     (501) staff       (20)    14168 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/celery-banner-small.png
--rw-r--r--   0 nusnus     (501) staff       (20)    14038 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/celery-banner.png
--rw-r--r--   0 nusnus     (501) staff       (20)     2556 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/celery_128.png
--rw-r--r--   0 nusnus     (501) staff       (20)     8658 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/celery_512.png
--rw-r--r--   0 nusnus     (501) staff       (20)    77397 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/celeryevshotsm.jpg
--rw-r--r--   0 nusnus     (501) staff       (20)    88879 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/dashboard.png
--rw-r--r--   0 nusnus     (501) staff       (20)     4286 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/favicon.ico
--rw-r--r--   0 nusnus     (501) staff       (20)   146412 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/monitor.png
--rw-r--r--   0 nusnus     (501) staff       (20)    35894 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/result_graph.png
--rw-r--r--   0 nusnus     (501) staff       (20)    99783 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/images/worker_graph_full.png
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.290511 celery-5.3.0rc1/docs/includes/
--rw-r--r--   0 nusnus     (501) staff       (20)     4023 2023-02-01 19:42:55.000000 celery-5.3.0rc1/docs/includes/installation.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     6422 2023-05-11 11:45:05.000000 celery-5.3.0rc1/docs/includes/introduction.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1375 2023-02-01 19:42:55.000000 celery-5.3.0rc1/docs/includes/resources.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1613 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/index.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.292671 celery-5.3.0rc1/docs/internals/
--rw-r--r--   0 nusnus     (501) staff       (20)     5985 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/internals/app-overview.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5696 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/internals/deprecation.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8586 2023-02-01 20:37:32.000000 celery-5.3.0rc1/docs/internals/guide.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      206 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     9898 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/internals/protocol.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.302573 celery-5.3.0rc1/docs/internals/reference/
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery._state.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.app.annotations.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      224 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.app.routes.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.app.trace.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.arangodb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.asynchronous.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.azureblockblob.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      243 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.cache.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.cassandra.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      253 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.consul.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      284 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.cosmosdbsql.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      270 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.couchbase.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      262 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.couchdb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      276 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.database.models.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.database.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      283 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.database.session.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      265 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.dynamodb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      280 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.elasticsearch.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      269 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.filesystem.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.mongodb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.redis.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.rpc.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      206 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.backends.s3.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      270 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.concurrency.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      310 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.concurrency.eventlet.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.concurrency.gevent.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      307 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.concurrency.prefork.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      229 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.concurrency.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      310 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.concurrency.solo.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.concurrency.thread.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.events.cursesmon.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      251 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.events.dumper.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.events.snapshot.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      231 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.platforms.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      272 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.security.certificate.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      248 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.security.key.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.security.serialization.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.security.utils.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.abstract.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      252 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.collections.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.deprecated.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      252 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.dispatch.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      295 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.dispatch.signal.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      282 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.functional.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.graph.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.imports.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.iso8601.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.log.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.nodenames.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.objects.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      195 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.saferepr.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.serialization.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.sysinfo.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.term.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.text.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      251 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.threads.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.time.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      224 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.utils.timer2.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.worker.autoscale.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      259 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.worker.components.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.worker.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      266 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.worker.heartbeat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.worker.loops.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/reference/celery.worker.pidbox.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1960 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/internals/reference/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1452 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/internals/worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     7675 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/make.bat
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.313002 celery-5.3.0rc1/docs/reference/
--rw-r--r--   0 nusnus     (501) staff       (20)     1379 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.amqp.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.autoretry.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      234 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.backends.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      268 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.builtins.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      265 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.defaults.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      222 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      213 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.log.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      228 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.registry.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.task.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      219 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.app.utils.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      253 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.apps.beat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.apps.multi.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.apps.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      220 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.beat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      189 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/reference/celery.bin.amqp.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      216 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      254 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.beat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.call.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.celery.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.graph.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      258 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.list.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.logtool.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.migrate.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      249 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.multi.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.purge.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      264 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.result.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.shell.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      267 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.upgrade.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      242 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bin.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.bootsteps.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.abortable.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      230 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.migrate.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.pytest.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      256 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.rdb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      184 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.sphinx.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.testing.app.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.testing.manager.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.testing.mocks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      297 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.contrib.testing.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      304 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.events.dispatcher.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.events.event.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.events.receiver.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      194 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.events.state.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      222 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.exceptions.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      227 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.loaders.app.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      250 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.loaders.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      255 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.loaders.default.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.loaders.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      204 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.result.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     3497 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/reference/celery.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      261 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.schedules.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      200 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.security.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      257 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.signals.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      106 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.states.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      871 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.utils.debug.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.agent.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      306 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.connection.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.consumer.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      297 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.control.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.events.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.gossip.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.heart.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.mingle.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      273 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      291 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.consumer.tasks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      244 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.request.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      236 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.state.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      245 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.strategy.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      239 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/reference/celery.worker.worker.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      143 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/reference/cli.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1952 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/reference/index.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.313424 celery-5.3.0rc1/docs/sec/
--rw-r--r--   0 nusnus     (501) staff       (20)     2921 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/sec/CELERYSA-0001.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     2656 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/sec/CELERYSA-0002.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1551 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/sec/CELERYSA-0003.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     4879 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/spelling_wordlist.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.313574 celery-5.3.0rc1/docs/templates/
--rw-r--r--   0 nusnus     (501) staff       (20)     1186 2023-02-01 19:42:55.000000 celery-5.3.0rc1/docs/templates/readme.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.314234 celery-5.3.0rc1/docs/tutorials/
--rw-r--r--   0 nusnus     (501) staff       (20)       86 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/tutorials/daemonizing.html
--rw-r--r--   0 nusnus     (501) staff       (20)       91 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/tutorials/debugging.html
--rw-r--r--   0 nusnus     (501) staff       (20)      121 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/tutorials/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2766 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/tutorials/task-cookbook.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.319825 celery-5.3.0rc1/docs/userguide/
--rw-r--r--   0 nusnus     (501) staff       (20)    14779 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/userguide/application.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    25233 2023-02-19 13:53:35.000000 celery-5.3.0rc1/docs/userguide/calling.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    38007 2023-05-10 13:34:51.000000 celery-5.3.0rc1/docs/userguide/canvas.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.320381 celery-5.3.0rc1/docs/userguide/concurrency/
--rw-r--r--   0 nusnus     (501) staff       (20)     2665 2023-02-01 19:42:55.000000 celery-5.3.0rc1/docs/userguide/concurrency/eventlet.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      140 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/userguide/concurrency/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    98436 2023-04-19 13:29:15.000000 celery-5.3.0rc1/docs/userguide/configuration.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    17699 2023-02-01 19:42:55.000000 celery-5.3.0rc1/docs/userguide/daemonizing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     3131 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/userguide/debugging.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    30057 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/userguide/extending.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      372 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/userguide/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    21759 2023-02-19 13:53:35.000000 celery-5.3.0rc1/docs/userguide/monitoring.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8437 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/userguide/optimizing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    20950 2023-03-24 12:39:07.000000 celery-5.3.0rc1/docs/userguide/periodic-tasks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    24323 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/userguide/routing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     8693 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/userguide/security.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    18113 2023-04-09 22:45:48.000000 celery-5.3.0rc1/docs/userguide/signals.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      345 2022-08-03 16:05:58.000000 celery-5.3.0rc1/docs/userguide/sphinx.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    64543 2023-02-01 10:58:20.000000 celery-5.3.0rc1/docs/userguide/tasks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    11146 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/userguide/testing.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    34758 2023-02-01 19:42:55.000000 celery-5.3.0rc1/docs/userguide/workers.rst
--rw-r--r--   0 nusnus     (501) staff       (20)    12812 2022-12-29 15:36:27.000000 celery-5.3.0rc1/docs/whatsnew-5.2.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.320842 celery-5.3.0rc1/examples/
--rw-r--r--   0 nusnus     (501) staff       (20)     6148 2023-04-12 11:27:42.000000 celery-5.3.0rc1/examples/.DS_Store
--rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/README.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.321058 celery-5.3.0rc1/examples/app/
--rw-r--r--   0 nusnus     (501) staff       (20)      822 2023-05-03 10:04:11.000000 celery-5.3.0rc1/examples/app/myapp.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.322236 celery-5.3.0rc1/examples/celery_http_gateway/
--rw-r--r--   0 nusnus     (501) staff       (20)     1382 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/celery_http_gateway/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/celery_http_gateway/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      385 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/celery_http_gateway/manage.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3001 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/celery_http_gateway/settings.py
--rw-r--r--   0 nusnus     (501) staff       (20)       88 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/celery_http_gateway/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      678 2023-02-01 17:22:50.000000 celery-5.3.0rc1/examples/celery_http_gateway/urls.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.322749 celery-5.3.0rc1/examples/django/
--rw-r--r--   0 nusnus     (501) staff       (20)     1546 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/README.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.323205 celery-5.3.0rc1/examples/django/demoapp/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/django/demoapp/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.323614 celery-5.3.0rc1/examples/django/demoapp/migrations/
--rw-r--r--   0 nusnus     (501) staff       (20)      486 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/django/demoapp/migrations/0001_initial.py
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/django/demoapp/migrations/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      103 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/demoapp/models.py
--rw-r--r--   0 nusnus     (501) staff       (20)      437 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/demoapp/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)       26 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/demoapp/views.py
--rwxr-xr-x   0 nusnus     (501) staff       (20)      248 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/manage.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.324324 celery-5.3.0rc1/examples/django/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)      174 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      659 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/proj/celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3639 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/proj/settings.py
--rw-r--r--   0 nusnus     (501) staff       (20)      556 2023-02-01 17:22:50.000000 celery-5.3.0rc1/examples/django/proj/urls.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1132 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/django/proj/wsgi.py
--rw-r--r--   0 nusnus     (501) staff       (20)       47 2023-02-01 10:58:20.000000 celery-5.3.0rc1/examples/django/requirements.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.324952 celery-5.3.0rc1/examples/eventlet/
--rw-r--r--   0 nusnus     (501) staff       (20)     1449 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/eventlet/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1673 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/eventlet/bulk_task_producer.py
--rw-r--r--   0 nusnus     (501) staff       (20)      312 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/eventlet/celeryconfig.py
--rw-r--r--   0 nusnus     (501) staff       (20)      306 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/eventlet/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2009 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/eventlet/webcrawler.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.325244 celery-5.3.0rc1/examples/gevent/
--rw-r--r--   0 nusnus     (501) staff       (20)      255 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/gevent/celeryconfig.py
--rw-r--r--   0 nusnus     (501) staff       (20)      325 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/gevent/tasks.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.325382 celery-5.3.0rc1/examples/next-steps/
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.325730 celery-5.3.0rc1/examples/next-steps/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/next-steps/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      294 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/next-steps/proj/celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)      167 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/next-steps/proj/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1224 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/next-steps/setup.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.325861 celery-5.3.0rc1/examples/periodic-tasks/
--rw-r--r--   0 nusnus     (501) staff       (20)     1518 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/periodic-tasks/myapp.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.325996 celery-5.3.0rc1/examples/resultgraph/
--rw-r--r--   0 nusnus     (501) staff       (20)     2860 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/resultgraph/tasks.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.326132 celery-5.3.0rc1/examples/security/
--rw-r--r--   0 nusnus     (501) staff       (20)     1058 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/security/mysecureapp.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.326467 celery-5.3.0rc1/examples/security/ssl/
--rw-r--r--   0 nusnus     (501) staff       (20)     3243 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/security/ssl/worker.key
--rw-r--r--   0 nusnus     (501) staff       (20)     1923 2022-08-03 16:05:58.000000 celery-5.3.0rc1/examples/security/ssl/worker.pem
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.327773 celery-5.3.0rc1/examples/stamping/
--rw-r--r--   0 nusnus     (501) staff       (20)      103 2023-02-22 16:00:00.000000 celery-5.3.0rc1/examples/stamping/config.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1358 2023-02-22 16:00:00.000000 celery-5.3.0rc1/examples/stamping/examples.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1806 2023-02-15 16:17:24.000000 celery-5.3.0rc1/examples/stamping/myapp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2548 2023-03-27 21:41:42.000000 celery-5.3.0rc1/examples/stamping/revoke_example.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3311 2023-02-22 16:00:00.000000 celery-5.3.0rc1/examples/stamping/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2410 2023-02-15 16:17:24.000000 celery-5.3.0rc1/examples/stamping/visitors.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.328003 celery-5.3.0rc1/examples/tutorial/
--rw-r--r--   0 nusnus     (501) staff       (20)      158 2022-12-29 15:36:27.000000 celery-5.3.0rc1/examples/tutorial/tasks.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.249477 celery-5.3.0rc1/extra/
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.328160 celery-5.3.0rc1/extra/bash-completion/
--rw-r--r--   0 nusnus     (501) staff       (20)      636 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/bash-completion/celery.bash
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.328634 celery-5.3.0rc1/extra/generic-init.d/
--rwxr-xr-x   0 nusnus     (501) staff       (20)     9068 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/generic-init.d/celerybeat
--rwxr-xr-x   0 nusnus     (501) staff       (20)    10813 2023-02-19 13:53:35.000000 celery-5.3.0rc1/extra/generic-init.d/celeryd
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.329124 celery-5.3.0rc1/extra/macOS/
--rw-r--r--   0 nusnus     (501) staff       (20)      751 2022-08-03 16:05:58.000000 celery-5.3.0rc1/extra/macOS/org.celeryq.beat.plist
--rw-r--r--   0 nusnus     (501) staff       (20)      757 2022-08-03 16:05:58.000000 celery-5.3.0rc1/extra/macOS/org.celeryq.worker.plist
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.329968 celery-5.3.0rc1/extra/supervisord/
--rw-r--r--   0 nusnus     (501) staff       (20)      134 2022-08-03 16:05:58.000000 celery-5.3.0rc1/extra/supervisord/celery.sh
--rw-r--r--   0 nusnus     (501) staff       (20)      699 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/supervisord/celerybeat.conf
--rw-r--r--   0 nusnus     (501) staff       (20)      949 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/supervisord/celeryd.conf
--rw-r--r--   0 nusnus     (501) staff       (20)      982 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/supervisord/supervisord.conf
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.330823 celery-5.3.0rc1/extra/systemd/
--rw-r--r--   0 nusnus     (501) staff       (20)      506 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/systemd/celery.conf
--rw-r--r--   0 nusnus     (501) staff       (20)      740 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/systemd/celery.service
--rw-r--r--   0 nusnus     (501) staff       (20)       78 2022-08-03 16:05:58.000000 celery-5.3.0rc1/extra/systemd/celery.tmpfiles
--rw-r--r--   0 nusnus     (501) staff       (20)      395 2022-12-29 15:36:27.000000 celery-5.3.0rc1/extra/systemd/celerybeat.service
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.330984 celery-5.3.0rc1/extra/zsh-completion/
--rw-r--r--   0 nusnus     (501) staff       (20)     6244 2022-08-03 16:05:58.000000 celery-5.3.0rc1/extra/zsh-completion/celery.zsh
--rw-r--r--   0 nusnus     (501) staff       (20)     1216 2023-03-15 18:36:50.000000 celery-5.3.0rc1/pyproject.toml
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.333318 celery-5.3.0rc1/requirements/
--rw-r--r--   0 nusnus     (501) staff       (20)     1454 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      251 2023-04-09 22:45:48.000000 celery-5.3.0rc1/requirements/default.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.333474 celery-5.3.0rc1/requirements/deps/
--rw-r--r--   0 nusnus     (501) staff       (20)       10 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/deps/mock.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      151 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/dev.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      187 2023-05-08 23:34:52.000000 celery-5.3.0rc1/requirements/docs.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.337421 celery-5.3.0rc1/requirements/extras/
--rw-r--r--   0 nusnus     (501) staff       (20)       16 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/arangodb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       21 2023-04-04 02:08:30.000000 celery-5.3.0rc1/requirements/extras/auth.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       28 2023-03-24 12:39:07.000000 celery-5.3.0rc1/requirements/extras/azureblockblob.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      111 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/extras/brotli.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       28 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/cassandra.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       22 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/consul.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       20 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/cosmosdbsql.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      119 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/couchbase.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       18 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/couchdb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       15 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/extras/django.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/dynamodb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       18 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/elasticsearch.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       40 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/eventlet.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/gevent.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       19 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/extras/librabbitmq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       45 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/memcache.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       20 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/mongodb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       15 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/extras/msgpack.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       23 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/pymemcache.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        6 2023-03-05 11:09:02.000000 celery-5.3.0rc1/requirements/extras/pyro.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       21 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/pytest.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       20 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/extras/redis.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       17 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/extras/s3.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/extras/slmq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       53 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/extras/solar.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/sphinxautobuild.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       24 2023-03-24 12:39:07.000000 celery-5.3.0rc1/requirements/extras/sqlalchemy.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       20 2023-04-09 22:45:48.000000 celery-5.3.0rc1/requirements/extras/sqs.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       73 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/extras/tblib.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       39 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/extras/thread.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/extras/yaml.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       14 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/extras/zeromq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/extras/zookeeper.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       18 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/extras/zstd.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      235 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/pkgutils.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       19 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/security.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      175 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/test-ci-base.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      539 2022-12-29 15:36:27.000000 celery-5.3.0rc1/requirements/test-ci-default.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      160 2023-04-19 13:29:15.000000 celery-5.3.0rc1/requirements/test-integration.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       17 2022-08-03 16:05:58.000000 celery-5.3.0rc1/requirements/test-pypy3.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      306 2023-05-10 13:34:09.000000 celery-5.3.0rc1/requirements/test.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      485 2023-05-11 12:00:34.369533 celery-5.3.0rc1/setup.cfg
--rwxr-xr-x   0 nusnus     (501) staff       (20)     5077 2023-05-09 00:06:55.000000 celery-5.3.0rc1/setup.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.337614 celery-5.3.0rc1/t/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.337746 celery-5.3.0rc1/t/benchmarks/
--rw-r--r--   0 nusnus     (501) staff       (20)     2816 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/benchmarks/bench_worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.340220 celery-5.3.0rc1/t/integration/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/integration/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2350 2023-05-03 13:09:34.000000 celery-5.3.0rc1/t/integration/conftest.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12427 2023-03-24 12:39:07.000000 celery-5.3.0rc1/t/integration/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1120 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/integration/test_backend.py
--rw-r--r--   0 nusnus     (501) staff       (20)   132248 2023-03-24 18:03:27.000000 celery-5.3.0rc1/t/integration/test_canvas.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7796 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/integration/test_inspect.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3459 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/integration/test_security.py
--rw-r--r--   0 nusnus     (501) staff       (20)    18238 2023-05-03 10:04:14.000000 celery-5.3.0rc1/t/integration/test_tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      688 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/integration/test_worker.py
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/integration/test_worker_config.py
--rw-r--r--   0 nusnus     (501) staff       (20)      226 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/skip.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.340746 celery-5.3.0rc1/t/unit/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.344391 celery-5.3.0rc1/t/unit/app/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/app/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13768 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_amqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1338 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_annotations.py
--rw-r--r--   0 nusnus     (501) staff       (20)    41390 2023-04-09 22:45:48.000000 celery-5.3.0rc1/t/unit/app/test_app.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4542 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/app/test_backends.py
--rw-r--r--   0 nusnus     (501) staff       (20)    29065 2023-04-09 22:45:48.000000 celery-5.3.0rc1/t/unit/app/test_beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5528 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_builtins.py
--rw-r--r--   0 nusnus     (501) staff       (20)      356 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/app/test_celery.py
--rw-r--r--   0 nusnus     (501) staff       (20)    19105 2023-03-27 21:22:03.000000 celery-5.3.0rc1/t/unit/app/test_control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1608 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_defaults.py
--rw-r--r--   0 nusnus     (501) staff       (20)      801 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/app/test_exceptions.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8823 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_loaders.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11820 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2349 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_registry.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8026 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/app/test_routes.py
--rw-r--r--   0 nusnus     (501) staff       (20)    37835 2023-04-09 22:45:48.000000 celery-5.3.0rc1/t/unit/app/test_schedules.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1790 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/app/test_utils.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.344659 celery-5.3.0rc1/t/unit/apps/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/apps/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16234 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/apps/test_multi.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.351142 celery-5.3.0rc1/t/unit/backends/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/backends/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4362 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_arangodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6874 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/backends/test_asynchronous.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6794 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_azureblockblob.py
--rw-r--r--   0 nusnus     (501) staff       (20)    45945 2023-03-11 14:59:39.000000 celery-5.3.0rc1/t/unit/backends/test_base.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10318 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_cache.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8669 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_cassandra.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1448 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_consul.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4994 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_cosmosdbsql.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4846 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_couchbase.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3971 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_couchdb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14891 2023-02-01 17:22:50.000000 celery-5.3.0rc1/t/unit/backends/test_database.py
--rw-r--r--   0 nusnus     (501) staff       (20)    19214 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_dynamodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    32601 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_elasticsearch.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4435 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_filesystem.py
--rw-r--r--   0 nusnus     (501) staff       (20)    28352 2023-04-09 22:45:48.000000 celery-5.3.0rc1/t/unit/backends/test_mongodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)    50595 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_redis.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3692 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/backends/test_rpc.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6654 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/backends/test_s3.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.351723 celery-5.3.0rc1/t/unit/bin/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/bin/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)       18 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/bin/celery.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.352393 celery-5.3.0rc1/t/unit/bin/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)       64 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/bin/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      121 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/bin/proj/app.py
--rw-r--r--   0 nusnus     (501) staff       (20)       22 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/bin/proj/app2.py
--rw-r--r--   0 nusnus     (501) staff       (20)      109 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/bin/proj/scheduler.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1116 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/bin/test_beat.py
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/bin/test_multi.py
--rw-r--r--   0 nusnus     (501) staff       (20)      529 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/bin/test_worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.353691 celery-5.3.0rc1/t/unit/concurrency/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/concurrency/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5687 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/concurrency/test_concurrency.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4721 2023-02-01 17:22:50.000000 celery-5.3.0rc1/t/unit/concurrency/test_eventlet.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3146 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/concurrency/test_gevent.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1837 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/concurrency/test_pool.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16398 2023-04-09 22:45:48.000000 celery-5.3.0rc1/t/unit/concurrency/test_prefork.py
--rw-r--r--   0 nusnus     (501) staff       (20)      848 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/concurrency/test_solo.py
--rw-r--r--   0 nusnus     (501) staff       (20)      728 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/concurrency/test_thread.py
--rw-r--r--   0 nusnus     (501) staff       (20)    23214 2023-05-03 13:09:34.000000 celery-5.3.0rc1/t/unit/conftest.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.355139 celery-5.3.0rc1/t/unit/contrib/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/contrib/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.356190 celery-5.3.0rc1/t/unit/contrib/proj/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/contrib/proj/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      183 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/contrib/proj/conf.py
--rw-r--r--   0 nusnus     (501) staff       (20)       93 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/contrib/proj/contents.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      249 2023-02-01 17:22:50.000000 celery-5.3.0rc1/t/unit/contrib/proj/foo.py
--rw-r--r--   0 nusnus     (501) staff       (20)      113 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/contrib/proj/xyzzy.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1394 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/contrib/test_abortable.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10615 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/contrib/test_migrate.py
--rw-r--r--   0 nusnus     (501) staff       (20)      785 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/contrib/test_pytest.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3146 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/contrib/test_rdb.py
--rw-r--r--   0 nusnus     (501) staff       (20)      731 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/contrib/test_sphinx.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1474 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/contrib/test_worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.357212 celery-5.3.0rc1/t/unit/events/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/events/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2304 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/events/test_cursesmon.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11372 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/events/test_events.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3359 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/events/test_snapshot.py
--rw-r--r--   0 nusnus     (501) staff       (20)    22261 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/events/test_state.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.357673 celery-5.3.0rc1/t/unit/fixups/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/fixups/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11013 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/fixups/test_django.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.358806 celery-5.3.0rc1/t/unit/security/
--rw-r--r--   0 nusnus     (501) staff       (20)     7344 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/security/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      109 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/security/case.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3333 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/security/test_certificate.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1570 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/security/test_key.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6219 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/security/test_security.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2224 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/security/test_serialization.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.362287 celery-5.3.0rc1/t/unit/tasks/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/tasks/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    68472 2023-02-08 16:42:25.000000 celery-5.3.0rc1/t/unit/tasks/test_canvas.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12308 2023-02-08 16:42:25.000000 celery-5.3.0rc1/t/unit/tasks/test_chord.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3134 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/tasks/test_context.py
--rw-r--r--   0 nusnus     (501) staff       (20)    34984 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/tasks/test_result.py
--rw-r--r--   0 nusnus     (501) staff       (20)    52722 2023-03-24 18:03:27.000000 celery-5.3.0rc1/t/unit/tasks/test_stamping.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1085 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/tasks/test_states.py
--rw-r--r--   0 nusnus     (501) staff       (20)    56857 2023-03-24 12:39:07.000000 celery-5.3.0rc1/t/unit/tasks/test_tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)    21991 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/tasks/test_trace.py
--rw-r--r--   0 nusnus     (501) staff       (20)       78 2022-08-17 13:45:35.000000 celery-5.3.0rc1/t/unit/tasks/unit_tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      989 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/test_canvas.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.366351 celery-5.3.0rc1/t/unit/utils/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/utils/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12855 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/utils/test_collections.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2357 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_debug.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1739 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_deprecated.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5233 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_dispatcher.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13576 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/utils/test_functional.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1935 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_graph.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3272 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_imports.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8515 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_local.py
--rw-r--r--   0 nusnus     (501) staff       (20)      202 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_nodenames.py
--rw-r--r--   0 nusnus     (501) staff       (20)      172 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_objects.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1386 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_pickle.py
--rw-r--r--   0 nusnus     (501) staff       (20)    32949 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_platforms.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5555 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_saferepr.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3219 2023-04-09 22:45:48.000000 celery-5.3.0rc1/t/unit/utils/test_serialization.py
--rw-r--r--   0 nusnus     (501) staff       (20)      751 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_sysinfo.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1734 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_term.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1935 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_text.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2427 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_threads.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11465 2023-04-09 22:45:48.000000 celery-5.3.0rc1/t/unit/utils/test_time.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3215 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_timer2.py
--rw-r--r--   0 nusnus     (501) staff       (20)      624 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/utils/test_utils.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2023-05-11 12:00:34.368870 celery-5.3.0rc1/t/unit/worker/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-08-03 16:05:58.000000 celery-5.3.0rc1/t/unit/worker/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7574 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/worker/test_autoscale.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9415 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/worker/test_bootsteps.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2461 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/worker/test_components.py
--rw-r--r--   0 nusnus     (501) staff       (20)    30428 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/worker/test_consumer.py
--rw-r--r--   0 nusnus     (501) staff       (20)    27905 2023-05-03 10:04:14.000000 celery-5.3.0rc1/t/unit/worker/test_control.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2384 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/worker/test_heartbeat.py
--rw-r--r--   0 nusnus     (501) staff       (20)    18256 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/worker/test_loops.py
--rw-r--r--   0 nusnus     (501) staff       (20)    47040 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/worker/test_request.py
--rw-r--r--   0 nusnus     (501) staff       (20)      238 2022-12-29 15:36:27.000000 celery-5.3.0rc1/t/unit/worker/test_revoke.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6339 2023-05-03 10:04:14.000000 celery-5.3.0rc1/t/unit/worker/test_state.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10989 2023-02-01 10:58:20.000000 celery-5.3.0rc1/t/unit/worker/test_strategy.py
--rw-r--r--   0 nusnus     (501) staff       (20)    39912 2023-02-01 19:42:55.000000 celery-5.3.0rc1/t/unit/worker/test_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.539767 celery-5.3.0rc2/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8184 2023-02-02 09:58:18.000000 celery-5.3.0rc2/CONTRIBUTORS.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24179 2023-05-31 14:38:43.000000 celery-5.3.0rc2/Changelog.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2631 2021-10-12 14:26:47.000000 celery-5.3.0rc2/LICENSE
+-rw-rw-r--   0 asif      (1000) asif      (1000)      709 2021-10-12 14:26:47.000000 celery-5.3.0rc2/MANIFEST.in
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17914 2023-05-31 14:55:48.539767 celery-5.3.0rc2/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15859 2023-05-31 14:43:46.000000 celery-5.3.0rc2/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)       84 2021-10-12 14:26:47.000000 celery-5.3.0rc2/TODO
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.443765 celery-5.3.0rc2/celery/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5951 2023-05-31 14:42:37.000000 celery-5.3.0rc2/celery/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      409 2022-04-28 06:12:03.000000 celery-5.3.0rc2/celery/__main__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5029 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/_state.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.447766 celery-5.3.0rc2/celery/app/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2430 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/app/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    23151 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1445 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/annotations.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2489 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/app/autoretry.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2702 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/backends.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    50088 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/app/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6673 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/builtins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    29170 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15014 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/defaults.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1326 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9067 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2001 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/registry.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4527 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/routes.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    43264 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/app/task.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28320 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/app/trace.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13160 2022-07-28 12:22:51.000000 celery-5.3.0rc2/celery/app/utils.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.451766 celery-5.3.0rc2/celery/apps/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/apps/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5724 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/apps/beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16360 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/apps/multi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13208 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/apps/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.451766 celery-5.3.0rc2/celery/backends/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       23 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7739 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/backends/arangodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10309 2021-11-21 13:37:38.000000 celery-5.3.0rc2/celery/backends/asynchronous.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5127 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/backends/azureblockblob.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    43970 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/backends/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4817 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/cache.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9006 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/cassandra.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3816 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6777 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/cosmosdbsql.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3393 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/backends/couchbase.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2935 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/couchdb.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/backends/database/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7751 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/database/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3351 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/database/models.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3011 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/database/session.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17179 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/dynamodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8319 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/elasticsearch.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3776 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/backends/filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10666 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    26389 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12077 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/rpc.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2752 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/s3.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24338 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/beat.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/bin/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10023 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/bin/amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8525 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/bin/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2592 2022-07-28 12:22:51.000000 celery-5.3.0rc2/celery/bin/beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2370 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/call.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7317 2023-05-31 06:35:39.000000 celery-5.3.0rc2/celery/bin/celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7058 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2794 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5796 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/graph.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/list.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/logtool.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2108 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/migrate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15364 2023-05-31 06:35:39.000000 celery-5.3.0rc2/celery/bin/multi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2547 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/purge.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      976 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/result.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4778 2023-05-31 06:35:39.000000 celery-5.3.0rc2/celery/bin/shell.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3064 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/upgrade.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12884 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/bin/worker.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12277 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/bootsteps.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    95874 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/canvas.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/concurrency/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1457 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    51471 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/concurrency/asynpool.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4706 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5126 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/concurrency/eventlet.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3387 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/gevent.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5850 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/prefork.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      754 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/solo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1920 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/thread.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/contrib/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/contrib/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5003 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/contrib/abortable.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14361 2022-04-28 06:12:03.000000 celery-5.3.0rc2/celery/contrib/migrate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6754 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/pytest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5005 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/contrib/rdb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3391 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/sphinx.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/contrib/testing/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/contrib/testing/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3112 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/contrib/testing/app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7739 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/testing/manager.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4182 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/testing/mocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      208 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/contrib/testing/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5792 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/testing/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/events/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      477 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17961 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/events/cursesmon.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8987 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/dispatcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3116 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/dumper.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1736 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/event.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4998 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/receiver.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/snapshot.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25648 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/events/state.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9086 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/exceptions.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/fixups/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/fixups/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7161 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/fixups/django.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/loaders/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      490 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/loaders/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      199 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/loaders/app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8825 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/loaders/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1520 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/loaders/default.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16087 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/local.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25290 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/platforms.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    35282 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/result.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32003 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/schedules.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/security/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2363 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/security/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4008 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/security/certificate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1189 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/security/key.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4248 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/security/serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      845 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/security/utils.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4384 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/signals.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3324 2022-04-28 06:12:03.000000 celery-5.3.0rc2/celery/states.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.463766 celery-5.3.0rc2/celery/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      935 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2874 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/abstract.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25427 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/collections.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4709 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3620 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/deprecated.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.463766 celery-5.3.0rc2/celery/utils/dispatch/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       74 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/dispatch/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13603 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/dispatch/signal.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12017 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9041 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/graph.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5032 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2871 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/iso8601.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8757 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/nodenames.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4215 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8945 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/saferepr.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8209 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/serialization.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.463766 celery-5.3.0rc2/celery/utils/static/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      299 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/static/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/static/celery_128.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/sysinfo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4532 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/term.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5844 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/text.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9552 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/threads.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14987 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4813 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/timer2.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.467766 celery-5.3.0rc2/celery/worker/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       95 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4593 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/autoscale.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7497 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/worker/components.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.467766 celery-5.3.0rc2/celery/worker/consumer/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      391 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      525 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/agent.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1026 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28320 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/worker/consumer/consumer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      946 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2054 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6833 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/gossip.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      930 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/heart.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2519 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/mingle.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/worker/consumer/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    19884 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/worker/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2107 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/heartbeat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4433 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/loops.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3630 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/pidbox.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    27229 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/worker/request.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8583 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/worker/state.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7349 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/strategy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14460 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/worker/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.443765 celery-5.3.0rc2/celery.egg-info/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17914 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21130 2023-05-31 14:55:48.000000 celery-5.3.0rc2/celery.egg-info/SOURCES.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/dependency_links.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       49 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/entry_points.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1623 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/requires.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        7 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/top_level.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5293 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/AUTHORS.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8111 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/Makefile
+-rw-rw-r--   0 asif      (1000) asif      (1000)      494 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/THANKS
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/_ext/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5164 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/_ext/celerydocs.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/_static/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/_static/.keep
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/_templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/_templates/sidebardonations.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/changelog.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      981 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/community.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2597 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/conf.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       83 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/configuration.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       33 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/contributing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      931 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/copyright.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/django/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7886 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/django/first-steps-with-django.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      137 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/django/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    29852 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/faq.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/getting-started/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3903 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5010 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/rabbitmq.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7239 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/redis.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10843 2022-03-18 11:40:50.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/sqs.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14995 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/getting-started/first-steps-with-celery.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/getting-started/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10903 2021-12-29 05:20:59.000000 celery-5.3.0rc2/docs/getting-started/introduction.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    22787 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/getting-started/next-steps.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      132 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/getting-started/resources.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4448 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/glossary.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.475766 celery-5.3.0rc2/docs/history/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    58104 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/history/changelog-1.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34009 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    23550 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-2.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    33558 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11200 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13012 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.4.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5414 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-2.5.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    49344 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-3.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    52336 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-3.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6432 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8950 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13593 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17251 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24332 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/changelog-4.4.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5720 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-5.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5592 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-5.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      675 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16026 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-2.5.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    30892 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/whatsnew-3.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    44129 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-3.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    76466 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/history/whatsnew-4.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8244 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-4.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    35711 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-4.2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16865 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-4.3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6999 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/whatsnew-4.4.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10957 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-5.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14128 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/history/whatsnew-5.1.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.479766 celery-5.3.0rc2/docs/images/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14168 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery-banner-small.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14038 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery-banner.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery_128.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8658 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery_512.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    77397 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celeryevshotsm.jpg
+-rw-rw-r--   0 asif      (1000) asif      (1000)    88879 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/dashboard.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4286 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/favicon.ico
+-rw-rw-r--   0 asif      (1000) asif      (1000)   146412 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/monitor.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    35894 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/result_graph.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    99783 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/worker_graph_full.png
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.479766 celery-5.3.0rc2/docs/includes/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4023 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/includes/installation.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6422 2023-05-31 14:43:08.000000 celery-5.3.0rc2/docs/includes/introduction.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1375 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/includes/resources.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1613 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/index.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.479766 celery-5.3.0rc2/docs/internals/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5985 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/app-overview.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5696 2022-04-28 06:12:03.000000 celery-5.3.0rc2/docs/internals/deprecation.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8586 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/guide.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9898 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/protocol.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.487766 celery-5.3.0rc2/docs/internals/reference/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery._state.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.app.annotations.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.app.routes.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.app.trace.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.arangodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.asynchronous.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.azureblockblob.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      243 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.cache.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.cassandra.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.consul.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.cosmosdbsql.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.couchbase.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      262 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.couchdb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      276 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.database.models.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.database.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      283 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.database.session.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.dynamodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.elasticsearch.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      269 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.filesystem.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.mongodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.redis.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.rpc.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.s3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.eventlet.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.gevent.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      307 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.prefork.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      229 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.solo.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.thread.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.events.cursesmon.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.events.dumper.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.events.snapshot.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      231 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.platforms.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      272 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.certificate.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.key.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.utils.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.abstract.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.collections.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.deprecated.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.dispatch.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      295 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.dispatch.signal.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      282 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.functional.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.graph.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.imports.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.iso8601.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.log.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.nodenames.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.objects.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      195 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.saferepr.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.sysinfo.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.term.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.text.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.threads.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.time.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.timer2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.autoscale.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      259 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.components.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.heartbeat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.loops.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.pidbox.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1452 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7675 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/make.bat
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/reference/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1379 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.amqp.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.autoretry.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      234 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.backends.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      268 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.builtins.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.defaults.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      213 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.log.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      228 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.registry.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.task.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      219 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.utils.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.apps.beat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.apps.multi.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.apps.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      220 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.beat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      189 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/reference/celery.bin.amqp.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.beat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.call.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.celery.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.graph.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.list.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.logtool.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.migrate.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.multi.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.purge.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.result.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.shell.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.upgrade.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bootsteps.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.abortable.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      230 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.migrate.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.pytest.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.rdb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      184 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.sphinx.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.app.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.manager.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.mocks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.dispatcher.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.event.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.receiver.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      194 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.state.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.exceptions.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      227 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.app.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      250 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.default.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      204 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.result.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3497 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.schedules.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      200 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.security.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.signals.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      106 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.states.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      871 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.utils.debug.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.agent.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      306 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.consumer.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.gossip.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.heart.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.mingle.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.tasks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      244 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.request.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.state.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.strategy.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      143 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/cli.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1952 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/index.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/sec/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2921 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/sec/CELERYSA-0001.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2656 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/sec/CELERYSA-0002.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1551 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/sec/CELERYSA-0003.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4879 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/spelling_wordlist.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1186 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/templates/readme.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/tutorials/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       86 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/daemonizing.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       91 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/debugging.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)      121 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2766 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/task-cookbook.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/docs/userguide/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14779 2022-04-28 06:12:03.000000 celery-5.3.0rc2/docs/userguide/application.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25233 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/calling.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    38007 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/canvas.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/docs/userguide/concurrency/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2665 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/concurrency/eventlet.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      140 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/concurrency/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    98436 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/configuration.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17699 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/daemonizing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3131 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/debugging.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    30057 2022-03-18 11:40:50.000000 celery-5.3.0rc2/docs/userguide/extending.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      372 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21759 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/monitoring.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8437 2021-12-29 05:20:59.000000 celery-5.3.0rc2/docs/userguide/optimizing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    20950 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/periodic-tasks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24323 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/routing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8693 2022-07-28 12:22:51.000000 celery-5.3.0rc2/docs/userguide/security.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18113 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/signals.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      345 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/sphinx.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    64543 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/tasks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11146 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/testing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34758 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/workers.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12812 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/whatsnew-5.2.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/README.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/app/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      822 2022-06-29 10:52:39.000000 celery-5.3.0rc2/examples/app/myapp.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/celery_http_gateway/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1382 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      385 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/manage.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3001 2021-11-21 13:37:38.000000 celery-5.3.0rc2/examples/celery_http_gateway/settings.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       88 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      678 2022-03-18 11:40:50.000000 celery-5.3.0rc2/examples/celery_http_gateway/urls.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/django/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1546 2022-08-01 10:53:57.000000 celery-5.3.0rc2/examples/django/README.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/django/demoapp/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/django/demoapp/migrations/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/migrations/0001_initial.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/migrations/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      103 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/models.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      437 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       26 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/views.py
+-rwxrwxr-x   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/manage.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/django/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      174 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      659 2022-06-29 10:52:39.000000 celery-5.3.0rc2/examples/django/proj/celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3639 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/settings.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      556 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/urls.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/wsgi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       47 2023-02-02 09:58:18.000000 celery-5.3.0rc2/examples/django/requirements.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/eventlet/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1449 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/eventlet/bulk_task_producer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      312 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/celeryconfig.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      306 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2009 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/webcrawler.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/gevent/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/gevent/celeryconfig.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      325 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/gevent/tasks.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/next-steps/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/next-steps/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/proj/celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      167 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/proj/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1224 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/setup.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/periodic-tasks/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1518 2022-08-01 10:53:57.000000 celery-5.3.0rc2/examples/periodic-tasks/myapp.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/resultgraph/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2860 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/resultgraph/tasks.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/security/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/security/mysecureapp.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/security/ssl/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3243 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/security/ssl/worker.key
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1923 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/security/ssl/worker.pem
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/stamping/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      103 2023-02-02 09:58:18.000000 celery-5.3.0rc2/examples/stamping/config.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1358 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/examples.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1806 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/myapp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2548 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/revoke_example.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3311 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2410 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/visitors.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/tutorial/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/tutorial/tasks.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.439766 celery-5.3.0rc2/extra/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/extra/bash-completion/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      636 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/bash-completion/celery.bash
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/extra/generic-init.d/
+-rwxrwxr-x   0 asif      (1000) asif      (1000)     9068 2022-08-01 10:53:57.000000 celery-5.3.0rc2/extra/generic-init.d/celerybeat
+-rwxrwxr-x   0 asif      (1000) asif      (1000)    10813 2023-05-31 06:35:53.000000 celery-5.3.0rc2/extra/generic-init.d/celeryd
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/extra/macOS/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/macOS/org.celeryq.beat.plist
+-rw-rw-r--   0 asif      (1000) asif      (1000)      757 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/macOS/org.celeryq.worker.plist
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/extra/supervisord/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      134 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/supervisord/celery.sh
+-rw-rw-r--   0 asif      (1000) asif      (1000)      699 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/supervisord/celerybeat.conf
+-rw-rw-r--   0 asif      (1000) asif      (1000)      949 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/supervisord/celeryd.conf
+-rw-rw-r--   0 asif      (1000) asif      (1000)      982 2023-02-02 09:58:18.000000 celery-5.3.0rc2/extra/supervisord/supervisord.conf
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/extra/systemd/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      506 2022-08-01 10:53:57.000000 celery-5.3.0rc2/extra/systemd/celery.conf
+-rw-rw-r--   0 asif      (1000) asif      (1000)      740 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/systemd/celery.service
+-rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/systemd/celery.tmpfiles
+-rw-rw-r--   0 asif      (1000) asif      (1000)      395 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/systemd/celerybeat.service
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/extra/zsh-completion/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6244 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/zsh-completion/celery.zsh
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1216 2023-05-31 06:35:53.000000 celery-5.3.0rc2/pyproject.toml
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/requirements/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1454 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      276 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/default.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/requirements/deps/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/deps/mock.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      151 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/dev.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      187 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/docs.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.515767 celery-5.3.0rc2/requirements/extras/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       16 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/arangodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       21 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/auth.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       28 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/azureblockblob.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/brotli.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       28 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/cassandra.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       22 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/consul.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.0rc2/requirements/extras/cosmosdbsql.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      119 2021-12-29 05:20:59.000000 celery-5.3.0rc2/requirements/extras/couchbase.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/couchdb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/django.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       14 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/dynamodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-03-18 11:40:50.000000 celery-5.3.0rc2/requirements/extras/elasticsearch.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       40 2021-11-21 13:37:38.000000 celery-5.3.0rc2/requirements/extras/eventlet.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-11-21 13:37:38.000000 celery-5.3.0rc2/requirements/extras/gevent.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/librabbitmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       45 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/extras/memcache.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.0rc2/requirements/extras/mongodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/msgpack.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-04-28 06:12:03.000000 celery-5.3.0rc2/requirements/extras/pymemcache.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/pyro.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       21 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/pytest.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/redis.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       16 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/s3.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/slmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       53 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/solar.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/sphinxautobuild.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       24 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/sqlalchemy.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       21 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/sqs.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       73 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/tblib.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       39 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/thread.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/yaml.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       14 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/extras/zeromq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/zookeeper.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/zstd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      212 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/pkgutils.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/security.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      175 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/test-ci-base.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      539 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/test-ci-default.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      160 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/test-integration.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       17 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/test-pypy3.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      307 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/test.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      485 2023-05-31 14:55:48.539767 celery-5.3.0rc2/setup.cfg
+-rwxrwxr-x   0 asif      (1000) asif      (1000)     4509 2023-05-31 06:54:18.000000 celery-5.3.0rc2/setup.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.515767 celery-5.3.0rc2/t/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.515767 celery-5.3.0rc2/t/benchmarks/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2816 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/benchmarks/bench_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/integration/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/integration/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2350 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/integration/conftest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12427 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/integration/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1120 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/integration/test_backend.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)   132248 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/integration/test_canvas.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7796 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/integration/test_inspect.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3459 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/integration/test_security.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18656 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/integration/test_tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      688 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/integration/test_worker.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/integration/test_worker_config.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/skip.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/unit/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/unit/app/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13768 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1338 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_annotations.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    41390 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/app/test_app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4542 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_backends.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    29065 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/app/test_beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5528 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_builtins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      356 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    19105 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1608 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_defaults.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      801 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_exceptions.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8823 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_loaders.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11820 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2349 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_registry.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8026 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_routes.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    37835 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/app/test_schedules.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1790 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_utils.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/unit/apps/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/apps/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16234 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/apps/test_multi.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/backends/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/backends/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4362 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_arangodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6874 2021-11-21 13:37:38.000000 celery-5.3.0rc2/t/unit/backends/test_asynchronous.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6794 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_azureblockblob.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    45945 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/backends/test_base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10318 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_cache.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8669 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_cassandra.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1448 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4994 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_cosmosdbsql.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4846 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_couchbase.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3971 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_couchdb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15087 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/backends/test_database.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    19214 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_dynamodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32601 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_elasticsearch.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4435 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28352 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/backends/test_mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    50595 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3692 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_rpc.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6654 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/backends/test_s3.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/bin/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/celery.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/bin/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       64 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      121 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/unit/bin/proj/app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       22 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/bin/proj/app2.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      109 2022-07-28 12:22:51.000000 celery-5.3.0rc2/t/unit/bin/proj/scheduler.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1116 2022-07-28 12:22:51.000000 celery-5.3.0rc2/t/unit/bin/test_beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/test_multi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      529 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/unit/bin/test_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/concurrency/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/concurrency/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5687 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_concurrency.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4721 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_eventlet.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3146 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_gevent.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1837 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_pool.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16398 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/concurrency/test_prefork.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      848 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/concurrency/test_solo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      728 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/concurrency/test_thread.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    23214 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/conftest.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/contrib/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/contrib/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      183 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/conf.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       93 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/contents.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/foo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      113 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/xyzzy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1394 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/contrib/test_abortable.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10615 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/contrib/test_migrate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      785 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/test_pytest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3146 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/test_rdb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      731 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/contrib/test_sphinx.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1474 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/contrib/test_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/events/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/events/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2304 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/events/test_cursesmon.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11372 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/events/test_events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3359 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/events/test_snapshot.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    22261 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/events/test_state.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/fixups/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/fixups/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11013 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/fixups/test_django.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.531767 celery-5.3.0rc2/t/unit/security/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7344 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      109 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/case.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3333 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/test_certificate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1570 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/test_key.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6219 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/test_security.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2224 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/security/test_serialization.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.531767 celery-5.3.0rc2/t/unit/tasks/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/tasks/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    68472 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_canvas.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12308 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_chord.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3134 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/unit/tasks/test_context.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34984 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/tasks/test_result.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    52722 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_stamping.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/tasks/test_states.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    56857 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21991 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/tasks/test_trace.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/tasks/unit_tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      989 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/test_canvas.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.535767 celery-5.3.0rc2/t/unit/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12855 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_collections.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2357 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1739 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_deprecated.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5233 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_dispatcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13576 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_graph.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3272 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/utils/test_imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8515 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_local.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      202 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_nodenames.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      172 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1386 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_pickle.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32949 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_platforms.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5555 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_saferepr.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3219 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/utils/test_serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_sysinfo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1734 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_term.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/utils/test_text.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2427 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/utils/test_threads.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11465 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/utils/test_time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3215 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_timer2.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      624 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_utils.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.539767 celery-5.3.0rc2/t/unit/worker/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/worker/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7574 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_autoscale.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9415 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_bootsteps.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2461 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_components.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    30428 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_consumer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28334 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/worker/test_control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2384 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/worker/test_heartbeat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18256 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_loops.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    48131 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/worker/test_request.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      238 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/worker/test_revoke.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6339 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/worker/test_state.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10989 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_strategy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    39912 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_worker.py
```

### Comparing `celery-5.3.0rc1/CONTRIBUTORS.txt` & `celery-5.3.0rc2/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/LICENSE` & `celery-5.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/MANIFEST.in` & `celery-5.3.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/PKG-INFO` & `celery-5.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.3.0rc1
+Version: 5.3.0rc2
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
@@ -16,61 +16,59 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Framework :: Celery
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Provides-Extra: redis
-Provides-Extra: sqs
-Provides-Extra: zstd
-Provides-Extra: pymemcache
-Provides-Extra: sqlalchemy
-Provides-Extra: memcache
 Provides-Extra: arangodb
 Provides-Extra: auth
-Provides-Extra: slmq
-Provides-Extra: dynamodb
-Provides-Extra: yaml
-Provides-Extra: s3
-Provides-Extra: librabbitmq
-Provides-Extra: gevent
-Provides-Extra: tblib
-Provides-Extra: pytest
-Provides-Extra: elasticsearch
-Provides-Extra: cassandra
+Provides-Extra: azureblockblob
 Provides-Extra: brotli
-Provides-Extra: pyro
-Provides-Extra: mongodb
+Provides-Extra: cassandra
+Provides-Extra: consul
+Provides-Extra: cosmosdbsql
 Provides-Extra: couchbase
-Provides-Extra: eventlet
 Provides-Extra: couchdb
-Provides-Extra: solar
-Provides-Extra: msgpack
-Provides-Extra: cosmosdbsql
 Provides-Extra: django
-Provides-Extra: consul
-Provides-Extra: azureblockblob
+Provides-Extra: dynamodb
+Provides-Extra: elasticsearch
+Provides-Extra: eventlet
+Provides-Extra: gevent
+Provides-Extra: librabbitmq
+Provides-Extra: memcache
+Provides-Extra: mongodb
+Provides-Extra: msgpack
+Provides-Extra: pymemcache
+Provides-Extra: pyro
+Provides-Extra: pytest
+Provides-Extra: redis
+Provides-Extra: s3
+Provides-Extra: slmq
+Provides-Extra: solar
+Provides-Extra: sqlalchemy
+Provides-Extra: sqs
+Provides-Extra: tblib
+Provides-Extra: yaml
 Provides-Extra: zookeeper
+Provides-Extra: zstd
 License-File: LICENSE
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0rc1 (dawn-chorus)
+:Version: 5.3.0rc2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -120,16 +118,16 @@
 .. _rusty-celery: https://github.com/rusty-celery/rusty-celery
 
 What do I need?
 ===============
 
 Celery version 5.3.0a1 runs on,
 
-- Python (3.7, 3.8, 3.9, 3.10)
-- PyPy3.7 (7.3.7+)
+- Python (3.8, 3.9, 3.10)
+- PyPy3.8+ (v7.3.11+)
 
 
 This is the version of celery which will support Python 3.7 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
@@ -602,7 +600,9 @@
 .. |ocsponsorbadge| image:: https://opencollective.com/celery/sponsors/badge.svg
     :alt: Sponsors on Open Collective
     :target: #sponsors
 
 .. |downloads| image:: https://pepy.tech/badge/celery
     :alt: Downloads
     :target: https://pepy.tech/project/celery
+
+
```

### Comparing `celery-5.3.0rc1/README.rst` & `celery-5.3.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0rc1 (dawn-chorus)
+:Version: 5.3.0rc2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -56,16 +56,16 @@
 .. _rusty-celery: https://github.com/rusty-celery/rusty-celery
 
 What do I need?
 ===============
 
 Celery version 5.3.0a1 runs on,
 
-- Python (3.7, 3.8, 3.9, 3.10)
-- PyPy3.7 (7.3.7+)
+- Python (3.8, 3.9, 3.10)
+- PyPy3.8+ (v7.3.11+)
 
 
 This is the version of celery which will support Python 3.7 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
```

### Comparing `celery-5.3.0rc1/celery/__init__.py` & `celery-5.3.0rc2/celery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from collections import namedtuple
 
 # Lazy loading
 from . import local
 
 SERIES = 'dawn-chorus'
 
-__version__ = '5.3.0rc1'
+__version__ = '5.3.0rc2'
 __author__ = 'Ask Solem'
 __contact__ = 'auvipy@gmail.com'
 __homepage__ = 'https://docs.celeryq.dev/'
 __docformat__ = 'restructuredtext'
 __keywords__ = 'task job queue distributed messaging actor'
 
 # -eof meta-
```

### Comparing `celery-5.3.0rc1/celery/_state.py` & `celery-5.3.0rc2/celery/_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/__init__.py` & `celery-5.3.0rc2/celery/app/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/amqp.py` & `celery-5.3.0rc2/celery/app/amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/annotations.py` & `celery-5.3.0rc2/celery/app/annotations.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/autoretry.py` & `celery-5.3.0rc2/celery/app/autoretry.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/backends.py` & `celery-5.3.0rc2/celery/app/backends.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/base.py` & `celery-5.3.0rc2/celery/app/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/builtins.py` & `celery-5.3.0rc2/celery/app/builtins.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/control.py` & `celery-5.3.0rc2/celery/app/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/defaults.py` & `celery-5.3.0rc2/celery/app/defaults.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/events.py` & `celery-5.3.0rc2/celery/app/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/log.py` & `celery-5.3.0rc2/celery/app/log.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/registry.py` & `celery-5.3.0rc2/celery/app/registry.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/routes.py` & `celery-5.3.0rc2/celery/app/routes.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/task.py` & `celery-5.3.0rc2/celery/app/task.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/app/trace.py` & `celery-5.3.0rc2/celery/app/trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
         exc = get_pickleable_exception(orig_exc)
         if exc.__traceback__ is None:
             # `get_pickleable_exception` may have created a new exception without
             # a traceback.
             _, _, exc.__traceback__ = sys.exc_info()
 
-        exc_type = get_pickleable_etype(orig_exc)
+        exc_type = get_pickleable_etype(type(orig_exc))
 
         # make sure we only send pickleable exceptions back to parent.
         einfo = ExceptionInfo(exc_info=(exc_type, exc, exc.__traceback__))
 
         task.backend.mark_as_failure(
             req.id, exc, einfo.traceback,
             request=req, store_result=store_errors,
```

### Comparing `celery-5.3.0rc1/celery/app/utils.py` & `celery-5.3.0rc2/celery/app/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/apps/beat.py` & `celery-5.3.0rc2/celery/apps/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/apps/multi.py` & `celery-5.3.0rc2/celery/apps/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/apps/worker.py` & `celery-5.3.0rc2/celery/apps/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/arangodb.py` & `celery-5.3.0rc2/celery/backends/arangodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/asynchronous.py` & `celery-5.3.0rc2/celery/backends/asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/azureblockblob.py` & `celery-5.3.0rc2/celery/backends/azureblockblob.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/base.py` & `celery-5.3.0rc2/celery/backends/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/cache.py` & `celery-5.3.0rc2/celery/backends/cache.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/cassandra.py` & `celery-5.3.0rc2/celery/backends/cassandra.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/consul.py` & `celery-5.3.0rc2/celery/backends/consul.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/cosmosdbsql.py` & `celery-5.3.0rc2/celery/backends/cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/couchbase.py` & `celery-5.3.0rc2/celery/backends/couchbase.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/couchdb.py` & `celery-5.3.0rc2/celery/backends/couchdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/database/__init__.py` & `celery-5.3.0rc2/celery/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/database/models.py` & `celery-5.3.0rc2/celery/backends/database/models.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/database/session.py` & `celery-5.3.0rc2/celery/backends/database/session.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/dynamodb.py` & `celery-5.3.0rc2/celery/backends/dynamodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/elasticsearch.py` & `celery-5.3.0rc2/celery/backends/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/filesystem.py` & `celery-5.3.0rc2/celery/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/mongodb.py` & `celery-5.3.0rc2/celery/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/redis.py` & `celery-5.3.0rc2/celery/backends/redis.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/rpc.py` & `celery-5.3.0rc2/celery/backends/rpc.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/backends/s3.py` & `celery-5.3.0rc2/celery/backends/s3.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/beat.py` & `celery-5.3.0rc2/celery/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/amqp.py` & `celery-5.3.0rc2/celery/bin/amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/base.py` & `celery-5.3.0rc2/celery/bin/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/beat.py` & `celery-5.3.0rc2/celery/bin/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/call.py` & `celery-5.3.0rc2/celery/bin/call.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/celery.py` & `celery-5.3.0rc2/celery/bin/celery.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/control.py` & `celery-5.3.0rc2/celery/bin/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/events.py` & `celery-5.3.0rc2/celery/bin/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/graph.py` & `celery-5.3.0rc2/celery/bin/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/list.py` & `celery-5.3.0rc2/celery/bin/list.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/logtool.py` & `celery-5.3.0rc2/celery/bin/logtool.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/migrate.py` & `celery-5.3.0rc2/celery/bin/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/multi.py` & `celery-5.3.0rc2/celery/bin/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/purge.py` & `celery-5.3.0rc2/celery/bin/purge.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/result.py` & `celery-5.3.0rc2/celery/bin/result.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/shell.py` & `celery-5.3.0rc2/celery/bin/shell.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/upgrade.py` & `celery-5.3.0rc2/celery/bin/upgrade.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bin/worker.py` & `celery-5.3.0rc2/celery/bin/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/bootsteps.py` & `celery-5.3.0rc2/celery/bootsteps.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/canvas.py` & `celery-5.3.0rc2/celery/canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/__init__.py` & `celery-5.3.0rc2/celery/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/asynpool.py` & `celery-5.3.0rc2/celery/concurrency/asynpool.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/base.py` & `celery-5.3.0rc2/celery/concurrency/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/eventlet.py` & `celery-5.3.0rc2/celery/concurrency/eventlet.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/gevent.py` & `celery-5.3.0rc2/celery/concurrency/gevent.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/prefork.py` & `celery-5.3.0rc2/celery/concurrency/prefork.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/solo.py` & `celery-5.3.0rc2/celery/concurrency/solo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/concurrency/thread.py` & `celery-5.3.0rc2/celery/concurrency/thread.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/abortable.py` & `celery-5.3.0rc2/celery/contrib/abortable.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/migrate.py` & `celery-5.3.0rc2/celery/contrib/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/pytest.py` & `celery-5.3.0rc2/celery/contrib/pytest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/rdb.py` & `celery-5.3.0rc2/celery/contrib/rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/sphinx.py` & `celery-5.3.0rc2/celery/contrib/sphinx.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/testing/app.py` & `celery-5.3.0rc2/celery/contrib/testing/app.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/testing/manager.py` & `celery-5.3.0rc2/celery/contrib/testing/manager.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/testing/mocks.py` & `celery-5.3.0rc2/celery/contrib/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/contrib/testing/worker.py` & `celery-5.3.0rc2/celery/contrib/testing/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/events/cursesmon.py` & `celery-5.3.0rc2/celery/events/cursesmon.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/events/dispatcher.py` & `celery-5.3.0rc2/celery/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/events/dumper.py` & `celery-5.3.0rc2/celery/events/dumper.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/events/event.py` & `celery-5.3.0rc2/celery/events/event.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/events/receiver.py` & `celery-5.3.0rc2/celery/events/receiver.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/events/snapshot.py` & `celery-5.3.0rc2/celery/events/snapshot.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/events/state.py` & `celery-5.3.0rc2/celery/events/state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/exceptions.py` & `celery-5.3.0rc2/celery/exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/fixups/django.py` & `celery-5.3.0rc2/celery/fixups/django.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/loaders/base.py` & `celery-5.3.0rc2/celery/loaders/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/loaders/default.py` & `celery-5.3.0rc2/celery/loaders/default.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/local.py` & `celery-5.3.0rc2/celery/local.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/platforms.py` & `celery-5.3.0rc2/celery/platforms.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/result.py` & `celery-5.3.0rc2/celery/result.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/schedules.py` & `celery-5.3.0rc2/celery/schedules.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/security/__init__.py` & `celery-5.3.0rc2/celery/security/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/security/certificate.py` & `celery-5.3.0rc2/celery/security/certificate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/security/key.py` & `celery-5.3.0rc2/celery/security/key.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/security/serialization.py` & `celery-5.3.0rc2/celery/security/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/security/utils.py` & `celery-5.3.0rc2/celery/security/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/signals.py` & `celery-5.3.0rc2/celery/signals.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/states.py` & `celery-5.3.0rc2/celery/states.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/__init__.py` & `celery-5.3.0rc2/celery/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/abstract.py` & `celery-5.3.0rc2/celery/utils/abstract.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/collections.py` & `celery-5.3.0rc2/celery/utils/collections.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/debug.py` & `celery-5.3.0rc2/celery/utils/debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/deprecated.py` & `celery-5.3.0rc2/celery/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/dispatch/signal.py` & `celery-5.3.0rc2/celery/utils/dispatch/signal.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/functional.py` & `celery-5.3.0rc2/celery/utils/functional.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/graph.py` & `celery-5.3.0rc2/celery/utils/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/imports.py` & `celery-5.3.0rc2/celery/utils/imports.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/iso8601.py` & `celery-5.3.0rc2/celery/utils/iso8601.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/log.py` & `celery-5.3.0rc2/celery/utils/log.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/nodenames.py` & `celery-5.3.0rc2/celery/utils/nodenames.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/objects.py` & `celery-5.3.0rc2/celery/utils/objects.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/saferepr.py` & `celery-5.3.0rc2/celery/utils/saferepr.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/serialization.py` & `celery-5.3.0rc2/celery/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/static/celery_128.png` & `celery-5.3.0rc2/celery/utils/static/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/sysinfo.py` & `celery-5.3.0rc2/celery/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/term.py` & `celery-5.3.0rc2/celery/utils/term.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/text.py` & `celery-5.3.0rc2/celery/utils/text.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/threads.py` & `celery-5.3.0rc2/celery/utils/threads.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/time.py` & `celery-5.3.0rc2/celery/utils/time.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/utils/timer2.py` & `celery-5.3.0rc2/celery/utils/timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/autoscale.py` & `celery-5.3.0rc2/celery/worker/autoscale.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/components.py` & `celery-5.3.0rc2/celery/worker/components.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/agent.py` & `celery-5.3.0rc2/celery/worker/consumer/agent.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/connection.py` & `celery-5.3.0rc2/celery/worker/consumer/connection.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/consumer.py` & `celery-5.3.0rc2/celery/worker/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/control.py` & `celery-5.3.0rc2/celery/worker/consumer/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/events.py` & `celery-5.3.0rc2/celery/worker/consumer/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/gossip.py` & `celery-5.3.0rc2/celery/worker/consumer/gossip.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/heart.py` & `celery-5.3.0rc2/celery/worker/consumer/heart.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/mingle.py` & `celery-5.3.0rc2/celery/worker/consumer/mingle.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/consumer/tasks.py` & `celery-5.3.0rc2/celery/worker/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/control.py` & `celery-5.3.0rc2/celery/worker/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Worker remote control command implementations."""
 import io
 import tempfile
-import warnings
-from collections import UserDict, namedtuple
+from collections import UserDict, defaultdict, namedtuple
 
 from billiard.common import TERM_SIGNAME
 from kombu.utils.encoding import safe_repr
 
-from celery.exceptions import CeleryWarning, WorkerShutdown
+from celery.exceptions import WorkerShutdown
 from celery.platforms import signals as _signals
 from celery.utils.functional import maybe_list
 from celery.utils.log import get_logger
 from celery.utils.serialization import jsonify, strtobool
 from celery.utils.time import rate
 
 from . import state as worker_state
@@ -157,62 +156,62 @@
     variadic='headers',
     signature='[key1=value1 [key2=value2 [... [keyN=valueN]]]]',
 )
 def revoke_by_stamped_headers(state, headers, terminate=False, signal=None, **kwargs):
     """Revoke task by header (or list of headers).
 
     Keyword Arguments:
+        headers(dictionary): Dictionary that contains stamping scheme name as keys and stamps as values.
+                             If headers is a list, it will be converted to a dictionary.
         terminate (bool): Also terminate the process if the task is active.
         signal (str): Name of signal to use for terminate (e.g., ``KILL``).
+    Sample headers input:
+        {'mtask_id': [id1, id2, id3]}
     """
     # pylint: disable=redefined-outer-name
     # XXX Note that this redefines `terminate`:
     #     Outside of this scope that is a function.
     # supports list argument since 3.1
+    signum = _signals.signum(signal or TERM_SIGNAME)
+
     if isinstance(headers, list):
         headers = {h.split('=')[0]: h.split('=')[1] for h in headers}
 
-    worker_state.revoked_stamps.update(headers)
+    for header, stamps in headers.items():
+        updated_stamps = maybe_list(worker_state.revoked_stamps.get(header) or []) + list(maybe_list(stamps))
+        worker_state.revoked_stamps[header] = updated_stamps
 
     if not terminate:
-        return ok(f'headers {headers} flagged as revoked')
+        return ok(f'headers {headers} flagged as revoked, but not terminated')
 
-    task_ids = set()
     active_requests = list(worker_state.active_requests)
 
+    terminated_scheme_to_stamps_mapping = defaultdict(set)
+
     # Terminate all running tasks of matching headers
-    if active_requests:
-        warnings.warn(
-            "Terminating tasks by headers does not scale well when worker concurrency is high",
-            CeleryWarning
-        )
-
-        # Go through all active requests, and check if one of the
-        # requests has a stamped header that matches the given headers to revoke
-
-        req: Request
-        for req in active_requests:
-            # Check stamps exist
-            if req.stamped_headers and req.stamps:
-                # if so, check if any of the stamped headers match the given headers
-                for expected_header_key, expected_header_value in headers.items():
-                    if expected_header_key in req.stamps:
-                        actual_header = req.stamps[expected_header_key]
-                        # Check any possible match regardless if the stamps are a sequence or not
-                        if any([
-                            header in maybe_list(expected_header_value)
-                            for header in maybe_list(actual_header)
-                        ]):
-                            task_ids.add(req.task_id)
-                            continue
+    # Go through all active requests, and check if one of the
+    # requests has a stamped header that matches the given headers to revoke
 
-    task_ids = _revoke(state, task_ids, terminate, signal, **kwargs)
-    if isinstance(task_ids, dict):
-        return task_ids
-    return ok(list(task_ids))
+    for req in active_requests:
+        # Check stamps exist
+        if hasattr(req, "stamps") and req.stamps:
+            # if so, check if any stamps match a revoked stamp
+            for expected_header_key, expected_header_value in headers.items():
+                if expected_header_key in req.stamps:
+                    expected_header_value = maybe_list(expected_header_value)
+                    actual_header = maybe_list(req.stamps[expected_header_key])
+                    matching_stamps_for_request = set(actual_header) & set(expected_header_value)
+                    # Check any possible match regardless if the stamps are a sequence or not
+                    if matching_stamps_for_request:
+                        terminated_scheme_to_stamps_mapping[expected_header_key].update(matching_stamps_for_request)
+                        req.terminate(state.consumer.pool, signal=signum)
+
+    if not terminated_scheme_to_stamps_mapping:
+        return ok(f'headers {headers} were not terminated')
+    return ok(f'headers {terminated_scheme_to_stamps_mapping} revoked')
 
 
 def _revoke(state, task_ids, terminate=False, signal=None, **kwargs):
     size = len(task_ids)
     terminated = set()
 
     worker_state.revoked.update(task_ids)
```

### Comparing `celery-5.3.0rc1/celery/worker/heartbeat.py` & `celery-5.3.0rc2/celery/worker/heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/loops.py` & `celery-5.3.0rc2/celery/worker/loops.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/pidbox.py` & `celery-5.3.0rc2/celery/worker/pidbox.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/request.py` & `celery-5.3.0rc2/celery/worker/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,19 +319,20 @@
 
     @property
     def groups(self):
         return self._request_dict.get('groups', [])
 
     @property
     def stamped_headers(self) -> list:
-        return self._request_dict.get('stamped_headers', [])
+        return self._request_dict.get('stamped_headers') or []
 
     @property
     def stamps(self) -> dict:
-        return {header: self._request_dict['stamps'][header] for header in self.stamped_headers}
+        stamps = self._request_dict.get('stamps') or {}
+        return {header: stamps.get(header) for header in self.stamped_headers}
 
     @property
     def correlation_id(self):
         # used similarly to reply_to
         return self._request_dict['correlation_id']
 
     def execute_using_pool(self, pool: BasePool, **kwargs):
@@ -477,15 +478,18 @@
                     if isinstance(stamped_header, (list, tuple)):
                         for stamped_value in stamped_header:
                             if stamped_value in maybe_list(revoked_header):
                                 revoked_by_header = True
                                 revoking_header = {stamp: stamped_value}
                                 break
                     else:
-                        revoked_by_header = stamped_header in revoked_stamps[stamp]
+                        revoked_by_header = any([
+                            stamped_header in maybe_list(revoked_header),
+                            stamped_header == revoked_header,  # When the header is a single set value
+                        ])
                         revoking_header = {stamp: stamped_header}
                     break
 
         if any((expired, revoked_by_id, revoked_by_header)):
             log_msg = 'Discarding revoked task: %s[%s]'
             if revoked_by_header:
                 log_msg += ' (revoked by header: %s)' % revoking_header
```

### Comparing `celery-5.3.0rc1/celery/worker/state.py` & `celery-5.3.0rc2/celery/worker/state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/strategy.py` & `celery-5.3.0rc2/celery/worker/strategy.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery/worker/worker.py` & `celery-5.3.0rc2/celery/worker/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/celery.egg-info/PKG-INFO` & `celery-5.3.0rc2/celery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.3.0rc1
+Version: 5.3.0rc2
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
@@ -16,61 +16,59 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Framework :: Celery
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Provides-Extra: redis
-Provides-Extra: sqs
-Provides-Extra: zstd
-Provides-Extra: pymemcache
-Provides-Extra: sqlalchemy
-Provides-Extra: memcache
 Provides-Extra: arangodb
 Provides-Extra: auth
-Provides-Extra: slmq
-Provides-Extra: dynamodb
-Provides-Extra: yaml
-Provides-Extra: s3
-Provides-Extra: librabbitmq
-Provides-Extra: gevent
-Provides-Extra: tblib
-Provides-Extra: pytest
-Provides-Extra: elasticsearch
-Provides-Extra: cassandra
+Provides-Extra: azureblockblob
 Provides-Extra: brotli
-Provides-Extra: pyro
-Provides-Extra: mongodb
+Provides-Extra: cassandra
+Provides-Extra: consul
+Provides-Extra: cosmosdbsql
 Provides-Extra: couchbase
-Provides-Extra: eventlet
 Provides-Extra: couchdb
-Provides-Extra: solar
-Provides-Extra: msgpack
-Provides-Extra: cosmosdbsql
 Provides-Extra: django
-Provides-Extra: consul
-Provides-Extra: azureblockblob
+Provides-Extra: dynamodb
+Provides-Extra: elasticsearch
+Provides-Extra: eventlet
+Provides-Extra: gevent
+Provides-Extra: librabbitmq
+Provides-Extra: memcache
+Provides-Extra: mongodb
+Provides-Extra: msgpack
+Provides-Extra: pymemcache
+Provides-Extra: pyro
+Provides-Extra: pytest
+Provides-Extra: redis
+Provides-Extra: s3
+Provides-Extra: slmq
+Provides-Extra: solar
+Provides-Extra: sqlalchemy
+Provides-Extra: sqs
+Provides-Extra: tblib
+Provides-Extra: yaml
 Provides-Extra: zookeeper
+Provides-Extra: zstd
 License-File: LICENSE
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0rc1 (dawn-chorus)
+:Version: 5.3.0rc2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -120,16 +118,16 @@
 .. _rusty-celery: https://github.com/rusty-celery/rusty-celery
 
 What do I need?
 ===============
 
 Celery version 5.3.0a1 runs on,
 
-- Python (3.7, 3.8, 3.9, 3.10)
-- PyPy3.7 (7.3.7+)
+- Python (3.8, 3.9, 3.10)
+- PyPy3.8+ (v7.3.11+)
 
 
 This is the version of celery which will support Python 3.7 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
@@ -602,7 +600,9 @@
 .. |ocsponsorbadge| image:: https://opencollective.com/celery/sponsors/badge.svg
     :alt: Sponsors on Open Collective
     :target: #sponsors
 
 .. |downloads| image:: https://pepy.tech/badge/celery
     :alt: Downloads
     :target: https://pepy.tech/project/celery
+
+
```

### Comparing `celery-5.3.0rc1/celery.egg-info/SOURCES.txt` & `celery-5.3.0rc2/celery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 celery/schedules.py
 celery/signals.py
 celery/states.py
 celery.egg-info/PKG-INFO
 celery.egg-info/SOURCES.txt
 celery.egg-info/dependency_links.txt
 celery.egg-info/entry_points.txt
-celery.egg-info/not-zip-safe
 celery.egg-info/requires.txt
 celery.egg-info/top_level.txt
 celery/app/__init__.py
 celery/app/amqp.py
 celery/app/annotations.py
 celery/app/autoretry.py
 celery/app/backends.py
@@ -414,15 +413,14 @@
 docs/userguide/signals.rst
 docs/userguide/sphinx.rst
 docs/userguide/tasks.rst
 docs/userguide/testing.rst
 docs/userguide/workers.rst
 docs/userguide/concurrency/eventlet.rst
 docs/userguide/concurrency/index.rst
-examples/.DS_Store
 examples/README.rst
 examples/app/myapp.py
 examples/celery_http_gateway/README.rst
 examples/celery_http_gateway/__init__.py
 examples/celery_http_gateway/manage.py
 examples/celery_http_gateway/settings.py
 examples/celery_http_gateway/tasks.py
```

### Comparing `celery-5.3.0rc1/celery.egg-info/requires.txt` & `celery-5.3.0rc2/celery.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 billiard<5.0,>=4.1.0
-kombu<6.0,>=5.3.0b3
-vine<6.0,>=5.0.0
-click<9.0,>=8.1.2
 click-didyoumean>=0.3.0
-click-repl>=0.2.0
 click-plugins>=1.1.1
+click-repl>=0.2.0
+click<9.0,>=8.1.2
+kombu<6.0,>=5.3.0rc2
+python-dateutil>=2.8.2
 tzdata>=2022.7
+vine<6.0,>=5.0.0
 
 [:python_version < "3.8"]
 importlib-metadata>=3.6
 
 [:python_version < "3.9"]
 backports.zoneinfo>=0.2.1
 
 [arangodb]
 pyArango>=2.0.1
 
 [auth]
-cryptography==40.0.1
+cryptography==40.0.2
 
 [azureblockblob]
 azure-storage-blob>=12.15.0
 
 [brotli]
 
 [brotli:platform_python_implementation == "CPython"]
@@ -78,38 +79,38 @@
 [msgpack]
 msgpack==1.0.5
 
 [pymemcache]
 python-memcached==1.59
 
 [pyro]
-pyro5
+pyro4
 
 [pytest]
 pytest-celery==0.0.0
 
 [redis]
-redis<4.4.0,>=4.3.6
+redis>=4.5.2
 
 [s3]
-boto3==1.26.110
+boto3>=1.26.139
 
 [slmq]
 softlayer_messaging>=1.0.3
 
 [solar]
 
 [solar:platform_python_implementation != "PyPy"]
 ephem==4.1.4
 
 [sqlalchemy]
-sqlalchemy<2.0,>=1.4.47
+sqlalchemy<2.1,>=1.4.48
 
 [sqs]
-kombu[sqs]~=5.3.0b3
+kombu[sqs]>=5.3.0rc2
 
 [tblib]
 
 [tblib:python_version < "3.8.0"]
 tblib>=1.3.0
 
 [tblib:python_version >= "3.8.0"]
@@ -118,8 +119,8 @@
 [yaml]
 PyYAML>=3.10
 
 [zookeeper]
 kazoo>=1.3.1
 
 [zstd]
-zstandard==0.20.0
+zstandard==0.21.0
```

### Comparing `celery-5.3.0rc1/docs/AUTHORS.txt` & `celery-5.3.0rc2/docs/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/Makefile` & `celery-5.3.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/_ext/celerydocs.py` & `celery-5.3.0rc2/docs/_ext/celerydocs.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/community.rst` & `celery-5.3.0rc2/docs/community.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/conf.py` & `celery-5.3.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/copyright.rst` & `celery-5.3.0rc2/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/django/first-steps-with-django.rst` & `celery-5.3.0rc2/docs/django/first-steps-with-django.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/faq.rst` & `celery-5.3.0rc2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/getting-started/backends-and-brokers/index.rst` & `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/getting-started/backends-and-brokers/rabbitmq.rst` & `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/rabbitmq.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/getting-started/backends-and-brokers/redis.rst` & `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/redis.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/getting-started/backends-and-brokers/sqs.rst` & `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/sqs.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/getting-started/first-steps-with-celery.rst` & `celery-5.3.0rc2/docs/getting-started/first-steps-with-celery.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/getting-started/introduction.rst` & `celery-5.3.0rc2/docs/getting-started/introduction.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/getting-started/next-steps.rst` & `celery-5.3.0rc2/docs/getting-started/next-steps.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/glossary.rst` & `celery-5.3.0rc2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-1.0.rst` & `celery-5.3.0rc2/docs/history/changelog-1.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-2.0.rst` & `celery-5.3.0rc2/docs/history/changelog-2.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-2.1.rst` & `celery-5.3.0rc2/docs/history/changelog-2.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-2.2.rst` & `celery-5.3.0rc2/docs/history/changelog-2.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-2.3.rst` & `celery-5.3.0rc2/docs/history/changelog-2.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-2.4.rst` & `celery-5.3.0rc2/docs/history/changelog-2.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-2.5.rst` & `celery-5.3.0rc2/docs/history/changelog-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-3.0.rst` & `celery-5.3.0rc2/docs/history/changelog-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-3.1.rst` & `celery-5.3.0rc2/docs/history/changelog-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-4.0.rst` & `celery-5.3.0rc2/docs/history/changelog-4.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-4.1.rst` & `celery-5.3.0rc2/docs/history/changelog-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-4.2.rst` & `celery-5.3.0rc2/docs/history/changelog-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-4.3.rst` & `celery-5.3.0rc2/docs/history/changelog-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-4.4.rst` & `celery-5.3.0rc2/docs/history/changelog-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-5.0.rst` & `celery-5.3.0rc2/docs/history/changelog-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/changelog-5.1.rst` & `celery-5.3.0rc2/docs/history/changelog-5.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/index.rst` & `celery-5.3.0rc2/docs/history/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-2.5.rst` & `celery-5.3.0rc2/docs/history/whatsnew-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-3.0.rst` & `celery-5.3.0rc2/docs/history/whatsnew-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-3.1.rst` & `celery-5.3.0rc2/docs/history/whatsnew-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-4.0.rst` & `celery-5.3.0rc2/docs/history/whatsnew-4.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-4.1.rst` & `celery-5.3.0rc2/docs/history/whatsnew-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-4.2.rst` & `celery-5.3.0rc2/docs/history/whatsnew-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-4.3.rst` & `celery-5.3.0rc2/docs/history/whatsnew-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-4.4.rst` & `celery-5.3.0rc2/docs/history/whatsnew-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-5.0.rst` & `celery-5.3.0rc2/docs/history/whatsnew-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/history/whatsnew-5.1.rst` & `celery-5.3.0rc2/docs/history/whatsnew-5.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/celery-banner-small.png` & `celery-5.3.0rc2/docs/images/celery-banner-small.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/celery-banner.png` & `celery-5.3.0rc2/docs/images/celery-banner.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/celery_128.png` & `celery-5.3.0rc2/docs/images/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/celery_512.png` & `celery-5.3.0rc2/docs/images/celery_512.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/celeryevshotsm.jpg` & `celery-5.3.0rc2/docs/images/celeryevshotsm.jpg`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/dashboard.png` & `celery-5.3.0rc2/docs/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/favicon.ico` & `celery-5.3.0rc2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/monitor.png` & `celery-5.3.0rc2/docs/images/monitor.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/result_graph.png` & `celery-5.3.0rc2/docs/images/result_graph.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/images/worker_graph_full.png` & `celery-5.3.0rc2/docs/images/worker_graph_full.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/includes/installation.txt` & `celery-5.3.0rc2/docs/includes/installation.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/includes/introduction.txt` & `celery-5.3.0rc2/docs/includes/introduction.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:Version: 5.3.0rc1 (dawn-chorus)
+:Version: 5.3.0rc2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 --
```

### Comparing `celery-5.3.0rc1/docs/includes/resources.txt` & `celery-5.3.0rc2/docs/includes/resources.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/index.rst` & `celery-5.3.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/internals/app-overview.rst` & `celery-5.3.0rc2/docs/internals/app-overview.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/internals/deprecation.rst` & `celery-5.3.0rc2/docs/internals/deprecation.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/internals/guide.rst` & `celery-5.3.0rc2/docs/internals/guide.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/internals/protocol.rst` & `celery-5.3.0rc2/docs/internals/protocol.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/internals/reference/index.rst` & `celery-5.3.0rc2/docs/internals/reference/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/internals/worker.rst` & `celery-5.3.0rc2/docs/internals/worker.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/make.bat` & `celery-5.3.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/reference/celery.app.amqp.rst` & `celery-5.3.0rc2/docs/reference/celery.app.amqp.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/reference/celery.rst` & `celery-5.3.0rc2/docs/reference/celery.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/reference/celery.utils.debug.rst` & `celery-5.3.0rc2/docs/reference/celery.utils.debug.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/reference/index.rst` & `celery-5.3.0rc2/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/sec/CELERYSA-0001.txt` & `celery-5.3.0rc2/docs/sec/CELERYSA-0001.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/sec/CELERYSA-0002.txt` & `celery-5.3.0rc2/docs/sec/CELERYSA-0002.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/sec/CELERYSA-0003.txt` & `celery-5.3.0rc2/docs/sec/CELERYSA-0003.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/spelling_wordlist.txt` & `celery-5.3.0rc2/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/templates/readme.txt` & `celery-5.3.0rc2/docs/templates/readme.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/tutorials/task-cookbook.rst` & `celery-5.3.0rc2/docs/tutorials/task-cookbook.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/application.rst` & `celery-5.3.0rc2/docs/userguide/application.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/calling.rst` & `celery-5.3.0rc2/docs/userguide/calling.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/canvas.rst` & `celery-5.3.0rc2/docs/userguide/canvas.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/concurrency/eventlet.rst` & `celery-5.3.0rc2/docs/userguide/concurrency/eventlet.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/configuration.rst` & `celery-5.3.0rc2/docs/userguide/configuration.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/daemonizing.rst` & `celery-5.3.0rc2/docs/userguide/daemonizing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/debugging.rst` & `celery-5.3.0rc2/docs/userguide/debugging.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/extending.rst` & `celery-5.3.0rc2/docs/userguide/extending.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/monitoring.rst` & `celery-5.3.0rc2/docs/userguide/monitoring.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/optimizing.rst` & `celery-5.3.0rc2/docs/userguide/optimizing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/periodic-tasks.rst` & `celery-5.3.0rc2/docs/userguide/periodic-tasks.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/routing.rst` & `celery-5.3.0rc2/docs/userguide/routing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/security.rst` & `celery-5.3.0rc2/docs/userguide/security.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/signals.rst` & `celery-5.3.0rc2/docs/userguide/signals.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/tasks.rst` & `celery-5.3.0rc2/docs/userguide/tasks.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/testing.rst` & `celery-5.3.0rc2/docs/userguide/testing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/userguide/workers.rst` & `celery-5.3.0rc2/docs/userguide/workers.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/docs/whatsnew-5.2.rst` & `celery-5.3.0rc2/docs/whatsnew-5.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/app/myapp.py` & `celery-5.3.0rc2/examples/app/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/celery_http_gateway/README.rst` & `celery-5.3.0rc2/examples/celery_http_gateway/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/celery_http_gateway/settings.py` & `celery-5.3.0rc2/examples/celery_http_gateway/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/celery_http_gateway/urls.py` & `celery-5.3.0rc2/examples/celery_http_gateway/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/django/README.rst` & `celery-5.3.0rc2/examples/django/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/django/proj/celery.py` & `celery-5.3.0rc2/examples/django/proj/celery.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/django/proj/settings.py` & `celery-5.3.0rc2/examples/django/proj/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/django/proj/urls.py` & `celery-5.3.0rc2/examples/django/proj/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/django/proj/wsgi.py` & `celery-5.3.0rc2/examples/django/proj/wsgi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/eventlet/README.rst` & `celery-5.3.0rc2/examples/eventlet/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/eventlet/bulk_task_producer.py` & `celery-5.3.0rc2/examples/eventlet/bulk_task_producer.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/eventlet/webcrawler.py` & `celery-5.3.0rc2/examples/eventlet/webcrawler.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/next-steps/setup.py` & `celery-5.3.0rc2/examples/next-steps/setup.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/periodic-tasks/myapp.py` & `celery-5.3.0rc2/examples/periodic-tasks/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/resultgraph/tasks.py` & `celery-5.3.0rc2/examples/resultgraph/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/security/mysecureapp.py` & `celery-5.3.0rc2/examples/security/mysecureapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/security/ssl/worker.key` & `celery-5.3.0rc2/examples/security/ssl/worker.key`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/security/ssl/worker.pem` & `celery-5.3.0rc2/examples/security/ssl/worker.pem`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/stamping/examples.py` & `celery-5.3.0rc2/examples/stamping/examples.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/stamping/myapp.py` & `celery-5.3.0rc2/examples/stamping/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/stamping/revoke_example.py` & `celery-5.3.0rc2/examples/stamping/revoke_example.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/stamping/tasks.py` & `celery-5.3.0rc2/examples/stamping/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/examples/stamping/visitors.py` & `celery-5.3.0rc2/examples/stamping/visitors.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/bash-completion/celery.bash` & `celery-5.3.0rc2/extra/bash-completion/celery.bash`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/generic-init.d/celerybeat` & `celery-5.3.0rc2/extra/generic-init.d/celerybeat`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/generic-init.d/celeryd` & `celery-5.3.0rc2/extra/generic-init.d/celeryd`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/macOS/org.celeryq.beat.plist` & `celery-5.3.0rc2/extra/macOS/org.celeryq.beat.plist`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/macOS/org.celeryq.worker.plist` & `celery-5.3.0rc2/extra/macOS/org.celeryq.worker.plist`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/supervisord/celerybeat.conf` & `celery-5.3.0rc2/extra/supervisord/celerybeat.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/supervisord/celeryd.conf` & `celery-5.3.0rc2/extra/supervisord/celeryd.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/supervisord/supervisord.conf` & `celery-5.3.0rc2/extra/supervisord/supervisord.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/systemd/celery.service` & `celery-5.3.0rc2/extra/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/extra/zsh-completion/celery.zsh` & `celery-5.3.0rc2/extra/zsh-completion/celery.zsh`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/pyproject.toml` & `celery-5.3.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/requirements/README.rst` & `celery-5.3.0rc2/requirements/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/requirements/test-ci-default.txt` & `celery-5.3.0rc2/requirements/test-ci-default.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/setup.py` & `celery-5.3.0rc2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 import codecs
 import os
 import re
-import sys
 
 import setuptools
 import setuptools.command.test
 
 NAME = 'celery'
 
 # -*- Extras -*-
@@ -128,30 +127,14 @@
 
 def long_description():
     try:
         return codecs.open('README.rst', 'r', 'utf-8').read()
     except OSError:
         return 'Long description error: Missing README.rst file'
 
-# -*- Command: setup.py test -*-
-
-
-class pytest(setuptools.command.test.test):
-    user_options = [('pytest-args=', 'a', 'Arguments to pass to pytest')]
-
-    def initialize_options(self):
-        super().initialize_options()
-        self.pytest_args = []
-
-    def run_tests(self):
-        import pytest as _pytest
-        sys.exit(_pytest.main(self.pytest_args))
-
-# -*- %%% -*-
-
 
 meta = parse_dist_meta()
 setuptools.setup(
     name=NAME,
     packages=setuptools.find_packages(exclude=['t', 't.*']),
     version=meta['version'],
     description=meta['doc'],
@@ -162,17 +145,14 @@
     url=meta['homepage'],
     license='BSD-3-Clause',
     platforms=['any'],
     install_requires=install_requires(),
     python_requires=">=3.7",
     tests_require=reqs('test.txt'),
     extras_require=extras_require(),
-    cmdclass={'test': pytest},
-    include_package_data=True,
-    zip_safe=False,
     entry_points={
         'console_scripts': [
             'celery = celery.__main__:main',
         ]
     },
     project_urls={
         "Documentation": "https://docs.celeryq.dev/en/stable/",
@@ -185,16 +165,14 @@
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Topic :: System :: Distributed Computing",
         "Topic :: Software Development :: Object Brokering",
         "Framework :: Celery",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent"
     ]
```

### Comparing `celery-5.3.0rc1/t/benchmarks/bench_worker.py` & `celery-5.3.0rc2/t/benchmarks/bench_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/integration/conftest.py` & `celery-5.3.0rc2/t/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/integration/tasks.py` & `celery-5.3.0rc2/t/integration/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/integration/test_backend.py` & `celery-5.3.0rc2/t/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/integration/test_canvas.py` & `celery-5.3.0rc2/t/integration/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/integration/test_inspect.py` & `celery-5.3.0rc2/t/integration/test_inspect.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/integration/test_security.py` & `celery-5.3.0rc2/t/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/integration/test_tasks.py` & `celery-5.3.0rc2/t/integration/test_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,21 @@
                 assert result.successful() is False
             else:
                 assert result.get() == 2
                 assert result.status == 'SUCCESS'
                 assert result.ready() is True
                 assert result.failed() is False
                 assert result.successful() is True
-        worker_state.revoked_stamps.clear()
+
+            # Clear the set of revoked stamps in the worker state.
+            # This step is performed in each iteration of the loop to ensure that only tasks
+            # stamped with a specific monitoring ID will be revoked.
+            # For subsequent iterations with different monitoring IDs, the revoked stamps will
+            # not match the task's stamps, allowing those tasks to proceed successfully.
+            worker_state.revoked_stamps.clear()
 
         # Try to purge the queue after we're done
         # to attempt to avoid interference to other tests
         while True:
             count = manager.app.control.purge()
             if count == 0:
                 break
```

### Comparing `celery-5.3.0rc1/t/integration/test_worker.py` & `celery-5.3.0rc2/t/integration/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_amqp.py` & `celery-5.3.0rc2/t/unit/app/test_amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_annotations.py` & `celery-5.3.0rc2/t/unit/app/test_annotations.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_app.py` & `celery-5.3.0rc2/t/unit/app/test_app.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_backends.py` & `celery-5.3.0rc2/t/unit/app/test_backends.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_beat.py` & `celery-5.3.0rc2/t/unit/app/test_beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_builtins.py` & `celery-5.3.0rc2/t/unit/app/test_builtins.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_control.py` & `celery-5.3.0rc2/t/unit/app/test_control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_defaults.py` & `celery-5.3.0rc2/t/unit/app/test_defaults.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_exceptions.py` & `celery-5.3.0rc2/t/unit/app/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_loaders.py` & `celery-5.3.0rc2/t/unit/app/test_loaders.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_log.py` & `celery-5.3.0rc2/t/unit/app/test_log.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_registry.py` & `celery-5.3.0rc2/t/unit/app/test_registry.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_routes.py` & `celery-5.3.0rc2/t/unit/app/test_routes.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_schedules.py` & `celery-5.3.0rc2/t/unit/app/test_schedules.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/app/test_utils.py` & `celery-5.3.0rc2/t/unit/app/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/apps/test_multi.py` & `celery-5.3.0rc2/t/unit/apps/test_multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_arangodb.py` & `celery-5.3.0rc2/t/unit/backends/test_arangodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_asynchronous.py` & `celery-5.3.0rc2/t/unit/backends/test_asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_azureblockblob.py` & `celery-5.3.0rc2/t/unit/backends/test_azureblockblob.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_base.py` & `celery-5.3.0rc2/t/unit/backends/test_base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_cache.py` & `celery-5.3.0rc2/t/unit/backends/test_cache.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_cassandra.py` & `celery-5.3.0rc2/t/unit/backends/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_consul.py` & `celery-5.3.0rc2/t/unit/backends/test_consul.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_cosmosdbsql.py` & `celery-5.3.0rc2/t/unit/backends/test_cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_couchbase.py` & `celery-5.3.0rc2/t/unit/backends/test_couchbase.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_couchdb.py` & `celery-5.3.0rc2/t/unit/backends/test_couchdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_database.py` & `celery-5.3.0rc2/t/unit/backends/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,20 @@
         of database tables by multiple workers is racy. This test patches
         the used method to always raise, so we can verify that it does
         eventually terminate.
         """
         from sqlalchemy.dialects.sqlite import dialect
         from sqlalchemy.exc import DatabaseError
 
-        sqlite = dialect.dbapi()
+        if hasattr(dialect, 'dbapi'):
+            # Method name in SQLAlchemy < 2.0
+            sqlite = dialect.dbapi()
+        else:
+            # Newer method name in SQLAlchemy 2.0
+            sqlite = dialect.import_dbapi()
         manager = SessionManager()
         engine = manager.get_engine('dburi')
 
         def raise_err(bind):
             raise DatabaseError("", "", [], sqlite.DatabaseError)
 
         patch_create_all = patch.object(
```

### Comparing `celery-5.3.0rc1/t/unit/backends/test_dynamodb.py` & `celery-5.3.0rc2/t/unit/backends/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_elasticsearch.py` & `celery-5.3.0rc2/t/unit/backends/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_filesystem.py` & `celery-5.3.0rc2/t/unit/backends/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_mongodb.py` & `celery-5.3.0rc2/t/unit/backends/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_redis.py` & `celery-5.3.0rc2/t/unit/backends/test_redis.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_rpc.py` & `celery-5.3.0rc2/t/unit/backends/test_rpc.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/backends/test_s3.py` & `celery-5.3.0rc2/t/unit/backends/test_s3.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/bin/test_beat.py` & `celery-5.3.0rc2/t/unit/bin/test_beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/bin/test_worker.py` & `celery-5.3.0rc2/t/unit/bin/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/concurrency/test_concurrency.py` & `celery-5.3.0rc2/t/unit/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/concurrency/test_eventlet.py` & `celery-5.3.0rc2/t/unit/concurrency/test_eventlet.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/concurrency/test_gevent.py` & `celery-5.3.0rc2/t/unit/concurrency/test_gevent.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/concurrency/test_pool.py` & `celery-5.3.0rc2/t/unit/concurrency/test_pool.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/concurrency/test_prefork.py` & `celery-5.3.0rc2/t/unit/concurrency/test_prefork.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/concurrency/test_solo.py` & `celery-5.3.0rc2/t/unit/concurrency/test_solo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/concurrency/test_thread.py` & `celery-5.3.0rc2/t/unit/concurrency/test_thread.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/conftest.py` & `celery-5.3.0rc2/t/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/contrib/test_abortable.py` & `celery-5.3.0rc2/t/unit/contrib/test_abortable.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/contrib/test_migrate.py` & `celery-5.3.0rc2/t/unit/contrib/test_migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/contrib/test_pytest.py` & `celery-5.3.0rc2/t/unit/contrib/test_pytest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/contrib/test_rdb.py` & `celery-5.3.0rc2/t/unit/contrib/test_rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/contrib/test_sphinx.py` & `celery-5.3.0rc2/t/unit/contrib/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/contrib/test_worker.py` & `celery-5.3.0rc2/t/unit/contrib/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/events/test_cursesmon.py` & `celery-5.3.0rc2/t/unit/events/test_cursesmon.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/events/test_events.py` & `celery-5.3.0rc2/t/unit/events/test_events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/events/test_snapshot.py` & `celery-5.3.0rc2/t/unit/events/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/events/test_state.py` & `celery-5.3.0rc2/t/unit/events/test_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/fixups/test_django.py` & `celery-5.3.0rc2/t/unit/fixups/test_django.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/security/__init__.py` & `celery-5.3.0rc2/t/unit/security/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/security/test_certificate.py` & `celery-5.3.0rc2/t/unit/security/test_certificate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/security/test_key.py` & `celery-5.3.0rc2/t/unit/security/test_key.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/security/test_security.py` & `celery-5.3.0rc2/t/unit/security/test_security.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/security/test_serialization.py` & `celery-5.3.0rc2/t/unit/security/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_canvas.py` & `celery-5.3.0rc2/t/unit/tasks/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_chord.py` & `celery-5.3.0rc2/t/unit/tasks/test_chord.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_context.py` & `celery-5.3.0rc2/t/unit/tasks/test_context.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_result.py` & `celery-5.3.0rc2/t/unit/tasks/test_result.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_stamping.py` & `celery-5.3.0rc2/t/unit/tasks/test_stamping.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_states.py` & `celery-5.3.0rc2/t/unit/tasks/test_states.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_tasks.py` & `celery-5.3.0rc2/t/unit/tasks/test_tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/tasks/test_trace.py` & `celery-5.3.0rc2/t/unit/tasks/test_trace.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/test_canvas.py` & `celery-5.3.0rc2/t/unit/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_collections.py` & `celery-5.3.0rc2/t/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_debug.py` & `celery-5.3.0rc2/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_deprecated.py` & `celery-5.3.0rc2/t/unit/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_dispatcher.py` & `celery-5.3.0rc2/t/unit/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_functional.py` & `celery-5.3.0rc2/t/unit/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_graph.py` & `celery-5.3.0rc2/t/unit/utils/test_graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_imports.py` & `celery-5.3.0rc2/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_local.py` & `celery-5.3.0rc2/t/unit/utils/test_local.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_pickle.py` & `celery-5.3.0rc2/t/unit/utils/test_pickle.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_platforms.py` & `celery-5.3.0rc2/t/unit/utils/test_platforms.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_saferepr.py` & `celery-5.3.0rc2/t/unit/utils/test_saferepr.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_serialization.py` & `celery-5.3.0rc2/t/unit/utils/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_sysinfo.py` & `celery-5.3.0rc2/t/unit/utils/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_term.py` & `celery-5.3.0rc2/t/unit/utils/test_term.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_text.py` & `celery-5.3.0rc2/t/unit/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_threads.py` & `celery-5.3.0rc2/t/unit/utils/test_threads.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_time.py` & `celery-5.3.0rc2/t/unit/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_timer2.py` & `celery-5.3.0rc2/t/unit/utils/test_timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/utils/test_utils.py` & `celery-5.3.0rc2/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_autoscale.py` & `celery-5.3.0rc2/t/unit/worker/test_autoscale.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_bootsteps.py` & `celery-5.3.0rc2/t/unit/worker/test_bootsteps.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_components.py` & `celery-5.3.0rc2/t/unit/worker/test_components.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_consumer.py` & `celery-5.3.0rc2/t/unit/worker/test_consumer.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_control.py` & `celery-5.3.0rc2/t/unit/worker/test_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from unittest.mock import Mock, call, patch
 
 import pytest
 from kombu import pidbox
 from kombu.utils.uuid import uuid
 
 from celery.utils.collections import AttributeDict
+from celery.utils.functional import maybe_list
 from celery.utils.timer2 import Timer
 from celery.worker import WorkController as _WC
 from celery.worker import consumer, control
 from celery.worker import state as worker_state
 from celery.worker.pidbox import Pidbox, gPidbox
 from celery.worker.request import Request
 from celery.worker.state import REVOKE_EXPIRES, revoked, revoked_stamps
@@ -540,29 +541,32 @@
             assert 'terminate:' in r['ok']
             # unknown task id only revokes
             r = control.revoke(state, uuid(), terminate=True)
             assert 'tasks unknown' in r['ok']
         finally:
             worker_state.task_ready(request)
 
-    def test_revoke_by_stamped_headers_terminate(self):
+    @pytest.mark.parametrize(
+        "terminate", [True, False],
+    )
+    def test_revoke_by_stamped_headers_terminate(self, terminate):
         request = Mock()
         request.id = uuid()
         request.options = stamped_header = {'stamp': 'foo'}
         request.options['stamped_headers'] = ['stamp']
         state = self.create_state()
         state.consumer = Mock()
         worker_state.task_reserved(request)
         try:
-            r = control.revoke_by_stamped_headers(state, stamped_header, terminate=True)
-            assert stamped_header == revoked_stamps
-            assert 'terminate:' in r['ok']
-            # unknown task id only revokes
-            r = control.revoke_by_stamped_headers(state, stamped_header, terminate=True)
-            assert 'tasks unknown' in r['ok']
+            worker_state.revoked_stamps.clear()
+            assert stamped_header.keys() != revoked_stamps.keys()
+            control.revoke_by_stamped_headers(state, stamped_header, terminate=terminate)
+            assert stamped_header.keys() == revoked_stamps.keys()
+            for key in stamped_header.keys():
+                assert maybe_list(stamped_header[key]) == revoked_stamps[key]
         finally:
             worker_state.task_ready(request)
 
     @pytest.mark.parametrize(
         "header_to_revoke",
         [
             {'header_A': 'value_1'},
@@ -601,16 +605,21 @@
 
         state = self.create_state()
         state.consumer = Mock()
         # Revoke by header
         revoked_stamps.clear()
         r = control.revoke_by_stamped_headers(state, header_to_revoke, terminate=True)
         # Check all of the requests were revoked by a single header
-        assert all([id in r['ok'] for id in ids]), "All requests should be revoked"
-        assert revoked_stamps == header_to_revoke
+        for header, stamp in header_to_revoke.items():
+            assert header in r['ok']
+            for s in maybe_list(stamp):
+                assert str(s) in r['ok']
+        assert header_to_revoke.keys() == revoked_stamps.keys()
+        for key in header_to_revoke.keys():
+            assert list(maybe_list(header_to_revoke[key])) == revoked_stamps[key]
         revoked_stamps.clear()
 
     def test_revoke_return_value_terminate_true(self):
         header_to_revoke = {'foo': 'bar'}
         headers = {
             "id": uuid(),
             "task": self.mytask.name,
@@ -626,17 +635,17 @@
             message,
             app=self.app,
         )
         worker_state.active_requests.add(request)
         worker_state.task_reserved(request)
         state = self.create_state()
         state.consumer = Mock()
-        r = control.revoke(state, headers["id"], terminate=True)
         r_headers = control.revoke_by_stamped_headers(state, header_to_revoke, terminate=True)
-        assert r["ok"] == r_headers["ok"]
+        # revoke & revoke_by_stamped_headers are not aligned anymore in their return values
+        assert "{'foo': {'bar'}}" in r_headers["ok"]
 
     def test_autoscale(self):
         self.panel.state.consumer = Mock()
         self.panel.state.consumer.controller = Mock()
         sc = self.panel.state.consumer.controller.autoscaler = Mock()
         sc.update.return_value = 10, 2
         m = {'method': 'autoscale',
```

### Comparing `celery-5.3.0rc1/t/unit/worker/test_heartbeat.py` & `celery-5.3.0rc2/t/unit/worker/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_loops.py` & `celery-5.3.0rc2/t/unit/worker/test_loops.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_request.py` & `celery-5.3.0rc2/t/unit/worker/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from celery.backends.base import BaseDictBackend
 from celery.exceptions import Ignore, InvalidTaskError, Reject, Retry, TaskRevokedError, Terminated, WorkerLostError
 from celery.signals import task_failure, task_retry, task_revoked
 from celery.worker import request as module
 from celery.worker import strategy
 from celery.worker.request import Request, create_request_cls
 from celery.worker.request import logger as req_logger
-from celery.worker.state import revoked
+from celery.worker.state import revoked, revoked_stamps
 
 
 class RequestCase:
 
     def setup_method(self):
         self.app.conf.result_serializer = 'pickle'
 
@@ -575,14 +575,41 @@
                 task_revoked, sender=job.task, request=job._context,
                 terminated=False, expired=False, signum=None):
             revoked.add(job.id)
             assert job.revoked()
             assert job._already_revoked
             assert job.acknowledged
 
+    @pytest.mark.parametrize(
+        "header_to_revoke",
+        [
+            {'header_A': 'value_1'},
+            {'header_B': ['value_2', 'value_3']},
+            {'header_C': ('value_2', 'value_3')},
+            {'header_D': {'value_2', 'value_3'}},
+            {'header_E': [1, '2', 3.0]},
+        ],
+    )
+    def test_revoked_by_stamped_headers(self, header_to_revoke):
+        revoked_stamps.clear()
+        job = self.xRequest()
+        stamps = header_to_revoke
+        stamped_headers = list(header_to_revoke.keys())
+        job._message.headers['stamps'] = stamps
+        job._message.headers['stamped_headers'] = stamped_headers
+        job._request_dict['stamps'] = stamps
+        job._request_dict['stamped_headers'] = stamped_headers
+        with self.assert_signal_called(
+                task_revoked, sender=job.task, request=job._context,
+                terminated=False, expired=False, signum=None):
+            revoked_stamps.update(stamps)
+            assert job.revoked()
+            assert job._already_revoked
+            assert job.acknowledged
+
     def test_execute_does_not_execute_revoked(self):
         job = self.xRequest()
         revoked.add(job.id)
         job.execute()
 
     def test_execute_acks_late(self):
         self.mytask_raising.acks_late = True
```

### Comparing `celery-5.3.0rc1/t/unit/worker/test_state.py` & `celery-5.3.0rc2/t/unit/worker/test_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_strategy.py` & `celery-5.3.0rc2/t/unit/worker/test_strategy.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc1/t/unit/worker/test_worker.py` & `celery-5.3.0rc2/t/unit/worker/test_worker.py`

 * *Files identical despite different names*

