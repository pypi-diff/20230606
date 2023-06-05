# Comparing `tmp/fluxoperator-0.0.24.tar.gz` & `tmp/fluxoperator-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.24.tar", last modified: Tue May 16 20:42:54 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.26.tar", last modified: Mon Jun  5 22:27:40 2023, max compression
```

## Comparing `fluxoperator-0.0.24.tar` & `fluxoperator-0.0.26.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13483 2023-05-16 20:42:46.000000 fluxoperator-0.0.24/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6639 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5986 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 20:42:53.000000 fluxoperator-0.0.24/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-05-16 20:42:54.000000 fluxoperator-0.0.24/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-16 20:42:53.000000 fluxoperator-0.0.24/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-16 20:42:53.000000 fluxoperator-0.0.24/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-16 20:42:54.000000 fluxoperator-0.0.24/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-16 20:42:46.000000 fluxoperator-0.0.24/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.694054 fluxoperator-0.0.26/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13596 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8265 2023-06-05 22:23:54.000000 fluxoperator-0.0.26/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6217 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7727 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-10 21:19:30.000000 fluxoperator-0.0.26/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.26/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-10 21:19:30.000000 fluxoperator-0.0.26/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-10 23:12:41.000000 fluxoperator-0.0.26/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-10 23:12:41.000000 fluxoperator-0.0.26/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.24/PKG-INFO` & `fluxoperator-0.0.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.24
+Version: 0.0.26
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.24/fluxoperator/__init__.py` & `fluxoperator-0.0.26/fluxoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/api_client.py` & `fluxoperator-0.0.26/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/client.py` & `fluxoperator-0.0.26/fluxoperator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,25 +137,28 @@
                 # There will be a few connection errors before everything is ready
                 except Exception:
                     pass
 
             print()
             yield url
 
-    def stream_output(self, filename, stdout=True, timestamps=False):
+    def stream_output(self, filename, stdout=True, timestamps=False, pod=None):
         """
         Stream output, optionally printing also to stdout.
+
+        We allow specifying the pod if we don't want output from the broker.
         """
+        pod = pod or self.broker_pod
         return self.ctrl.stream_output(
             filename=filename,
             stdout=stdout,
             namespace=self.namespace,
             timestamps=timestamps,
             name=self.name,
-            pod=self.broker_pod,
+            pod=pod,
         )
 
     @timed
     def delete(self):
         """
         Deletion (and time the deletion of) the MiniCluster
         """
```

### Comparing `fluxoperator-0.0.24/fluxoperator/configuration.py` & `fluxoperator-0.0.26/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/decorator.py` & `fluxoperator-0.0.26/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/exceptions.py` & `fluxoperator-0.0.26/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/__init__.py` & `fluxoperator-0.0.26/fluxoperator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/commands.py` & `fluxoperator-0.0.26/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.26/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.26/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.26/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/flux_spec.py` & `fluxoperator-0.0.26/fluxoperator/models/flux_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,44 +32,54 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'connect_timeout': 'str',
         'install_root': 'str',
         'log_level': 'int',
-        'option_flags': 'str'
+        'minimal_service': 'bool',
+        'option_flags': 'str',
+        'wrap': 'str'
     }
 
     attribute_map = {
         'connect_timeout': 'connectTimeout',
         'install_root': 'installRoot',
         'log_level': 'logLevel',
-        'option_flags': 'optionFlags'
+        'minimal_service': 'minimalService',
+        'option_flags': 'optionFlags',
+        'wrap': 'wrap'
     }
 
-    def __init__(self, connect_timeout='5s', install_root='/usr', log_level=6, option_flags='', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, connect_timeout='5s', install_root='/usr', log_level=6, minimal_service=False, option_flags='', wrap=None, local_vars_configuration=None):  # noqa: E501
         """FluxSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._connect_timeout = None
         self._install_root = None
         self._log_level = None
+        self._minimal_service = None
         self._option_flags = None
+        self._wrap = None
         self.discriminator = None
 
         if connect_timeout is not None:
             self.connect_timeout = connect_timeout
         if install_root is not None:
             self.install_root = install_root
         if log_level is not None:
             self.log_level = log_level
+        if minimal_service is not None:
+            self.minimal_service = minimal_service
         if option_flags is not None:
             self.option_flags = option_flags
+        if wrap is not None:
+            self.wrap = wrap
 
     @property
     def connect_timeout(self):
         """Gets the connect_timeout of this FluxSpec.  # noqa: E501
 
         Single user executable to provide to flux start  # noqa: E501
 
@@ -133,14 +143,37 @@
         :param log_level: The log_level of this FluxSpec.  # noqa: E501
         :type log_level: int
         """
 
         self._log_level = log_level
 
     @property
+    def minimal_service(self):
+        """Gets the minimal_service of this FluxSpec.  # noqa: E501
+
+        Only expose the broker service (to reduce load on DNS)  # noqa: E501
+
+        :return: The minimal_service of this FluxSpec.  # noqa: E501
+        :rtype: bool
+        """
+        return self._minimal_service
+
+    @minimal_service.setter
+    def minimal_service(self, minimal_service):
+        """Sets the minimal_service of this FluxSpec.
+
+        Only expose the broker service (to reduce load on DNS)  # noqa: E501
+
+        :param minimal_service: The minimal_service of this FluxSpec.  # noqa: E501
+        :type minimal_service: bool
+        """
+
+        self._minimal_service = minimal_service
+
+    @property
     def option_flags(self):
         """Gets the option_flags of this FluxSpec.  # noqa: E501
 
         Flux option flags, usually provided with -o optional - if needed, default option flags for the server These can also be set in the user interface to override here. This is only valid for a FluxRunner \"runFlux\" true  # noqa: E501
 
         :return: The option_flags of this FluxSpec.  # noqa: E501
         :rtype: str
@@ -155,14 +188,37 @@
 
         :param option_flags: The option_flags of this FluxSpec.  # noqa: E501
         :type option_flags: str
         """
 
         self._option_flags = option_flags
 
+    @property
+    def wrap(self):
+        """Gets the wrap of this FluxSpec.  # noqa: E501
+
+        Commands for flux start --wrap  # noqa: E501
+
+        :return: The wrap of this FluxSpec.  # noqa: E501
+        :rtype: str
+        """
+        return self._wrap
+
+    @wrap.setter
+    def wrap(self, wrap):
+        """Sets the wrap of this FluxSpec.
+
+        Commands for flux start --wrap  # noqa: E501
+
+        :param wrap: The wrap of this FluxSpec.  # noqa: E501
+        :type wrap: str
+        """
+
+        self._wrap = wrap
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = inspect.getargspec(x.to_dict).args
```

### Comparing `fluxoperator-0.0.24/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.26/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.26/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.26/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,84 +31,89 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'claim_name': 'str',
         'path': 'str',
-        'read_only': 'bool'
+        'read_only': 'bool',
+        'secret_name': 'str'
     }
 
     attribute_map = {
         'claim_name': 'claimName',
         'path': 'path',
-        'read_only': 'readOnly'
+        'read_only': 'readOnly',
+        'secret_name': 'secretName'
     }
 
-    def __init__(self, claim_name='', path='', read_only=False, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, claim_name=None, path=None, read_only=False, secret_name=None, local_vars_configuration=None):  # noqa: E501
         """MiniClusterExistingVolume - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._claim_name = None
         self._path = None
         self._read_only = None
+        self._secret_name = None
         self.discriminator = None
 
-        self.claim_name = claim_name
-        self.path = path
+        if claim_name is not None:
+            self.claim_name = claim_name
+        if path is not None:
+            self.path = path
         if read_only is not None:
             self.read_only = read_only
+        if secret_name is not None:
+            self.secret_name = secret_name
 
     @property
     def claim_name(self):
         """Gets the claim_name of this MiniClusterExistingVolume.  # noqa: E501
 
+        Claim name if the existing volume is a PVC  # noqa: E501
 
         :return: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
         :rtype: str
         """
         return self._claim_name
 
     @claim_name.setter
     def claim_name(self, claim_name):
         """Sets the claim_name of this MiniClusterExistingVolume.
 
+        Claim name if the existing volume is a PVC  # noqa: E501
 
         :param claim_name: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
         :type claim_name: str
         """
-        if self.local_vars_configuration.client_side_validation and claim_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `claim_name`, must not be `None`")  # noqa: E501
 
         self._claim_name = claim_name
 
     @property
     def path(self):
         """Gets the path of this MiniClusterExistingVolume.  # noqa: E501
 
-        Path and claim name are always required  # noqa: E501
+        Path and claim name are always required if a secret isn't defined  # noqa: E501
 
         :return: The path of this MiniClusterExistingVolume.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
         """Sets the path of this MiniClusterExistingVolume.
 
-        Path and claim name are always required  # noqa: E501
+        Path and claim name are always required if a secret isn't defined  # noqa: E501
 
         :param path: The path of this MiniClusterExistingVolume.  # noqa: E501
         :type path: str
         """
-        if self.local_vars_configuration.client_side_validation and path is None:  # noqa: E501
-            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
         self._path = path
 
     @property
     def read_only(self):
         """Gets the read_only of this MiniClusterExistingVolume.  # noqa: E501
 
@@ -125,14 +130,37 @@
 
         :param read_only: The read_only of this MiniClusterExistingVolume.  # noqa: E501
         :type read_only: bool
         """
 
         self._read_only = read_only
 
+    @property
+    def secret_name(self):
+        """Gets the secret_name of this MiniClusterExistingVolume.  # noqa: E501
+
+        An existing secret  # noqa: E501
+
+        :return: The secret_name of this MiniClusterExistingVolume.  # noqa: E501
+        :rtype: str
+        """
+        return self._secret_name
+
+    @secret_name.setter
+    def secret_name(self, secret_name):
+        """Sets the secret_name of this MiniClusterExistingVolume.
+
+        An existing secret  # noqa: E501
+
+        :param secret_name: The secret_name of this MiniClusterExistingVolume.  # noqa: E501
+        :type secret_name: str
+        """
+
+        self._secret_name = secret_name
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = inspect.getargspec(x.to_dict).args
```

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.26/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/models/security_context.py` & `fluxoperator-0.0.26/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/resource/network.py` & `fluxoperator-0.0.26/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/resource/pods.py` & `fluxoperator-0.0.26/fluxoperator/resource/pods.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator/rest.py` & `fluxoperator-0.0.26/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.26/fluxoperator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.24
+Version: 0.0.26
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.24/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.26/fluxoperator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/setup.py` & `fluxoperator-0.0.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.24",
+        version="0.0.26",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.24/test/test_commands.py` & `fluxoperator-0.0.26/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_container_resources.py` & `fluxoperator-0.0.26/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_container_volume.py` & `fluxoperator-0.0.26/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_flux_restful.py` & `fluxoperator-0.0.26/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_flux_spec.py` & `fluxoperator-0.0.26/test/test_flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_flux_user.py` & `fluxoperator-0.0.26/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_life_cycle.py` & `fluxoperator-0.0.26/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_logging_spec.py` & `fluxoperator-0.0.26/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster.py` & `fluxoperator-0.0.26/test/test_mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.26/test/test_mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_container.py` & `fluxoperator-0.0.26/test/test_mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.26/test/test_mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_list.py` & `fluxoperator-0.0.26/test/test_mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_spec.py` & `fluxoperator-0.0.26/test/test_mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_status.py` & `fluxoperator-0.0.26/test/test_mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_user.py` & `fluxoperator-0.0.26/test/test_mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.26/test/test_mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_pod_spec.py` & `fluxoperator-0.0.26/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.24/test/test_security_context.py` & `fluxoperator-0.0.26/test/test_security_context.py`

 * *Files identical despite different names*

