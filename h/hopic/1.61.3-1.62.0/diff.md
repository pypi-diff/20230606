# Comparing `tmp/hopic-1.61.3.tar.gz` & `tmp/hopic-1.62.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/jenkins/workspace/hopic_release_1/dist/tmpj_4svkro/hopic-1.61.3.tar", last modified: Mon May 29 07:39:23 2023, max compression
+gzip compressed data, was "/jenkins/workspace/hopic_release_1/dist/tmplqr65_b0/hopic-1.62.0.tar", last modified: Tue Jun  6 13:56:15 2023, max compression
```

## Comparing `hopic-1.61.3.tar` & `hopic-1.62.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2021-11-04 10:44:59.000000 hopic-1.61.3/permissions.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8331 2022-02-25 14:42:15.000000 hopic-1.61.3/hopic/git_time.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    71062 2023-03-23 08:27:04.000000 hopic-1.61.3/hopic/config_reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23237 2021-12-23 16:07:43.000000 hopic-1.61.3/hopic/versioning.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2020-08-29 06:53:11.000000 hopic-1.61.3/hopic/test/test_credentials.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26412 2022-02-01 16:50:00.000000 hopic-1.61.3/hopic/test/test_extensions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2021-03-31 09:46:20.000000 hopic-1.61.3/hopic/test/test_approvals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2020-08-29 06:53:11.000000 hopic-1.61.3/hopic/test/test_versioning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12161 2023-03-22 11:36:07.000000 hopic-1.61.3/hopic/test/test_checkout.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2021-08-16 11:43:03.000000 hopic-1.61.3/hopic/test/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54517 2022-08-05 08:34:03.000000 hopic-1.61.3/hopic/test/test_build.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7576 2021-05-21 10:41:19.000000 hopic-1.61.3/hopic/test/test_version_bump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85299 2023-03-22 11:36:07.000000 hopic-1.61.3/hopic/test/test_merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-05-29 07:22:41.000000 hopic-1.61.3/hopic/test/markers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11571 2022-07-28 12:30:27.000000 hopic-1.61.3/hopic/test/test_show_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10668 2022-03-22 15:11:48.000000 hopic-1.61.3/hopic/test/test_getinfo.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2491 2021-05-21 10:41:19.000000 hopic-1.61.3/hopic/test/test_execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    57112 2022-03-17 09:16:40.000000 hopic-1.61.3/hopic/test/test_config_reader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic/test/docker-images/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic/test/docker-images/python/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1383 2020-08-27 06:38:21.000000 hopic-1.61.3/hopic/test/docker-images/python/Dockerfile
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1325 2020-08-13 10:49:20.000000 hopic-1.61.3/hopic/test/docker-images/python/entrypoint.sh
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      671 2020-08-13 10:49:20.000000 hopic-1.61.3/hopic/test/docker-images/python/ssh.sh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3292 2021-04-28 11:03:59.000000 hopic-1.61.3/hopic/test/test_template_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      871 2021-07-09 16:01:55.000000 hopic-1.61.3/hopic/test/test_examples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8679 2021-08-17 09:13:44.000000 hopic-1.61.3/hopic/test/conftest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic/cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4674 2021-12-23 16:07:43.000000 hopic-1.61.3/hopic/cli/global_obj.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6427 2021-08-16 11:43:03.000000 hopic-1.61.3/hopic/cli/extensions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32740 2022-11-01 11:29:21.000000 hopic-1.61.3/hopic/cli/build.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8214 2022-11-01 11:29:21.000000 hopic-1.61.3/hopic/cli/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67209 2023-05-05 13:49:16.000000 hopic-1.61.3/hopic/cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2021-02-12 14:05:19.000000 hopic-1.61.3/hopic/cli/autocomplete.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3083 2023-05-17 13:31:10.000000 hopic-1.61.3/hopic/cli/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7240 2021-07-16 13:21:22.000000 hopic-1.61.3/hopic/build.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2021-08-16 11:43:03.000000 hopic-1.61.3/hopic/compat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2019-09-09 14:49:54.000000 hopic-1.61.3/hopic/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      637 2020-09-30 09:14:13.000000 hopic-1.61.3/hopic/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2021-06-16 17:22:49.000000 hopic-1.61.3/hopic/types.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3316 2022-07-01 09:56:14.000000 hopic-1.61.3/hopic/execution.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic/template/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-03-23 14:28:09.000000 hopic-1.61.3/hopic/template/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2919 2021-05-07 15:03:02.000000 hopic-1.61.3/hopic/template/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4759 2021-05-07 15:03:02.000000 hopic-1.61.3/hopic/credentials.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2021-06-10 12:40:43.000000 hopic-1.61.3/hopic/errors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15611 2022-07-22 09:51:20.000000 hopic-1.61.3/hopic/binary_normalize.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/doc/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/doc/source/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2021-01-22 10:18:40.000000 hopic-1.61.3/doc/source/index.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26379 2019-10-29 14:49:42.000000 hopic-1.61.3/doc/source/parallel-phases.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.61.3/doc/source/CONTRIBUTING.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37971 2023-03-22 14:23:47.000000 hopic-1.61.3/doc/source/changes.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2020-09-21 14:42:29.000000 hopic-1.61.3/doc/source/usage.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2021-05-21 10:41:19.000000 hopic-1.61.3/doc/source/hotfix.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46784 2022-03-24 15:28:49.000000 hopic-1.61.3/doc/source/config.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2019-10-29 14:49:42.000000 hopic-1.61.3/doc/source/intro.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11086 2020-11-20 17:31:32.000000 hopic-1.61.3/doc/source/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2019-02-04 16:02:23.000000 hopic-1.61.3/doc/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7693 2019-02-04 16:02:23.000000 hopic-1.61.3/doc/Makefile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2778 2023-03-17 09:31:31.000000 hopic-1.61.3/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-05-29 07:39:23.000000 hopic-1.61.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.61.3/CONTRIBUTING.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2018-09-11 09:38:00.000000 hopic-1.61.3/.git_archival.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      661 2019-11-07 14:38:21.000000 hopic-1.61.3/examples/upload-artifactory.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1051 2020-12-04 14:21:57.000000 hopic-1.61.3/examples/with-credentials.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2021-01-21 19:52:27.000000 hopic-1.61.3/examples/upload-on-fail.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      823 2019-11-07 14:38:21.000000 hopic-1.61.3/examples/artifactory-promote.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      473 2020-10-28 13:20:54.000000 hopic-1.61.3/examples/stash.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2019-11-19 12:22:45.000000 hopic-1.61.3/examples/version-bump-constant.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2022-03-22 15:11:48.000000 hopic-1.61.3/examples/finally.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2019-11-05 15:44:39.000000 hopic-1.61.3/examples/archive.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.61.3/examples/dependency_manifest.xml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      358 2021-01-22 15:16:09.000000 hopic-1.61.3/examples/docker-extra-args.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      428 2019-11-05 15:44:39.000000 hopic-1.61.3/examples/with-volumes.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2021-01-21 19:52:27.000000 hopic-1.61.3/examples/post-submit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2021-02-09 11:51:15.000000 hopic-1.61.3/examples/allow-missing-archive.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2019-11-25 06:27:20.000000 hopic-1.61.3/examples/clean.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2021-06-09 10:59:19.000000 hopic-1.61.3/examples/timeout.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2020-08-19 12:54:41.000000 hopic-1.61.3/examples/with-keyring-credentials.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2021-02-09 11:51:15.000000 hopic-1.61.3/examples/allow-missing-junit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      140 2021-10-06 13:00:51.000000 hopic-1.61.3/examples/allow-failures-junit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2020-10-19 07:55:45.000000 hopic-1.61.3/examples/config.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2019-11-07 14:38:21.000000 hopic-1.61.3/examples/fingerprint.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2021-01-21 19:52:27.000000 hopic-1.61.3/examples/version-bump-conventional.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2545 2019-10-29 14:49:42.000000 hopic-1.61.3/examples/parallel-phases.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2020-08-12 13:05:54.000000 hopic-1.61.3/examples/disable-etc-volumes.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      274 2020-01-10 14:03:05.000000 hopic-1.61.3/examples/image-mapping.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2021-01-21 19:52:27.000000 hopic-1.61.3/examples/docker-in-docker.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2019-11-18 07:58:57.000000 hopic-1.61.3/examples/description.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/examples/embed/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      230 2020-08-27 06:38:21.000000 hopic-1.61.3/examples/embed/yaml-generation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2020-05-15 09:48:27.000000 hopic-1.61.3/examples/embed/embed.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      166 2020-09-14 14:10:55.000000 hopic-1.61.3/examples/pip.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2020-11-30 14:08:37.000000 hopic-1.61.3/examples/ci-locks.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      223 2019-11-05 15:44:39.000000 hopic-1.61.3/examples/image-ivy-manifest.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2020-12-03 13:52:01.000000 hopic-1.61.3/examples/environment.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2019-11-07 14:38:21.000000 hopic-1.61.3/examples/run-on-change.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2021-01-21 19:52:27.000000 hopic-1.61.3/examples/volumes-override.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/examples/simple/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.61.3/examples/simple/dependency_manifest.xml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2492 2021-01-21 19:52:27.000000 hopic-1.61.3/examples/simple/hopic-ci-config.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1839 2020-09-28 15:18:56.000000 hopic-1.61.3/examples/simple/Jenkinsfile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2021-06-09 12:02:18.000000 hopic-1.61.3/examples/timeout-variant.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2019-11-07 14:38:21.000000 hopic-1.61.3/examples/node-label.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2019-11-07 14:38:21.000000 hopic-1.61.3/examples/junit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      188 2020-12-04 14:21:57.000000 hopic-1.61.3/examples/pass-through-env-vars.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-29 07:39:23.000000 hopic-1.61.3/hopic.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1279 2020-08-21 14:01:27.000000 hopic-1.61.3/README.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10757 2019-09-25 13:48:29.000000 hopic-1.61.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2021-02-19 11:08:41.000000 hopic-1.61.3/pytest.ini
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/src/com/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/src/com/tomtom/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/src/com/tomtom/hopic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2022-06-14 09:15:10.000000 hopic-1.61.3/src/com/tomtom/hopic/HopicEventCallbacks.groovy
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1728 2023-03-21 12:05:25.000000 hopic-1.61.3/tox.ini
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/vars/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5706 2021-05-11 08:24:17.000000 hopic-1.61.3/vars/printMetrics.groovy
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84346 2023-03-24 13:43:41.000000 hopic-1.61.3/vars/getCiDriver.groovy
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2019-11-11 15:31:32.000000 hopic-1.61.3/.gitattributes
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      557 2021-05-07 15:03:02.000000 hopic-1.61.3/mypy.ini
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-29 07:39:23.000000 hopic-1.61.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2021-05-07 15:03:02.000000 hopic-1.61.3/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2021-11-15 13:30:02.000000 hopic-1.61.3/doc-requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6351 2022-03-18 16:12:34.000000 hopic-1.61.3/hopic-ci-config.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/.github/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/.github/actions/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/.github/actions/submit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3290 2023-05-26 12:14:43.000000 hopic-1.61.3/.github/actions/submit/action.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 07:39:23.000000 hopic-1.61.3/.github/actions/checkout/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-05-05 13:49:16.000000 hopic-1.61.3/.github/actions/checkout/hopic-version-dump.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9884 2023-05-26 13:13:45.000000 hopic-1.61.3/.github/actions/checkout/action.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2260 2022-01-28 10:24:00.000000 hopic-1.61.3/Jenkinsfile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2019-01-04 15:25:30.000000 hopic-1.61.3/REQUIREMENTS.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-03-17 09:31:31.000000 hopic-1.61.3/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2019-01-17 16:44:37.000000 hopic-1.61.3/USAGE.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2021-11-04 10:44:59.000000 hopic-1.62.0/permissions.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8331 2022-02-25 14:42:15.000000 hopic-1.62.0/hopic/git_time.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    71062 2023-03-23 08:27:04.000000 hopic-1.62.0/hopic/config_reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23237 2021-12-23 16:07:43.000000 hopic-1.62.0/hopic/versioning.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2020-08-29 06:53:11.000000 hopic-1.62.0/hopic/test/test_credentials.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26412 2022-02-01 16:50:00.000000 hopic-1.62.0/hopic/test/test_extensions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2021-03-31 09:46:20.000000 hopic-1.62.0/hopic/test/test_approvals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2020-08-29 06:53:11.000000 hopic-1.62.0/hopic/test/test_versioning.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12161 2023-03-22 11:36:07.000000 hopic-1.62.0/hopic/test/test_checkout.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2021-08-16 11:43:03.000000 hopic-1.62.0/hopic/test/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54517 2022-08-05 08:34:03.000000 hopic-1.62.0/hopic/test/test_build.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7576 2021-05-21 10:41:19.000000 hopic-1.62.0/hopic/test/test_version_bump.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85299 2023-03-22 11:36:07.000000 hopic-1.62.0/hopic/test/test_merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-06-06 13:47:08.000000 hopic-1.62.0/hopic/test/markers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11571 2022-07-28 12:30:27.000000 hopic-1.62.0/hopic/test/test_show_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10668 2022-03-22 15:11:48.000000 hopic-1.62.0/hopic/test/test_getinfo.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2491 2021-05-21 10:41:19.000000 hopic-1.62.0/hopic/test/test_execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    57112 2022-03-17 09:16:40.000000 hopic-1.62.0/hopic/test/test_config_reader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic/test/docker-images/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic/test/docker-images/python/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1383 2020-08-27 06:38:21.000000 hopic-1.62.0/hopic/test/docker-images/python/Dockerfile
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1325 2020-08-13 10:49:20.000000 hopic-1.62.0/hopic/test/docker-images/python/entrypoint.sh
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      671 2020-08-13 10:49:20.000000 hopic-1.62.0/hopic/test/docker-images/python/ssh.sh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3292 2021-04-28 11:03:59.000000 hopic-1.62.0/hopic/test/test_template_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      871 2021-07-09 16:01:55.000000 hopic-1.62.0/hopic/test/test_examples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8679 2021-08-17 09:13:44.000000 hopic-1.62.0/hopic/test/conftest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4674 2021-12-23 16:07:43.000000 hopic-1.62.0/hopic/cli/global_obj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6427 2021-08-16 11:43:03.000000 hopic-1.62.0/hopic/cli/extensions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32740 2022-11-01 11:29:21.000000 hopic-1.62.0/hopic/cli/build.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9521 2023-06-05 14:30:27.000000 hopic-1.62.0/hopic/cli/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67209 2023-05-05 13:49:16.000000 hopic-1.62.0/hopic/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2021-02-12 14:05:19.000000 hopic-1.62.0/hopic/cli/autocomplete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3083 2023-05-17 13:31:10.000000 hopic-1.62.0/hopic/cli/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7240 2021-07-16 13:21:22.000000 hopic-1.62.0/hopic/build.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2021-08-16 11:43:03.000000 hopic-1.62.0/hopic/compat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2019-09-09 14:49:54.000000 hopic-1.62.0/hopic/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      637 2020-09-30 09:14:13.000000 hopic-1.62.0/hopic/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2021-06-16 17:22:49.000000 hopic-1.62.0/hopic/types.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3316 2022-07-01 09:56:14.000000 hopic-1.62.0/hopic/execution.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic/template/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-03-23 14:28:09.000000 hopic-1.62.0/hopic/template/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2919 2021-05-07 15:03:02.000000 hopic-1.62.0/hopic/template/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4759 2021-05-07 15:03:02.000000 hopic-1.62.0/hopic/credentials.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2021-06-10 12:40:43.000000 hopic-1.62.0/hopic/errors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15611 2022-07-22 09:51:20.000000 hopic-1.62.0/hopic/binary_normalize.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/doc/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/doc/source/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2021-01-22 10:18:40.000000 hopic-1.62.0/doc/source/index.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26379 2019-10-29 14:49:42.000000 hopic-1.62.0/doc/source/parallel-phases.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.62.0/doc/source/CONTRIBUTING.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37971 2023-03-22 14:23:47.000000 hopic-1.62.0/doc/source/changes.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2020-09-21 14:42:29.000000 hopic-1.62.0/doc/source/usage.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2021-05-21 10:41:19.000000 hopic-1.62.0/doc/source/hotfix.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46784 2022-03-24 15:28:49.000000 hopic-1.62.0/doc/source/config.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2019-10-29 14:49:42.000000 hopic-1.62.0/doc/source/intro.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11086 2020-11-20 17:31:32.000000 hopic-1.62.0/doc/source/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2019-02-04 16:02:23.000000 hopic-1.62.0/doc/.gitignore
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7693 2019-02-04 16:02:23.000000 hopic-1.62.0/doc/Makefile
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2778 2023-03-17 09:31:31.000000 hopic-1.62.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-06-06 13:56:15.000000 hopic-1.62.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.62.0/CONTRIBUTING.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2018-09-11 09:38:00.000000 hopic-1.62.0/.git_archival.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/examples/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      661 2019-11-07 14:38:21.000000 hopic-1.62.0/examples/upload-artifactory.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1051 2020-12-04 14:21:57.000000 hopic-1.62.0/examples/with-credentials.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2021-01-21 19:52:27.000000 hopic-1.62.0/examples/upload-on-fail.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      823 2019-11-07 14:38:21.000000 hopic-1.62.0/examples/artifactory-promote.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      473 2020-10-28 13:20:54.000000 hopic-1.62.0/examples/stash.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2019-11-19 12:22:45.000000 hopic-1.62.0/examples/version-bump-constant.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2022-03-22 15:11:48.000000 hopic-1.62.0/examples/finally.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2019-11-05 15:44:39.000000 hopic-1.62.0/examples/archive.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.62.0/examples/dependency_manifest.xml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      358 2021-01-22 15:16:09.000000 hopic-1.62.0/examples/docker-extra-args.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      428 2019-11-05 15:44:39.000000 hopic-1.62.0/examples/with-volumes.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2021-01-21 19:52:27.000000 hopic-1.62.0/examples/post-submit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2021-02-09 11:51:15.000000 hopic-1.62.0/examples/allow-missing-archive.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2019-11-25 06:27:20.000000 hopic-1.62.0/examples/clean.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2021-06-09 10:59:19.000000 hopic-1.62.0/examples/timeout.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2020-08-19 12:54:41.000000 hopic-1.62.0/examples/with-keyring-credentials.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2021-02-09 11:51:15.000000 hopic-1.62.0/examples/allow-missing-junit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      140 2021-10-06 13:00:51.000000 hopic-1.62.0/examples/allow-failures-junit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2020-10-19 07:55:45.000000 hopic-1.62.0/examples/config.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2019-11-07 14:38:21.000000 hopic-1.62.0/examples/fingerprint.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2021-01-21 19:52:27.000000 hopic-1.62.0/examples/version-bump-conventional.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2545 2019-10-29 14:49:42.000000 hopic-1.62.0/examples/parallel-phases.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2020-08-12 13:05:54.000000 hopic-1.62.0/examples/disable-etc-volumes.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      274 2020-01-10 14:03:05.000000 hopic-1.62.0/examples/image-mapping.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2021-01-21 19:52:27.000000 hopic-1.62.0/examples/docker-in-docker.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2019-11-18 07:58:57.000000 hopic-1.62.0/examples/description.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/examples/embed/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      230 2020-08-27 06:38:21.000000 hopic-1.62.0/examples/embed/yaml-generation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2020-05-15 09:48:27.000000 hopic-1.62.0/examples/embed/embed.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      166 2020-09-14 14:10:55.000000 hopic-1.62.0/examples/pip.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2020-11-30 14:08:37.000000 hopic-1.62.0/examples/ci-locks.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      223 2019-11-05 15:44:39.000000 hopic-1.62.0/examples/image-ivy-manifest.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2020-12-03 13:52:01.000000 hopic-1.62.0/examples/environment.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2019-11-07 14:38:21.000000 hopic-1.62.0/examples/run-on-change.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2021-01-21 19:52:27.000000 hopic-1.62.0/examples/volumes-override.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/examples/simple/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.62.0/examples/simple/dependency_manifest.xml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2492 2021-01-21 19:52:27.000000 hopic-1.62.0/examples/simple/hopic-ci-config.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1839 2020-09-28 15:18:56.000000 hopic-1.62.0/examples/simple/Jenkinsfile
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2021-06-09 12:02:18.000000 hopic-1.62.0/examples/timeout-variant.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2019-11-07 14:38:21.000000 hopic-1.62.0/examples/node-label.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2019-11-07 14:38:21.000000 hopic-1.62.0/examples/junit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      188 2020-12-04 14:21:57.000000 hopic-1.62.0/examples/pass-through-env-vars.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-06 13:56:14.000000 hopic-1.62.0/hopic.egg-info/zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-06 13:56:15.000000 hopic-1.62.0/hopic.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1279 2020-08-21 14:01:27.000000 hopic-1.62.0/README.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10757 2019-09-25 13:48:29.000000 hopic-1.62.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2021-02-19 11:08:41.000000 hopic-1.62.0/pytest.ini
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/src/com/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/src/com/tomtom/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/src/com/tomtom/hopic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2022-06-14 09:15:10.000000 hopic-1.62.0/src/com/tomtom/hopic/HopicEventCallbacks.groovy
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1728 2023-03-21 12:05:25.000000 hopic-1.62.0/tox.ini
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/vars/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5706 2021-05-11 08:24:17.000000 hopic-1.62.0/vars/printMetrics.groovy
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84346 2023-03-24 13:43:41.000000 hopic-1.62.0/vars/getCiDriver.groovy
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2019-11-11 15:31:32.000000 hopic-1.62.0/.gitattributes
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      557 2021-05-07 15:03:02.000000 hopic-1.62.0/mypy.ini
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-06 13:56:15.000000 hopic-1.62.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2021-05-07 15:03:02.000000 hopic-1.62.0/.gitignore
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2021-11-15 13:30:02.000000 hopic-1.62.0/doc-requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6351 2022-03-18 16:12:34.000000 hopic-1.62.0/hopic-ci-config.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/.github/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/.github/actions/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/.github/actions/submit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3290 2023-06-06 12:49:09.000000 hopic-1.62.0/.github/actions/submit/action.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 13:56:15.000000 hopic-1.62.0/.github/actions/checkout/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-05-05 13:49:16.000000 hopic-1.62.0/.github/actions/checkout/hopic-version-dump.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9940 2023-06-06 12:59:09.000000 hopic-1.62.0/.github/actions/checkout/action.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2260 2022-01-28 10:24:00.000000 hopic-1.62.0/Jenkinsfile
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2019-01-04 15:25:30.000000 hopic-1.62.0/REQUIREMENTS.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-03-17 09:31:31.000000 hopic-1.62.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2019-01-17 16:44:37.000000 hopic-1.62.0/USAGE.md
```

### Comparing `hopic-1.61.3/permissions.txt` & `hopic-1.62.0/permissions.txt`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/git_time.py` & `hopic-1.62.0/hopic/git_time.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/config_reader.py` & `hopic-1.62.0/hopic/config_reader.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/versioning.py` & `hopic-1.62.0/hopic/versioning.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_credentials.py` & `hopic-1.62.0/hopic/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_extensions.py` & `hopic-1.62.0/hopic/test/test_extensions.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_approvals.py` & `hopic-1.62.0/hopic/test/test_approvals.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_versioning.py` & `hopic-1.62.0/hopic/test/test_versioning.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_checkout.py` & `hopic-1.62.0/hopic/test/test_checkout.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/__init__.py` & `hopic-1.62.0/hopic/test/__init__.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_build.py` & `hopic-1.62.0/hopic/test/test_build.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_version_bump.py` & `hopic-1.62.0/hopic/test/test_version_bump.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_merge.py` & `hopic-1.62.0/hopic/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_show_config.py` & `hopic-1.62.0/hopic/test/test_show_config.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_getinfo.py` & `hopic-1.62.0/hopic/test/test_getinfo.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_execution.py` & `hopic-1.62.0/hopic/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_config_reader.py` & `hopic-1.62.0/hopic/test/test_config_reader.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/docker-images/python/Dockerfile` & `hopic-1.62.0/hopic/test/docker-images/python/Dockerfile`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/docker-images/python/entrypoint.sh` & `hopic-1.62.0/hopic/test/docker-images/python/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/docker-images/python/ssh.sh` & `hopic-1.62.0/hopic/test/docker-images/python/ssh.sh`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_template_utils.py` & `hopic-1.62.0/hopic/test/test_template_utils.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/test_examples.py` & `hopic-1.62.0/hopic/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/test/conftest.py` & `hopic-1.62.0/hopic/test/conftest.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/cli/global_obj.py` & `hopic-1.62.0/hopic/cli/global_obj.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/cli/extensions.py` & `hopic-1.62.0/hopic/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/cli/build.py` & `hopic-1.62.0/hopic/cli/build.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/cli/main.py` & `hopic-1.62.0/hopic/cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -85,23 +85,55 @@
             exception_raiser=exception_raiser,
         )
 
     def register_dependent_attribute(self, name, dependency):
         self._missing_parameters[name] = self._missing_parameters[dependency]
 
 
+class GitHubLogFormatter(logging.Formatter):
+    level_prefix = (
+        (logging.ERROR  , "error"  ),
+        (logging.WARNING, "warning"),
+        (logging.INFO   , "notice" ),
+        (logging.DEBUG  , "debug"  ),
+    )
+
+    def __init__(self):
+        super().__init__("%(message)s", style="%")
+
+    def format(self, record):
+        msg = super().format(record)
+
+        # turn into GitHub diagnostic emitting command
+        for min_level, prefix in self.level_prefix:
+            if record.levelno >= min_level:
+                break
+        else:
+            # no known way to encode this for GitHub, just emit this as is
+            return msg
+
+        # percent-encode the strict set of characters that's both required and permitted by GitHub
+        msg = msg.replace("%", "%25").replace("\n", "%0A").replace("\r", "%0D")
+        msg = f"::{prefix}::{msg}"
+        return msg
+
+
+def on_github_actions():
+    return os.environ.get("CI") == "true" and os.environ.get("GITHUB_JOB")
+
+
 @click.group(context_settings=dict(help_option_names=('-h', '--help')))
 @click.option('--color'          , type=click.Choice(('always', 'auto', 'never'))                                                  , default='auto'      , show_default=True)  # noqa: E501
 @click.option('--config'         , type=click.Path(exists=False, file_okay=True , dir_okay=False, readable=True, resolve_path=True), default=lambda: None, show_default='${WORKSPACE}/hopic-ci-config.yaml')  # noqa: E501
 @click.option('--workspace'      , type=click.Path(exists=False, file_okay=False, dir_okay=True)                                   , default=lambda: None, show_default='git work tree of config file or current working directory')  # noqa: E501
 @click.option('--whitelisted-var', multiple=True                                                                                   , default=['CT_DEVENV_HOME'], hidden=True)  # noqa: E501
 @click.option('--publishable-version', is_flag=True                                                                                , default=False, hidden=True, help='''Indicate if change is publishable or not''')  # noqa: E501
 @click.version_option(get_package_version(PACKAGE))
-@click_log.simple_verbosity_option(PACKAGE                 , envvar='HOPIC_VERBOSITY', autocompletion=autocomplete.click_log_verbosity)
-@click_log.simple_verbosity_option('git', '--git-verbosity', envvar='GIT_VERBOSITY'  , autocompletion=autocomplete.click_log_verbosity)
+@click_log.simple_verbosity_option(PACKAGE                 , envvar='HOPIC_VERBOSITY', autocompletion=autocomplete.click_log_verbosity, default=lambda: "DEBUG" if on_github_actions() and os.environ.get("RUNNER_DEBUG") == "1" else "INFO")
+@click_log.simple_verbosity_option('git', '--git-verbosity', envvar='GIT_VERBOSITY'  , autocompletion=autocomplete.click_log_verbosity, default=lambda: "DEBUG" if on_github_actions() and os.environ.get("RUNNER_DEBUG") == "1" else "INFO")
 @click.pass_context
 def main(ctx, color, config, workspace, whitelisted_var, publishable_version):
     if color == 'always':
         ctx.color = True
     elif color == 'never':
         ctx.color = False
     # Force or suppress colors according to http://bixense.com/clicolors/ convention.
@@ -109,15 +141,17 @@
         ctx.color = True
     elif os.environ.get("CLICOLOR", "1") == "0":
         ctx.color = False
     else:
         # leave as is: 'auto' is the default for Click
         pass
 
-    click_log.basic_config()
+    global_logger = click_log.basic_config()
+    if on_github_actions():
+        global_logger.handlers[0].formatter = GitHubLogFormatter()
 
     ctx.obj = OptionContext()
     for param in ctx.command.params:
         ctx.obj.register_parameter(ctx=ctx, param=param)
         if param.human_readable_name == 'workspace' and workspace is not None:
             workspace = Path(workspace)
             if ctx.invoked_subcommand != 'checkout-source-tree':
```

### Comparing `hopic-1.61.3/hopic/cli/__init__.py` & `hopic-1.62.0/hopic/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/cli/autocomplete.py` & `hopic-1.62.0/hopic/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/cli/utils.py` & `hopic-1.62.0/hopic/cli/utils.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/build.py` & `hopic-1.62.0/hopic/build.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/compat.py` & `hopic-1.62.0/hopic/compat.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/__main__.py` & `hopic-1.62.0/hopic/__main__.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/types.py` & `hopic-1.62.0/hopic/types.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/execution.py` & `hopic-1.62.0/hopic/execution.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/template/utils.py` & `hopic-1.62.0/hopic/template/utils.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/credentials.py` & `hopic-1.62.0/hopic/credentials.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/errors.py` & `hopic-1.62.0/hopic/errors.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic/binary_normalize.py` & `hopic-1.62.0/hopic/binary_normalize.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/source/index.rst` & `hopic-1.62.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/source/parallel-phases.svg` & `hopic-1.62.0/doc/source/parallel-phases.svg`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/source/CONTRIBUTING.md` & `hopic-1.62.0/doc/source/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/source/changes.rst` & `hopic-1.62.0/doc/source/changes.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/source/hotfix.rst` & `hopic-1.62.0/doc/source/hotfix.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/source/config.rst` & `hopic-1.62.0/doc/source/config.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/source/conf.py` & `hopic-1.62.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/doc/Makefile` & `hopic-1.62.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/setup.py` & `hopic-1.62.0/setup.py`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/PKG-INFO` & `hopic-1.62.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopic
-Version: 1.61.3
+Version: 1.62.0
 Summary: In order to simplify the CI configuration we are switching away from the generic jenkins shared pipeline which is completely written in Groovy. Instead we are switching to the Hopic project which only has a minimal CI driver component written in Groovy with the rest written in Python. With Hopic local debugging is made significantly easier.
 Home-page: https://github.com/tomtom-international/hopic
 Author: TomTom N.V.
 License: Apache License 2.0
 Project-URL: Documentation, https://tomtom-international.github.io/hopic/
 Project-URL: Change Log, https://tomtom-international.github.io/hopic/changes.html
 Project-URL: Source Code, https://github.com/tomtom-international/hopic
```

### Comparing `hopic-1.61.3/CONTRIBUTING.md` & `hopic-1.62.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/upload-artifactory.yaml` & `hopic-1.62.0/examples/upload-artifactory.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/with-credentials.yaml` & `hopic-1.62.0/examples/with-credentials.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/artifactory-promote.yaml` & `hopic-1.62.0/examples/artifactory-promote.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/archive.yaml` & `hopic-1.62.0/examples/archive.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/parallel-phases.yaml` & `hopic-1.62.0/examples/parallel-phases.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/volumes-override.yaml` & `hopic-1.62.0/examples/volumes-override.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/simple/hopic-ci-config.yml` & `hopic-1.62.0/examples/simple/hopic-ci-config.yml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/examples/simple/Jenkinsfile` & `hopic-1.62.0/examples/simple/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic.egg-info/SOURCES.txt` & `hopic-1.62.0/hopic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic.egg-info/PKG-INFO` & `hopic-1.62.0/hopic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopic
-Version: 1.61.3
+Version: 1.62.0
 Summary: In order to simplify the CI configuration we are switching away from the generic jenkins shared pipeline which is completely written in Groovy. Instead we are switching to the Hopic project which only has a minimal CI driver component written in Groovy with the rest written in Python. With Hopic local debugging is made significantly easier.
 Home-page: https://github.com/tomtom-international/hopic
 Author: TomTom N.V.
 License: Apache License 2.0
 Project-URL: Documentation, https://tomtom-international.github.io/hopic/
 Project-URL: Change Log, https://tomtom-international.github.io/hopic/changes.html
 Project-URL: Source Code, https://github.com/tomtom-international/hopic
```

### Comparing `hopic-1.61.3/README.rst` & `hopic-1.62.0/README.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/LICENSE` & `hopic-1.62.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/src/com/tomtom/hopic/HopicEventCallbacks.groovy` & `hopic-1.62.0/src/com/tomtom/hopic/HopicEventCallbacks.groovy`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/tox.ini` & `hopic-1.62.0/tox.ini`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/vars/printMetrics.groovy` & `hopic-1.62.0/vars/printMetrics.groovy`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/vars/getCiDriver.groovy` & `hopic-1.62.0/vars/getCiDriver.groovy`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/mypy.ini` & `hopic-1.62.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/hopic-ci-config.yaml` & `hopic-1.62.0/hopic-ci-config.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/.github/actions/submit/action.yaml` & `hopic-1.62.0/.github/actions/submit/action.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
       id: unbundle
       shell: bash
       env:
         CLICOLOR_FORCE: '1'
         LC_ALL: C.UTF-8
         TZ: UTC
       run: |
+        set -x
         declare -a config_params
         if [ ! -e "${GITHUB_WORKSPACE}/hopic-ci-config.yaml" -a ! -e "${GITHUB_WORKSPACE}/.ci/hopic-ci-config.yaml" ]; then
           config_params+=("--config=${GITHUB_ACTION_PATH}/../checkout/hopic-version-dump.yaml")
         fi
-        set -x
         git fetch hopic-merge-transfer.bundle refs/hopic/bundle/meta
         echo -n 'hopic-meta=' >> "$GITHUB_OUTPUT"
         git show FETCH_HEAD:hopic-meta >> "$GITHUB_OUTPUT"
         echo >> "$GITHUB_OUTPUT"
         python3 -m hopic --workspace="${GITHUB_WORKSPACE}" unbundle hopic-merge-transfer.bundle
         if python3 -m hopic --workspace="${GITHUB_WORKSPACE}" "${config_params[@]}" may-publish; then
           echo 'may-publish=true' >> "${GITHUB_OUTPUT}"
@@ -61,13 +61,13 @@
       if: ${{ steps.download-bundle.outcome == 'success' && !fromJSON(steps.unbundle.outputs.hopic-meta).autosquashed-commit && fromJSON(steps.unbundle.outputs.hopic-meta).refspecs }}
       shell: bash
       env:
         CLICOLOR_FORCE: '1'
         LC_ALL: C.UTF-8
         TZ: UTC
       run: |
+        set -x
         declare -a config_params
         if [ ! -e "${GITHUB_WORKSPACE}/hopic-ci-config.yaml" -a ! -e "${GITHUB_WORKSPACE}/.ci/hopic-ci-config.yaml" ]; then
           config_params+=("--config=${GITHUB_ACTION_PATH}/../checkout/hopic-version-dump.yaml")
         fi
-        set -x
         python3 -m hopic --workspace="${GITHUB_WORKSPACE}" "${config_params[@]}" --publishable-version submit
```

### Comparing `hopic-1.61.3/.github/actions/checkout/hopic-version-dump.yaml` & `hopic-1.62.0/.github/actions/checkout/hopic-version-dump.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/.github/actions/checkout/action.yaml` & `hopic-1.62.0/.github/actions/checkout/action.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,21 @@
     - name: Prepare Source Tree with Hopic
       if: ${{ steps.download-bundle.outcome != 'success' && startsWith(github.event_name, 'pull_request') }}
       shell: bash
       env:
         CLICOLOR_FORCE: '1'
         LC_ALL: C.UTF-8
         TZ: UTC
+        GH_PR_TITLE: ${{ github.event.pull_request.title }}
+        GH_PR_BODY: ${{ github.event.pull_request.body }}
       run: |
+        set -x
         declare -a config_params extra_cr_params extra_prep_params
-        if [ -n '${{github.event.pull_request.body}}' ]; then
-          extra_cr_params+=("--description=$(echo -n '${{github.event.pull_request.body}}' | awk 'BEGIN { output=1 } /^(- )?\[[ x]\] / { output=0 } output')")
+        if [ -n "${GH_PR_BODY:-}" ]; then
+          extra_cr_params+=("--description=$(echo -n "${GH_PR_BODY:-}" | awk 'BEGIN { output=1 } /^(- )?\[[ x]\] / { output=0 } output')")
         fi
         extra_prep_params+=('--author-email=${{github.event.pull_request.user.id}}+${{github.event.pull_request.user.login}}@users.noreply.github.com')
         if curl --fail -o "${RUNNER_TEMP}/pr-author.json" -u 'x-access-token:${{github.token}}' -H 'Accept: application/json' '${{github.event.pull_request.user.url}}'; then
           extra_prep_params+=("--author-name=$(python -c 'import os, json; print(json.load(open(os.path.join(os.environ["RUNNER_TEMP"], "pr-author.json")))["name"], end="")')")
         fi
         if curl --fail -o "${RUNNER_TEMP}/pr-reviews.json" -u 'x-access-token:${{github.token}}' -H 'Accept: application/json' '${{github.event.pull_request.url}}/reviews?per_page=100'; then
           while read review_commit review_user_login review_user_url; do
@@ -101,38 +104,37 @@
           done < <(python -c 'import os, json; print("\n".join(review["commit_id"] + " " + review["user"]["login"] + " " + review["user"]["url"] for review in json.load(open(os.path.join(os.environ["RUNNER_TEMP"], "pr-reviews.json"))) if review["state"] == "APPROVED"))')
         fi
         # Pass our own Hopic config file if no such config file exists after merging this PR
         git fetch "${GITHUB_SERVER_URL}/${GITHUB_REPOSITORY}" "${GITHUB_REF}:${GITHUB_REF}"
         if ! git show "${GITHUB_REF}:hopic-ci-config.yaml" > /dev/null && ! git show "${GITHUB_REF}:.ci/hopic-ci-config.yaml" > /dev/null; then
           config_params+=("--config=${GITHUB_ACTION_PATH}/hopic-version-dump.yaml")
         fi
-        set -x
-        python3 -m hopic --workspace="${GITHUB_WORKSPACE}" "${config_params[@]}" prepare-source-tree --author-date='${{github.event.pull_request.updated_at}}' "${extra_prep_params[@]}" --bundle="hopic-merge-transfer.bundle" merge-change-request "${extra_cr_params[@]}" --source-remote='${{github.event.pull_request.head.repo.clone_url}}' --source-ref='${{ github.event.pull_request.head.ref }}' --change-request='${{github.event.pull_request.number}}' --title='${{github.event.pull_request.title}}'
+        python3 -m hopic --workspace="${GITHUB_WORKSPACE}" "${config_params[@]}" prepare-source-tree --author-date='${{github.event.pull_request.updated_at}}' "${extra_prep_params[@]}" --bundle="hopic-merge-transfer.bundle" merge-change-request "${extra_cr_params[@]}" --source-remote='${{github.event.pull_request.head.repo.clone_url}}' --source-ref='${{ github.event.pull_request.head.ref }}' --change-request='${{github.event.pull_request.number}}' --title="${GH_PR_TITLE}"
 
     - name: Bump Version with Hopic
       if: ${{ steps.download-bundle.outcome != 'success' && !startsWith(github.event_name, 'pull_request') && inputs.modality && inputs.modality != 'NORMAL' }}
       shell: bash
       env:
         CLICOLOR_FORCE: '1'
         LC_ALL: C.UTF-8
         TZ: UTC
         MODALITY: ${{ inputs.modality }}
       run: |
+        set -x
         declare -a config_params modality_params
         # Pass our own Hopic config file if no such config file exists after merging this PR
         git fetch "${GITHUB_SERVER_URL}/${GITHUB_REPOSITORY}" "${GITHUB_REF}:${GITHUB_REF}"
         if [ ! -e "${GITHUB_WORKSPACE}/hopic-ci-config.yaml" -a ! -e "${GITHUB_WORKSPACE}/.ci/hopic-ci-config.yaml" ]; then
           config_params+=("--config=${GITHUB_ACTION_PATH}/hopic-version-dump.yaml")
         fi
         if [ "${MODALITY}" = 'BUMP_VERSION' ]; then
           modality_params+=(bump-version)
         else
           modality_params+=(apply-modality-change "${MODALITY}")
         fi
-        set -x
         python3 -m hopic --workspace="${GITHUB_WORKSPACE}" "${config_params[@]}" prepare-source-tree --bundle="hopic-merge-transfer.bundle" "${modality_params[@]}" > "${RUNNER_TEMP}/prep-tree.txt"
         set +x
         if [ ! -s "${RUNNER_TEMP}/prep-tree.txt" ]; then
           echo "##[warning]no changes to build" >&2
           exit 2
         fi
 
@@ -148,19 +150,19 @@
       shell: bash
       env:
         CLICOLOR_FORCE: '1'
         LC_ALL: C.UTF-8
         TZ: UTC
         MODALITY: ${{ inputs.modality }}
       run: |
+        set -x
         declare -a config_params global_options
         if [ ! -e "${GITHUB_WORKSPACE}/hopic-ci-config.yaml" -a ! -e "${GITHUB_WORKSPACE}/.ci/hopic-ci-config.yaml" ]; then
           config_params+=("--config=${GITHUB_ACTION_PATH}/hopic-version-dump.yaml")
         fi
-        set -x
         if [[ "${GITHUB_EVENT_NAME}" == pull_request* || ( -n "${MODALITY}" && "${MODALITY}" != NORMAL ) ]] && python3 -m hopic --workspace="${GITHUB_WORKSPACE}" "${config_params[@]}" may-publish; then
           # TODO: check PR approval state too
           #global_options+=('--publishable-version')
           echo 'may-publish=true' >> "${GITHUB_OUTPUT}"
         else
           echo 'may-publish=false' >> "${GITHUB_OUTPUT}"
         fi
```

### Comparing `hopic-1.61.3/Jenkinsfile` & `hopic-1.62.0/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `hopic-1.61.3/REQUIREMENTS.md` & `hopic-1.62.0/REQUIREMENTS.md`

 * *Files identical despite different names*

