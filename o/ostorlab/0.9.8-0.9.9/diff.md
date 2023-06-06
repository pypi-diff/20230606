# Comparing `tmp/ostorlab-0.9.8.tar.gz` & `tmp/ostorlab-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ostorlab-0.9.8.tar", last modified: Fri Sep  9 07:47:02 2022, max compression
+gzip compressed data, was "ostorlab-0.9.9.tar", last modified: Fri Sep 16 15:15:57 2022, max compression
```

## Comparing `ostorlab-0.9.8.tar` & `ostorlab-0.9.9.tar`

### file list

```diff
@@ -1,1117 +1,1117 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-09 07:46:48.000000 ostorlab-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-09-09 07:47:02.867612 ostorlab-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9572 2022-09-09 07:46:48.000000 ostorlab-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-09-09 07:47:02.871612 ostorlab-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-09 07:46:48.000000 ostorlab-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.767610 ostorlab-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.787611 ostorlab-0.9.8/src/ostorlab/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.787611 ostorlab-0.9.8/src/ostorlab/agent/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15099 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.787611 ostorlab-0.9.8/src/ostorlab/agent/kb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.779610 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CLASSES/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CLASSES/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CLASSES/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CLASSES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.791611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.795611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_EXPORTED/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_EXPORTED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_EXPORTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_EXPORTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_LIST/
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.799611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_MANIFEST/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_MANIFEST/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_MANIFEST/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_MANIFEST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.803611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AUTHENTICATION/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AUTHENTICATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AUTHENTICATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AUTHENTICATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CORDOVA_XSS/
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CORDOVA_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CORDOVA_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CORDOVA_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.807611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     4979 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.811611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.815611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXPANSION_APK/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXPANSION_APK/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXPANSION_APK/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXPANSION_APK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.819611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_BITCODE/
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_BITCODE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_BITCODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_BITCODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.823611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/MEMORY_LEAK/
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/MEMORY_LEAK/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/MEMORY_LEAK/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/MEMORY_LEAK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.827612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_API/
--rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_API/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_API/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_API/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SQL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SQL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SQL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SQL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.831611 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HTTP/
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HTTP/description.md
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HTTP/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HTTP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.835612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/USER_ENUMERATION/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/USER_ENUMERATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/USER_ENUMERATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/USER_ENUMERATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.839612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.839612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.839612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.839612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_GENERIC/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_GENERIC/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_GENERIC/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_GENERIC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.839612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.839612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.839612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_IDOR/
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_IDOR/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_IDOR/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_IDOR/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)     5705 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_XSS/
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-09-09 07:46:49.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_XSS/recommendation.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/kb/kb.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/message/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/message.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/common/x509/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/common/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20774 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.843612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/agent/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10922 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/source/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3249 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6433 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14713 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.847612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6371 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14713 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/link/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22845 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4045 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/artifact/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/request/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9180 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/response/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7777 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/logs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/request_response/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/request_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13089 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4492 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4478 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.851612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/healthcheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/status/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12857 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/proto_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/message/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5129 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     7198 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_mq_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10398 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     7764 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_persist_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/mixins/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/mixins/protocols/emit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.855612 ostorlab-0.9.8/src/ostorlab/agent/schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4365 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/schema/agent_group_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     5796 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/schema/agent_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/schema/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/agent/schema/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/apis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/agent_details.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/agent_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/agent_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/create_agent_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/create_api_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/login.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/revoke_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/apis/runners/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6227 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/runners/authenticated_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/runners/login_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/runners/public_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/runners/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/scan_create.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/scan_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/scan_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/scan_stop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/vulnz_describe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/apis/vulnz_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/assets/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/TODO.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/agent.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/domain_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/ip.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/assets/link.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/cli/agent/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/cli/agent/build/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5006 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/build/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/build/build_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/cli/agent/delete/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/delete/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.859612 ostorlab-0.9.8/src/ostorlab/cli/agent/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/healthcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/healthcheck/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/agent/install/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/install/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/install/install_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/agent/list/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/list/list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/agent/search/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agent/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/agentgroup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agentgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/agentgroup/agentgroup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/auth/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/auth/login/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/auth/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/auth/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/auth/revoke/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/auth/revoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/auth/revoke/revoke.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/ci_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/mobile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/docker_requirements_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/dumpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/input_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     5495 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/install_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/rootcli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/scan/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/scan/list/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/list/list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/scan/run/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/agent.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/domain_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/run/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/scan/stop/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/stop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/scan/stop/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.863612 ostorlab-0.9.8/src/ostorlab/cli/vulnz/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/cli/vulnz/describe/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/describe/describe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/cli/vulnz/dump/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/dump/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/cli/vulnz/list/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/list/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/cli/vulnz/vulnz.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/main.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/runtimes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/runtimes/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16413 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/cloud/runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/runtimes/lite_local/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/lite_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14418 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/lite_local/agent_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)    14570 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/lite_local/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/runtimes/local/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14051 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/agent_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/log_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/runtimes/local/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5750 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/models/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    26550 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/runtimes/local/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/services/jaeger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/services/mq.py
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/local/services/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/runtimes/proto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13736 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/runtimes/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6857 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/testing/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.867612 ostorlab-0.9.8/src/ostorlab/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/defintions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/dictionary_minifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/risk_rating.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/styles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-09-09 07:46:48.000000 ostorlab-0.9.8/src/ostorlab/utils/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 07:47:02.787611 ostorlab-0.9.8/src/ostorlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-09-09 07:47:02.000000 ostorlab-0.9.8/src/ostorlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    47554 2022-09-09 07:47:02.000000 ostorlab-0.9.8/src/ostorlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 07:47:02.000000 ostorlab-0.9.8/src/ostorlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-09 07:47:02.000000 ostorlab-0.9.8/src/ostorlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 07:47:02.000000 ostorlab-0.9.8/src/ostorlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-09 07:47:02.000000 ostorlab-0.9.8/src/ostorlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-09 07:47:02.000000 ostorlab-0.9.8/src/ostorlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-16 15:15:31.000000 ostorlab-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-09-16 15:15:57.745262 ostorlab-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9572 2022-09-16 15:15:31.000000 ostorlab-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-09-16 15:15:57.749262 ostorlab-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-16 15:15:31.000000 ostorlab-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.621259 ostorlab-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.641260 ostorlab-0.9.9/src/ostorlab/
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.641260 ostorlab-0.9.9/src/ostorlab/agent/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15099 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.641260 ostorlab-0.9.9/src/ostorlab/agent/kb/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.633259 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.641260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ANALYZE_JNI_ELF/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.641260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_INFO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CERTIFICAT_OUTDATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CHECK_ROOT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CLASSES/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CLASSES/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CLASSES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CLASSES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_CONST_STRINGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CODE_LOAD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_COMMAND_EXEC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.645260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_FILESYSTEM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HASH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_HTTP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_INTENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_PROCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SERIALIZATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SHARED_PREFERENCES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SSL_PINNING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.649260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_TLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_EXPORTED/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_EXPORTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_EXPORTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_EXPORTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FACEBOOK_DEBUG_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_LIST/
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_SQLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HARDCODED_URLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_HAS_FRAGILE_USER_DATA_NOT_SET/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_DOWNLOAD_MANAGER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.653260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_NOT_USED_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_LIST_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_MANIFEST/
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_MANIFEST/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_MANIFEST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_MANIFEST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOTIFICATION_SPOOFING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_USES_CLEAR_TEXT_TRAFFIC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.657260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WEBVIEWCLIENT_IMPL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AUTHENTICATION/
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AUTHENTICATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AUTHENTICATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AUTHENTICATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AWS_S3_PUBLIC_FILELIST_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BINARY_DISASSEMBLY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CORDOVA_XSS/
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CORDOVA_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CORDOVA_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CORDOVA_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_KEY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.661260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_BLUETOOTH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DELETE_FILE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_DYNAMIC_CODE_LOADING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXEC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4979 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_NATIVE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_RANDOM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_REFLECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      770 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.665260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SOCKET/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SSLTLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ZIP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_MEMORY_CORRUPTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPRECATED_COMPONENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXPANSION_APK/
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXPANSION_APK/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXPANSION_APK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXPANSION_APK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/EXTERNAL_DNS_INTERACTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.669260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_API_BLUETOOTH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_DIRECT_OBJECT_REFERENCE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_HOSTNAME_VALIDATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_SHARED_PREFERENCES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ASLR_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.673260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_BITCODE/
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_BITCODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_BITCODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_BITCODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENTITLEMENTS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FILE_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_FRAMEWORKS_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_PLIST_FILES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_SYMBOLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.677260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/MEMORY_LEAK/
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/MEMORY_LEAK/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/MEMORY_LEAK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/MEMORY_LEAK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/NETWORK_PORT_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/OUTDATED_VULNERABLE_COMPONENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_DEBUG_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.681260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PORT_OPEN_LOCALHOST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_API/
+-rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_API/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_API/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_API/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/REDIS_LIBRARY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_TO_SINK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SQL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SQL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SQL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SQL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STRINGS_BPLIST_FILES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_ANONSERVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.685260 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HTTP/
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HTTP/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HTTP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HTTP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SELFSIGNED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_SERVER_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_WEAK_TLS_VERSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/USER_ENUMERATION/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/USER_ENUMERATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/USER_ENUMERATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/USER_ENUMERATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/VIRUSTOTAL_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.689261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_GENERIC/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_GENERIC/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_GENERIC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_GENERIC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/
+-rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HEADER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_RP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_X_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_IDOR/
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_IDOR/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_IDOR/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_IDOR/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.693261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INTERESTING_RESPONSE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_NO_STRICT_TRANSPORT_SECURITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5705 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_XSS/
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_XSS/recommendation.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/kb/kb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/message.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/common/x509/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/common/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20774 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/agent/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10922 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.697261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/ios/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/ios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/source/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3249 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/
+-rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6433 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14713 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.701261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6371 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14713 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/link/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22845 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.705261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.709261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4045 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.709261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.709261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/artifact/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.709261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.709261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/request/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9180 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.709261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/response/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7777 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.709261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/logs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/request_response/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/request_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13089 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/ui_call/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/ui_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4492 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.713261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4478 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.717261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/healthcheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/healthcheck/ping/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/healthcheck/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.721261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.725261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.725261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/done/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.725261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/start/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.725261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.725261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/status/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.725261 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/vulnerability/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/vulnerability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12857 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/proto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/message/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.729261 ostorlab-0.9.9/src/ostorlab/agent/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5129 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7198 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_mq_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10398 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7764 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_persist_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.729261 ostorlab-0.9.9/src/ostorlab/agent/mixins/protocols/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/mixins/protocols/emit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.729261 ostorlab-0.9.9/src/ostorlab/agent/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4365 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/schema/agent_group_schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5796 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/schema/agent_schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/schema/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/agent/schema/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.733261 ostorlab-0.9.9/src/ostorlab/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/agent_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/agent_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/agent_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/assets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/create_agent_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/create_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/login.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/revoke_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.733261 ostorlab-0.9.9/src/ostorlab/apis/runners/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6227 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/runners/authenticated_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/runners/login_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/runners/public_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/runners/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/scan_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)      931 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/scan_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/scan_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/scan_stop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/vulnz_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/apis/vulnz_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.733261 ostorlab-0.9.9/src/ostorlab/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/assets/link.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.733261 ostorlab-0.9.9/src/ostorlab/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.733261 ostorlab-0.9.9/src/ostorlab/cli/agent/
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/agent/build/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5006 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/build/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/build/build_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/agent/delete/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/delete/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/agent/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/healthcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/healthcheck/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/agent/install/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/install/install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/install/install_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/agent/list/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/list/list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/agent/search/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agent/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/agentgroup/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agentgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/agentgroup/agentgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/auth/login/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/auth/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/auth/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/auth/revoke/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/auth/revoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/auth/revoke/revoke.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/ci_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/mobile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/docker_requirements_checker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/input_validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5495 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/install_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/rootcli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/scan/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/scan/list/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/list/list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.737262 ostorlab-0.9.9/src/ostorlab/cli/scan/run/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.741262 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/run/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.741262 ostorlab-0.9.9/src/ostorlab/cli/scan/stop/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/stop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/scan/stop/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.741262 ostorlab-0.9.9/src/ostorlab/cli/vulnz/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.741262 ostorlab-0.9.9/src/ostorlab/cli/vulnz/describe/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/describe/describe.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/cli/vulnz/dump/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/dump/dump.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/cli/vulnz/list/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/list/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/cli/vulnz/vulnz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/runtimes/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16413 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/cloud/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/runtimes/lite_local/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/lite_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14418 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/lite_local/agent_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14570 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/lite_local/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/runtimes/local/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14051 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/agent_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/log_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/runtimes/local/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5750 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26550 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/runtimes/local/services/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/services/jaeger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6429 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/services/mq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/local/services/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/runtimes/proto/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13736 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/runtimes/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6857 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/testing/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.745262 ostorlab-0.9.9/src/ostorlab/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/defintions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/dictionary_minifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/risk_rating.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/styles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-09-16 15:15:31.000000 ostorlab-0.9.9/src/ostorlab/utils/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:15:57.641260 ostorlab-0.9.9/src/ostorlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-09-16 15:15:57.000000 ostorlab-0.9.9/src/ostorlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    47554 2022-09-16 15:15:57.000000 ostorlab-0.9.9/src/ostorlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 15:15:57.000000 ostorlab-0.9.9/src/ostorlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-16 15:15:57.000000 ostorlab-0.9.9/src/ostorlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 15:15:57.000000 ostorlab-0.9.9/src/ostorlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-16 15:15:57.000000 ostorlab-0.9.9/src/ostorlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-16 15:15:57.000000 ostorlab-0.9.9/src/ostorlab.egg-info/top_level.txt
```

### Comparing `ostorlab-0.9.8/LICENSE` & `ostorlab-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/PKG-INFO` & `ostorlab-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ostorlab
-Version: 0.9.8
+Version: 0.9.9
 Summary: Ostorlab Agent and Extensibility CLI and SDK
 Home-page: https://github.com/Ostorlab/ostorlab
 Author: ostorlab team
 Author-email: legends@ostorlab.dev
 License: Apache-2.0
 Project-URL: Documentation, https://docs.ostorlab.co/
 Project-URL: Source, https://github.com/Ostorlab/ostorlab
```

### Comparing `ostorlab-0.9.8/README.md` & `ostorlab-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/setup.cfg` & `ostorlab-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = ostorlab team
 author_email = legends@ostorlab.dev
 license = Apache-2.0
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Ostorlab/ostorlab
-version = 0.9.8
+version = 0.9.9
 project_urls = 
 	Documentation = https://docs.ostorlab.co/
 	Source = https://github.com/Ostorlab/ostorlab
 	Changelog = https://docs.ostorlab.co/changelog/
 	Tracker = https://github.com/Ostorlab/ostorlab/issues
 	Twitter = https://twitter.com/OstorlabSec
 platforms = any
```

### Comparing `ostorlab-0.9.8/setup.py` & `ostorlab-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/agent.py` & `ostorlab-0.9.9/src/ostorlab/agent/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/definitions.py` & `ostorlab-0.9.9/src/ostorlab/agent/definitions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ATTACK_SURFACE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_SECURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_BACKUP_TITLE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_SECURE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DEBUG_TITLE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_CRYPTO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_IPC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_LOGGING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_NO_PERMISSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_RECEIVER_POOR_PERMISSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_SQLITE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_DYNAMIC_WEBVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_ELF_NOTPROTECTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_EXPORTED/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_EXPORTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILEOBSERVER_IMPL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_LIST/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_LIST/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_EXEC_CMD/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_MANIFEST/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_MANIFEST/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_NOT_OBFUSCATED/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_OBFUSCTAED/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_TASK_HIJACKING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_UNDECLARED_PERMISSIONS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/APK_WIFI_API_PII/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AUTHENTICATION/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AUTHENTICATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/AUTHENTICATION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/AUTHENTICATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CORDOVA_XSS/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CORDOVA_XSS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CORDOVA_XSS/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CORDOVA_XSS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CORDOVA_XSS/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CORDOVA_XSS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CROSS_ORIGIN_RESOURCE_SHARING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/CRYPTO_INSECURE_IV/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_ANDROIDSECURITY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_CRYPTO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_IPC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_LOG/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_SQL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_API_XML/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DANGEROUS_WIFI_API_PII/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/DEPENDENCY_CONFUSION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_CLASS_LOADING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PASSWORD_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_PERMISSION_FILESYSTEM/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INSECURE_RANDOM_SEED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/INTENT_SPOOFING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ANTI_DEBUG/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ARC_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_DEBUG_SYMBOL_PRESENT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_ENCRYPTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_INSECURE_TAP/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_KEYBOARD_CACHE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_STACK_SMASHING_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_HIJACKING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_INJIECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/IPA_URL_SCHEME_LIST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_LOGS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_CREDENTIALS_REQUEST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_HEALTH_INFORMATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/LEAKING_PERSONAL_INFORMATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/MEMORY_LEAK/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/MEMORY_LEAK/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PHONEGAP_WHITELIST_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PLIST_INSECURE_UI_FILE_SHARING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PRIVACY_API/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PRIVACY_API/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/PROCESS_CRASHES/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_NETWORK_REVIEW/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SECRETS_REVIEW/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SOURCE_MAP_CODE_LEAK/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/SQL_INJECTION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/SQL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_DEPRECATED_PROTOCOL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HEARTBLEED/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HTTP/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HTTP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_HTTP/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_HTTP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INSECURE_CIPHER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/TLS_INVALIDHOSTNAME/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNIQUE_USER_IDENTIFICATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/USER_ENUMERATION/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/USER_ENUMERATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEBVIEW_LOADURL_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CSP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_CT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_HSTS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_HTTP_XFO/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_IDOR/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_IDOR/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_ACCESS_CONTROL/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_XSS/description.md` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_XSS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/KB/WEB_XSS/meta.json` & `ostorlab-0.9.9/src/ostorlab/agent/kb/KB/WEB_XSS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/kb/kb.py` & `ostorlab-0.9.9/src/ostorlab/agent/kb/kb.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/message.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/message.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/proto_dict.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/proto_dict.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/message/serializer.py` & `ostorlab-0.9.9/src/ostorlab/agent/message/serializer.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py` & `ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_mq_mixin.py` & `ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_mq_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py` & `ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_persist_mixin.py` & `ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_persist_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py` & `ostorlab-0.9.9/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/mixins/protocols/emit.py` & `ostorlab-0.9.9/src/ostorlab/agent/mixins/protocols/emit.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/schema/agent_group_schema.json` & `ostorlab-0.9.9/src/ostorlab/agent/schema/agent_group_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/schema/agent_schema.json` & `ostorlab-0.9.9/src/ostorlab/agent/schema/agent_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/schema/loader.py` & `ostorlab-0.9.9/src/ostorlab/agent/schema/loader.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/agent/schema/validator.py` & `ostorlab-0.9.9/src/ostorlab/agent/schema/validator.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/agent_details.py` & `ostorlab-0.9.9/src/ostorlab/apis/agent_details.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/agent_group.py` & `ostorlab-0.9.9/src/ostorlab/apis/agent_group.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/agent_search.py` & `ostorlab-0.9.9/src/ostorlab/apis/agent_search.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/assets.py` & `ostorlab-0.9.9/src/ostorlab/apis/assets.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/create_agent_scan.py` & `ostorlab-0.9.9/src/ostorlab/apis/create_agent_scan.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/create_api_key.py` & `ostorlab-0.9.9/src/ostorlab/apis/create_api_key.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/login.py` & `ostorlab-0.9.9/src/ostorlab/apis/login.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/request.py` & `ostorlab-0.9.9/src/ostorlab/apis/request.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/revoke_api_key.py` & `ostorlab-0.9.9/src/ostorlab/apis/revoke_api_key.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/runners/authenticated_runner.py` & `ostorlab-0.9.9/src/ostorlab/apis/runners/authenticated_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/runners/login_runner.py` & `ostorlab-0.9.9/src/ostorlab/apis/runners/login_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/runners/public_runner.py` & `ostorlab-0.9.9/src/ostorlab/apis/runners/public_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/runners/runner.py` & `ostorlab-0.9.9/src/ostorlab/apis/runners/runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/scan_create.py` & `ostorlab-0.9.9/src/ostorlab/apis/scan_create.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/scan_info.py` & `ostorlab-0.9.9/src/ostorlab/apis/scan_info.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/scan_list.py` & `ostorlab-0.9.9/src/ostorlab/apis/scan_list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/scan_stop.py` & `ostorlab-0.9.9/src/ostorlab/apis/scan_stop.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/vulnz_describe.py` & `ostorlab-0.9.9/src/ostorlab/apis/vulnz_describe.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/apis/vulnz_list.py` & `ostorlab-0.9.9/src/ostorlab/apis/vulnz_list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/assets/agent.py` & `ostorlab-0.9.9/src/ostorlab/assets/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/assets/asset.py` & `ostorlab-0.9.9/src/ostorlab/assets/asset.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/build/build.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/build/build.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/build/build_progress.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/build/build_progress.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/delete/delete.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/delete/delete.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/healthcheck/healthcheck.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/healthcheck/healthcheck.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/install/install.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/install/install.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/install/install_progress.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/install/install_progress.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/list/list.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/agent/search/search.py` & `ostorlab-0.9.9/src/ostorlab/cli/agent/search/search.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/auth/login/login.py` & `ostorlab-0.9.9/src/ostorlab/cli/auth/login/login.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/auth/revoke/revoke.py` & `ostorlab-0.9.9/src/ostorlab/cli/auth/revoke/revoke.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/android_aab.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/android_apk.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/assets/mobile.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/assets/mobile.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/ci_scan/run/run.py` & `ostorlab-0.9.9/src/ostorlab/cli/ci_scan/run/run.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/console.py` & `ostorlab-0.9.9/src/ostorlab/cli/console.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/docker_requirements_checker.py` & `ostorlab-0.9.9/src/ostorlab/cli/docker_requirements_checker.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/dumpers.py` & `ostorlab-0.9.9/src/ostorlab/cli/dumpers.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/input_validators.py` & `ostorlab-0.9.9/src/ostorlab/cli/input_validators.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/install_agent.py` & `ostorlab-0.9.9/src/ostorlab/cli/install_agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/rootcli.py` & `ostorlab-0.9.9/src/ostorlab/cli/rootcli.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/list/list.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/agent.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/android_aab.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/android_apk.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/domain_name.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/domain_name.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/file.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/file.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/ios_ipa.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/ip.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/ip.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/assets/link.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/assets/link.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/run/run.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/run/run.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/scan.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/scan.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/scan/stop/stop.py` & `ostorlab-0.9.9/src/ostorlab/cli/scan/stop/stop.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/vulnz/describe/describe.py` & `ostorlab-0.9.9/src/ostorlab/cli/vulnz/describe/describe.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/vulnz/dump/dump.py` & `ostorlab-0.9.9/src/ostorlab/cli/vulnz/dump/dump.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/vulnz/list/list.py` & `ostorlab-0.9.9/src/ostorlab/cli/vulnz/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/cli/vulnz/vulnz.py` & `ostorlab-0.9.9/src/ostorlab/cli/vulnz/vulnz.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/configuration_manager.py` & `ostorlab-0.9.9/src/ostorlab/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/cloud/runtime.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/cloud/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/definitions.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/definitions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/lite_local/agent_runtime.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/lite_local/agent_runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/lite_local/runtime.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/lite_local/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/local/agent_runtime.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/local/agent_runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/local/log_streamer.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/local/log_streamer.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/local/models/models.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/local/models/models.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/local/runtime.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/local/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/local/services/jaeger.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/local/services/jaeger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/local/services/mq.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/local/services/mq.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """RabbitMQ service in charge of routing Agent messages."""
+import hashlib
 import binascii
 import logging
 import os
+import uuid
+import pathlib
 from typing import Dict
 
 import docker
 import tenacity
 from docker import errors
 from docker import types
 from docker.models import services
 
 logger = logging.getLogger(__name__)
 
 MQ_IMAGE = 'rabbitmq:3.9-management'
-
+MQ_ADVANCED_CONF_PATH='/etc/rabbitmq/advanced.config'
 
 class LocalRabbitMQ:
     """RabbitMQ service spawned a docker swarm service."""
 
     def __init__(self,
                  name: str,
                  network: str,
@@ -26,14 +29,15 @@
         """Initialize the MQ service parameters.
         Args:
             name: Name of the service.
             network: Network used for the Docker MQ service.
             exposed_ports: The list of MQ service exposed ports
             image: MQ Docker image
         """
+        self._uuid = uuid.uuid4()
         self._name = name
         self._docker_client = docker.from_env()
         # images
         self._mq_image = image
         self._network = network
         self._mq_host = f'mq_{self._name}'
         # service
@@ -49,31 +53,33 @@
     @property
     def vhost(self):
         """Default vhost."""
         return '/'
 
     @property
     def service(self):
+        """The RabbitMQ corresponding docker service."""
         return self._mq_service
 
     @property
     def management_url(self) -> str:
         """URL to connect to the management interface of the RabbitMQ instance."""
         return f'http://guest:guest@{self._mq_host}:15672/'
 
     def start(self) -> None:
-        """Start local rabbit mq instance."""
+        """Start local Rabbit MQ instance."""
         self._create_network()
         self._mq_service = self._start_mq()
 
         if self._mq_service is not None and not self._is_service_healthy():
             logger.error('MQ container for service %s is not ready', self._mq_service.id)
             return
 
     def stop(self):
+        """Stop local Rabiit MQ instance."""
         for service in self._docker_client.services.list():
             universe = service.attrs['Spec']['Labels'].get('ostorlab.universe')
             if universe is not None and service.name.startswith('mq_') and self._name in universe:
                 service.remove()
 
     def _create_network(self):
         if any(network.name == self._network for network in self._docker_client.networks.list()):
@@ -84,31 +90,57 @@
                 name=self._network,
                 driver='overlay',
                 attachable=True,
                 labels={'ostorlab.universe': self._name},
                 check_duplicate=True
             )
 
+    def _create_mq_advanced_config(self) -> types.services.ConfigReference:
+        conf_path = pathlib.Path(__file__).parent / 'configurations/mq_advanced_conf.config'
+        with open(conf_path, 'rb') as conf_file:
+            mq_advanced_configuration = conf_file.read()
+        config_name = hashlib.md5(
+            f'mq_advanced_config_{self._name}_{self._uuid}'.encode()).hexdigest()
+
+        try:
+            mq_advanced_config = self._docker_client.configs.get(config_name)
+            logging.warning('found existing config %s, config will removed', config_name)
+            mq_advanced_config.remove()
+        except docker.errors.NotFound:
+            logging.debug('all good, config %s is new', config_name)
+
+        docker_config = self._docker_client.configs.create(
+            name=config_name,
+            labels={'ostorlab.universe': self._name, 'ostorlab.mq.advanced.config': 'true'},
+            data=mq_advanced_configuration
+        )
+        return types.services.ConfigReference(config_id=docker_config.id,
+                                       config_name=config_name,
+                                       filename=MQ_ADVANCED_CONF_PATH)
+
     def _start_mq(self) -> services.Service:
         try:
             logger.info('starting MQ')
             endpoint_spec = types.services.EndpointSpec(mode='vip', ports=self._exposed_ports)
             service_mode = types.services.ServiceMode('replicated', replicas=1)
+            mq_advanced_configuration = self._create_mq_advanced_config()
+            configs = [mq_advanced_configuration]
             return self._docker_client.services.create(
                 image=self._mq_image,
                 networks=[self._network],
                 name=self._mq_host,
                 env=[
                     'TASK_ID={{.Task.Slot}}',
                     f'MQ_SERVICE_NAME={self._mq_host}',
                     f'RABBITMQ_ERLANG_COOKIE={binascii.hexlify(os.urandom(10)).decode()}',
                 ],
                 restart_policy=types.RestartPolicy(condition='any'),
                 mode=service_mode,
                 labels={'ostorlab.universe': self._name, 'ostorlab.mq': ''},
+                configs=configs,
                 endpoint_spec=endpoint_spec)
         except docker.errors.APIError as e:
             error_message = f'MQ service could not be started. Reason: {e}.'
             logger.error(error_message)
             return
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(20),
@@ -118,12 +150,17 @@
                     retry=tenacity.retry_if_result(lambda v: v is False))
     def _is_service_healthy(self) -> bool:
         logger.info('checking service %s', self._mq_service.name)
         return self.is_healthy
 
     @property
     def is_healthy(self) -> bool:
+        """Check if the local Rabbit MQ instance is healthy.
+
+        Returns:
+            True if the instance is healthy, False otherwise.
+        """
         try:
             return self._mq_service is not None and \
                    len([task for task in self._mq_service.tasks() if task['Status']['State'] == 'running']) == 1
         except errors.DockerException:
             return False
```

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/local/services/redis.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/local/services/redis.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/registry.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/registry.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/runtimes/runtime.py` & `ostorlab-0.9.9/src/ostorlab/runtimes/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/testing/agent.py` & `ostorlab-0.9.9/src/ostorlab/testing/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/utils/defintions.py` & `ostorlab-0.9.9/src/ostorlab/utils/defintions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/utils/dictionary_minifier.py` & `ostorlab-0.9.9/src/ostorlab/utils/dictionary_minifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,16 @@
         s: the string or bytes value.
         truncate_size: how much to truncate.
 
     Returns:
         the truncated string or bytes value.
     """
     if isinstance(value, (str, bytes)):
-        value = value[:TRUNCATE_SIZE]
+        # The casting to string is specific to the bytes case, to prevent the json encoding from failing later.
+        value = str(value)[:TRUNCATE_SIZE]
     return value
 
 
 def minify_dict(value: Any, handler: Callable[[object], object]) -> Union[Dict[object, object], List[object], object]:
     """Recursive approach to minify dictionary values.
 
     Args:
```

### Comparing `ostorlab-0.9.8/src/ostorlab/utils/risk_rating.py` & `ostorlab-0.9.9/src/ostorlab/utils/risk_rating.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/utils/strings.py` & `ostorlab-0.9.9/src/ostorlab/utils/strings.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/utils/styles.py` & `ostorlab-0.9.9/src/ostorlab/utils/styles.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/utils/version.py` & `ostorlab-0.9.9/src/ostorlab/utils/version.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab/utils/volumes.py` & `ostorlab-0.9.9/src/ostorlab/utils/volumes.py`

 * *Files identical despite different names*

### Comparing `ostorlab-0.9.8/src/ostorlab.egg-info/PKG-INFO` & `ostorlab-0.9.9/src/ostorlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ostorlab
-Version: 0.9.8
+Version: 0.9.9
 Summary: Ostorlab Agent and Extensibility CLI and SDK
 Home-page: https://github.com/Ostorlab/ostorlab
 Author: ostorlab team
 Author-email: legends@ostorlab.dev
 License: Apache-2.0
 Project-URL: Documentation, https://docs.ostorlab.co/
 Project-URL: Source, https://github.com/Ostorlab/ostorlab
```

### Comparing `ostorlab-0.9.8/src/ostorlab.egg-info/SOURCES.txt` & `ostorlab-0.9.9/src/ostorlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

