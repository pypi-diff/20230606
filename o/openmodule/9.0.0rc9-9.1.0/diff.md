# Comparing `tmp/openmodule-9.0.0rc9.tar.gz` & `tmp/openmodule-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule-9.0.0rc9.tar", last modified: Wed Dec 22 10:26:39 2021, max compression
+gzip compressed data, was "openmodule-9.1.0.tar", last modified: Wed Mar  9 10:32:53 2022, max compression
```

## Comparing `openmodule-9.0.0rc9.tar` & `openmodule-9.1.0.tar`

### file list

```diff
@@ -1,163 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.338649 openmodule-9.0.0rc9/
--rw-rw-rw-   0 root         (0) root         (0)     1620 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.326731 openmodule-9.0.0rc9/.idea/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.idea/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.326731 openmodule-9.0.0rc9/.idea/inspectionProfiles/
--rw-rw-rw-   0 root         (0) root         (0)     1319 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0 root         (0) root         (0)      174 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0 root         (0) root         (0)      195 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      272 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)     1016 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.idea/openmodule.iml
--rw-rw-rw-   0 root         (0) root         (0)      180 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/.idea/vcs.xml
--rw-r--r--   0 root         (0) root         (0)      262 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     7099 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)    18074 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7062 2021-12-22 10:26:39.338649 openmodule-9.0.0rc9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6375 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.327648 openmodule-9.0.0rc9/docs/
--rw-rw-rw-   0 root         (0) root         (0)      954 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/docs/coding_standard.md
--rw-rw-rw-   0 root         (0) root         (0)     3322 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/docs/database.md
--rw-rw-rw-   0 root         (0) root         (0)     2838 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/docs/known_issues.md
--rw-rw-rw-   0 root         (0) root         (0)     3434 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/docs/migrations.md
--rw-rw-rw-   0 root         (0) root         (0)     2374 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/docs/rpc.md
--rw-rw-rw-   0 root         (0) root         (0)     3704 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/docs/testing.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.328565 openmodule-9.0.0rc9/openmodule/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/alert.py
--rw-rw-rw-   0 root         (0) root         (0)     1060 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/checks.py
--rw-rw-rw-   0 root         (0) root         (0)    13192 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/config.py
--rw-rw-rw-   0 root         (0) root         (0)     5613 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.329481 openmodule-9.0.0rc9/openmodule/database/
--rw-rw-rw-   0 root         (0) root         (0)     1242 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/database/custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/database/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1983 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/database/env.py
--rw-rw-rw-   0 root         (0) root         (0)     7974 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2259 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/health.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     2871 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/messaging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.329481 openmodule-9.0.0rc9/openmodule/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/alert.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3527 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/presence.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2928 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2882 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/models/vehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.331315 openmodule-9.0.0rc9/openmodule/rpc/
--rw-rw-rw-   0 root         (0) root         (0)      107 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/rpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5655 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/rpc/client.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/rpc/common.py
--rw-rw-rw-   0 root         (0) root         (0)     9659 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/rpc/server.py
--rw-rw-rw-   0 root         (0) root         (0)     2930 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/sentry.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.332232 openmodule-9.0.0rc9/openmodule/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3034 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/api.py
--rw-rw-rw-   0 root         (0) root         (0)     4865 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/charset.py
--rw-rw-rw-   0 root         (0) root         (0)     1351 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/connection_status.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/db_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     8974 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/io.py
--rw-rw-rw-   0 root         (0) root         (0)    17100 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/matching.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/presence.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule/utils/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.328565 openmodule-9.0.0rc9/openmodule.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7062 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/openmodule.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3967 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/openmodule.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/openmodule.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/openmodule.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      209 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/openmodule.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-12-22 10:26:39.000000 openmodule-9.0.0rc9/openmodule.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.334065 openmodule-9.0.0rc9/openmodule_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/alert.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/api.py
--rw-rw-rw-   0 root         (0) root         (0)     9515 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/backend.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/core.py
--rw-rw-rw-   0 root         (0) root         (0)     2323 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/database.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/database_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/eventlistener.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/files.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/gate.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/health.py
--rw-rw-rw-   0 root         (0) root         (0)     3582 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/interrupt.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/io.py
--rw-rw-rw-   0 root         (0) root         (0)     5263 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/presence.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1840 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      521 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    18426 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/openmodule_test/zeromq.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      725 2021-12-22 10:26:39.338649 openmodule-9.0.0rc9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      444 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       74 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/test-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.335899 openmodule-9.0.0rc9/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.335899 openmodule-9.0.0rc9/tests/invalid_database/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.336815 openmodule-9.0.0rc9/tests/invalid_database/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/invalid_database/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/invalid_database/alembic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/invalid_database/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/invalid_database/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.336815 openmodule-9.0.0rc9/tests/invalid_database/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)      771 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/invalid_database/alembic/versions/ff26e54332f9_datetime_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2039 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/invalid_database/alembic.ini
--rwxrwxrwx   0 root         (0) root         (0)      832 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/invalid_database/makemigration.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.325815 openmodule-9.0.0rc9/tests/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.336815 openmodule-9.0.0rc9/tests/resources/configs/
--rw-rw-rw-   0 root         (0) root         (0)      263 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/configs/config.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/configs/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/configs/test_config_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.337732 openmodule-9.0.0rc9/tests/resources/utils_matching/
--rw-rw-rw-   0 root         (0) root         (0)      285 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/A-10.yml
--rw-rw-rw-   0 root         (0) root         (0)      210 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/A-20.yml
--rw-rw-rw-   0 root         (0) root         (0)       91 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/DEFAULT-10.yml
--rw-rw-rw-   0 root         (0) root         (0)      183 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/DEFAULT-20.yml
--rw-rw-rw-   0 root         (0) root         (0)       94 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/DEFAULT-30.yml
--rw-rw-rw-   0 root         (0) root         (0)      230 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/LEGACY-0.yml
--rw-rw-rw-   0 root         (0) root         (0)       95 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/TEST-10.yml
--rw-rw-rw-   0 root         (0) root         (0)       96 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/TEST-20.yml
--rw-rw-rw-   0 root         (0) root         (0)       95 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/TEST-30.yml
--rw-rw-rw-   0 root         (0) root         (0)       95 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/resources/utils_matching/TEST-40.yml
--rw-rw-rw-   0 root         (0) root         (0)     1235 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_alert.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_checks.py
--rw-rw-rw-   0 root         (0) root         (0)    10855 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)    10984 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.337732 openmodule-9.0.0rc9/tests/test_database_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.337732 openmodule-9.0.0rc9/tests/test_database_data/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database_data/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database_data/alembic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database_data/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database_data/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 10:26:39.338649 openmodule-9.0.0rc9/tests/test_database_data/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)     1238 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database_data/alembic/versions/32b8c728abbf_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database_data/alembic.ini
--rwxrwxrwx   0 root         (0) root         (0)      840 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_database_data/makemigration.sh
--rw-rw-rw-   0 root         (0) root         (0)     6636 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1393 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_health.py
--rw-rw-rw-   0 root         (0) root         (0)     3583 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_interrupt.py
--rw-rw-rw-   0 root         (0) root         (0)     7194 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_io_listen.py
--rw-rw-rw-   0 root         (0) root         (0)     4520 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     4781 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     8726 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_models_backend.py
--rw-rw-rw-   0 root         (0) root         (0)    25116 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8609 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2155 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_sentry.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_test_alert.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_test_gate.py
--rw-rw-rw-   0 root         (0) root         (0)    10252 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_test_zeromq.py
--rw-rw-rw-   0 root         (0) root         (0)     2287 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_utils_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14424 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_utils_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_utils_charset.py
--rw-rw-rw-   0 root         (0) root         (0)     4231 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_utils_connection_status.py
--rw-rw-rw-   0 root         (0) root         (0)    19072 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_utils_matching.py
--rw-rw-rw-   0 root         (0) root         (0)     8348 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_utils_presence.py
--rw-rw-rw-   0 root         (0) root         (0)     4629 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tests/test_utils_vehicle.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2021-12-22 10:26:25.000000 openmodule-9.0.0rc9/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.400077 openmodule-9.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2022-03-09 10:32:38.000000 openmodule-9.1.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      228 2022-03-09 10:32:53.000000 openmodule-9.1.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     6770 2022-03-09 10:32:53.000000 openmodule-9.1.0/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)    18074 2022-03-09 10:32:38.000000 openmodule-9.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9764 2022-03-09 10:32:53.400077 openmodule-9.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9080 2022-03-09 10:32:38.000000 openmodule-9.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.389112 openmodule-9.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      954 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/coding_standard.md
+-rw-rw-rw-   0 root         (0) root         (0)      870 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/core.md
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/database.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.389112 openmodule-9.1.0/docs/deprecated_code/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/deprecated_code/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.386371 openmodule-9.1.0/docs/deprecated_code/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.386371 openmodule-9.1.0/docs/deprecated_code/api/openmodule/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.389112 openmodule-9.1.0/docs/deprecated_code/api/openmodule/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3324 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/deprecated_code/api/openmodule/utils/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.389112 openmodule-9.1.0/docs/deprecated_code/api/openmodule_test/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/deprecated_code/api/openmodule_test/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.389112 openmodule-9.1.0/docs/deprecated_code/api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/deprecated_code/api/tests/test_utils_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/known_issues.md
+-rw-rw-rw-   0 root         (0) root         (0)     4321 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/migrations.md
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/rpc.md
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2022-03-09 10:32:38.000000 openmodule-9.1.0/docs/testing.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.390026 openmodule-9.1.0/openmodule/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)    13612 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7744 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.390940 openmodule-9.1.0/openmodule/database/
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/database/custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/database/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/database/env.py
+-rw-rw-rw-   0 root         (0) root         (0)    12889 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2259 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3173 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/messaging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.392767 openmodule-9.1.0/openmodule/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     2056 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/presence.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/privacy.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/models/vehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.392767 openmodule-9.1.0/openmodule/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/rpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6379 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/rpc/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/rpc/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11450 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/rpc/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/sentry.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.394595 openmodule-9.1.0/openmodule/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4865 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/charset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/connection_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/db_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9568 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    17100 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/matching.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/misc_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7225 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/package_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7382 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/presence.py
+-rw-rw-rw-   0 root         (0) root         (0)     6844 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule/utils/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.390940 openmodule-9.1.0/openmodule.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9764 2022-03-09 10:32:53.000000 openmodule-9.1.0/openmodule.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4132 2022-03-09 10:32:53.000000 openmodule-9.1.0/openmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-09 10:32:53.000000 openmodule-9.1.0/openmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-09 10:32:53.000000 openmodule-9.1.0/openmodule.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2022-03-09 10:32:53.000000 openmodule-9.1.0/openmodule.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      231 2022-03-09 10:32:53.000000 openmodule-9.1.0/openmodule.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-03-09 10:32:53.000000 openmodule-9.1.0/openmodule.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.395509 openmodule-9.1.0/openmodule_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     9515 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/database.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/database_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3001 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/eventlistener.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     3192 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/gate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     4157 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/interrupt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/presence.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      521 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18818 2022-03-09 10:32:38.000000 openmodule-9.1.0/openmodule_test/zeromq.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2022-03-09 10:32:38.000000 openmodule-9.1.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2022-03-09 10:32:53.400991 openmodule-9.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      444 2022-03-09 10:32:38.000000 openmodule-9.1.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       74 2022-03-09 10:32:38.000000 openmodule-9.1.0/test-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.398250 openmodule-9.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.398250 openmodule-9.1.0/tests/invalid_database/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.398250 openmodule-9.1.0/tests/invalid_database/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/invalid_database/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/invalid_database/alembic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/invalid_database/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/invalid_database/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.398250 openmodule-9.1.0/tests/invalid_database/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/invalid_database/alembic/versions/ff26e54332f9_datetime_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/invalid_database/alembic.ini
+-rwxrwxrwx   0 root         (0) root         (0)      832 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/invalid_database/makemigration.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.387285 openmodule-9.1.0/tests/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.399164 openmodule-9.1.0/tests/resources/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/configs/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/configs/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/configs/test_config_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.400077 openmodule-9.1.0/tests/resources/utils_matching/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/A-10.yml
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/A-20.yml
+-rw-rw-rw-   0 root         (0) root         (0)       91 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/DEFAULT-10.yml
+-rw-rw-rw-   0 root         (0) root         (0)      183 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/DEFAULT-20.yml
+-rw-rw-rw-   0 root         (0) root         (0)       94 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/DEFAULT-30.yml
+-rw-rw-rw-   0 root         (0) root         (0)      230 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/LEGACY-0.yml
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/TEST-10.yml
+-rw-rw-rw-   0 root         (0) root         (0)       96 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/TEST-20.yml
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/TEST-30.yml
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/resources/utils_matching/TEST-40.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)    11211 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)    11008 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.400077 openmodule-9.1.0/tests/test_database_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.400077 openmodule-9.1.0/tests/test_database_data/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database_data/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database_data/alembic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database_data/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database_data/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 10:32:53.400077 openmodule-9.1.0/tests/test_database_data/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database_data/alembic/versions/32b8c728abbf_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database_data/alembic.ini
+-rwxrwxrwx   0 root         (0) root         (0)      840 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_database_data/makemigration.sh
+-rw-rw-rw-   0 root         (0) root         (0)     8515 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_health.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_interrupt.py
+-rw-rw-rw-   0 root         (0) root         (0)     7379 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_io_listen.py
+-rw-rw-rw-   0 root         (0) root         (0)     4619 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     4781 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8726 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_models_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5898 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_package_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    26138 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     8639 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     5972 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_sentry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_test_alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_test_gate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10252 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_test_zeromq.py
+-rw-rw-rw-   0 root         (0) root         (0)    14223 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_charset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4231 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_connection_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    19072 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_matching.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_misc_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10712 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_presence.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4629 2022-03-09 10:32:38.000000 openmodule-9.1.0/tests/test_utils_vehicle.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2022-03-09 10:32:38.000000 openmodule-9.1.0/tox.ini
```

### Comparing `openmodule-9.0.0rc9/.gitlab-ci.yml` & `openmodule-9.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/ChangeLog` & `openmodule-9.1.0/ChangeLog`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,19 @@
 CHANGES
 =======
 
-v9.0.0.rc9
-----------
-
-* added base64 validator to payload added some models added default source entry to validate response
-
-v9.0.0.rc8
-----------
-
-* added cost entries to the access model
-
-v9.0.0.rc7
-----------
-
-* renamed status to state
-* ¯\\_(ツ)\_/¯
-* added base64\_validator
-* added timezone\_validator
-* dependencies fix because i forgot setting python interpreter
-* changed some validation model typings
-* added validation provider template class
-* added validatino provider models
-* minor change in deprecation warnings [skip ci]
-* use assert warnings instead of assert logs for failing testcase
-* some docs
-* assertion replaced with a warning to prevent unnecessary crashes as it's not breaking
-
-v9.0.0.rc6
-----------
-
-* additional logs during startup, and a better default value for broker sub port and broker pub port in the backwards compatibility functions
-
-v9.0.0.rc5
-----------
-
-* fixes in the count message definition
-
-v9.0.0.rc4
-----------
-
-* refactoring for backends aswell as some message definition cleanups
-
-v9.0.0.rc3
-----------
-
-* backwardscompatibility fix for vehicle (all ids must be empty by default)
-
-v9.0.0.rc2
-----------
+v9.1.0
+------
 
-* trigger for dev releases
+* Feature/privacy
 
-v9.0.0.rc1
-----------
+v9.0.0
+------
 
-* refactored rpc client, some cleanup and fixes across the board
+* Version 9 Release
 
 v8.1.3
 ------
 
 * Additions to Vehicle and Presence messages
 
 v8.1.2
@@ -170,19 +124,39 @@
 v6.1.0
 ------
 
 * docs [skip-ci]
 * relative path fix again
 * relative path fix
 * lazy config
+* openmodule config
 * docs [skip ci]
 
 v6.0.1
 ------
 
 * allow import of checking module
 * documentation [skip ci]
 
 v6.0.0
 ------
 
 * requirements
+* known issues
+* fixes an issue with .timestamp() and testing
+* name function which has no doc string in assertion
+* why did i do that?
+* recurrence allows empty strings again now, wait\_for\_reject raises an assertion instead of timeout error if the barrier actually opened
+* testcase for datetime-naive saves
+* git stash popMerge branch 'timezone\_checks' of gitlab.com:arivo-public/device-python/openmodule into timezone\_checks
+* why was this ignored?
+* developer error, test gate
+* check on migration/make\_migration if DateTime is used + testcase, custom types are now imported correctly
+* fix in timezone validator for optional fields
+* v6 breaking changes, added timezone / datetime checks
+* added database flush and a known issues list
+
+v5.0.1
+------
+
+* fixes a bug in the database code, which swallowed exceptions during commit()
+* api changes
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openmodule-9.0.0rc9/LICENSE` & `openmodule-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/PKG-INFO` & `openmodule-9.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule
-Version: 9.0.0rc9
+Version: 9.1.0
 Summary: Libraries for developing the arivo openmodule
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule
 Platform: UNKNOWN
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 License-File: LICENSE
 
 # OpenModule V2
 
+Some additional documentation:
+
+* [Openmodule Core](docs/core.md)
+* [RPC Server / Client](docs/rpc.md)
+
 ## Changes
 
 Breaking changes are annotated [here](docs/migrations.md).
 
 To quickly check if your service is susceptible to a known issue have a look [here](docs/migrations.md).
 
 ## Coding Standard
@@ -31,23 +36,24 @@
 
 ## Features
 
 The openmodule package provides a lot of features:
 
 ### Settings
 
-The openmodule package uses a global lazy configuration `openmodule.config.settings`. 
-This setting includes some standard parameters defined in `openmodule.config.GlobalSettings` and parameters from a customizable module.
-To specify the module you can call `settings.configure(module)` or you can set the environment variable `SETTINGS_MODULE`.
-Per default settings looks for the `config` module (it also looks for the `tests/config` module first for test cases)
+The openmodule package uses a global lazy configuration `openmodule.config.settings`. This setting includes some
+standard parameters defined in `openmodule.config.GlobalSettings` and parameters from a customizable module. To specify
+the module you can call `settings.configure(module)` or you can set the environment variable `SETTINGS_MODULE`. Per
+default settings looks for the `config` module (it also looks for the `tests/config` module first for test cases)
 
 #### Models
 
-Inherit from `OpenModuleModel` or in case of ZMQ messages from `ZMQMessage`.
-Models use pydantic ([docs](https://pydantic-docs.helpmanual.io/usage/types/)), check openmodule.models.* for some examples (e.g. PresenceBaseMessage for alias)
+Inherit from `OpenModuleModel` or in case of ZMQ messages from `ZMQMessage`. Models use
+pydantic ([docs](https://pydantic-docs.helpmanual.io/usage/types/)), check openmodule.models.* for some examples (e.g.
+PresenceBaseMessage for alias)
 
 ### Core
 
 The base of the new openmodule, every package should have exactly one. The core handles various things:
 
 * sentry
 * logging
@@ -147,15 +153,17 @@
 rpc_server.register_handler("backend", "auth", request_class=AccessRequest,
                             response_class=AccessResponse, handler=handler, register_schema=True)
 rpc.run()
 ```
 
 ### Utils
 
-#### Api
+#### Api (**DEPRECATED**)
+
+
 
 We implemented a very basic Api class you can use for http request and that handles errors and authentication. Either
 inherit it or create a class.
 
 ```python
 api = Api(**kwargs)
 try:
@@ -204,14 +212,56 @@
 Helper class for listening to presence messages.
 
 ```python
 presence_listener = PresenceListener(core.messages)
 presence_listener.on_enter.append(some_function)
 ```
 
+#### Package Reader
+
+Helper class to read settings (env, yml) of specified services. The services are only considered valid and parsed if a revision file for the service exists.
+Functions: 
+* **installed_services:** Returns a list of installed services, based on prefix
+* **load_setting:** Loads the setting of a single service
+* **load_with_service_prefix:** Loads the setting of all services starting with the prefix (no or empty prefix means no filter)
+* **load_with_hardware_type_prefix:** Load the setting of all services with the given hardware type (i.e. `cam-ip`)
+* **load_with_parent_type_prefix:**  Load the setting of all services with the given parent type (i.e. `cam-ip`)
+
+##### Bridged Slave Detection
+
+Some services behave differently if they are started on a bridged slave device. The function `is_bridged_slave()` is a helper function to detect this. To use this function on the device, you need to mount the dist folder (/opt/openmodule/dist2).
+The function returns:
+* None: No dist directory, no bridge service installed, multiple bridges installed
+* True: Bridge service is installed and `MASTER` is set there
+* False: Bridge service is installed and `MASTER` is not set there
+
+You can also set the env variable `BRIDGED_SLAVE` to True/False directly, so you do not need to care about the service settings.
+This is useful for testing (@override_settings(BRIDGED_SLAVE=True)) or running local (set env var BRIDGED_SLAVE)
+
+### Anonymization
+
+The openmodule framework uses rpc requests and messages to trigger the anonymization of data.
+* **Message:** You can send a AnonymizeMessage (topic: `privacy`). The message includes a session_id and vehicle_ids to delete
+* **RPC Request:** You can send an AnonymizeRequest with channel=`privacy`, type=`anonymize` to the DSGVO container. This session only includes session_ids.
+The DSGVO container will then match vehicle_ids to the session_ids and redistribute the request with the prior mentioned message.
+
+A container with sensible data then needs to implement the message listener for the privacy messages:
+
+**Example:**
+```python
+core.messages.register("privacy", AnonymizeMessage, anonymize_data)
+
+def anonymize_data(message: AnonymizeMessage):
+    for vid in message.vehicle_ids:
+        delete_vehicle_image_by_vehicle_id(vid)
+```
+
+**IMPORTANT** You still have to take care of data retention in each service separately, meaning you have to delete data independently of these anonymization messages.
+i.e. the DSGVO service deletes data if we need disk space or the eventlog deletes events after 30 days by default 
+
 ## Documentation
 
 Openmodule >= 3.0.5 features automatic generation of Rpc and Message Schemas including their models. The generation uses
 data that is generated during the test runs to create an OpenApi Schema. Your RPCs and Message handlers are
 automatically documented if:
 
 * You use the message dispatcher of the core (OpenModuleCoreTestMixin)
```

### Comparing `openmodule-9.0.0rc9/README.md` & `openmodule-9.1.0/openmodule.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,33 @@
+Metadata-Version: 2.1
+Name: openmodule
+Version: 9.1.0
+Summary: Libraries for developing the arivo openmodule
+Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
+Author: ARIVO
+Author-email: support@arivo.co
+License: GNU General Public License v2 (GPLv2)
+Keywords: arivo openmodule
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: test
+License-File: LICENSE
+
 # OpenModule V2
 
+Some additional documentation:
+
+* [Openmodule Core](docs/core.md)
+* [RPC Server / Client](docs/rpc.md)
+
 ## Changes
 
 Breaking changes are annotated [here](docs/migrations.md).
 
 To quickly check if your service is susceptible to a known issue have a look [here](docs/migrations.md).
 
 ## Coding Standard
@@ -12,23 +36,24 @@
 
 ## Features
 
 The openmodule package provides a lot of features:
 
 ### Settings
 
-The openmodule package uses a global lazy configuration `openmodule.config.settings`. 
-This setting includes some standard parameters defined in `openmodule.config.GlobalSettings` and parameters from a customizable module.
-To specify the module you can call `settings.configure(module)` or you can set the environment variable `SETTINGS_MODULE`.
-Per default settings looks for the `config` module (it also looks for the `tests/config` module first for test cases)
+The openmodule package uses a global lazy configuration `openmodule.config.settings`. This setting includes some
+standard parameters defined in `openmodule.config.GlobalSettings` and parameters from a customizable module. To specify
+the module you can call `settings.configure(module)` or you can set the environment variable `SETTINGS_MODULE`. Per
+default settings looks for the `config` module (it also looks for the `tests/config` module first for test cases)
 
 #### Models
 
-Inherit from `OpenModuleModel` or in case of ZMQ messages from `ZMQMessage`.
-Models use pydantic ([docs](https://pydantic-docs.helpmanual.io/usage/types/)), check openmodule.models.* for some examples (e.g. PresenceBaseMessage for alias)
+Inherit from `OpenModuleModel` or in case of ZMQ messages from `ZMQMessage`. Models use
+pydantic ([docs](https://pydantic-docs.helpmanual.io/usage/types/)), check openmodule.models.* for some examples (e.g.
+PresenceBaseMessage for alias)
 
 ### Core
 
 The base of the new openmodule, every package should have exactly one. The core handles various things:
 
 * sentry
 * logging
@@ -128,15 +153,17 @@
 rpc_server.register_handler("backend", "auth", request_class=AccessRequest,
                             response_class=AccessResponse, handler=handler, register_schema=True)
 rpc.run()
 ```
 
 ### Utils
 
-#### Api
+#### Api (**DEPRECATED**)
+
+
 
 We implemented a very basic Api class you can use for http request and that handles errors and authentication. Either
 inherit it or create a class.
 
 ```python
 api = Api(**kwargs)
 try:
@@ -185,14 +212,56 @@
 Helper class for listening to presence messages.
 
 ```python
 presence_listener = PresenceListener(core.messages)
 presence_listener.on_enter.append(some_function)
 ```
 
+#### Package Reader
+
+Helper class to read settings (env, yml) of specified services. The services are only considered valid and parsed if a revision file for the service exists.
+Functions: 
+* **installed_services:** Returns a list of installed services, based on prefix
+* **load_setting:** Loads the setting of a single service
+* **load_with_service_prefix:** Loads the setting of all services starting with the prefix (no or empty prefix means no filter)
+* **load_with_hardware_type_prefix:** Load the setting of all services with the given hardware type (i.e. `cam-ip`)
+* **load_with_parent_type_prefix:**  Load the setting of all services with the given parent type (i.e. `cam-ip`)
+
+##### Bridged Slave Detection
+
+Some services behave differently if they are started on a bridged slave device. The function `is_bridged_slave()` is a helper function to detect this. To use this function on the device, you need to mount the dist folder (/opt/openmodule/dist2).
+The function returns:
+* None: No dist directory, no bridge service installed, multiple bridges installed
+* True: Bridge service is installed and `MASTER` is set there
+* False: Bridge service is installed and `MASTER` is not set there
+
+You can also set the env variable `BRIDGED_SLAVE` to True/False directly, so you do not need to care about the service settings.
+This is useful for testing (@override_settings(BRIDGED_SLAVE=True)) or running local (set env var BRIDGED_SLAVE)
+
+### Anonymization
+
+The openmodule framework uses rpc requests and messages to trigger the anonymization of data.
+* **Message:** You can send a AnonymizeMessage (topic: `privacy`). The message includes a session_id and vehicle_ids to delete
+* **RPC Request:** You can send an AnonymizeRequest with channel=`privacy`, type=`anonymize` to the DSGVO container. This session only includes session_ids.
+The DSGVO container will then match vehicle_ids to the session_ids and redistribute the request with the prior mentioned message.
+
+A container with sensible data then needs to implement the message listener for the privacy messages:
+
+**Example:**
+```python
+core.messages.register("privacy", AnonymizeMessage, anonymize_data)
+
+def anonymize_data(message: AnonymizeMessage):
+    for vid in message.vehicle_ids:
+        delete_vehicle_image_by_vehicle_id(vid)
+```
+
+**IMPORTANT** You still have to take care of data retention in each service separately, meaning you have to delete data independently of these anonymization messages.
+i.e. the DSGVO service deletes data if we need disk space or the eventlog deletes events after 30 days by default 
+
 ## Documentation
 
 Openmodule >= 3.0.5 features automatic generation of Rpc and Message Schemas including their models. The generation uses
 data that is generated during the test runs to create an OpenApi Schema. Your RPCs and Message handlers are
 automatically documented if:
 
 * You use the message dispatcher of the core (OpenModuleCoreTestMixin)
@@ -213,7 +282,10 @@
 With default parameters, you need to document your handler functions with a doc string, that is then included as a
 description.
 
 ## Testing
 
 A separate package for testing openmodule packages exists within openmodule - openmodule-test. For more infos
 see [here](docs/testing.md)
+
+
+
```

### Comparing `openmodule-9.0.0rc9/docs/coding_standard.md` & `openmodule-9.1.0/docs/coding_standard.md`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/docs/database.md` & `openmodule-9.1.0/docs/database.md`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/docs/known_issues.md` & `openmodule-9.1.0/docs/known_issues.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Known Issues
 
 Similar to the changelog, we write a list of known issues here, so it is easy to identify issues for a particular
 version. The changelog may contain many other notes aswell.
 
 The version numbers below always note the _version through which the issue was fixed_.
 
+## 9.0.0
+
+* Under certain conditions calling the rpc client from a RPC Server or Message handler could cause a deadlock until the
+  timout occurs
+* Up until this version the rpc client had a potential race condition where the result of the first RPC request was not
+  received, even tough the called service responded. This has been fixed by calling `wait_for_connection` on any new
+  channels.
+
 ## 8.1.2
 
 * the main test mixin and it's utility function manipulated low level python things and could break the test runner
   under certain circumstances.
 * the rpc test server mixin's `wait_for_rpc_server` function did not work if a RPC handler was registered without a type
   filter. It now uses the same approach as `wait_for_dispatcher` by assuming that if the last subscribed topic works,
   all previously subscribed topics will work too.
```

### Comparing `openmodule-9.0.0rc9/docs/migrations.md` & `openmodule-9.1.0/docs/migrations.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 # Breaking Version Changes
 
 ## 9.0.0
 
 This version refactored the RPC client, especially asynchronous retrieval of rpc results. See
-the [RPC Documentation](./rpc.md) for more information about asynchronous rpc calls and the RPC Client.
+the [RPC Documentation](./rpc.md) for more information about asynchronous rpc calls and the RPC Client. Critically the
+common issue of "cannot do RPC's while inside an RPC handler" has been solved by creating a dedicated thread for the rpc
+client and some future openmodule core internals which should not be blocked by badly behaving user code anyways.
 
 * the `RPCClient.check_results()` function was removed, and is replaced by a `.result()`.
+* The RPCClient together with the HealthHandler how has a dedicated thread in the open module core. It is discouraged to
+  create an rpc client of your own. Please use the rpc client of openmodule core. A deprecation warning hints this also.
 
 Also some things have been deprecated and will be removed
 
+* the RPC Server no longer requires a config object to be passed. It takes the global openmodule settings instead.
 * the RPC Client now warns if a `OpenModuleCore` is passed to it's constructor
 * the RPC Client now warns if a dictionary is used for RPC requests
 * MockEvent's `reset_call_count()` and `reset_all_call_counts()` was replaced by analog `reset_mock()`
   and `reset_all_mocks()`
 
 Furthermore, fields were renamed in python (with aliases, so the serialized version stays the same):
 
 * `Backend -> AccessRequest: id -> medium_id`
 * `Backend -> MediumAccesses: id -> medium_id, type -> medium_type`
 * `Backend -> CountMessage: id -> medium_id`
 * `Backend -> CountMessage: previous_id ->  previous_medium_id`
 
 In the backend test utils the `create_access_request()` method was removed.
 
+The default value for `match_type` in `MessageDispatcher.register_handler` is now `True`.
+
+The `api` class, aswell as the test utils were removed from the framework. You can still find it
+in [docs/deprecated_code/api](./deprecated_code/README.md) if you used it in your service.
+
 ## 8.1.1
 
 This version includes breaking changes for testcases only.
 
 * The main test mixin was refactored and `exception_in_function` was removed.
 
 ## 8.0.0
```

### Comparing `openmodule-9.0.0rc9/docs/testing.md` & `openmodule-9.1.0/docs/testing.md`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/alert.py` & `openmodule-9.1.0/openmodule/alert.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/checks.py` & `openmodule-9.1.0/openmodule/checks.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/config.py` & `openmodule-9.1.0/openmodule/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
     if "DEBUG" in os.environ:
         return bool("DEBUG", default=False)
     elif testing():
         return False
     else:
         return version() == "unknown" and not _inside_docker()
 
+def bridged_slave():
+    if "BRIDGED_SLAVE" in os.environ:
+        return bool("BRIDGED_SLAVE", default=False)
+    else:
+        return None
 
 def settings_module():
     if testing() and os.path.exists("../tests/config.py"):
         return string("SETTINGS_MODULE", "tests.config")
     return string("SETTINGS_MODULE", "config")
 
 
@@ -379,15 +384,20 @@
     def clear_override(self, **options):
         for k in options.keys():
             if self.overrides.get(k):
                 self.overrides[k].pop()
                 if self.lazy_setting is not None:
                     if len(self.overrides[k]) == 1:
                         self.lazy_setting._wrapped._explicit_settings.remove(k)
-                    setattr(self.lazy_setting, k, self.overrides[k][-1])
+
+                    if len(self.overrides[k]) == 0:
+                        # deletes the attribute if it never existed in the base config in the first place
+                        delattr(self.lazy_setting, k)
+                    else:
+                        setattr(self.lazy_setting, k, self.overrides[k][-1])
 
     def set_base(self, lazy_setting, options):
         assert self.lazy_setting is None, "Do not use multiple settings"
         self.lazy_setting = lazy_setting
         overrides = {}
         for k, v in options.items():
             if self.overrides.get(k):
@@ -438,11 +448,12 @@
     DATABASE_FOLDER = database_folder()
 
     # broker env vars
     BROKER_SUB = broker_sub()
     BROKER_PUB = broker_pub()
 
     LOCAL_DEVELOPMENT = bool("LOCAL_DEVELOPMENT", False)
+    BRIDGED_SLAVE = bridged_slave()
 
 
 settings = LazySettings()
 _override_settings = OverrideSettings()
```

### Comparing `openmodule-9.0.0rc9/openmodule/core.py` & `openmodule-9.1.0/openmodule/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,106 @@
 import logging
 import os
 import shutil
 import signal
 import threading
+from concurrent.futures.thread import ThreadPoolExecutor
 from typing import Optional
 
 import zmq
 
 from openmodule.alert import AlertHandler
 from openmodule.config import validate_config_module
 from openmodule.database.database import Database
 from openmodule.dispatcher import ZMQMessageDispatcher
 from openmodule.health import HealthHandlerType, Healthz, HealthPingMessage
 from openmodule.logging import init_logging
 from openmodule.messaging import get_pub_socket, get_sub_socket, receive_message_from_socket, wait_for_connection
 from openmodule.models.base import ZMQMessage
-from openmodule.sentry import init_sentry
+from openmodule.sentry import init_sentry, should_activate_sentry, deinit_sentry
 from openmodule.threading import get_thread_wrapper
 
 
 class OpenModuleCore(threading.Thread):
     database: Optional[Database] = None
 
-    def __init__(self, context, config):
+    def __init__(self, context, config, messages_executor=None):
         super().__init__(target=get_thread_wrapper(self._run))
+        self.internal_thread = threading.Thread(target=get_thread_wrapper(self._run_internal))
+
         self.context = context
         self.config = config
+        self.sentry_was_initialized = False
 
         self.pub_lock = threading.Lock()
         self.sub_lock = threading.Lock()
 
         self.pub_socket = get_pub_socket(self.context, self.config, linger=1000)
         self.sub_socket = get_sub_socket(self.context, self.config)
-        self.messages = ZMQMessageDispatcher(self.sub_socket)
+        self.sub_socket_internal = get_sub_socket(self.context, self.config)
+
+        self.messages = ZMQMessageDispatcher(self.sub_socket, executor=messages_executor)
+        self._messages_internal = ZMQMessageDispatcher(self.sub_socket_internal)
 
         from openmodule.rpc import RPCClient
-        self.rpc_client = RPCClient(self.messages)
+        self.rpc_client = RPCClient(self._messages_internal, _warn=False)
 
         self.log = logging.getLogger(self.__class__.__name__)
         self.health = Healthz(self)
         self.alerts = AlertHandler(self)
-        self.messages.register_handler(b"healthz", HealthPingMessage, self.health.process_message,
-                                       match_type=True, register_schema=False)
-
-    def _subscribe(self, topic: bytes):
-        with self.sub_lock:
-            self.sub_socket.subscribe(topic)
+        self._messages_internal.register_handler(b"healthz", HealthPingMessage, self.health.process_message,
+                                                 match_type=True, register_schema=False)
 
     def init_database(self):
         if self.config.TESTING:
             self.database = Database(self.config.DATABASE_FOLDER, self.config.NAME, alembic_path="../src/database")
         else:
             self.database = Database(self.config.DATABASE_FOLDER, self.config.NAME)
 
+    def start(self) -> None:
+        super().start()
+        self.internal_thread.start()
+
+    def join(self, timeout: Optional[float] = None) -> None:
+        super().join(timeout)
+        self.internal_thread.join(timeout)
+
     def _run(self):
         try:
             while True:
                 topic, message = receive_message_from_socket(self.sub_socket)
                 self.messages.dispatch(topic, message)
         except zmq.ContextTerminated:
             self.log.debug("context terminated, core shutting down")
         finally:
-            self.pub_socket.close()
+            with self.pub_lock:
+                self.pub_socket.close()
             self.sub_socket.close()
 
+    def _run_internal(self):
+        try:
+            while True:
+                topic, message = receive_message_from_socket(self.sub_socket_internal)
+                self._messages_internal.dispatch(topic, message)
+        except zmq.ContextTerminated:
+            pass
+        finally:
+            self.sub_socket_internal.close()
+
     def publish(self, message: ZMQMessage, topic: bytes):
         with self.pub_lock:
             message.publish_on_topic(self.pub_socket, topic)
 
+    def shutdown(self):
+        self._messages_internal.shutdown(wait=True)
+        self.messages.shutdown(wait=True)
+        if self.database:
+            self.database.shutdown()
+        self.context.term()
+
 
 _core_thread: Optional[OpenModuleCore] = None
 
 
 def sigterm_handler(*_):
     raise KeyboardInterrupt()
 
@@ -92,33 +121,55 @@
             "\n"
             "        DEBUG MODE is active.\n"
             "        Deactivate by setting environment variable DEBUG=False.\n"
             "        Debug is disabled per default when a version string is set or ran inside docker.\n"
         )
 
 
-def init_openmodule(config, sentry=True, logging=True, dsgvo=True,
+def init_openmodule(config, sentry=None, logging=True, dsgvo=True,
                     health_handler: Optional[HealthHandlerType] = None,
-                    context=None, database=False, catch_sigterm=True) -> OpenModuleCore:
+                    context=None, database=False, catch_sigterm=True,
+                    dispatcher_max_threads=1) -> OpenModuleCore:
     context = context or zmq.Context()
     validate_config_module(config)
 
     global _core_thread
     assert not _core_thread, "openmodule core already running"
-    _core_thread = OpenModuleCore(context, config)
+
+    if dispatcher_max_threads > 1:
+        executor = ThreadPoolExecutor(max_workers=dispatcher_max_threads)
+    else:
+        executor = None
+
+    _core_thread = OpenModuleCore(context, config, messages_executor=executor)
     _core_thread.start()
 
     if logging:
         init_logging(_core_thread)
     print_environment(_core_thread)
 
     _core_thread.log.info("connecting to the message broker")
     wait_for_connection(_core_thread.messages, _core_thread.pub_socket, _core_thread.pub_lock)
+    wait_for_connection(_core_thread._messages_internal, _core_thread.pub_socket, _core_thread.pub_lock)
+    _core_thread.log.info("connection established")
 
-    if sentry:
+    # we activate sentry if
+    # -> sentry=None (default) -> then we only activate in production
+    # -> sentry=True/False this overrides and we activate/deactivate as desired
+    activate_sentry = False
+    if sentry is None:
+        if should_activate_sentry(config):
+            activate_sentry = True
+        else:
+            _core_thread.log.info("not activating sentry in debug or test mode")
+    else:
+        activate_sentry = sentry
+
+    if activate_sentry:
+        _core_thread.sentry_was_initialized = True
         init_sentry(_core_thread)
 
     if dsgvo:
         init_dsgvo_config()
 
     if health_handler:
         _core_thread.health.health_handler = health_handler
@@ -140,28 +191,29 @@
 def shutdown_openmodule():
     global _core_thread
     assert _core_thread is not None, (
         "core thread is not running, did you call init_openmodule(...)?\n"
         "if its a testcase, maybe you forgot to call super().setUp()"
     )
 
+    # we de-init sentry mostly to ensure consistency between testcases
+    if _core_thread.sentry_was_initialized:
+        deinit_sentry()
+
     signal.signal(signal.SIGTERM, signal.SIG_DFL)
     current_core: OpenModuleCore = _core_thread
     _core_thread = None
 
     shutdown_done = threading.Event()
 
     def last_will():
-        if not shutdown_done.wait(timeout=3):
+        if not shutdown_done.wait(timeout=10):
             os._exit(99)
 
     if not (current_core.config.TESTING or current_core.config.DEBUG):
         last_will_thread = threading.Thread(target=last_will)
         last_will_thread.setDaemon(True)
         last_will_thread.start()
 
-    if current_core.database:
-        current_core.database.shutdown()
-
-    current_core.context.term()
+    current_core.shutdown()
     current_core.join()
     shutdown_done.set()
```

### Comparing `openmodule-9.0.0rc9/openmodule/database/custom_types.py` & `openmodule-9.1.0/openmodule/database/custom_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from datetime import datetime
+
 from sqlalchemy import DateTime
 from sqlalchemy.sql.visitors import VisitableType
 from sqlalchemy.types import TypeDecorator
 
 
 class MetaOptions(VisitableType):
     """
@@ -32,9 +34,11 @@
 
 
 class TZDateTime(CustomType):
     impl = DateTime
 
     def process_bind_param(self, value, dialect):
         if value is not None:
-            assert value.tzinfo is None, "You need to convert a datetime to a naive time, because sqlite loses tz infos"
+            assert not isinstance(value, datetime) or value.tzinfo is None, (
+                "You need to convert a datetime to a naive time, because sqlite loses tz infos. "
+            )
         return value
```

### Comparing `openmodule-9.0.0rc9/openmodule/database/database.py` & `openmodule-9.1.0/openmodule/database/database.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/database/env.py` & `openmodule-9.1.0/openmodule/database/env.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/dispatcher.py` & `openmodule-9.1.0/openmodule/dispatcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,63 @@
+import gzip
+import json
 import logging
+import threading
 import warnings
 from collections import defaultdict
-from typing import Union, Optional, Callable, DefaultDict, List, Dict, TypeVar, Type, Any, Generic
+from concurrent.futures._base import Executor
+from concurrent.futures.process import ProcessPoolExecutor
+from concurrent.futures.thread import ThreadPoolExecutor
+from pathlib import Path
+from typing import Union, Optional, Callable, DefaultDict, List, Dict, TypeVar, Type, Generic
 
 import zmq
 from pydantic import ValidationError, BaseModel
 
 from openmodule.config import settings
 from openmodule.models.base import ZMQMessage
 from openmodule.utils.schema import Schema
 
 
+class DummyExecutor(Executor):
+    def __init__(self):
+        self._shutdown = False
+        self._shutdown_lock = threading.Lock()
+
+    def submit(self, fn, *args, **kwargs):
+        with self._shutdown_lock:
+            if self._shutdown:
+                raise RuntimeError('cannot schedule new futures after shutdown')
+
+            fn(*args, **kwargs)
+
+    def shutdown(self, wait=True):
+        if wait:
+            with self._shutdown_lock:
+                self._shutdown = True
+        else:
+            self._shutdown = True
+
+
 class Listener:
-    def __init__(self, message_class: Type[ZMQMessage], filter: Optional[Dict], handler: Callable):
+    def __init__(self, message_class: Type[ZMQMessage], type: Optional[str], filter: Optional[Callable],
+                 handler: Callable):
         self.filter = filter
         self.handler = handler
+        self.type = type
         self.message_class = message_class
 
     def matches(self, message: Dict):
-        if self.filter is None:
-            return True
+        if self.type and message.get("type") != self.type:
+            return False
+
+        if self.filter:
+            return self.filter(message)
         else:
-            return message.items() >= self.filter.items()
+            return True
 
 
 EventArgs = TypeVar("EventArgs")
 
 
 class EventListener(Generic[EventArgs], list):
     """
@@ -52,27 +84,52 @@
                     self.log.exception(e)
 
 
 ZMQMessageSub = TypeVar('ZMQMessageSub', bound=ZMQMessage)
 
 
 class MessageDispatcher:
-    def __init__(self, name=None, *, raise_validation_errors=False, raise_handler_errors=False):
+    def __init__(self, name=None, *, raise_validation_errors=False, raise_handler_errors=False,
+                 executor: Optional[Executor] = None):
         """
         :param name: optionally name the dispatcher for logging purposes
         :param raise_validation_errors: if true and received messages do not match a validation error is raised,
                                         this is useful in restricive code or testcases
         :param raise_handler_errors: if true and a message handler raises an exception, the exception is raised,
                                      this is useful in restricive code or testcases
         """
+
+        assert executor is None or not (raise_handler_errors or raise_validation_errors), (
+            "raise errors is only supported if no executor is used."
+        )
+
         self.name = name
         self.log = logging.getLogger(f"{self.__class__.__name__}({self.name})")
         self.listeners: DefaultDict[bytes, List[Listener]] = defaultdict(list)
         self.raise_validation_errors = raise_validation_errors
         self.raise_handler_errors = raise_handler_errors
+        self.executor = executor or DummyExecutor()
+
+    @property
+    def is_multi_threaded(self):
+        if isinstance(self.executor, DummyExecutor):
+            return False
+
+        if isinstance(self.executor, (ThreadPoolExecutor, ProcessPoolExecutor)):
+            # noinspection PyProtectedMember
+            if self.executor._max_workers > 1:
+                return True
+            else:
+                return False
+
+        # unknown executor? assume multithreaded
+        return True
+
+    def shutdown(self, wait=True):
+        self.executor.shutdown(wait=wait)
 
     def unregister_handler(self, listener: Listener):
         for topic, listeners in self.listeners.items():
             try:
                 listeners.remove(listener)
             except ValueError:
                 pass
@@ -86,53 +143,69 @@
             return True
         else:
             return False
 
     def register_handler(self, topic: Union[bytes, str],
                          message_class: Type[ZMQMessageSub],
                          handler: Callable[[ZMQMessageSub], None], *,
-                         filter: Optional[Dict] = None,
-                         match_type=False,
+                         filter: Optional[Union[Dict, Callable[[Dict], bool]]] = None,
+                         match_type=True,
                          register_schema=True):
         """
         registers a message handler. without any filters all messages from the topic are
         sent to the message handler.
         :param filter: a dictionary of values which must match in order for the message to
                        be further processed
         :param match_type: if set to true the message_class's type field is used as a filter.
                            equivalent to setting filter={"type": message_class.fields["type"].default}
         """
 
         if hasattr(topic, "encode"):
             topic = topic.encode()
 
+        # deprecation warning for old style filters
+        if isinstance(filter, dict):
+            warnings.warn(
+                "\n\nDict-style filters are deprecated and will be removed in the next version. Please migrate to\n"
+                "using function-style filters. For an equal filter (albeit maybe an ugly solution) you can\n"
+                "use\n"
+                f"  register_handler(..., filter=lambda msg: (msg.items() >= {filter}.items())\n"
+                "\n"
+                "If you were previously filtering for gate+direction you now HAVE TO re-write your filter to \n"
+                "**only match the gate name** and **not the direction!**\n", stacklevel=3
+            )
+            filter_dict = filter
+            filter = lambda msg: (msg.items() >= filter_dict.items())
+
         if match_type:
             assert "type" in message_class.__fields__ and message_class.__fields__["type"].default, (
-                "Your message class definition does not set a `type` field, or the type field "
-                "does not have a default value!"
+                "\n\nYour message class definition does not set a `type` field, or the type field "
+                "does not have a default value! To receive all message type pass `match_type=False` to "
+                "`register_handler`. Otherwise please define a `type` for your message class."
             )
-            filter = filter or {}
-            filter["type"] = message_class.__fields__["type"].default
+            type = message_class.__fields__["type"].default
+        else:
+            type = None
 
-        listener = Listener(message_class, filter, handler)
+        listener = Listener(message_class, type, filter, handler)
         self.listeners[topic].append(listener)
 
         if register_schema and not self._is_test_handler(handler):
             Schema.save_message(topic, message_class, handler, filter)
 
         return listener
 
     def dispatch(self, topic: bytes, message: Union[Dict, BaseModel]):
         if isinstance(message, BaseModel):
             message = message.dict()
 
         listeners = self.listeners.get(topic, [])
         for listener in listeners:
             if listener.matches(message):
-                self.execute(listener, message)
+                self.executor.submit(self.execute, listener, message)
 
     def execute(self, listener: Listener, message: Dict):
         try:
             parsed_message = listener.message_class.parse_obj(message)
         except ValidationError as e:
             if self.raise_validation_errors:
                 raise e from None
@@ -148,26 +221,27 @@
                     raise e from None
                 else:
                     self.log.exception("Error in message handler")
 
 
 class SubscribingMessageDispatcher(MessageDispatcher):
     def __init__(self, subscribe: Callable[[bytes], None], name=None, *, raise_validation_errors=False,
-                 raise_handler_errors=False, unsubscribe: Optional[Callable[[bytes], None]] = None):
+                 raise_handler_errors=False, unsubscribe: Optional[Callable[[bytes], None]] = None,
+                 executor: Optional[Executor] = None):
         super().__init__(name=name, raise_validation_errors=raise_validation_errors,
-                         raise_handler_errors=raise_handler_errors)
+                         raise_handler_errors=raise_handler_errors, executor=executor)
         self.subscribe = subscribe
         self.unsubscribe = unsubscribe
 
     def register_handler(self, topic: Union[bytes, str],
                          message_class: Type[ZMQMessageSub],
                          handler: Callable[[ZMQMessageSub], None], *,
                          filter: Optional[Dict] = None,
                          register_schema=True,
-                         match_type=False):
+                         match_type=True):
         if topic and hasattr(topic, "encode"):
             topic = topic.encode()
         self.subscribe(topic)
         return super().register_handler(topic, message_class, handler, filter=filter,
                                         register_schema=register_schema, match_type=match_type)
 
     def unregister_handler(self, listener: Listener):
@@ -185,15 +259,74 @@
         if warn_no_unsubscribe:
             warnings.warn("All handlers were unregistered from a topic, but no unsubscribe method was configured. "
                           "This may cause a performance overhead if too many unused subscriptions are kept. "
                           "Consider passing a unsubscribe method.", UserWarning, stacklevel=2)
 
 
 class ZMQMessageDispatcher(SubscribingMessageDispatcher):
-    def __init__(self, sub_socket: zmq.Socket, name=None, *, raise_validation_errors=False, raise_handler_errors=False):
+    def __init__(self, sub_socket: zmq.Socket, name=None, *, raise_validation_errors=False, raise_handler_errors=False,
+                 executor: Optional[Executor] = None):
         super().__init__(
             subscribe=lambda x: sub_socket.subscribe(x),
             unsubscribe=lambda x: sub_socket.unsubscribe(x),
             name=name,
             raise_validation_errors=raise_validation_errors,
-            raise_handler_errors=raise_handler_errors
+            raise_handler_errors=raise_handler_errors,
+            executor=executor
         )
+
+
+class DeeplogMessageDispatcher(MessageDispatcher):
+    def __init__(self, path: Union[Path, str], name=None, *, raise_validation_errors=False, raise_handler_errors=False,
+                 executor: Optional[Executor] = None):
+        super().__init__(name, raise_validation_errors=raise_validation_errors,
+                         raise_handler_errors=raise_handler_errors, executor=executor)
+        if not isinstance(path, Path):
+            path = Path(path)
+
+        assert path.is_dir()
+        self.path = path
+        self.current_timestamp = None
+
+    def dispatch_hour(self, date_string):
+        logging.info(f"Dispatching {date_string}")
+        # prefer .gz files over .log since gz are finished
+        gz_path = self.path / f"hour_{date_string}.log.gz"
+        raw_path = self.path / f"hour_{date_string}.log"
+        file_handle = None
+
+        try:
+            if gz_path.exists():
+                file_handle = gzip.open(gz_path, "rb")
+
+            elif raw_path.exists():
+                file_handle = open(raw_path, "rb")
+
+            else:
+                raise FileNotFoundError(f"log file for hour {date_string} does not exist")
+
+            try:
+                for line in file_handle.readlines():
+                    try:
+                        topic, message = json.loads(line)
+                    except:
+                        logging.warning("broken message skipped")
+                    else:
+                        self.current_timestamp = message.get("timestamp")
+                        self.dispatch(topic.encode(), message)
+            except EOFError as e:
+                logging.error(str(e))
+
+        finally:
+            if file_handle:
+                file_handle.close()
+
+    def dispatch_all(self):
+        hours = []
+        for file in self.path.iterdir():
+            if file.is_file() and file.name.startswith("hour_"):
+                date_string = file.name[5:].split(".")[0]
+                hours.append(date_string)
+
+        hours.sort()
+        for hour in hours:
+            self.dispatch_hour(hour)
```

### Comparing `openmodule-9.0.0rc9/openmodule/health.py` & `openmodule-9.1.0/openmodule/health.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/messaging.py` & `openmodule-9.1.0/openmodule/messaging.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,33 +22,40 @@
 def get_pub_socket(context, config, linger=100) -> zmq.Socket:
     socket = context.socket(zmq.PUB)
     socket.setsockopt(zmq.LINGER, linger)
     socket.connect(config.BROKER_SUB)
     return socket
 
 
-def wait_for_connection(dispatcher: MessageDispatcher, pub_socket, pub_lock=None, timeout=100):
+def wait_for_connection(dispatcher: MessageDispatcher, pub_socket=None, pub_lock=None, timeout=100):
     """
     waits until the pub_socket's messages can be received at the dispatcher.
     This dispatcher needs to run in a separate thread as this method is blocking
     :param pub_lock: optionally locks the lock during publishing
     """
 
+    if pub_socket is None:
+        from openmodule.core import core
+        current_core = core()
+        assert current_core, "either a core must be running or you have to pass a pub_socket"
+        pub_socket = current_core.pub_socket
+        pub_lock = current_core.pub_lock
+
     pub_lock = pub_lock or contextlib.nullcontext()
     received = False
 
     def handler(_):
         nonlocal received
         received = True
 
     # topic needs to start with __ping because these messages are ignored by the deeplog
     random_topic = "__ping_" + "".join(random.choices(string.ascii_letters, k=10))
     random_topic = random_topic.encode()
 
-    listener = dispatcher.register_handler(random_topic, ZMQMessage, handler, register_schema=False)
+    listener = dispatcher.register_handler(random_topic, ZMQMessage, handler, register_schema=False, match_type=False)
 
     check_delay = 0.1
     check_iterations = int(timeout / check_delay) + 1
 
     message = ZMQMessage(type="connection-check")
     for x in range(check_iterations):
         with pub_lock:
```

### Comparing `openmodule-9.0.0rc9/openmodule/models/alert.py` & `openmodule-9.1.0/openmodule/models/alert.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/models/backend.py` & `openmodule-9.1.0/openmodule/models/backend.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/models/base.py` & `openmodule-9.1.0/openmodule/models/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import base64
+import binascii
 import re
 from datetime import datetime
+from decimal import Decimal
 from enum import Enum
 from json.encoder import ESCAPE_ASCII
 
 import orjson
 import zmq
 from dateutil.tz import UTC
 from pydantic import Field, BaseModel, validator
@@ -41,26 +43,32 @@
         return '\\u%04x\\u%04x' % (s1, s2)
 
 
 def _unicode_escape(data):
     return ESCAPE_ASCII.sub(replace, data)
 
 
+def default(obj):
+    if isinstance(obj, Decimal):
+        return str(obj)
+    raise TypeError
+
+
 class OpenModuleModel(BaseModel, **meta_kwargs):
     class Config:
         validate_assignment = True
 
         json_loads = orjson.loads
         json_dumps = _donotuse
 
     def json_bytes(self):
         data = self.dict()
         if self.__custom_root_type__:
             data = data[ROOT_KEY]
-        return _unicode_escape(orjson.dumps(data).decode()).encode("ascii")
+        return _unicode_escape(orjson.dumps(data, default=default).decode()).encode("ascii")
 
     def dict(self, **kwargs):
         kwargs.setdefault("by_alias", True)
         kwargs.setdefault("exclude_none", True)
         return super().dict(**kwargs)
 
 
@@ -75,19 +83,20 @@
         return dt
 
 
 def timezone_validator(field):
     return validator(field, allow_reuse=True)(_timezone_validator)
 
 
-def _base64_validator(cls, string: str, values, **kwargs):
-    if base64.b64encode(base64.b64decode(string)).decode("utf-8") == string:
-        return string
-    else:
-        raise ValueError("'payload' must be base64-encoded")
+def _base64_validator(cls, data, values, **kwargs):
+    try:
+        base64.b64decode(data)
+    except (binascii.Error, TypeError, ValueError):
+        raise ValueError("must be a bse64 string")
+    return data
 
 
 def base64_validator(field):
     return validator(field, allow_reuse=True)(_base64_validator)
 
 
 _EPOCH_UTC = datetime(1970, 1, 1, tzinfo=UTC)
```

### Comparing `openmodule-9.0.0rc9/openmodule/models/io.py` & `openmodule-9.1.0/openmodule/models/io.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/models/presence.py` & `openmodule-9.1.0/openmodule/models/presence.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,35 @@
 class PresenceMedia(OpenModuleModel):
     lpr: Optional[LPRMedium]
     qr: Optional[Medium]
     nfc: Optional[Medium]
     pin: Optional[Medium]
 
 
-class PresenceBaseMessage(ZMQMessage):
+class PresenceBaseData(OpenModuleModel):
     vehicle_id: int
     source: str
     present_area_name: str = Field(..., alias="present-area-name")
     last_update: datetime
     gateway: Gateway
     medium: PresenceMedia
     make_model: Optional[MakeModel]
     all_ids: PresenceAllIds
 
     _tz_last_update = timezone_validator("last_update")
 
+    class Config:
+        # allows setting attributes both via the alias, and the field name.
+        # is used to rename old variables which are hard to understand by their name (e.g. id -> medium id)
+        allow_population_by_field_name = True
+
+
+class PresenceBaseMessage(PresenceBaseData, ZMQMessage):
+    pass
+
 
 class PresenceBackwardMessage(PresenceBaseMessage):
     type: str = "backward"
     unsure: bool = False
     leave_time: datetime = Field(..., alias="leave-time")
     bidirectional_inverse: bool = False
 
@@ -53,7 +62,15 @@
 class PresenceEnterMessage(PresenceBaseMessage):
     type: str = "enter"
 
 
 class PresenceChangeMessage(PresenceBaseMessage):
     type: str = "change"
     change_vehicle_id: Optional[bool]
+
+
+class PresenceRPCRequest(OpenModuleModel):
+    gate: str
+
+
+class PresenceRPCResponse(OpenModuleModel):
+    presents: List[PresenceBaseData]
```

### Comparing `openmodule-9.0.0rc9/openmodule/models/validation.py` & `openmodule-9.1.0/openmodule/models/validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,83 @@
-from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
-from openmodule.models.base import OpenModuleModel, ZMQMessage, timezone_validator, base64_validator, \
-    datetime_to_timestamp
+from openmodule.models.base import OpenModuleModel, ZMQMessage, base64_validator, Gateway
 
 
-class ValidationProviderRequestTicketType(str, Enum):
+class ValidateRequestTicketType(str, Enum):
     qr = "qr"
+    nfc = "nfc"
 
 
-class ValidationProviderResponseState(str, Enum):
+class ValidateResponseState(str, Enum):
     ok = "ok"
     not_applicable = "not_applicable"
 
 
-class ValidationProviderResponseCommonError(str, Enum):
-    # unique validation id was already used
+class ValidateResponseError(str, Enum):
+    # the ticket is valid but it was already used once and cannot be used multiple times
     already_used = "already_used"
-    # e.g. signature validation error
+
+    # the ticket is invalid, e.g. the signature is incorrect
     invalid = "invalid"
+
+    # the ticket is valid, but cannot be used for various reasons, please provide more
+    # information in the `message` field in this case.
+    excluded = "excluded"
+
+    # is expired or cannot be used at this point in time
     expired = "expired"
-    outside_timewindow = "outside_timewindow"
+
+    # an unknown error has occured while processing the ticket
+    unknown_error = "unknown_error"
 
 
-class ValidationProviderRegisterRequestMessage(ZMQMessage):
+class ValidationRegisterRequestMessage(ZMQMessage):
     """
     sent by the controller as a request to all validation providers
     each validation provider who wants to register itself at the controller has to answer
     with a register message
     """
     type: str = "register_request"
 
 
-class ValidationProviderRegisterMessage(ZMQMessage):
+class ValidationRegisterMessage(ZMQMessage):
     """
     sent by a validation provider if it wants to register itself at the controller
     """
     type: str = "register"
 
 
-class ValidationProviderUnregisterMessage(ZMQMessage):
+class ValidationUnregisterMessage(ZMQMessage):
     """
     sent by a validation provider if it shuts down and wants to unregister itself
     """
     type: str = "unregister"
 
 
 class ValidateRequest(OpenModuleModel):
     name: str
-    occupant_id: str
-    type: ValidationProviderRequestTicketType
-    # payload has to be base64 encoded
+    session_id: str
+    type: ValidateRequestTicketType
     payload: str
+    gateway: Optional[Gateway]
 
     _b64_payload = base64_validator("payload")
 
 
-class ValidateResponseError(OpenModuleModel):
-    type: ValidationProviderResponseCommonError
-    start: Optional[datetime]
-    end: Optional[datetime]
-
-    _tz_start = timezone_validator("start")
-    _tz_end = timezone_validator("end")
-
-    def dict(self, **kwargs):
-        data = super().dict(**kwargs)
-        if data.get("start") is not None:
-            data["start"] = datetime_to_timestamp(data["start"])
-        if data.get("end") is not None:
-            data["end"] = datetime_to_timestamp(data["end"])
-        return data
-
-
 class ValidateCostEntry(OpenModuleModel):
-    # common parameters
     group: Optional[str] = None
-
-    # if None, source will be set to service name on default: e.g. "service_iocontroller"
-    source: Optional[str] = None
-
-    # product item switches
+    source: Optional[str] = None  # if None, source will be set to service name on default: e.g. "service_iocontroller"
     product_item_id: Optional[str] = None
-
-    # enable/disable the cost group
     active: Optional[bool] = None
-
-    # time validations
     delta_time_seconds: Optional[int] = None
-
-    # amount payments
     delta_amount: Optional[int] = None
-
-
-class ValidateResponseCostEntry(ValidateCostEntry):
-    # common parameters
     source_id: Optional[str] = None
     idempotency_key: Optional[str] = None
 
 
 class ValidateResponse(OpenModuleModel):
-    occupant_id: str
-    state: ValidationProviderResponseState
+    state: ValidateResponseState
     error: Optional[ValidateResponseError]
     cost_entries: Optional[List[dict]]
+    message: Optional[str]
```

### Comparing `openmodule-9.0.0rc9/openmodule/models/vehicle.py` & `openmodule-9.1.0/openmodule/models/vehicle.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,14 +109,17 @@
         if self.qr:
             yield self.qr
         if self.nfc:
             yield self.nfc
         if self.pin:
             yield self.pin
 
+    def has_media(self):
+        return bool(self.lpr or self.qr or self.nfc or self.pin)
+
     def __str__(self):
         media = ", ".join(str(x) for x in [self.lpr, self.qr, self.nfc] if x)
         if media:
             media = ", " + media
         if self.make_model:
             media += (" " if media else "") + str(self.make_model)
         return f"Vehicle<id:{str(self.id)[-7:]}{media}>"
```

### Comparing `openmodule-9.0.0rc9/openmodule/rpc/client.py` & `openmodule-9.1.0/openmodule/rpc/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from uuid import uuid4
 
 from pydantic import BaseModel
 
 from openmodule.config import settings
 from openmodule.core import OpenModuleCore, core
 from openmodule.dispatcher import MessageDispatcher
+from openmodule.messaging import wait_for_connection
 from openmodule.models.rpc import RPCResponse, RPCRequest, RPCResult
 from openmodule.rpc.common import channel_to_response_topic, channel_to_request_topic
 
 
 class RPCClient:
     class RPCEntry:
         def __init__(self, timeout):
@@ -42,46 +43,58 @@
 
                 if not self.ready.wait(timeout=maximum_wait_time):
                     raise TimeoutError()
 
                 assert self.response is not None, "internal error, this must not happen"
                 return self.response
 
-    def __init__(self, dispatcher: Union[OpenModuleCore, MessageDispatcher], channels=None, default_timeout=3.):
+    def __init__(self, dispatcher: Union[OpenModuleCore, MessageDispatcher], channels=None, default_timeout=3.,
+                 _warn=True):
         # TODO: backwards compatibiltiy, remove in next major version
         if isinstance(dispatcher, OpenModuleCore):
             warnings.warn(
                 '\n\npassing an `OpenModuleCore` instance to the RPC Client is deprecated. Please migrate to '
                 'passing a `MessageDispatcher` instead.\n',
                 DeprecationWarning, stacklevel=2
             )
             dispatcher = dispatcher.messages
         # backwards compatibiltiy
 
+        # the new design with one dedicated thread for the rpc client in the core discourages instantiating the
+        # rpc client on its own. so we warn every user about this
+        if _warn:
+            warnings.warn(
+                "\n\nInstantiating the RPC Client on your own is discouraged. PLease use the open module core's rpc "
+                "client. For testcases or if you absolutely MUST for whatever reason instantiate the client pass "
+                "`_warn=False` to the constructor.", DeprecationWarning, stacklevel=2
+            )
+
         if channels is None:
             channels = []
 
         self.dispatcher = dispatcher
         self.log = logging.getLogger("rcp-client")
         self.lock = threading.Lock()
         self.results = dict()
         self.default_timeout = default_timeout
         self.running = True
 
         self.channels = []
         for channel in channels:
             self.register_channel(channel)
+        if self.channels:
+            wait_for_connection(self.dispatcher)
 
     def register_channel(self, channel):
         assert self.running, "Cannot register channels when rpc client is shutdown"
         if channel not in self.channels:
             self.channels.append(channel)
             topic = channel_to_response_topic(channel)
             self.log.debug("Registering channel: {}".format(topic))
-            self.dispatcher.register_handler(topic, RPCResponse, self.receive)
+            self.dispatcher.register_handler(topic, RPCResponse, self.receive, match_type=False)
 
     def unregister_channel(self, channel):
         self.channels.remove(channel)
         topic = channel_to_response_topic(channel)
         self.log.debug("Unregistering channel: {}".format(topic))
         self.dispatcher.unsubscribe(topic)
 
@@ -94,16 +107,15 @@
                     to_delete.append(rpc_id)
             for rpc_id in to_delete:
                 self.results.pop(rpc_id, None)
 
     def _call(self, channel: bytes, typ: str, request: Dict, timeout: float):
         rpc_id = str(uuid4())
 
-        request = RPCRequest(rpc_id=rpc_id, resource=settings.RESOURCE, name=settings.NAME,
-                             request=request, type=typ)
+        request = RPCRequest(rpc_id=rpc_id, name=settings.NAME, request=request, type=typ)
         topic = channel_to_request_topic(channel)
         entry = self.RPCEntry(timeout=timeout)
         self.results[rpc_id] = entry
         core().publish(topic=topic, message=request)
         return entry
 
     def rpc(self, channel: bytes, type: str, request: [Dict, BaseModel],
@@ -118,14 +130,15 @@
             )
 
         if timeout is None:
             timeout = self.default_timeout
 
         if channel not in self.channels:
             self.register_channel(channel)
+            wait_for_connection(self.dispatcher)
 
         entry = self._call(channel, type, request, timeout)
         if blocking:
             return entry.result(timeout=timeout)
         else:
             return entry
```

### Comparing `openmodule-9.0.0rc9/openmodule/rpc/server.py` & `openmodule-9.1.0/openmodule/rpc/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 import threading
+import warnings
 from collections import namedtuple
-from typing import Callable, Dict, Optional, Type, Union, get_origin, get_args, TypeVar
+from typing import Callable, Dict, Optional, Type, Union, TypeVar
 
 import zmq
 from pydantic import ValidationError, BaseModel
 from pydantic.main import ROOT_KEY
 
 from openmodule.config import settings
+from openmodule.dispatcher import DummyExecutor
 from openmodule.messaging import get_sub_socket, get_pub_socket, receive_message_from_socket
 from openmodule.models.rpc import RPCResponse, RPCRequest
 from openmodule.rpc.common import channel_to_request_topic, channel_to_response_topic
 from openmodule.threading import get_thread_wrapper
 from openmodule.utils.schema import Schema
 
 CallbackEntry = namedtuple("CallbackEntry", ["timestamp", "result"])
@@ -45,24 +47,41 @@
 
 
 RequestType = TypeVar("RequestType")
 ResponseType = TypeVar("ResponseType")
 
 
 class RPCServer(object):
-    def __init__(self, context, config, filter_resource=True):
+    def __init__(self, context, config=None, *, filter_resource=True, executor=None):
+        """
+        :param: executor: The executor to use for scheduling messages. The executor is shutdown
+                          if the RPC Server is shutdown
+        """
+        if config:
+            warnings.warn(
+                "\n\nThe RPC Server no longer requires the config, but takes the openmodule global config instead. "
+                "Please remove the argument. Future versions will remove the argument and leat to an error",
+                DeprecationWarning, stacklevel=2
+            )
+
+        config = config or settings
         self.name = config.NAME
         self.sub = get_sub_socket(context, config)
         self.pub = get_pub_socket(context, config)
+        self.pub_lock = threading.Lock()
         self.handlers: Dict[tuple, HandlerEntry] = {}
         self.filters = []
         self.running = True
         self.log = logging.getLogger(self.__class__.__name__)
         self.thread = None
         self.resource = None
+        self.executor = executor or DummyExecutor()
+        # since zmq does prefix matching we keep a list of unique channel names here
+        # so we do not log a warning "unknown handler" if our channel is a prefix of a different channel
+        self.registered_channels = set()
         if filter_resource:
             if config.RESOURCE:
                 self.resource = config.RESOURCE
             else:
                 self.log.error(
                     "Resource filter is active, but no resource is available. All RPCs requests will be processed. "
                     "This is ok for debugging / testing containers, but must not happen in production."
@@ -72,18 +91,23 @@
         """
         :param filter: filter function with paramters reqeust, message, handler
         :param channel: specific channel to filter or all channels if None
         :param type: specific type to filter or all types if None
         """
         self.filters.append(Filter(filter=filter, channel=channel, type=type))
 
-    def shutdown(self, timeout=3):
+    def shutdown(self, timeout=10):
         self.running = False
+        self.executor.shutdown(wait=True)
         if self.thread:
             self.thread.join(timeout=timeout)
+        else:
+            with self.pub_lock:
+                self.pub.close()
+            self.sub.close()
 
     def register_handler(self, channel: str, type: str,
                          request_class: Type[RequestType],
                          response_class: Type[ResponseType],
                          handler: Callable[[RequestType, BaseModel], Union[ResponseType, Dict, None]],
                          register_schema=True):
         """
@@ -99,14 +123,15 @@
         """
         if (channel, type) in self.handlers:
             raise ValueError(f"handler for {channel}:{type} is already registered")
 
         self.log.debug("register handler {}:{} -> {}".format(channel, type, handler))
         self.sub.subscribe(channel_to_request_topic(channel.encode("ascii")))
         self.handlers[(channel, type)] = HandlerEntry(request_class, response_class, handler)
+        self.registered_channels = set(x[0] for x in self.handlers.keys())
         if register_schema:
             Schema.save_rpc(channel, type, request_class, response_class, handler)
 
     def _channel_from_topic(self, topic: bytes) -> str:
         return topic.split(b"-", 2)[-1].decode("ascii")
 
     def should_process_message(self, request, message, handler, channel):
@@ -174,50 +199,67 @@
             except Exception as e:
                 self.log.exception("exception in handler {}:{}".format(channel, message.type))
                 return {"status": "handler_error", "exception": str(e)}
         else:
             self.log.warning("no handler found for {}:{}".format(channel, message.type))
             return None
 
+    def _process_rpc_message(self, topic, message):
+        try:
+            channel = self._channel_from_topic(topic)
+
+            # this filters prefix-matched topics from other channels early
+            if channel not in self.registered_channels:
+                return
+
+            try:
+                message = RPCRequest(**message)
+                message_type = message.type
+                rpc_id = message.rpc_id
+            except ValidationError as e:
+                message_type = "unknown"
+                rpc_id = None
+                response = {"status": "validation_error", "exception": e.json()}
+            else:
+                response = self.process_rpc(channel, message)
+
+            if response is not None:
+                self.log.debug("response: {}".format(response))
+                if "status" not in response:
+                    response["status"] = "ok"
+
+                result = RPCResponse(
+                    type=message_type,
+                    rpc_id=rpc_id,
+                    response=response,
+                    name=self.name
+                )
+                with self.pub_lock:
+                    result.publish_on_topic(
+                        self.pub,
+                        channel_to_response_topic(channel.encode("ascii")),
+                    )
+        except Exception:
+            self.log.exception("Unknown exception while processing an rpc. No answer could was sent to the caller.")
+        except zmq.ContextTerminated:
+            self.log.warning(
+                "context terminated while RPC request was being processed. The result might not have been sent."
+            )
+
     def run(self):
         poller = zmq.Poller()
         poller.register(self.sub, zmq.POLLIN)
         try:
             while self.running:
                 socks = dict(poller.poll(timeout=1000))
                 if socks.get(self.sub) != zmq.POLLIN:
                     continue
                 topic, message = receive_message_from_socket(self.sub)
                 if topic is None:
                     continue
-                channel = self._channel_from_topic(topic)
-                try:
-                    message = RPCRequest(**message)
-                    message_type = message.type
-                    rpc_id = message.rpc_id
-                except ValidationError as e:
-                    message_type = "unknown"
-                    rpc_id = None
-                    response = {"status": "validation_error", "exception": e.json()}
-                else:
-                    response = self.process_rpc(channel, message)
-
-                if response is not None:
-                    self.log.debug("response: {}".format(response))
-                    if "status" not in response:
-                        response["status"] = "ok"
-
-                    result = RPCResponse(
-                        type=message_type,
-                        rpc_id=rpc_id,
-                        response=response,
-                        name=self.name
-                    )
-                    result.publish_on_topic(
-                        self.pub,
-                        channel_to_response_topic(channel.encode("ascii")),
-                    )
+                self.executor.submit(self._process_rpc_message, topic, message)
         except zmq.ContextTerminated:
             pass
         finally:
             self.sub.close()
-            self.pub.close()
+            with self.pub_lock:
+                self.pub.close()
```

### Comparing `openmodule-9.0.0rc9/openmodule/sentry.py` & `openmodule-9.1.0/openmodule/sentry.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,45 +41,49 @@
     This function initializes Sentry with our predefined values. This function also check if Sentry should be
     initialized.
 
     :param core: openmodule core instance
     :param extras: global extras that should be added to message
     :param kwargs: client supported **kwargs see ClientOptions
     """
-    if should_activate_sentry(core.config):
-        zmq_transport = ZeroMQTransport(core)
-        environment = environment_from_config(core.config)
-        server_name = core.config.RESOURCE
-        if not server_name:
-            core.log.warning("resource not available using hostname instead for sentry tag")
-            server_name = gethostname()
-        sentry_sdk.init(
-            dsn=None, release=core.config.VERSION, server_name=server_name, environment=environment,
-            transport=zmq_transport, **kwargs
-        )
-
-        extras = extras or {}
-        extras.update(extra_from_config(core.config))
-        with sentry_sdk.configure_scope() as scope:
-            for key, value in extras.items():
-                scope.set_extra(key, value)
-    else:
-        core.log.info("not activating sentry in debug or test mode")
+    zmq_transport = ZeroMQTransport(core)
+    environment = environment_from_config(core.config)
+    server_name = core.config.RESOURCE
+    if not server_name:
+        core.log.warning("resource not available using hostname instead for sentry tag")
+        server_name = gethostname()
+    sentry_sdk.init(
+        dsn=None, release=core.config.VERSION, server_name=server_name, environment=environment,
+        transport=zmq_transport, **kwargs
+    )
+
+    extras = extras or {}
+    extras.update(extra_from_config(core.config))
+    with sentry_sdk.configure_scope() as scope:
+        for key, value in extras.items():
+            scope.set_extra(key, value)
+
+
+def deinit_sentry():
+    sentry_sdk.init(dsn=None)
 
 
 def should_activate_sentry(config) -> bool:
     """
     This function checks if for the given config Sentry should be activated or not.
+    This is only false for debug mode. During testing we do not have a sentry-sender
+    running anyways.
 
     :param config: current configuration
     :return: bool
     """
     if config.DEBUG or config.TESTING:
         return False
-    return True
+    else:
+        return True
 
 
 def environment_from_config(config) -> str:
     """
     This functions returns either the environment of the current configuration.
 
     :param config: current configuration
```

### Comparing `openmodule-9.0.0rc9/openmodule/threading.py` & `openmodule-9.1.0/openmodule/threading.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/utils/api.py` & `openmodule-9.1.0/docs/deprecated_code/api/openmodule/utils/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         return f"Api Error {self.status}: {self.msg}"
 
 
 class AuthMethod(str, Enum):
     digest = "digest"
     basic = "basic"
     none = "none"
+    header = "header"
 
 
 class Api:
     """
     Api template class
     provides basic request functionality
     """
@@ -41,14 +42,16 @@
 
     @classmethod
     def get_auth(cls, auth_type, user, password):
         if auth_type == AuthMethod.basic:
             return HTTPBasicAuth(user, password)
         elif auth_type == AuthMethod.digest:
             return HTTPDigestAuth(user, password)
+        elif auth_type == AuthMethod.header:
+            return {user: password}
         else:
             return None
 
     @classmethod
     def _common_headers(cls):
         return {}
 
@@ -56,16 +59,21 @@
         url = f"{self.server_host.rstrip('/')}/{url}"
         timeout = kwargs.pop("timeout", self.request_timeout)
         headers = self._common_headers()
         headers.update(kwargs.pop("headers", {}))
         result = None
         try:
             logging.debug(f"Sending {method} request to {url}")
+            if isinstance(self.auth, (HTTPBasicAuth, HTTPDigestAuth)):
+                kwargs["auth"] = self.auth
+            elif isinstance(self.auth, dict):
+                headers.update(self.auth)
+
             result = requests.request(method.upper(), url, **kwargs, timeout=timeout, headers=headers,
-                                      verify=self.verify_ssl, json=payload, auth=self.auth)
+                                      verify=self.verify_ssl, json=payload)
             if 200 <= result.status_code < 300:
                 if json_response:
                     return result.json()
                 return result.content
         except requests.Timeout:
             raise ApiException(status_code=408, msg=f"Timeout after {timeout}s")
         except Exception as e:
```

### Comparing `openmodule-9.0.0rc9/openmodule/utils/backend.py` & `openmodule-9.1.0/openmodule/utils/backend.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/utils/charset.py` & `openmodule-9.1.0/openmodule/utils/charset.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/utils/connection_status.py` & `openmodule-9.1.0/openmodule/utils/connection_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,15 @@
     connected: bool = True
     _first_message: bool = True
 
     def __init__(self, dispatcher: MessageDispatcher):
         self.log = logging.getLogger(self.__class__.__name__)
         self.on_connect = EventListener(log=self.log)
         self.on_disconnect = EventListener(log=self.log)
-        dispatcher.register_handler(b"connection_status",
-                                    ConnectionStatusMessage,
-                                    self.process_connection_status,
-                                    filter=dict(type="connection_status"))
+        dispatcher.register_handler(b"connection_status", ConnectionStatusMessage, self.process_connection_status)
 
     def process_connection_status(self, message: ConnectionStatusMessage):
         """
         Forwards the current connection status of the ogclient
         """
         new_connected = message.connected
         if new_connected != self.connected or self._first_message:
```

### Comparing `openmodule-9.0.0rc9/openmodule/utils/db_helper.py` & `openmodule-9.1.0/openmodule/utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/utils/io.py` & `openmodule-9.1.0/openmodule/utils/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,21 @@
     changes (or doesn't change) as registered (edge_rising, edge_falling, edge_any, edge_none).
     The IoListener additionally save the current stage of ALL pins.
     """
     current_states: Dict[str, IoState] = defaultdict(IoState)
     listeners: List[Listener] = list()
 
     def __init__(self, dispatcher: MessageDispatcher, raise_handler_errors=False):
+        assert not dispatcher.is_multi_threaded, (
+            "you cannot use a multithreaded message dispatcher for the presence listener. It is highly reliant "
+            "on receiving messages in the correct order!"
+        )
         self.log = logging.getLogger(self.__class__.__name__)
         self.raise_handler_errors = raise_handler_errors
-        dispatcher.register_handler(b"io", IoMessage, self._on_io_message)
+        dispatcher.register_handler(b"io", IoMessage, self._on_io_message, match_type=False)
 
     def add_listener_edge_rising(self, listen_to: Union[str, Gateway], callback: Callable[[IoState], None],
                                  io_type: Optional[str] = None):
         """
         Calls the given callback method whenever a message is received and the given pin or a pin of the given Gateway
         changes its value from 0 to 1 (rising edge)
         param listen_to: the pin or Gateway that needs to experience a rising edge to call the callback
@@ -66,29 +70,40 @@
         param callback: the function that is called when a message with the given listen_to is received
         param io_type: the io_type to filter for (input, output)
         """
         self._add_listener(edge="none", listen_to=listen_to, callback=callback, io_type=io_type)
 
     def _add_listener(self, edge: str, listen_to: Union[str, Gateway], callback: Callable[[IoState], None],
                       io_type: Optional[str] = None):
-        if type(listen_to) == str:
-            message_filter = {"pin": listen_to}
-        else:
-            message_filter = {"gateway": listen_to}
-        if edge == "rising":
-            message_filter.update(value=1, edge=1)
-        elif edge == "falling":
-            message_filter.update(value=0, edge=1)
-        elif edge == "any":
-            message_filter.update(edge=1)
-        elif edge == "none":
-            message_filter.update(edge=0)
-        if io_type is not None:
-            message_filter.update(type=io_type)
-        self.listeners.append(Listener(IoMessage, message_filter, callback))
+
+        assert isinstance(listen_to, (str, Gateway))
+
+        def message_filter(msg):
+            if isinstance(listen_to, str):
+                if msg.get("pin") != listen_to:
+                    return False
+            elif isinstance(listen_to, Gateway):
+                if (msg.get("gateway") or {}).get("gate") != listen_to.gate:
+                    return False
+
+            filter_dict = {}
+            if edge == "rising":
+                filter_dict.update(value=1, edge=1)
+            elif edge == "falling":
+                filter_dict.update(value=0, edge=1)
+            elif edge == "any":
+                filter_dict.update(edge=1)
+            elif edge == "none":
+                filter_dict.update(edge=0)
+            if io_type is not None:
+                filter_dict.update(type=io_type)
+
+            return msg.items() >= filter_dict.items()
+
+        self.listeners.append(Listener(IoMessage, None, message_filter, callback))
 
     def is_pin_valid(self, pin: str, timeout: Optional[int] = 5) -> bool:
         """
         Returns true if the given pin is present in the saved IoStates and it has received a message in the last
         'timeout' seconds (default 5)
         """
         return pin in self.current_states and \
@@ -112,16 +127,16 @@
 
     def get_gateway_states(self, gateway: Gateway) -> List[IoState]:
         """
         Returns a list the current IoStates of the given Gateway, or a list with 1 default IoState (all values 0) if
         the Gateway does not yet exist
         """
         x = list(filter(lambda state: state.gateway == gateway, self.current_states.values()))
-        return x if x else[IoState(pin="", gateway=Gateway(gate="", direction=""), type="", value=0, physical=0,
-                                   inverted=False, last_timestamp=datetime.fromtimestamp(0))]
+        return x if x else [IoState(pin="", gateway=Gateway(gate="", direction=""), type="", value=0, physical=0,
+                                    inverted=False, last_timestamp=datetime.fromtimestamp(0))]
 
     def _on_io_message(self, message: IoMessage):
         """
         This handler receives all IO Messages, saves any changes and calls any listeners registered in the IoListener
         """
         if message.pin not in self.current_states:
             """
@@ -133,15 +148,15 @@
                 message.physical = message.value if not message.inverted else 1 - message.value
             message.edge = 1
             self.current_states[message.pin] = IoState(pin=message.pin, gateway=message.gateway, type=message.type,
                                                        value=message.value, physical=message.physical,
                                                        inverted=message.inverted, last_timestamp=message.timestamp)
 
         elif (message.edge == 1) or (self.current_states[message.pin].value != message.value) or \
-             (self.current_states[message.pin].inverted != message.inverted):
+                (self.current_states[message.pin].inverted != message.inverted):
             """
             The state of this gate was changed, or edge is 1.
             The entry in the current_states dict needs to be updated.
             """
             if "physical" not in message:
                 message.physical = message.value if not message.inverted else 1 - message.value
             message.edge = 1
```

### Comparing `openmodule-9.0.0rc9/openmodule/utils/matching.py` & `openmodule-9.1.0/openmodule/utils/matching.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule/utils/presence.py` & `openmodule-9.1.0/openmodule/utils/presence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 from typing import Optional, Dict, Union, Type, Tuple
 
+from openmodule.core import init_openmodule, core
 from openmodule.dispatcher import EventListener, MessageDispatcher
 from openmodule.models.base import Gateway
 from openmodule.models.presence import PresenceBaseMessage, PresenceBackwardMessage, PresenceForwardMessage, \
-    PresenceChangeMessage, PresenceLeaveMessage, PresenceEnterMessage
+    PresenceChangeMessage, PresenceLeaveMessage, PresenceEnterMessage, PresenceRPCRequest, PresenceRPCResponse
 from openmodule.models.vehicle import Vehicle
+from openmodule.rpc import RPCClient
 
 
 def vehicle_from_presence_message(message: PresenceBaseMessage):
     return Vehicle(
         id=message.vehicle_id,
         lpr=message.medium.lpr,
         qr=message.medium.qr,
@@ -34,33 +36,44 @@
         assert self.gate is not None, (
             "`.present_vehicle` may only be used when listening for a specific gate, this presence listener"
             "listens to all gates, please access the present vehicle per gate via `.present_vehicles[gate]`"
         )
         return self.present_vehicles.get(self.gate)
 
     def __init__(self, dispatcher: MessageDispatcher, gate: Optional[str] = None):
-        self.log = logging.getLogger(self.__class__.__name__)
+        assert not dispatcher.is_multi_threaded, (
+            "you cannot use a multithreaded message dispatcher for the presence listener. It is highly reliant "
+            "on receiving messages in the correct order!"
+        )
+        self.log = logging.getLogger(self.__class__.__name__ + (" " + gate if gate else ""))
         self.on_forward = EventListener(log=self.log)
         self.on_backward = EventListener(log=self.log)
         self.on_enter = EventListener(log=self.log)
         self.on_change = EventListener(log=self.log)
         self.on_leave = EventListener(log=self.log)
         self.present_vehicles = dict()
         self.gate = gate
 
-        dispatcher.register_handler(b"presence", PresenceBackwardMessage,
-                                    self._on_backward, filter={"type": "backward"})
-        dispatcher.register_handler(b"presence", PresenceForwardMessage,
-                                    self._on_forward, filter={"type": "forward"})
-        dispatcher.register_handler(b"presence", PresenceChangeMessage,
-                                    self._on_change, filter={"type": "change"})
-        dispatcher.register_handler(b"presence", PresenceLeaveMessage,
-                                    self._on_leave, filter={"type": "leave"})
-        dispatcher.register_handler(b"presence", PresenceEnterMessage,
-                                    self._on_enter, filter={"type": "enter"})
+        dispatcher.register_handler(b"presence", PresenceBackwardMessage, self._on_backward)
+        dispatcher.register_handler(b"presence", PresenceForwardMessage, self._on_forward)
+        dispatcher.register_handler(b"presence", PresenceChangeMessage, self._on_change)
+        dispatcher.register_handler(b"presence", PresenceLeaveMessage, self._on_leave)
+        dispatcher.register_handler(b"presence", PresenceEnterMessage, self._on_enter)
+
+    def init_present_vehicles(self):
+        assert self.gate, "init present vehicles is only possible if the gate is set, otherwise we do not know" \
+                          "how many results to expect"
+        try:
+            result = core().rpc_client.rpc(b"tracking", "get-present", PresenceRPCRequest(gate=self.gate))
+            if result.status == "ok" and result.response:
+                response = PresenceRPCResponse(**result.response)
+                if response.presents:
+                    self._on_enter(response.presents[0])
+        except TimeoutError:
+            self.log.error(f"get-present RPC timeout for gate {self.gate}")
 
     def _gate_matches(self, message: PresenceBaseMessage):
         return (self.gate is None) or (message.gateway.gate == self.gate)
 
     def _on_backward(self, message: PresenceBackwardMessage):
         """
         This handler forwards presence backward  messages to the registered calls in the presence listener
```

### Comparing `openmodule-9.0.0rc9/openmodule/utils/schema.py` & `openmodule-9.1.0/openmodule/utils/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import functools
 import json
 import os
 from textwrap import dedent
 from typing import Callable, Any
 
+from openmodule.config import settings
+
 
 def active(f):
     def wrapper(*args, **kwargs):
-        if os.environ.get("TESTING") == "True":
-            f(*args, **kwargs)
+        if settings.TESTING:
+            return f(*args, **kwargs)
         return None
 
     return wrapper
 
 
 class RPCSchema:
     def __init__(self, channel, typ, request, response, handler: Callable[[Any], Any]):
@@ -44,25 +46,16 @@
         self.description = dedent(handler.__doc__.strip()) if handler.__doc__ else ""
 
     def render(self):
         res = dict(put=dict(summary=self.description, tags=["Messages"],
                             requestBody=dict(description=self.message_class, content={
                                 "application/json": dict(
                                     schema={"$ref": f"#/components/schemas/{self.message_class}"})})))
-        res["put"].update(self.render_filter())
         return res
 
-    def render_filter(self):
-        if not self.filter:
-            return {}
-        res = []
-        for key, value in self.filter.items():
-            res.append({"in": "filter", "name": key, "value": value})
-        return dict(parameters=res)
-
     @property
     def key(self):
         return f"/{self.topic}/{self.handler}"
 
     def check_new(self, message_list):
         for message in message_list:
             if self.topic == message.topic and self.handler == message.handler and self.filter == message.filter:
```

### Comparing `openmodule-9.0.0rc9/openmodule/utils/validation.py` & `openmodule-9.1.0/openmodule/utils/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
+import re
 
 from openmodule.core import OpenModuleCore
-from openmodule.models.backend import AccessRequest
-from openmodule.models.validation import ValidationProviderRegisterRequestMessage, ValidateResponse, ValidateRequest, \
-    ValidationProviderRegisterMessage, ValidationProviderUnregisterMessage
+from openmodule.models.validation import ValidationRegisterRequestMessage, ValidateResponse, ValidateRequest, \
+    ValidationRegisterMessage, ValidationUnregisterMessage
 from openmodule.rpc.server import RPCServer
+from openmodule.utils.misc_functions import clean_service_name
 
 
-class ValidationProvider:
+class Validation:
     """
     Validation provider template class
     provides basic functionality used for validation providers
-    * subscribes to ValidationProviderMessages and automatically registers validation_provider
+    * subscribes to ValidationMessages and automatically registers validation_provider
     * provides method for the validation_provider / validate rpc with the validate_ticket method
     """
 
     def __init__(self, core: OpenModuleCore, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.core = core
         self.log = logging.getLogger()
 
         self.register_at_controller()
         # BEWARE there is already a channel named "validation", see validation search in skidata-hostcom
-        self.core.messages.register_handler(b"validation_provider", ValidationProviderRegisterRequestMessage,
-                                            self.handle_validation_provider_register_request,
-                                            match_type=True)
+        self.core.messages.register_handler(b"validation_provider", ValidationRegisterRequestMessage,
+                                            self.handle_validation_provider_register_request)
 
     def register_rpcs(self, rpc_server: RPCServer):
         rpc_server.add_filter(self._validation_provider_filter, "validation_provider", "validate")
         rpc_server.register_handler("validation_provider", "validate", request_class=ValidateRequest,
                                     response_class=ValidateResponse, handler=self.rpc_validate_ticket)
 
     def _validation_provider_filter(self, request, message, handler) -> bool:
@@ -52,29 +52,26 @@
     def rpc_validate_ticket(self, request: ValidateRequest, _) -> ValidateResponse:
         """
         Checks and validates a ticket for an occupant
         """
 
         response: ValidateResponse = self.validate_ticket(request)
         if response.cost_entries:
+            cleaned_service_name: str = clean_service_name(self.core.config.NAME)
             for cost_entry in response.cost_entries:
-                # if no source is set, source will be set to service_name: e.g. "service_iocontroller"
-                if not cost_entry.source:
-                    # 1. replace: removing service prefix: "om_"
-                    # 2. replace: removing instance suffix: e.g. "_1", "_2"
-                    cost_entry.source = self.core.config.NAME \
-                        .replace(r"^om_", "") \
-                        .replace(r"_\d+$", "")
+                # if no source is set, source will be set to cleaned_service_name: e.g. "service_iocontroller"
+                if cost_entry.get("source", None) is None:
+                    cost_entry["source"] = cleaned_service_name
 
         return response
 
     def handle_validation_provider_register_request(self, _):
         """
         Registers the validation provider if the message type is register_request
         """
         self.register_at_controller()
 
     def register_at_controller(self):
-        self.core.publish(ValidationProviderRegisterMessage(), b"validation_provider")
+        self.core.publish(ValidationRegisterMessage(), b"validation_provider")
 
     def unregister_at_controller(self):
-        self.core.publish(ValidationProviderUnregisterMessage(), b"validation_provider")
+        self.core.publish(ValidationUnregisterMessage(), b"validation_provider")
```

### Comparing `openmodule-9.0.0rc9/openmodule.egg-info/PKG-INFO` & `openmodule-9.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,14 @@
-Metadata-Version: 2.1
-Name: openmodule
-Version: 9.0.0rc9
-Summary: Libraries for developing the arivo openmodule
-Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
-Author: ARIVO
-Author-email: support@arivo.co
-License: GNU General Public License v2 (GPLv2)
-Keywords: arivo openmodule
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: test
-License-File: LICENSE
-
 # OpenModule V2
 
+Some additional documentation:
+
+* [Openmodule Core](docs/core.md)
+* [RPC Server / Client](docs/rpc.md)
+
 ## Changes
 
 Breaking changes are annotated [here](docs/migrations.md).
 
 To quickly check if your service is susceptible to a known issue have a look [here](docs/migrations.md).
 
 ## Coding Standard
@@ -31,23 +17,24 @@
 
 ## Features
 
 The openmodule package provides a lot of features:
 
 ### Settings
 
-The openmodule package uses a global lazy configuration `openmodule.config.settings`. 
-This setting includes some standard parameters defined in `openmodule.config.GlobalSettings` and parameters from a customizable module.
-To specify the module you can call `settings.configure(module)` or you can set the environment variable `SETTINGS_MODULE`.
-Per default settings looks for the `config` module (it also looks for the `tests/config` module first for test cases)
+The openmodule package uses a global lazy configuration `openmodule.config.settings`. This setting includes some
+standard parameters defined in `openmodule.config.GlobalSettings` and parameters from a customizable module. To specify
+the module you can call `settings.configure(module)` or you can set the environment variable `SETTINGS_MODULE`. Per
+default settings looks for the `config` module (it also looks for the `tests/config` module first for test cases)
 
 #### Models
 
-Inherit from `OpenModuleModel` or in case of ZMQ messages from `ZMQMessage`.
-Models use pydantic ([docs](https://pydantic-docs.helpmanual.io/usage/types/)), check openmodule.models.* for some examples (e.g. PresenceBaseMessage for alias)
+Inherit from `OpenModuleModel` or in case of ZMQ messages from `ZMQMessage`. Models use
+pydantic ([docs](https://pydantic-docs.helpmanual.io/usage/types/)), check openmodule.models.* for some examples (e.g.
+PresenceBaseMessage for alias)
 
 ### Core
 
 The base of the new openmodule, every package should have exactly one. The core handles various things:
 
 * sentry
 * logging
@@ -147,15 +134,17 @@
 rpc_server.register_handler("backend", "auth", request_class=AccessRequest,
                             response_class=AccessResponse, handler=handler, register_schema=True)
 rpc.run()
 ```
 
 ### Utils
 
-#### Api
+#### Api (**DEPRECATED**)
+
+
 
 We implemented a very basic Api class you can use for http request and that handles errors and authentication. Either
 inherit it or create a class.
 
 ```python
 api = Api(**kwargs)
 try:
@@ -204,14 +193,56 @@
 Helper class for listening to presence messages.
 
 ```python
 presence_listener = PresenceListener(core.messages)
 presence_listener.on_enter.append(some_function)
 ```
 
+#### Package Reader
+
+Helper class to read settings (env, yml) of specified services. The services are only considered valid and parsed if a revision file for the service exists.
+Functions: 
+* **installed_services:** Returns a list of installed services, based on prefix
+* **load_setting:** Loads the setting of a single service
+* **load_with_service_prefix:** Loads the setting of all services starting with the prefix (no or empty prefix means no filter)
+* **load_with_hardware_type_prefix:** Load the setting of all services with the given hardware type (i.e. `cam-ip`)
+* **load_with_parent_type_prefix:**  Load the setting of all services with the given parent type (i.e. `cam-ip`)
+
+##### Bridged Slave Detection
+
+Some services behave differently if they are started on a bridged slave device. The function `is_bridged_slave()` is a helper function to detect this. To use this function on the device, you need to mount the dist folder (/opt/openmodule/dist2).
+The function returns:
+* None: No dist directory, no bridge service installed, multiple bridges installed
+* True: Bridge service is installed and `MASTER` is set there
+* False: Bridge service is installed and `MASTER` is not set there
+
+You can also set the env variable `BRIDGED_SLAVE` to True/False directly, so you do not need to care about the service settings.
+This is useful for testing (@override_settings(BRIDGED_SLAVE=True)) or running local (set env var BRIDGED_SLAVE)
+
+### Anonymization
+
+The openmodule framework uses rpc requests and messages to trigger the anonymization of data.
+* **Message:** You can send a AnonymizeMessage (topic: `privacy`). The message includes a session_id and vehicle_ids to delete
+* **RPC Request:** You can send an AnonymizeRequest with channel=`privacy`, type=`anonymize` to the DSGVO container. This session only includes session_ids.
+The DSGVO container will then match vehicle_ids to the session_ids and redistribute the request with the prior mentioned message.
+
+A container with sensible data then needs to implement the message listener for the privacy messages:
+
+**Example:**
+```python
+core.messages.register("privacy", AnonymizeMessage, anonymize_data)
+
+def anonymize_data(message: AnonymizeMessage):
+    for vid in message.vehicle_ids:
+        delete_vehicle_image_by_vehicle_id(vid)
+```
+
+**IMPORTANT** You still have to take care of data retention in each service separately, meaning you have to delete data independently of these anonymization messages.
+i.e. the DSGVO service deletes data if we need disk space or the eventlog deletes events after 30 days by default 
+
 ## Documentation
 
 Openmodule >= 3.0.5 features automatic generation of Rpc and Message Schemas including their models. The generation uses
 data that is generated during the test runs to create an OpenApi Schema. Your RPCs and Message handlers are
 automatically documented if:
 
 * You use the message dispatcher of the core (OpenModuleCoreTestMixin)
@@ -232,10 +263,7 @@
 With default parameters, you need to document your handler functions with a doc string, that is then included as a
 description.
 
 ## Testing
 
 A separate package for testing openmodule packages exists within openmodule - openmodule-test. For more infos
 see [here](docs/testing.md)
-
-
-
```

### Comparing `openmodule-9.0.0rc9/openmodule.egg-info/SOURCES.txt` & `openmodule-9.1.0/openmodule.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 LICENSE
 README.md
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
-.idea/.gitignore
-.idea/misc.xml
-.idea/modules.xml
-.idea/openmodule.iml
-.idea/vcs.xml
-.idea/inspectionProfiles/Project_Default.xml
-.idea/inspectionProfiles/profiles_settings.xml
 docs/coding_standard.md
+docs/core.md
 docs/database.md
 docs/known_issues.md
 docs/migrations.md
 docs/rpc.md
 docs/testing.md
+docs/deprecated_code/README.md
+docs/deprecated_code/api/openmodule/utils/api.py
+docs/deprecated_code/api/openmodule_test/api.py
+docs/deprecated_code/api/tests/test_utils_api.py
 openmodule/__init__.py
 openmodule/alert.py
 openmodule/checks.py
 openmodule/config.py
 openmodule/core.py
 openmodule/dispatcher.py
 openmodule/health.py
@@ -32,46 +30,48 @@
 openmodule/messaging.py
 openmodule/sentry.py
 openmodule/threading.py
 openmodule.egg-info/PKG-INFO
 openmodule.egg-info/SOURCES.txt
 openmodule.egg-info/dependency_links.txt
 openmodule.egg-info/not-zip-safe
+openmodule.egg-info/pbr.json
 openmodule.egg-info/requires.txt
 openmodule.egg-info/top_level.txt
 openmodule/database/custom_types.py
 openmodule/database/database.py
 openmodule/database/env.py
 openmodule/models/__init__.py
 openmodule/models/alert.py
 openmodule/models/backend.py
 openmodule/models/base.py
 openmodule/models/io.py
 openmodule/models/presence.py
+openmodule/models/privacy.py
 openmodule/models/rpc.py
 openmodule/models/validation.py
 openmodule/models/vehicle.py
 openmodule/rpc/__init__.py
 openmodule/rpc/client.py
 openmodule/rpc/common.py
 openmodule/rpc/server.py
 openmodule/utils/__init__.py
-openmodule/utils/api.py
 openmodule/utils/backend.py
 openmodule/utils/charset.py
 openmodule/utils/connection_status.py
 openmodule/utils/db_helper.py
 openmodule/utils/io.py
 openmodule/utils/matching.py
+openmodule/utils/misc_functions.py
+openmodule/utils/package_reader.py
 openmodule/utils/presence.py
 openmodule/utils/schema.py
 openmodule/utils/validation.py
 openmodule_test/__init__.py
 openmodule_test/alert.py
-openmodule_test/api.py
 openmodule_test/backend.py
 openmodule_test/core.py
 openmodule_test/database.py
 openmodule_test/database_models.py
 openmodule_test/eventlistener.py
 openmodule_test/files.py
 openmodule_test/gate.py
@@ -95,26 +95,28 @@
 tests/test_dispatcher.py
 tests/test_health.py
 tests/test_interrupt.py
 tests/test_io_listen.py
 tests/test_messaging.py
 tests/test_model.py
 tests/test_models_backend.py
+tests/test_package_reader.py
 tests/test_rpc.py
 tests/test_schema.py
 tests/test_sentry.py
 tests/test_test_alert.py
 tests/test_test_gate.py
 tests/test_test_zeromq.py
-tests/test_utils_api.py
 tests/test_utils_backend.py
 tests/test_utils_charset.py
 tests/test_utils_connection_status.py
 tests/test_utils_matching.py
+tests/test_utils_misc_functions.py
 tests/test_utils_presence.py
+tests/test_utils_validation.py
 tests/test_utils_vehicle.py
 tests/invalid_database/alembic.ini
 tests/invalid_database/makemigration.sh
 tests/invalid_database/alembic/README
 tests/invalid_database/alembic/__init__.py
 tests/invalid_database/alembic/env.py
 tests/invalid_database/alembic/script.py.mako
```

### Comparing `openmodule-9.0.0rc9/openmodule_test/alert.py` & `openmodule-9.1.0/openmodule_test/alert.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/api.py` & `openmodule-9.1.0/docs/deprecated_code/api/openmodule_test/api.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/backend.py` & `openmodule-9.1.0/openmodule_test/backend.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/core.py` & `openmodule-9.1.0/openmodule_test/core.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/database.py` & `openmodule-9.1.0/openmodule_test/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,30 +26,34 @@
     """
     Mixin for database cleanup in test cases
     * use create_database = True for an automatic generation of a database
     * use create_database = False and set the database directly
     """
     create_database = True
     database = None
-    database_folder: str = settings.DATABASE_FOLDER
+    database_folder: str = None  # defaults to settings.DATABASE_FOLDER
     alembic_path = "../src/database"
     database_name = "database"
 
     @classmethod
+    def get_database_folder(cls):
+        return cls.database_folder or settings.DATABASE_FOLDER
+
+    @classmethod
     def setUpClass(cls) -> None:
         # we only know which databases are in use on tear down, so truncating only works in teardown
         # but in order to not be annoyed by failed tests which left broken databases, we delete all databases
         # once initially
         global _first_start
         if _first_start:
-            for file in glob(os.path.join(cls.database_folder, "*.sqlite3")):
+            for file in glob(os.path.join(cls.get_database_folder(), "*.sqlite3")):
                 os.unlink(file)
             _first_start = False
         if cls.create_database:
-            cls.database = Database(cls.database_folder, cls.database_name, cls.alembic_path)
+            cls.database = Database(cls.get_database_folder(), cls.database_name, cls.alembic_path)
         return super().setUpClass()
 
     def delete_database(self, database: Database):
         assert not database.is_open(), "database must be shutdown before it can be deleted"
         try:
             os.unlink(database_path(database.db_folder, database.name))
         except FileNotFoundError:
```

### Comparing `openmodule-9.0.0rc9/openmodule_test/database_models.py` & `openmodule-9.1.0/openmodule_test/database_models.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/eventlistener.py` & `openmodule-9.1.0/openmodule_test/eventlistener.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/gate.py` & `openmodule-9.1.0/openmodule_test/gate.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
     open_count = 0
     reject_count = 0
 
     def __init__(self, gate: str, direction: Direction, dispatcher: MessageDispatcher):
         self.gate = gate
         self.direction = direction
-        dispatcher.register_handler(b"access_accept", TestGateAccessMessage, self._access_accept, register_schema=False)
-        dispatcher.register_handler(b"access_reject", TestGateAccessMessage, self._access_reject, register_schema=False)
+        dispatcher.register_handler(b"access_accept", TestGateAccessMessage, self._access_accept,
+                                    register_schema=False, match_type=False)
+        dispatcher.register_handler(b"access_reject", TestGateAccessMessage, self._access_reject,
+                                    register_schema=False, match_type=False)
         _all_gates.add(self)
 
     @classmethod
     def reset_all_counts(cls):
         for x in _all_gates:
             x.reset_call_count()
```

### Comparing `openmodule-9.0.0rc9/openmodule_test/health.py` & `openmodule-9.1.0/openmodule_test/health.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/interrupt.py` & `openmodule-9.1.0/openmodule_test/interrupt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import time
 from multiprocessing import Process, Event
 from signal import SIGINT, SIGKILL
-from typing import Callable, Union, Type
+from typing import Callable, Union, Type, Optional
 from unittest import TestCase
 
 import multiprocessing_logging
 
 from openmodule.core import shutdown_openmodule
 from openmodule.utils.schema import Schema
 from openmodule_test.health import HealthTestMixin
@@ -29,17 +29,30 @@
 
 class InterruptTestMixin(TestCase):
     """
     Helper class for testing interrupts and exceptions in code
     for usage, look at file tests/test_interrupt
     """
 
+    process: Optional[ExceptionProcess] = None
+
+    def _kill_process(self):
+        # this is called in tear down and as a cleanup to make sure that under any circumstances the process is killed
+        # otherwise you have processes lingering around, potentially blocking ports which is quite annoying
+        if self.process and self.process.is_alive():
+            os.kill(self.process.pid, SIGKILL)
+
+    def setUp(self) -> None:
+        self.addCleanup(self._kill_process)
+        super().setUp()
+
     def tearDown(self):
         super().tearDown()
         Schema.to_file()
+        self._kill_process()
 
     def wait_for_setup(self):
         pass
 
     def _wait_for_and_uninstall_mp_handler(self, logger=None):
         """
         waits until the multiprocessing logging handler has finished
@@ -54,17 +67,17 @@
         multiprocessing_logging.uninstall_mp_handler(logger)
 
     def start_process(self, f: Callable):
         """
         starts the process and waits until it is responsive by calling calls wait_for_setup()
         """
         multiprocessing_logging.install_mp_handler()
-        process = ExceptionProcess(target=f)
-        process.start()
-        return process
+        self.process = ExceptionProcess(target=f)
+        self.process.start()
+        return self.process
 
     def assertCleanShutdown(self, process, shutdown_timeout: float = 3.0):
         """
         asserts that the process shuts down cleanly
         """
         if process.is_finished.wait(timeout=shutdown_timeout):
             self._wait_for_and_uninstall_mp_handler()
@@ -72,15 +85,15 @@
         else:
             if process.is_alive():
                 os.kill(process.pid, SIGKILL)
                 raise TimeoutError("Process took to long for shutdown")
             else:
                 raise AssertionError("Process did not finish gracefully")
 
-    def send_signal_to_process(self, process, signal: Union[Type[KeyboardInterrupt], int]):
+    def send_signal_to_process(self, process: ExceptionProcess, signal: Union[Type[KeyboardInterrupt], int]):
         self.assertFalse(process.is_finished.is_set())
         if signal == KeyboardInterrupt:
             signal = SIGINT
         os.kill(process.pid, signal)
 
     def signal_in_function(self, f: Callable, signal: Union[Type[KeyboardInterrupt], int], *,
                            raise_exception_after: float = 3.0, shutdown_timeout: float = 3.0):
```

### Comparing `openmodule-9.0.0rc9/openmodule_test/io.py` & `openmodule-9.1.0/openmodule_test/io.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/presence.py` & `openmodule-9.1.0/openmodule_test/presence.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/rpc.py` & `openmodule-9.1.0/openmodule_test/rpc.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/setup.cfg` & `openmodule-9.1.0/openmodule_test/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/setup.py` & `openmodule-9.1.0/openmodule_test/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/utils.py` & `openmodule-9.1.0/openmodule_test/utils.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/openmodule_test/zeromq.py` & `openmodule-9.1.0/openmodule_test/zeromq.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,20 +347,28 @@
 
 
 class _TestRPCRequest(BaseModel):
     """
     we do not want to depend on openmodule, this is a minimal version of the zmq message for the rpc function
     """
     timestamp: float = Field(default_factory=time.time)
-    resource: Optional[str] = settings.RESOURCE
+    resource: Optional[str] = None
     name: str
     type: str
     rpc_id: UUID
     request: Optional[Dict]
 
+    def __init__(self, **kwargs):
+        resource = kwargs.pop("resource")
+        if not resource:
+            # this avoids evaluating settings.RESOURCE if resource is set in order to not trigger the settings module
+            # to start up unnecessarily (and maybe throw import errors)
+            resource = settings.RESOURCE
+        super().__init__(resource=resource, **kwargs)
+
 
 class ZMQProcotol(str, Enum):
     inproc = "inproc://"
     tcp = "tcp://"
 
 
 class ZMQTestMixin(TestCase):
@@ -414,15 +422,15 @@
 
         """
         waits until a message dispatcher receives messages, this assumes that the subscription we issue is the last
         and if it is connected, all previous subscriptions will also be connected
         """
         random_topic = "_test" + "".join(random.choices(string.ascii_letters, k=10))
         random_topic = random_topic.encode()
-        dispatcher.register_handler(random_topic, BaseModel, handler, register_schema=False)
+        dispatcher.register_handler(random_topic, BaseModel, handler, register_schema=False, match_type=False)
 
         for x in range(self.zmq_client.startup_check_iterations):
             self.zmq_client.send(random_topic, {"type": "connection-check"})
             time.sleep(self.zmq_client.startup_check_delay)
             if received:
                 break
         assert received, "error during startup and connect"
```

### Comparing `openmodule-9.0.0rc9/setup.cfg` & `openmodule-9.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/invalid_database/alembic/versions/ff26e54332f9_datetime_models.py` & `openmodule-9.1.0/tests/invalid_database/alembic/versions/ff26e54332f9_datetime_models.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/invalid_database/alembic.ini` & `openmodule-9.1.0/tests/invalid_database/alembic.ini`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/invalid_database/makemigration.sh` & `openmodule-9.1.0/tests/invalid_database/makemigration.sh`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_alert.py` & `openmodule-9.1.0/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_checks.py` & `openmodule-9.1.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_config.py` & `openmodule-9.1.0/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,15 +188,14 @@
 
         with temp_file(yaml) as f:
             model = config.yaml(TestModel, f)
 
         self.assertIsNone(model.some, msg="Not parsed custom elements must be none")
 
 
-
 class LegacyConfigSupportTest(EnvTestCase):
     def test_broker_pub(self):
         # nothing found -> defaults
         self.assertEqual("tcp://127.0.0.1:10200", config.broker_pub())
 
         # legacy configs
         self.env("1.2.3.4", "BROKER_HOST")
@@ -284,27 +283,36 @@
 
     def test_environment(self):
         os.environ["SETTINGS_MODULE"] = "tests.resources.configs.test_config_1"
         self.assertEqual("THIS_IS_MY_NAME_TOO", settings.NAME)
         self.assertEqual("bsdf", settings.TEST)
         del os.environ["SETTINGS_MODULE"]
 
-    @override_context(NAME="ABC")
+    @override_settings(NAME="ABC")
     def test_overwrite(self):
-        @override_context(NAME="ASDF")
+        @override_settings(NAME="ASDF")
         def asdf():
             self.assertEqual("ASDF", settings.NAME)
             self.assertTrue(settings._wrapped.is_overridden("NAME"))
 
         settings.configure(test_config)
         asdf()
 
         self.assertEqual("ABC", settings.NAME)
         self.assertTrue(settings._wrapped.is_overridden("NAME"))
 
+    def test_override_var_which_does_not_exist(self):
+        @override_settings(VAR_DOES_NOT_EXIST=True)
+        def testfunction():
+            self.assertEqual(True, settings.VAR_DOES_NOT_EXIST)
+
+        self.assertFalse(hasattr(settings, "VAR_DOES_NOT_EXIST"))
+        testfunction()
+        self.assertFalse(hasattr(settings, "VAR_DOES_NOT_EXIST"))
+
     def test_context(self):
         settings.configure(test_config)
         self.assertEqual("THIS_IS_MY_NAME", settings.NAME)
 
         with override_context(NAME="abc"):
             self.assertEqual("abc", settings.NAME)
         self.assertEqual("THIS_IS_MY_NAME", settings.NAME)
```

### Comparing `openmodule-9.0.0rc9/tests/test_core.py` & `openmodule-9.1.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_database.py` & `openmodule-9.1.0/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,21 +159,21 @@
             db.add(model)
             main_thread_position = "end"
 
         thread.join()
         self.assertEqual(second_thread_value, "changed")
 
     def test_multiple_databases(self):
-        db1 = Database(self.database_folder, name="asdf", alembic_path=self.alembic_path)
+        db1 = Database(self.get_database_folder(), name="asdf", alembic_path=self.alembic_path)
         with db1 as db:
             db.add(DatabaseTestModel(value1=0, value2=4))
         with self.assertRaises(Exception) as e:
-            db2 = Database(self.database_folder, name="asdf", alembic_path=self.alembic_path)
+            Database(self.get_database_folder(), name="asdf", alembic_path=self.alembic_path)
         self.assertIn("already exists", str(e.exception))
-        self.assertTrue(os.path.exists(os.path.join(self.database_folder, "asdf.sqlite3")))
+        self.assertTrue(os.path.exists(os.path.join(self.get_database_folder(), "asdf.sqlite3")))
 
     def test_get(self):
         with self.database as db:
             base = db.query(DatabaseTestModel)
             res = base.get("asdf")
             self.assertIsNone(res)
 
@@ -272,19 +272,19 @@
     """
     there was an issue, which prevented a database from beeing migrated multiple times in a single process
     """
     create_database = False
     alembic_path = "../tests/test_database_data"
 
     def test_migrate_1(self):
-        database = Database(self.database_folder, self.database_name, self.alembic_path)
+        database = Database(self.get_database_folder(), self.database_name, self.alembic_path)
         with database as db:
             self.assertEqual(0, db.query(DatabaseTestModel).count())
         database.shutdown()
         self.delete_database(database)
 
     def test_migrate_2(self):
-        database = Database(self.database_folder, self.database_name, self.alembic_path)
+        database = Database(self.get_database_folder(), self.database_name, self.alembic_path)
         with database as db:
             self.assertEqual(0, db.query(DatabaseTestModel).count())
         database.shutdown()
         self.delete_database(database)
```

### Comparing `openmodule-9.0.0rc9/tests/test_database_data/alembic/versions/32b8c728abbf_initial.py` & `openmodule-9.1.0/tests/test_database_data/alembic/versions/32b8c728abbf_initial.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_database_data/alembic.ini` & `openmodule-9.1.0/tests/test_database_data/alembic.ini`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_database_data/makemigration.sh` & `openmodule-9.1.0/tests/test_database_data/makemigration.sh`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_dispatcher.py` & `openmodule-9.1.0/tests/test_dispatcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from concurrent.futures.process import ProcessPoolExecutor
+from concurrent.futures.thread import ThreadPoolExecutor
 from functools import partial
 from typing import Any
 from unittest import TestCase
 
 from openmodule.config import settings
 from openmodule.dispatcher import MessageDispatcher, SubscribingMessageDispatcher
 from openmodule.models.base import ZMQMessage, OpenModuleModel
+from openmodule.utils.io import IoListener
+from openmodule.utils.presence import PresenceListener
 
 
 class MessageDispatcherBaseTest(TestCase):
     dispatcher: MessageDispatcher
     message: Any
 
     def dummy_message(self, type="test", **kwargs):
@@ -26,29 +30,31 @@
     def tearDown(self) -> None:
         settings.reset()
         super().tearDown()
 
 
 class MessageDispatcherBasicsTestCase(MessageDispatcherBaseTest):
     def test_topic_is_str(self):
-        self.dispatcher.register_handler("test", ZMQMessage, self._set_true_handler)
+        self.dispatcher.register_handler("test", ZMQMessage, self._set_true_handler, match_type=False)
         self.assertIsNone(self.message)
 
         self.dispatcher.dispatch(b"test", self.dummy_message())
         self.assertIsNotNone(self.message)
 
     def test_no_filter(self):
-        self.dispatcher.register_handler(b"test", ZMQMessage, self._set_true_handler)
+        self.dispatcher.register_handler(b"test", ZMQMessage, self._set_true_handler, match_type=False)
         self.assertIsNone(self.message)
 
         self.dispatcher.dispatch(b"test", self.dummy_message())
         self.assertIsNotNone(self.message)
 
     def test_filter(self):
-        self.dispatcher.register_handler(b"test", ZMQMessage, self._set_true_handler, filter={"type": "some-type"})
+        self.dispatcher.register_handler(b"test", ZMQMessage, self._set_true_handler,
+                                         match_type=False,
+                                         filter=lambda msg: msg.get("type") == "some-type")
 
         # filter does not match
         self.dispatcher.dispatch(b"test", self.dummy_message(type="incorrect"))
         self.assertIsNone(self.message)
 
         # filter matches
         self.dispatcher.dispatch(b"test", self.dummy_message("some-type"))
@@ -56,32 +62,34 @@
 
     def test_multiple_filter(self):
         # multiple handlers with identical filters and topics are allowed
         self.message1 = None
         self.message2 = None
 
         self.dispatcher.register_handler(b"test", ZMQMessage, partial(self._set_true_handler, var="message1"),
-                                         filter={"type": "some-type"})
+                                         match_type=False,
+                                         filter=lambda msg: msg.get("type") == "some-type")
         self.dispatcher.register_handler(b"test", ZMQMessage, partial(self._set_true_handler, var="message2"),
-                                         filter={"type": "some-type"})
+                                         match_type=False,
+                                         filter=lambda msg: msg.get("type") == "some-type")
 
         # filter does not match
         self.dispatcher.dispatch(b"test", self.dummy_message(type="incorrect"))
         self.assertIsNone(self.message1)
         self.assertIsNone(self.message2)
 
         # filter matches
         self.dispatcher.dispatch(b"test", self.dummy_message("some-type"))
         self.assertIsNotNone(self.message1)
         self.assertIsNotNone(self.message2)
 
     def test_prefix_does_not_match(self):
         # since zmq subscribes on all topics as prefixes, the dispatcher
         # has to full-match the topic
-        self.dispatcher.register_handler(b"test", ZMQMessage, self._set_true_handler)
+        self.dispatcher.register_handler(b"test", ZMQMessage, self._set_true_handler, match_type=False)
         self.dispatcher.dispatch(b"testp", self.dummy_message())
         self.assertIsNone(self.message)
 
         # exact match works
         self.dispatcher.dispatch(b"test", self.dummy_message())
         self.assertIsNotNone(self.message)
 
@@ -115,30 +123,49 @@
 
 class MessageDispatcherWithoutExecutorTestCase(MessageDispatcherBaseTest):
     def test_exception_in_handler(self):
         def raises_exception(message):
             raises_exception.register_schema = False
             raise Exception("something broke!")
 
-        self.dispatcher.register_handler(b"test", ZMQMessage, raises_exception, register_schema=False)
+        self.dispatcher.register_handler(b"test", ZMQMessage, raises_exception, register_schema=False, match_type=False)
         with self.assertLogs() as cm:
             self.dispatcher.dispatch(b"test", self.dummy_message())
         self.assertIn("something broke!", cm.output[0])
 
     def test_validation_error(self):
         def handler(x):
             pass
 
         handler.register_schema = False
-        self.dispatcher.register_handler("test", ZMQMessage, handler, register_schema=False)
+        self.dispatcher.register_handler("test", ZMQMessage, handler, register_schema=False, match_type=False)
         with self.assertLogs() as cm:
             self.dispatcher.dispatch(b"test", {})
         self.assertIn("validation error", cm.output[0])
 
 
+class MessageDispatcherWithExecutorTestCase(TestCase):
+    def test_is_multithreaded(self):
+        self.assertFalse(MessageDispatcher(executor=ThreadPoolExecutor(max_workers=1)).is_multi_threaded)
+        self.assertFalse(MessageDispatcher(executor=ProcessPoolExecutor(max_workers=1)).is_multi_threaded)
+        self.assertFalse(MessageDispatcher(executor=None).is_multi_threaded)
+
+        self.assertTrue(MessageDispatcher(executor=dict(a=1)).is_multi_threaded)  # default fallback -> multithreaded
+        self.assertTrue(MessageDispatcher(executor=ThreadPoolExecutor(max_workers=2)).is_multi_threaded)
+        self.assertTrue(MessageDispatcher(executor=ProcessPoolExecutor(max_workers=2)).is_multi_threaded)
+
+    def test_presence_listener_asserts_on_muiltithreaded_dispatcher(self):
+        with self.assertRaises(AssertionError):
+            PresenceListener(MessageDispatcher(executor=ThreadPoolExecutor(max_workers=2)))
+
+    def test_io_listener_asserts_on_muiltithreaded_dispatcher(self):
+        with self.assertRaises(AssertionError):
+            IoListener(MessageDispatcher(executor=ThreadPoolExecutor(max_workers=2)))
+
+
 class SubscribingMessageDispatcherTestCase(TestCase):
     subscriptions = set()
 
     def subscribe(self, topic):
         self.subscriptions.add(topic)
 
     def unsubscribe(self, topic):
@@ -148,20 +175,22 @@
         self.subscriptions.clear()
         self.dispatcher = SubscribingMessageDispatcher(
             subscribe=self.subscribe,
             unsubscribe=self.unsubscribe
         )
 
     def test_subscribe(self):
-        self.dispatcher.register_handler(b"topic1", ZMQMessage, lambda *x: x, register_schema=False)
+        self.dispatcher.register_handler(b"topic1", ZMQMessage, lambda *x: x, register_schema=False, match_type=False)
         self.assertEqual({b"topic1"}, self.subscriptions)
 
     def test_unsubscribe(self):
-        listener1 = self.dispatcher.register_handler(b"topic1", ZMQMessage, lambda *x: x, register_schema=False)
-        listener2 = self.dispatcher.register_handler(b"topic1", ZMQMessage, lambda *x: x, register_schema=False)
+        listener1 = self.dispatcher.register_handler(b"topic1", ZMQMessage, lambda *x: x,
+                                                     register_schema=False, match_type=False)
+        listener2 = self.dispatcher.register_handler(b"topic1", ZMQMessage, lambda *x: x,
+                                                     register_schema=False, match_type=False)
 
         self.assertEqual({b"topic1"}, self.subscriptions)
 
         # listener 2 is still subscribed, topic should still be listed in subscriptions
         self.dispatcher.unregister_handler(listener1)
         self.assertEqual({b"topic1"}, self.subscriptions)
```

### Comparing `openmodule-9.0.0rc9/tests/test_health.py` & `openmodule-9.1.0/tests/test_health.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_interrupt.py` & `openmodule-9.1.0/tests/test_interrupt.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     except Exception as e:
         logging.info(f"exception: {e}")
     else:
         logging.info("not running")
     finally:
         logging.info("killed")
 
+    # we have to sleep some so the logs make their way to the parent process
+    time.sleep(1)
+
 
 class InterruptTest(InterruptTestMixin, TestCase):
     def test_keyboard(self):
         with self.assertLogs() as cm:
             self.signal_in_function(test, KeyboardInterrupt)
         self.assertIn("Keyboard", str(cm.output))
 
@@ -120,8 +123,7 @@
 
 
 class ExceptionInFunctionTest(MainTestMixin):
     def test_uncaught_exception_in_function(self):
         with self.assertRaises(AssertionError) as e:
             self.signal_in_function(exception_raiser, KeyboardInterrupt)
         self.assertIn("Process did not finish gracefully", str(e.exception))
-
```

### Comparing `openmodule-9.0.0rc9/tests/test_io_listen.py` & `openmodule-9.1.0/tests/test_io_listen.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class IoTest(OpenModuleCoreTestMixin, TestCase):
     def setUp(self) -> None:
         super().setUp()
         self.io = IoListener(self.core.messages)
         io_init_event = MockEvent()
-        self.core.messages.register_handler(b"io", ZMQMessage, handler=io_init_event)
+        self.core.messages.register_handler(b"io", ZMQMessage, handler=io_init_event, match_type=False)
         self.wait_for_dispatcher(self.core.messages)
 
         self.io_sim = IoSimulator(generate_example_states(count=18), emit=lambda x: self.zmq_client.send(b"io", x))
 
         # we have to wait here for the initial io states to settle
         # IMO we should move this into the simulator itself, or construct the testcases
         # in a way to not depend on this.
@@ -98,15 +98,20 @@
         on_falling_edge.reset_all_mocks()
         self.io_sim.set_pin_low(pin)
         on_falling_edge.wait_for_call()
 
     def test_listen_to_gateway(self):
         on_any_edge = MockEvent()
         gw = list(self.io_sim.get_pin_states().values())[0].gateway
-        gateway = Gateway(gate=gw.gate, direction=gw.direction)
+
+        # check that the gateway direction does not matter for the filter
+        # by explicitly setting sthe wrong direction
+        self.assertEqual(gw.direction, "in")
+        gateway = Gateway(gate=gw.gate, direction="out")
+
         self.io.add_listener_edge_any(listen_to=gateway, callback=on_any_edge)
         self.io_sim.set_pin_high(list(self.io_sim.get_pin_states().keys())[0])
         on_any_edge.wait_for_call()
         on_any_edge.reset_all_mocks()
         self.io_sim.set_pin_high(list(self.io_sim.get_pin_states().keys())[1])
         on_any_edge.wait_for_call()
         on_any_edge.reset_all_mocks()
```

### Comparing `openmodule-9.0.0rc9/tests/test_messaging.py` & `openmodule-9.1.0/tests/test_messaging.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,17 @@
         self.assertEqual(res, (None, None))
         self.assertIn("not a dict", str(cm.output))
 
 
 class WaitForConnectionTestCase(OpenModuleCoreTestMixin, TestCase):
     protocol = "tcp://"
 
+    def test_wait_for_connection_uses_core(self):
+        wait_for_connection(self.core.messages)
+
     def test_wait_for_connection(self):
         pub_socket = get_pub_socket(self.zmq_context(), self.zmq_config())
         wait_for_connection(self.core.messages, pub_socket)
 
     def test_wait_for_connection_timeout(self):
         try:
             with override_context(BROKER_SUB="tcp://127.0.0.1:900"):
```

### Comparing `openmodule-9.0.0rc9/tests/test_model.py` & `openmodule-9.1.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_models_backend.py` & `openmodule-9.1.0/tests/test_models_backend.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_rpc.py` & `openmodule-9.1.0/tests/test_rpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import time
+from concurrent.futures import ThreadPoolExecutor
 from functools import partial
-from typing import Union
+from typing import Union, Callable
 from unittest import TestCase
 from uuid import uuid4
 
 from pydantic.types import conint
 
 from openmodule.config import settings, override_context
 from openmodule.models.base import OpenModuleModel, EmptyModel, ZMQMessage
@@ -83,23 +84,23 @@
 
 class TestRPCResponse2(OpenModuleModel):
     __test__ = False
     some_payload: str
 
 
 class RPCServerTestCase(RPCServerTestMixin):
-    rpc_channels = ["channel", "channel2"]
+    rpc_channels = ["channel", "channel2", "a", "ab"]
     topics = ["test"]
 
     server: RPCServer
 
     def setUp(self):
         super().setUp()
         self.called_types = {}
-        self.server = RPCServer(self.zmq_context(), self.zmq_config())
+        self.server = RPCServer(self.zmq_context())
         self.server_thread = self.server.run_as_thread()
 
     def tearDown(self):
         self.server.shutdown()
         self.server_thread.join()
         super().tearDown()
 
@@ -366,14 +367,33 @@
             response = self.rpc("channel", "test-type", {}, resource=settings.RESOURCE)
         self.assertRPCSuccess(response)
         self.assertIn("handler 1", str(cm.output))
 
         with self.assertRaises(TimeoutError):
             self.rpc("channel", "test-type", {}, resource="test-2")
 
+    def test_prefix_matched_topic(self):
+        def handler1(*_, **__):
+            """ test rpc handler"""
+            logging.info("handler 1")
+            return TestRPCResponse()
+
+        self.server.register_handler("a", "test-type", TestRPCRequest, TestRPCResponse, handler1)
+        self.wait_for_rpc_server(self.server)
+
+        with self.assertLogs() as cm:
+            # we use assertLogs here to capture log output, but we would need assertNoLogs from python3.10
+            # so we log some dummy message and check assertNotIn afterwards
+            logging.info("some-log-so assert works")
+
+            with self.assertRaises(TimeoutError):
+                self.rpc("ab", "test-type", {})
+
+        self.assertNotIn("no handler found", str(cm.output))
+
     def test_union_response_parsing(self):
         """
         tests that the rpc server correctly response when Union types are used as responses
         """
 
         class Integer(OpenModuleModel):
             some_int: int
@@ -478,21 +498,21 @@
         """test handler"""
         logging.info("timout_handler")
         time.sleep(3)
         return TestRPCResponse2(some_payload="abc")
 
     def setUp(self):
         super().setUp()
-        self.server = RPCServer(config=self.zmq_config(), context=self.zmq_context(), filter_resource=False)
+        self.server = RPCServer(context=self.zmq_context(), filter_resource=False)
         self.server.register_handler("channel", "test", TestRPCRequest, TestRPCResponse2, self.handler1)
         self.server.register_handler("channel", "timeout", TestRPCRequest, TestRPCResponse2, self.timeout_handler)
         self.server.run_as_thread()
         self.wait_for_rpc_server(self.server)
 
-        self.client = RPCClient(self.core.messages, channels=[b"channel"])
+        self.client = RPCClient(self.core.messages, channels=[b"channel"], _warn=False)
         self.wait_for_dispatcher(self.core.messages)
 
     def test_blocking(self):
         result = self.client.rpc(b"channel", "test", EmptyModel(), timeout=1)
         self.assertEqual("ok", result.status)
 
         with self.assertRaises(TimeoutError):
@@ -573,33 +593,51 @@
         time.sleep(3)
         self.assertTrue(result.done())
         result = result.result()
         self.assertEqual("ok", result.status)
         self.assertIn("some_payload", result.response)
 
 
-class RpcClientResourceTest(RPCServerTestMixin, OpenModuleCoreTestMixin):
-    rpc_channels = ["channel"]
+class TestRPCResponseNotSerializable(OpenModuleModel):
+    __test__ = False
+    some_payload: Callable
+
+
+class RPCServerMultithreadingTest(OpenModuleCoreTestMixin, TestCase):
+    """
+    serialization errors were not captured in multithreaded rpc server
+    this testcase ensures that this is not the case anymore
+    """
+
+    rpc_channels = ["test"]
+    topics = ["sentry"]
+    init_kwargs = {"sentry": True}
+
+    def raise_exception_handler(self, _, __):
+        """
+        returns a model which cannot be serialized to json
+        """
+        return {"some_payload": self.rpc}
 
     def setUp(self):
         super().setUp()
-        self.server = RPCServer(config=self.zmq_config(), context=self.zmq_context(), filter_resource=True)
-        self.server.register_handler("channel", "test", TestRPCRequest, TestRPCResponse2, RpcClientTest.handler1)
-        self.server.register_handler("channel", "timeout", TestRPCRequest, TestRPCResponse2,
-                                     RpcClientTest.timeout_handler)
+
+        self.executor = ThreadPoolExecutor(max_workers=3)
+        self.server = RPCServer(self.zmq_context(), executor=self.executor)
+        self.server.register_handler("test", "test", EmptyModel, TestRPCResponseNotSerializable,
+                                     self.raise_exception_handler, register_schema=False)
         self.server.run_as_thread()
-        self.wait_for_rpc_server(self.server)
 
-        self.client = RPCClient(self.core.messages, channels=[b"channel"])
-        self.wait_for_dispatcher(self.core.messages)
+    def tearDown(self):
+        super().tearDown()
+        self.server.shutdown()
 
-    def test_resource_filter(self):
-        result = self.client.rpc(b"channel", "test", EmptyModel(), timeout=1)
-        self.assertEqual("ok", result.status)
+    def test_executor_logs_exceptions(self):
+        """
+        ensures that when using a multiprocessing executor exceptions are logged to logging and sentry
+        """
+        with self.assertLogs(level=logging.ERROR) as cm:
+            self.rpc("test", "test", EmptyModel(), receive_response=False)
+            self.zmq_client.wait_for_message_on_topic(b"sentry")
+        self.assertTrue(cm.output)
 
-        with override_context(RESOURCE="asdf"):
-            with self.assertRaises(TimeoutError):
-                self.client.rpc(b"channel", "test", EmptyModel(), timeout=1)
 
-        with override_context(RESOURCE=""):
-            result = self.client.rpc(b"channel", "test", EmptyModel(), timeout=1)
-            self.assertEqual("ok", result.status)
```

### Comparing `openmodule-9.0.0rc9/tests/test_schema.py` & `openmodule-9.1.0/tests/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import os
 from functools import partial
 from unittest import TestCase
 
-from openmodule.config import settings
-from openmodule.models.backend import AccessRequest, AccessResponse
+from openmodule.config import override_settings, override_context
+from openmodule.models.backend import AccessRequest, AccessResponse, BackendRegisterMessage
 from openmodule.rpc.server import RPCServer
 from openmodule.utils.schema import Schema
 from openmodule_test.core import OpenModuleCoreTestMixin
 from openmodule_test.rpc import RPCServerTestMixin
 
 file_name = "../schemas.json"
 
+
 def test(*args, **kwargs):
     """
     Test
     """
     return None
 
 
@@ -190,53 +191,51 @@
     def test_save(self):
         Schema.save_rpc("backend", "abc", AccessRequest, AccessRequest, test)
         Schema.save_message("abc", AccessRequest, test)
         self.assertEqual(1, len(Schema.messages))
         self.assertEqual(1, len(Schema.rpcs))
         num_models = len(Schema.models)
 
-        os.environ["TESTING"] = "False"
-        Schema.save_rpc("backend", "abc", AccessRequest, AccessResponse, test)
-        Schema.save_message("abc", AccessRequest, test)
-        self.assertEqual(1, len(Schema.messages))
-        self.assertEqual(1, len(Schema.rpcs))
-        self.assertEqual(num_models, len(Schema.models))
-        os.environ["TESTING"] = "True"
+        with override_context(TESTING=False):
+            Schema.save_rpc("backend", "abc", AccessRequest, AccessResponse, test)
+            Schema.save_message("abc", AccessRequest, test)
+            self.assertEqual(1, len(Schema.messages))
+            self.assertEqual(1, len(Schema.rpcs))
+            self.assertEqual(num_models, len(Schema.models))
 
 
 class LiveTest(RPCServerTestMixin, OpenModuleCoreTestMixin):
     rpc_channels = ["backend"]
     topics = ["backend"]
 
     def setUp(self):
         super().setUp()
-        self.server = RPCServer(config=self.zmq_config(), context=self.zmq_context())
-        self.server.run_as_thread()
         try:
             os.remove(file_name)
         except:
             pass
         Schema.clear()
+        self.server = RPCServer(context=self.zmq_context())
+        self.server.run_as_thread()
 
     def tearDown(self) -> None:
         super().tearDown()
         try:
             os.remove(file_name)
         except:
             pass
         Schema.clear()
 
     def test_save(self):
         self.server.register_handler("backend", "test", AccessRequest, AccessResponse, test)
-        self.core.messages.register_handler("backend", AccessRequest, test)
+        self.core.messages.register_handler("backend", BackendRegisterMessage, test)
         self.wait_for_rpc_server(self.server)
         self.wait_for_dispatcher(self.core.messages)
         self.assertEqual(1, len(Schema.messages))
         self.assertEqual(1, len(Schema.rpcs))
 
         self.server.register_handler("backend", "abc", AccessRequest, AccessResponse, test3, register_schema=False)
-        self.core.messages.register_handler("abc", AccessRequest, test3, register_schema=False)
+        self.core.messages.register_handler("abc", BackendRegisterMessage, test3, register_schema=False)
         self.wait_for_rpc_server(self.server)
         self.wait_for_dispatcher(self.core.messages)
         self.assertEqual(1, len(Schema.messages))
         self.assertEqual(1, len(Schema.rpcs))
-
```

### Comparing `openmodule-9.0.0rc9/tests/test_test_alert.py` & `openmodule-9.1.0/tests/test_test_alert.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_test_gate.py` & `openmodule-9.1.0/tests/test_test_gate.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_test_zeromq.py` & `openmodule-9.1.0/tests/test_test_zeromq.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_utils_backend.py` & `openmodule-9.1.0/tests/test_utils_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from unittest import TestCase
-
 import json
 from textwrap import dedent
+from unittest import TestCase
 
-from openmodule.config import override_settings
 from openmodule.models.backend import CountMessage, AccessRequest, Access, AccessCategory, check_recurrence
 from openmodule.models.base import Gateway
 from openmodule.rpc.server import RPCServer
 from openmodule.utils.backend import Backend
 from openmodule_test.backend import TestBackend, BackendTestMixin
 from openmodule_test.eventlistener import MockEvent
 from openmodule_test.rpc import RPCServerTestMixin
@@ -129,29 +127,27 @@
 
         with self.assertRaises(Exception) as e:
             Access(user="asdf", category="permanent_employee", start=3,
                    recurrence="DTSTART:20180702T123000\nFREQ=WEEKLY;BYDAY=MO,TU,WE,TH,FR")
         self.assertIn("not a valid enumeration", str(e.exception))
 
 
-@override_settings(USER_PREFIX="backend")
 class NotImplementedTestCase(BackendTestMixin, TestCase):
     backend_class = Backend
 
     # noinspection PyTypeChecker
     def test_not_implemented(self):
         with self.assertRaises(NotImplementedError):
             self.backend.check_in(None)
         with self.assertRaises(NotImplementedError):
             self.backend.check_out(None)
         with self.assertRaises(NotImplementedError):
             self.backend.check_access(None)
 
 
-@override_settings(USER_PREFIX="backend")
 class FunctionTest(BackendTestMixin, TestCase):
     backend_class = TestBackend
 
     def test_check_in(self):
         transaction_id = self.check_in()
         message = self.messages_by_transaction.get(transaction_id)
         self.assertEqual(None, message.error)
@@ -246,23 +242,22 @@
         self.assertEqual(True, result.success)
         self.assertEqual([], result.medium.accesses)
 
         result = self.check_auth(medium_id="GARIVO1", medium_type="lpr", gateway=Gateway(gate="error", gateway="in"))
         self.assertEqual(False, result.success)
 
 
-@override_settings(USER_PREFIX="backend")
 class RpcTest(BackendTestMixin, RPCServerTestMixin, TestCase):
     rpc_channels = ["backend"]
     topics = [b"backend", b"count", b"healthz"]
     backend_class = TestBackend
 
     def setUp(self):
         super().setUp()
-        self.server = RPCServer(config=self.zmq_config(), context=self.zmq_context())
+        self.server = RPCServer(context=self.zmq_context())
         self.server.run_as_thread()
         self.backend.register_rpcs(self.server)
         self.wait_for_rpc_server(self.server)
 
     def tearDown(self):
         self.server.shutdown()
         super().tearDown()
```

### Comparing `openmodule-9.0.0rc9/tests/test_utils_charset.py` & `openmodule-9.1.0/tests/test_utils_charset.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_utils_connection_status.py` & `openmodule-9.1.0/tests/test_utils_connection_status.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_utils_matching.py` & `openmodule-9.1.0/tests/test_utils_matching.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tests/test_utils_presence.py` & `openmodule-9.1.0/tests/test_utils_presence.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from datetime import datetime
 from functools import partial
 
 import orjson
 from typing import Optional
 
 import time
 from unittest import TestCase
 
 from openmodule.core import init_openmodule, shutdown_openmodule
-from openmodule.models.base import Direction
-from openmodule.models.presence import PresenceBaseMessage
-from openmodule.models.vehicle import MakeModel
+from openmodule.models.base import Direction, Gateway
+from openmodule.models.presence import PresenceBaseMessage, PresenceRPCRequest, PresenceRPCResponse, PresenceBaseData, \
+    PresenceMedia
+from openmodule.models.vehicle import MakeModel, LPRMedium, LPRCountry, PresenceAllIds
+from openmodule.rpc import RPCServer
 from openmodule.utils.presence import PresenceListener
 from openmodule_test.eventlistener import MockEvent
 from openmodule_test.presence import PresenceSimulator
 from openmodule_test.zeromq import ZMQTestMixin
 
 
 class BasePresenceTest(ZMQTestMixin, TestCase):
@@ -204,7 +207,55 @@
 
     def test_presence_alias_fields_serialization(self):
         sim = PresenceSimulator("gate1", Direction.IN, partial(setattr, self, "message"))
         sim.enter(sim.vehicle().qr("test"))
         sim.forward()
         message = orjson.loads(self.message.json_bytes())
         self.assertIn("leave-time", message)
+
+
+class PresenceRPCTest(ZMQTestMixin, TestCase):
+    def setUp(self) -> None:
+        super().setUp()
+        self.core = init_openmodule(self.zmq_config(), context=self.zmq_context())
+        self.wait_for_dispatcher(self.core.messages)
+        self.presence_sim = PresenceSimulator("gate_in", Direction.IN, lambda x: self.zmq_client.send(b"presence", x))
+        self.rpc_server = RPCServer(context=self.core.context)
+        self.rpc_server.register_handler("tracking", "get-present", PresenceRPCRequest, PresenceRPCResponse,
+                                         self.on_reply)
+        self.rpc_server.run_as_thread()
+        self.present = False
+
+    def tearDown(self):
+        self.rpc_server.shutdown()
+        shutdown_openmodule()
+        super().tearDown()
+
+    def on_reply(self, request: PresenceRPCRequest, _) -> PresenceRPCResponse:
+        """
+        Emulates Trackings Presence RPC
+        """
+        if self.present:
+            return PresenceRPCResponse(presents=[
+                PresenceBaseData(vehicle_id=1, source="gate_in", present_area_name="gate_in",
+                                 last_update=datetime.utcnow(), gateway=Gateway(gate="gate_in", direction="in"),
+                                 medium=PresenceMedia(lpr=LPRMedium(id="T EST 1")), all_ids=PresenceAllIds())])
+        else:
+            return PresenceRPCResponse(presents=[])
+
+    def test_presence_rpc_plate(self):
+        self.present = True
+        self.presence = PresenceListener(self.core.messages, gate="gate_in")
+        self.presence.init_present_vehicles()
+        self.assertNotEqual({}, self.presence.present_vehicles)
+
+    def test_presence_rpc_no_plate(self):
+        self.present = False
+        self.presence = PresenceListener(self.core.messages, gate="gate_in")
+        self.presence.init_present_vehicles()
+        self.assertEqual({}, self.presence.present_vehicles)
+
+    def test_presence_rpc_only_allowed_for_gates(self):
+        self.presence = PresenceListener(self.core.messages)
+        with self.assertRaises(AssertionError) as e:
+            self.presence.init_present_vehicles()
+        self.assertIn("if the gate is set", str(e.exception))
```

### Comparing `openmodule-9.0.0rc9/tests/test_utils_vehicle.py` & `openmodule-9.1.0/tests/test_utils_vehicle.py`

 * *Files identical despite different names*

### Comparing `openmodule-9.0.0rc9/tox.ini` & `openmodule-9.1.0/tox.ini`

 * *Files identical despite different names*

