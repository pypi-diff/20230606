# Comparing `tmp/watchmen_data_kernel-16.5.3.tar.gz` & `tmp/watchmen_data_kernel-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_data_kernel-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_data_kernel-16.5.4.tar", max compression
```

## Comparing `watchmen_data_kernel-16.5.3.tar` & `watchmen_data_kernel-16.5.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/LICENSE
--rw-r--r--   0        0        0     1207 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/__init__.py
--rw-r--r--   0        0        0      187 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/__init__.py
--rw-r--r--   0        0        0     2808 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/cache_manager.py
--rw-r--r--   0        0        0     5679 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/cache_service.py
--rw-r--r--   0        0        0     1555 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/data_source_cache.py
--rw-r--r--   0        0        0     1048 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/external_writer_cache.py
--rw-r--r--   0        0        0     1097 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/internal_cache.py
--rw-r--r--   0        0        0     1442 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/key_store_cache.py
--rw-r--r--   0        0        0     1709 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py
--rw-r--r--   0        0        0     2595 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/pipeline_cache.py
--rw-r--r--   0        0        0      861 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/tenant_cache.py
--rw-r--r--   0        0        0     2811 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/topic_cache.py
--rw-r--r--   0        0        0      463 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/common/__init__.py
--rw-r--r--   0        0        0       44 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/common/exception.py
--rw-r--r--   0        0        0     3594 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/common/settings.py
--rw-r--r--   0        0        0      399 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/__init__.py
--rw-r--r--   0        0        0     1840 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/aes_encryptor.py
--rw-r--r--   0        0        0     4349 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/center_masker.py
--rw-r--r--   0        0        0     2642 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/date_masker.py
--rw-r--r--   0        0        0     1475 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/encryptor.py
--rw-r--r--   0        0        0     2936 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/encryptor_registry.py
--rw-r--r--   0        0        0     1607 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/last_masker.py
--rw-r--r--   0        0        0      776 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/mail_masker.py
--rw-r--r--   0        0        0      807 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/md5_encryptor.py
--rw-r--r--   0        0        0      968 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/sha256_encryptor.py
--rw-r--r--   0        0        0      340 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/external_writer/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py
--rw-r--r--   0        0        0     2006 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/external_writer/external_writer_registry.py
--rw-r--r--   0        0        0      285 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1410 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/data_source_service.py
--rw-r--r--   0        0        0     1993 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/external_writer_service.py
--rw-r--r--   0        0        0     1091 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/key_store_service.py
--rw-r--r--   0        0        0     2479 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/pipeline_service.py
--rw-r--r--   0        0        0     1343 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/tenant_service.py
--rw-r--r--   0        0        0     3683 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/topic_service.py
--rw-r--r--   0        0        0      162 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/service/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/service/service_helper.py
--rw-r--r--   0        0        0     1535 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/service/storage_helper.py
--rw-r--r--   0        0        0     3078 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/service/topic_structure_helper.py
--rw-r--r--   0        0        0      319 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/__init__.py
--rw-r--r--   0        0        0     7280 2023-06-05 01:29:03.500123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/data_entity_helper.py
--rw-r--r--   0        0        0    16187 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/data_service.py
--rw-r--r--   0        0        0     1560 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/factor_column_mapper.py
--rw-r--r--   0        0        0     4634 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/raw_data_service.py
--rw-r--r--   0        0        0     3146 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/regular_data_service.py
--rw-r--r--   0        0        0     2207 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/shaper.py
--rw-r--r--   0        0        0     3610 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/topic_storage.py
--rw-r--r--   0        0        0      639 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/__init__.py
--rw-r--r--   0        0        0      248 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/ask_action_defined_as.py
--rw-r--r--   0        0        0    36597 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py
--rw-r--r--   0        0        0    57849 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py
--rw-r--r--   0        0        0      250 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/time_utils.py
--rw-r--r--   0        0        0      941 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/topic_utils.py
--rw-r--r--   0        0        0     7540 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/utils.py
--rw-r--r--   0        0        0     3074 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/variables.py
--rw-r--r--   0        0        0      145 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/system/__init__.py
--rw-r--r--   0        0        0     1818 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/system/change_log_helper.py
--rw-r--r--   0        0        0     8102 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/system/operation_helper.py
--rw-r--r--   0        0        0       79 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/__init__.py
--rw-r--r--   0        0        0     2628 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py
--rw-r--r--   0        0        0     3235 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/date_time_factor.py
--rw-r--r--   0        0        0     2462 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/default_value_factor.py
--rw-r--r--   0        0        0     5245 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/encrypt_factor.py
--rw-r--r--   0        0        0      911 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/flatten_factor.py
--rw-r--r--   0        0        0     3656 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/topic_schema.py
--rw-r--r--   0        0        0     6189 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/utils.py
--rw-r--r--   0        0        0      113 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/utils/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-05 01:29:03.504123 watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/utils/variable_helper.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 watchmen_data_kernel-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/LICENSE
+-rw-r--r--   0        0        0     1207 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/__init__.py
+-rw-r--r--   0        0        0     2808 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/cache_manager.py
+-rw-r--r--   0        0        0     5679 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/cache_service.py
+-rw-r--r--   0        0        0     1555 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/data_source_cache.py
+-rw-r--r--   0        0        0     1048 2023-06-06 01:45:59.117402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/external_writer_cache.py
+-rw-r--r--   0        0        0     1097 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/internal_cache.py
+-rw-r--r--   0        0        0     1442 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/key_store_cache.py
+-rw-r--r--   0        0        0     1709 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py
+-rw-r--r--   0        0        0     2595 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/pipeline_cache.py
+-rw-r--r--   0        0        0      861 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/tenant_cache.py
+-rw-r--r--   0        0        0     2811 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/topic_cache.py
+-rw-r--r--   0        0        0      463 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/common/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/common/exception.py
+-rw-r--r--   0        0        0     3594 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/common/settings.py
+-rw-r--r--   0        0        0      399 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/__init__.py
+-rw-r--r--   0        0        0     1840 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/aes_encryptor.py
+-rw-r--r--   0        0        0     4349 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/center_masker.py
+-rw-r--r--   0        0        0     2642 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/date_masker.py
+-rw-r--r--   0        0        0     1475 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/encryptor.py
+-rw-r--r--   0        0        0     2936 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/encryptor_registry.py
+-rw-r--r--   0        0        0     1607 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/last_masker.py
+-rw-r--r--   0        0        0      776 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/mail_masker.py
+-rw-r--r--   0        0        0      807 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/md5_encryptor.py
+-rw-r--r--   0        0        0      968 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/sha256_encryptor.py
+-rw-r--r--   0        0        0      340 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/external_writer/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py
+-rw-r--r--   0        0        0     2006 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/external_writer/external_writer_registry.py
+-rw-r--r--   0        0        0      285 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1410 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/data_source_service.py
+-rw-r--r--   0        0        0     1993 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/external_writer_service.py
+-rw-r--r--   0        0        0     1091 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/key_store_service.py
+-rw-r--r--   0        0        0     2479 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/pipeline_service.py
+-rw-r--r--   0        0        0     1343 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/tenant_service.py
+-rw-r--r--   0        0        0     3683 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/topic_service.py
+-rw-r--r--   0        0        0      162 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/service/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/service/service_helper.py
+-rw-r--r--   0        0        0     1535 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/service/storage_helper.py
+-rw-r--r--   0        0        0     3078 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/service/topic_structure_helper.py
+-rw-r--r--   0        0        0      319 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     7280 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/data_entity_helper.py
+-rw-r--r--   0        0        0    16187 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/data_service.py
+-rw-r--r--   0        0        0     1560 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/factor_column_mapper.py
+-rw-r--r--   0        0        0     4634 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/raw_data_service.py
+-rw-r--r--   0        0        0     3146 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/regular_data_service.py
+-rw-r--r--   0        0        0     2207 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/shaper.py
+-rw-r--r--   0        0        0     3610 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/topic_storage.py
+-rw-r--r--   0        0        0      639 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/ask_action_defined_as.py
+-rw-r--r--   0        0        0    36597 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py
+-rw-r--r--   0        0        0    57849 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py
+-rw-r--r--   0        0        0      250 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/time_utils.py
+-rw-r--r--   0        0        0      941 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/topic_utils.py
+-rw-r--r--   0        0        0     7540 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/utils.py
+-rw-r--r--   0        0        0     3074 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/variables.py
+-rw-r--r--   0        0        0      145 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/system/__init__.py
+-rw-r--r--   0        0        0     1818 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/system/change_log_helper.py
+-rw-r--r--   0        0        0     8327 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/system/operation_helper.py
+-rw-r--r--   0        0        0       79 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/__init__.py
+-rw-r--r--   0        0        0     2628 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py
+-rw-r--r--   0        0        0     3235 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/date_time_factor.py
+-rw-r--r--   0        0        0     2462 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/default_value_factor.py
+-rw-r--r--   0        0        0     5245 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/encrypt_factor.py
+-rw-r--r--   0        0        0      911 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/flatten_factor.py
+-rw-r--r--   0        0        0     3656 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/topic_schema.py
+-rw-r--r--   0        0        0     6189 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/utils.py
+-rw-r--r--   0        0        0      113 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/utils/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-06 01:45:59.121402 watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/utils/variable_helper.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 watchmen_data_kernel-16.5.4/PKG-INFO
```

### Comparing `watchmen_data_kernel-16.5.3/LICENSE` & `watchmen_data_kernel-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/pyproject.toml` & `watchmen_data_kernel-16.5.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-data-kernel"
-version = "16.5.3"
+version = "16.5.4"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_data_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cacheout = "^0.13.1"
 pycryptodome = "^3.14.1"
-watchmen-meta = "16.5.3"
-watchmen-storage-mysql = { version = "16.5.3", optional = true }
-watchmen-storage-oracle = { version = "16.5.3", optional = true }
-watchmen-storage-mongodb = { version = "16.5.3", optional = true }
-watchmen-storage-mssql = { version = "16.5.3", optional = true }
-watchmen-storage-postgresql = { version = "16.5.3", optional = true }
-watchmen-storage-oss = { version = "16.5.3", optional = true }
-watchmen-storage-s3 = { version = "16.5.3", optional = true }
+watchmen-meta = "16.5.4"
+watchmen-storage-mysql = { version = "16.5.4", optional = true }
+watchmen-storage-oracle = { version = "16.5.4", optional = true }
+watchmen-storage-mongodb = { version = "16.5.4", optional = true }
+watchmen-storage-mssql = { version = "16.5.4", optional = true }
+watchmen-storage-postgresql = { version = "16.5.4", optional = true }
+watchmen-storage-oss = { version = "16.5.4", optional = true }
+watchmen-storage-s3 = { version = "16.5.4", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/cache_manager.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/cache_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/data_source_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/data_source_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/external_writer_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/external_writer_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/internal_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/internal_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/key_store_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/key_store_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/pipeline_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/pipeline_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/tenant_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/tenant_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/cache/topic_cache.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/cache/topic_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/common/settings.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/aes_encryptor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/aes_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/center_masker.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/center_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/date_masker.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/date_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/encryptor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/encryptor_registry.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/encryptor_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/last_masker.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/last_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/mail_masker.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/mail_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/md5_encryptor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/md5_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/encryption/sha256_encryptor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/encryption/sha256_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/external_writer/external_writer_registry.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/external_writer/external_writer_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/data_source_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/data_source_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/external_writer_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/external_writer_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/key_store_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/key_store_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/pipeline_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/tenant_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/tenant_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/meta/topic_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/meta/topic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/service/service_helper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/service/service_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/service/storage_helper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/service/storage_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/service/topic_structure_helper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/service/topic_structure_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/data_entity_helper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/data_entity_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/data_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/factor_column_mapper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/factor_column_mapper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/raw_data_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/raw_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/regular_data_service.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/regular_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/shaper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/shaper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage/topic_storage.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage/topic_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/__init__.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/topic_utils.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/utils.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/storage_bridge/variables.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/storage_bridge/variables.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/system/change_log_helper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/system/change_log_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/system/operation_helper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/system/operation_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 from pydantic import BaseModel
 from enum import Enum
-from typing import List, Tuple, Any, Optional
+from typing import List, Any, Optional
 from io import BytesIO, StringIO
 import zipfile
 
 from watchmen_data_kernel.meta import DataSourceService
 
 from watchmen_meta.admin import TopicService
 from watchmen_meta.common import RecordOperationService, ask_meta_storage_type, PackageVersionService
 
-from watchmen_model.system import Operation, DataSourceType, OperationType
+from watchmen_model.system import Operation, DataSourceType
 from watchmen_model.admin import Topic
 
 from watchmen_storage_rds import ScriptBuilder
 
 from watchmen_utilities import ArrayHelper
 from .change_log_helper import ChangelogXml
 
@@ -48,18 +48,22 @@
 	TupleType.PIPELINES: "0002",
 	TupleType.SPACES: "0003",
 	TupleType.SUBJECTS: "0004",
 	TupleType.REPORTS: "0005"
 }
 
 
+
+
+
 class OperationScriptBuilder:
 
-	def __init__(self, operation_service: RecordOperationService):
+	def __init__(self, operation_service: RecordOperationService,topic_service:TopicService):
 		self.operation_service = operation_service
+		self.topic_service = topic_service
 		self.meta_script_builder = script_builder_factory(ask_meta_storage_type())
 		self.package_version = PackageVersionService(operation_service.storage,
 		                                             operation_service.snowflakeGenerator,
 		                                             operation_service.principalService).find_one()
 		self.meta_files: List[SqlScriptFile] = []
 		self.data_files: List[SqlScriptFile] = []
 
@@ -68,70 +72,78 @@
 			.build(TupleType.PIPELINES) \
 			.build(TupleType.SPACES) \
 			.build(TupleType.SUBJECTS) \
 			.build(TupleType.REPORTS)
 
 	def build(self, tuple_type: TupleType):
 		record_ids = self.get_record_ids_with_current_version(tuple_type)
+		have_create_record = self.have_create_record(tuple_type)
 		if len(record_ids) != 0:
-			self.make_sql_scripts(record_ids, tuple_type)
+			self.make_sql_scripts(record_ids, tuple_type,have_create_record)
 		return self
 
 	def get_record_ids_with_current_version(self, tuple_type: TupleType) -> List[str]:
 		record_rows = self.operation_service.get_record_ids(self.package_version.currVersion,
 		                                                    tuple_type)
 		record_ids = ArrayHelper(record_rows).map(lambda x: x.get("record_id")).to_list()
 		return record_ids
 
-	def make_sql_scripts(self, record_ids: List[str], tuple_type: str):
+	def have_create_record(self,tuple_type: TupleType):
+		create_records = self.operation_service.get_record_with_create_type(self.package_version.currVersion,
+		                                                                    tuple_type)
+		if create_records:
+			return True
+		else:
+			return False
+
+	def make_sql_scripts(self, record_ids: List[str], tuple_type: str,have_create_record:bool):
 		# noinspection PyTypeChecker
 		file_name = f"{TUPLE_SEQUENCE.get(tuple_type)}-{tuple_type}.dml.sql"
 		file = StringIO()
 		try:
 			for sequence, record_id in enumerate(record_ids, start=1):
 				operation = self.operation_service.get_operation_by_id(record_id)
-				file.write(self.build_meta_script_file(operation))
+				file.write(self.build_meta_script_file(operation,have_create_record))
 				if operation.tupleType == TupleType.TOPICS:
 					self.build_data_script_file(operation, sequence)
 			# noinspection PyUnresolvedReferences,PyUnboundLocalVariable
 			self.meta_files.append(
 				SqlScriptFile(name=file_name, content=file.getvalue(), data_source_type=ask_meta_storage_type()))
 		finally:
 			file.close()
 
-	def build_meta_script_file(self, operation: Operation) -> str:
-		if operation.operationType == OperationType.UPDATE:
-			return self.meta_script_builder.sql_update(operation.tupleType, operation.tupleKey, operation.content)
-		elif operation.operationType == OperationType.CREATE:
+	def build_meta_script_file(self, operation: Operation,have_create_record:bool) -> str:
+		if have_create_record:
 			return self.meta_script_builder.sql_insert(operation.tupleType, operation.content)
 		else:
-			NotImplemented(
-				f"The operation type: {operation.operationType} is not supported. The record id: {operation.recordId}")
+			return self.meta_script_builder.sql_update(operation.tupleType, operation.tupleKey, operation.content)
+
+
 
 	# noinspection PyTypeChecker
 	def build_data_script_file(self, operation: Operation, sequence: int):
 
 		def create_topic_table_file(builder: ScriptBuilder, new: Topic) -> StringIO:
 			file.write(builder.sql_create_table(new))
 			return file
 
 		def alert_topic_table_file(builder: ScriptBuilder, new: Topic, old: Topic) -> StringIO:
 			file.write('\n'.join([*builder.sql_alert_table(new, old),
 			                      *builder.sql_unique_indexes(new),
 			                      *builder.sql_index(new)]))
 			return file
 
-		topic_service = get_topic_service(self.operation_service)
-		topic: Topic = topic_service.get_entity_shaper().deserialize(operation.content)
-
+		topic:Topic = self.topic_service.find_by_id(operation.tupleId)
+		if topic is None:
+			return
 		if topic.dataSourceId is None:
 			raise RuntimeError(f"{topic.name} doesn't have datasource.")
-
+		#
 		datasource = DataSourceService(self.operation_service.principalService).find_by_id(topic.dataSourceId)
-		data_script_builder = script_builder_factory(datasource.dataSourceType)
+		data_script_builder = script_builder_factory(DataSourceType.MYSQL)
 		file_name = build_file_name(sequence, f"topic_{topic.name}.ddl.sql")
 		file = StringIO()
 		try:
 			record_id = self.operation_service.get_previous_record_id(operation.tupleId, operation.versionNum)
 			if record_id:
 				previous_operation = self.operation_service.get_operation_by_id(record_id)
 				previous_topic = topic_service.get_entity_shaper().deserialize(previous_operation.content)
@@ -140,15 +152,15 @@
 					              content=alert_topic_table_file(data_script_builder, topic, previous_topic).getvalue(),
 					              data_source_type=datasource.dataSourceType)
 				)
 			else:
 				self.data_files.append(
 					SqlScriptFile(name=file_name,
 					              content=create_topic_table_file(data_script_builder, topic).getvalue(),
-					              data_source_type=datasource.dataSourceType)
+					              data_source_type=DataSourceType.MYSQL)
 				)
 		finally:
 			file.close()
 
 	def package_zip(self) -> PackageZipFile:
 		return build_package_zip(self.meta_files,
 		                         self.data_files,
```

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/date_time_factor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/date_time_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/default_value_factor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/default_value_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/encrypt_factor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/encrypt_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/flatten_factor.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/flatten_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/topic_schema.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/topic_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/topic_schema/utils.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/topic_schema/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/src/watchmen_data_kernel/utils/variable_helper.py` & `watchmen_data_kernel-16.5.4/src/watchmen_data_kernel/utils/variable_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.3/PKG-INFO` & `watchmen_data_kernel-16.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-data-kernel
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: cacheout (>=0.13.1,<0.14.0)
 Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
-Requires-Dist: watchmen-meta (==16.5.3)
-Requires-Dist: watchmen-storage-mongodb (==16.5.3) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.3) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.3) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.3) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.3) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.3) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.3) ; extra == "s3"
+Requires-Dist: watchmen-meta (==16.5.4)
+Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.4) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.4) ; extra == "s3"
```

