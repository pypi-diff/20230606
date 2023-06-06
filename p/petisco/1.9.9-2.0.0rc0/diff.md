# Comparing `tmp/petisco-1.9.9.tar.gz` & `tmp/petisco-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petisco-1.9.9.tar", last modified: Thu Sep 29 11:37:51 2022, max compression
+gzip compressed data, was "petisco-2.0.0rc0.tar", last modified: Thu May 25 14:20:09 2023, max compression
```

## Comparing `petisco-1.9.9.tar` & `petisco-2.0.0rc0.tar`

### file list

```diff
@@ -1,251 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-29 11:37:42.000000 petisco-1.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-29 11:37:42.000000 petisco-1.9.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-09-29 11:37:51.127008 petisco-1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-09-29 11:37:42.000000 petisco-1.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-29 11:37:43.000000 petisco-1.9.9/petisco/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/application.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/application_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/application_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/application/controller/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/controller_executor_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/error_map.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/controller/http_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco/base/application/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/container.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/dependency.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/dependency_injection/injector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/handlers/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/middleware/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/notifier_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/middleware/print_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/not_implemented_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/notifier_exception_message.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/notifier/notifier_message.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/patterns/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/app_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/inmemory_crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/patterns/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/application/use_case/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/use_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/use_case/use_case.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/application/use_case/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/domain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.111007 petisco-1.9.9/petisco/base/domain/errors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/critical_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/default_http_error_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/errors/defaults/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/already_exists.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/invalid_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/invalid_value_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/not_allowed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/defaults/not_found.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/domain_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/errors/unknown_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/message/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/all_message_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/message/chaos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/message_chaos_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/command.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/command_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/command_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/consumer_derived_action.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/domain_event_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_handler_returns_none_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/message_subscriber_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_message_comsumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/message/not_implemented_message_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/aggregate_root.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/model/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.115007 petisco-1.9.9/petisco/base/domain/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/interface_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/domain/persistence/persistence_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/base/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/singleton.py
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/misc/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/base/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/base/testing/assert_http.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/cli/petisco.py
--rw-r--r--   0 runner    (1001) docker     (121)     4920 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/cli/petisco_rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/elastic/
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_apm_monitoring_app_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_operational_database_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/elastic_session_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/elastic/is_elastic_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/application/fastapi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/controller/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_default_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_failure_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_success_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/is_fastapi_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/fastapi/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/fastapi/testing/assert_http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5180 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.119007 petisco-1.9.9/petisco/extra/rabbitmq/application/message/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     5320 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6962 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
--rw-r--r--   0 runner    (1001) docker     (121)    16386 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/is_pika_available.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/rabbitmq/shared/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/queue_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/rabbitmq/shared/specific_queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/slack/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/slack/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.123008 petisco-1.9.9/petisco/extra/slack/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/create_text_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     4763 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/slack/is_slack_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/base_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sql_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlalchemy/sqlalchemy_operational_database_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/sqlmodel/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlmodel/is_sqlmodel_available.py
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/extra/threading/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/extra/threading/pool_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/petisco/legacy/logger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/interface_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/log_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/logging_based_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/legacy/logger/not_implemented_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6043 2022-09-29 11:37:42.000000 petisco-1.9.9/petisco/public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.107006 petisco-1.9.9/petisco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7152 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9746 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-29 11:37:51.000000 petisco-1.9.9/petisco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-29 11:37:42.000000 petisco-1.9.9/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-29 11:37:51.127008 petisco-1.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-09-29 11:37:42.000000 petisco-1.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:51.127008 petisco-1.9.9/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 11:37:42.000000 petisco-1.9.9/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/application_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/application_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/chaos/chaos_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/chaos/check_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/async_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/controller/meta_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/dependency_injection/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/dependency_injection/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/handlers/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/notifier_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/middleware/print_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/not_implemented_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/notifier_exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/notifier/notifier_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/async_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/inmemory_crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/patterns/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/application/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/async_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/meta_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/application/use_case/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.869461 petisco-2.0.0rc0/petisco/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/critical_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/default_http_error_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/invalid_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/invalid_value_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/not_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/defaults/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/domain_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/errors/unknown_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/all_message_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/message/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/message_chaos_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/command_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/consumer_derived_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/domain_event_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_handler_returns_none_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/message_subscriber_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_comsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.873461 petisco-2.0.0rc0/petisco/base/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/aggregate_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/model/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/base/domain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/async_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/legacy_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/legacy_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/persistence_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/domain/persistence/sql_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/base/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/misc/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/base/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/base/testing/assert_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/petisco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/petisco_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/cli/petisco_rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/async_elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/elastic_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/elastic_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/is_elastic_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic/legacy_elastic_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/elastic_apm/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic_apm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/elastic_apm/is_elastic_apm_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.877461 petisco-2.0.0rc0/petisco/extra/fastapi/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/application/fastapi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/fastapi/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/as_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_default_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_failure_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_success_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/is_fastapi_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/fastapi/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/fastapi/testing/assert_http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/logging_based_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/loguru_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/logger/not_implemented_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.881461 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/is_pika_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/queue_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/specific_queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/application/message/bus/redis_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/redis/is_redis_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/slack/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/create_text_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/slack/is_slack_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/async_sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/base_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.885461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/petisco/extra/sqlmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlmodel/is_sqlmodel_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/petisco/extra/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/extra/threading/pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/petisco/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.865461 petisco-2.0.0rc0/petisco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 14:20:09.000000 petisco-2.0.0rc0/petisco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:09.889461 petisco-2.0.0rc0/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:20:07.000000 petisco-2.0.0rc0/tests/modules/__init__.py
```

### Comparing `petisco-1.9.9/LICENSE` & `petisco-2.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/base/application/application.py` & `petisco-2.0.0rc0/petisco/base/application/application.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime, timedelta
-from typing import Callable, List, Optional
+from typing import Any, Callable, Dict, List
 
+from loguru import logger
 from pydantic import BaseSettings, Field
 
 from petisco.base.application.application_configurer import ApplicationConfigurer
 from petisco.base.application.application_info import ApplicationInfo
 from petisco.base.application.dependency_injection.container import Container
 from petisco.base.application.dependency_injection.dependency import Dependency
 from petisco.base.application.notifier.notifier import Notifier
@@ -15,93 +16,123 @@
 from petisco.extra.slack.dependencies import get_default_notifier_dependencies
 
 
 class Application(BaseSettings):
     name: str
     version: str
     organization: str
-    deployed_at: Optional[datetime]
+    deployed_at: datetime
     environment: str = Field("local", env="ENVIRONMENT")
-    dependencies_provider: Optional[Callable[..., List[Dependency]]] = lambda: []
-    configurers: Optional[List[ApplicationConfigurer]] = []
+    dependencies_provider: Callable[..., List[Dependency]] = lambda: []
+    configurers: List[ApplicationConfigurer] = []
 
-    def __init__(self, **data) -> None:
-        ApplicationInfo(
+    def __init__(self, **data: Any) -> None:
+        info = ApplicationInfo(
             name=data["name"],
             organization=data["organization"],
             version=data["version"],
             deployed_at=data.get("deployed_at"),
+            force_recreation=True,
+        )
+        deployed_at = info.deployed_at.strftime("%m/%d/%Y, %H:%M:%S")
+        logger.info(
+            f"Application: {info.name} {info.version} ({info.organization}) deployed at {deployed_at}"
         )
         super().__init__(**data)
 
-    def configure(self, testing: bool = False):
+    def configure(
+        self, testing: bool = False, overwrite_dependencies: bool = False
+    ) -> None:
 
-        before_dependecies_configurers = [
+        before_dependencies_configurers = [
             configurer
             for configurer in self.configurers
             if configurer.execute_after_dependencies is False
         ]
-        for configurer in before_dependecies_configurers:
+        name_configurers = [
+            configurer.__class__.__name__
+            for configurer in before_dependencies_configurers
+        ]
+        logger.info(
+            f"Application: running configurators before setting dependencies {name_configurers}..."
+        )
+        for configurer in before_dependencies_configurers:
             configurer.execute(testing)
 
-        Container.set_dependencies(self.get_dependencies())
+        logger.info("Application: setting dependencies...")
+        Container.set_dependencies(self.get_dependencies(), overwrite_dependencies)
 
         after_dependencies_configurers = [
             configurer
             for configurer in self.configurers
             if configurer.execute_after_dependencies is True
         ]
+
+        name_configurers = [
+            configurer.__class__.__name__
+            for configurer in after_dependencies_configurers
+        ]
+        logger.info(
+            f"Application: running configurators after setting dependencies {name_configurers}..."
+        )
         for configurer in after_dependencies_configurers:
             configurer.execute(testing)
 
+        logger.info("Application: successful configuration")
+
     def get_dependencies(self) -> List[Dependency]:
+        # TODO: review default dependencies in v2
+
         default_dependencies = (
             get_default_message_dependencies() + get_default_notifier_dependencies()
         )
+        # TODO: the `dependency.type if not dependency.name else dependency.name` will be deprecated in v2 -> use
+        #  just `dependency.type` as key
         default_dependencies_dict = {
-            dependency.name: dependency for dependency in default_dependencies
+            dependency.get_key(): dependency for dependency in default_dependencies
         }
         provided_dependencies = self.dependencies_provider()
-        given_dependencies_dict = {
-            dependency.name: dependency for dependency in provided_dependencies
+        provided_dependencies_dict = {
+            dependency.get_key(): dependency for dependency in provided_dependencies
+        }
+        # This merged_dependencies will give preference to provided_dependencies_dict over default_dependencies_dict
+        merged_dependencies = {
+            **default_dependencies_dict,
+            **provided_dependencies_dict,
         }
-        merged_dependecies = {**default_dependencies_dict, **given_dependencies_dict}
-        return list(merged_dependecies.values())
+        return list(merged_dependencies.values())
 
-    def clear(self):
+    def clear(self) -> None:
         Container.clear()
 
-    def info(self):
+    def info(self) -> Dict[str, Any]:
         info = self.dict()
-        info["deployed_at"] = (
-            self.deployed_at.strftime("%m/%d/%Y, %H:%M:%S")
-            if self.deployed_at
-            else None
-        )
+        info["deployed_at"] = self.deployed_at.strftime("%m/%d/%Y, %H:%M:%S")
+
         info["dependencies"] = {
-            dependency.name: dependency.get_instance().info()
+            dependency.type.__name__: dependency.get_instance().info()
             for dependency in self.get_dependencies()
         }
         del info["dependencies_provider"]
         del info["configurers"]
         return info
 
-    def was_deploy_few_minutes_ago(self, minutes: int = 25):
+    def was_deploy_few_minutes_ago(self, minutes: int = 25) -> bool:
         return datetime.utcnow() < self.deployed_at + timedelta(minutes=minutes)
 
-    def publish_domain_event(self, domain_event: DomainEvent):
+    def publish_domain_event(self, domain_event: DomainEvent) -> None:
         try:
-            domain_event_bus: DomainEventBus = Container.get("domain_event_bus")
+            domain_event_bus = Container.get(DomainEventBus)
             domain_event_bus.publish(domain_event)
-        except:  # noqa
+        except Exception as exc:  # noqa
             raise TypeError(
-                'To publish an event to the domain event bus, please add a dependency with name "domain_event_bus" on Application dependencies'
+                f"To publish an event to the domain event bus, please add a dependency with type `DomainEventBus` on Application dependencies. {str(exc)}"
             )
 
-    def notify(self, message: NotifierMessage):
+    def notify(self, message: NotifierMessage) -> None:
         try:
-            notifier: Notifier = Container.get("notifier")
+            notifier = Container.get(Notifier)
             notifier.publish(message)
         except:  # noqa
             raise TypeError(
                 'To notify the deploy, please add a dependency with name "notifier" on Application dependencies'
             )
```

### Comparing `petisco-1.9.9/petisco/base/application/controller/controller.py` & `petisco-2.0.0rc0/petisco/base/application/controller/meta_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
+from inspect import iscoroutinefunction
 from types import FunctionType
-from typing import Any, List
+from typing import Any
 
-from meiga import Error, NotImplementedMethodError, Result
+from meiga import AnyResult, NotImplementedMethodError
 
-from petisco.base.misc.result_mapper import ResultMapper, default_failure_handler
+from petisco.base.application.middleware.middleware import Middleware
+from petisco.base.misc.async_wrapper import async_wrapper
+from petisco.base.misc.result_mapper import ResultMapper
 from petisco.base.misc.wrapper import wrapper
 
 
-def get_mapper(bases, config):
+def get_mapper(bases: tuple[Any], config: dict[str, Any] | None) -> ResultMapper:
     mapper = ResultMapper()
     if config:
         for base in bases:
             method = getattr(base, "get_config_mapper", None)
             if method:
                 mapper = method(config)
 
@@ -22,48 +27,35 @@
             if method:
                 mapper = method()
 
     return mapper
 
 
 class MetaController(type, ABC):
-    middlewares: List = {}
+    middlewares: list[Middleware] = []
 
-    def __new__(mcs, name, bases, namespace):
+    def __new__(
+        mcs, name: str, bases: tuple[Any], namespace: dict[str, Any]
+    ) -> MetaController:
         config = namespace.get("Config")
 
         mapper = get_mapper(bases, config)
 
         if "execute" not in namespace:
             raise NotImplementedError(
                 "Petisco Controller must implement an execute method"
             )
 
         new_namespace = {}
         for attributeName, attribute in namespace.items():
             if isinstance(attribute, FunctionType) and attribute.__name__ == "execute":
-                attribute = wrapper(attribute, name, config, mapper)
+                if iscoroutinefunction(attribute):
+                    attribute = async_wrapper(attribute, name, config, mapper)
+                else:
+                    attribute = wrapper(attribute, name, config, mapper)
             new_namespace[attributeName] = attribute
 
         return super().__new__(mcs, name, bases, new_namespace)
 
     @abstractmethod
-    def execute(self, *args, **kwargs) -> Result[Any, Error]:
-        return NotImplementedMethodError
-
-
-class Controller(metaclass=MetaController):
-    @staticmethod
-    def get_default_mapper() -> ResultMapper:
-        return ResultMapper()
-
-    @staticmethod
-    def get_config_mapper(config):
-        return ResultMapper(
-            error_map=getattr(config, "error_map", None),
-            success_handler=getattr(config, "success_handler", lambda result: result),
-            failure_handler=default_failure_handler,
-        )
-
-    @abstractmethod
-    def execute(self, *args, **kwargs) -> Result[Any, Error]:
+    def execute(self, *args: Any, **kwargs: Any) -> AnyResult:
         return NotImplementedMethodError
```

### Comparing `petisco-1.9.9/petisco/base/application/handlers/message_handler.py` & `petisco-2.0.0rc0/petisco/base/application/handlers/message_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from abc import ABC, abstractmethod
 from functools import wraps
 from types import FunctionType
-from typing import Any
+from typing import Any, Callable, Dict, Tuple
 
-from meiga import Error, Failure, NotImplementedMethodError, Result
+from meiga import AnyResult, Error, Failure, NotImplementedMethodError
 from meiga.on_failure_exception import OnFailureException
 
 from petisco.base.application.use_case.use_case_uncontrolled_error import (
     UseCaseUncontrolledError,
 )
 
 
-def wrapper(method):
+def wrapper(method: Callable[..., AnyResult]) -> Callable[..., Any]:
     @wraps(method)
-    def wrapped(*args, **kwargs):
+    def wrapped(*args: Any, **kwargs: Any) -> AnyResult:
         try:
             return method(*args, **kwargs)
         except OnFailureException as exception:
             return exception.result
         except Error as error:
             return Failure(error)
         except Exception as exception:
             return Failure(UseCaseUncontrolledError(exception))
 
     return wrapped
 
 
 class MetaUseCase(type, ABC):
-    def __new__(mcs, name, bases, namespace):
+    def __new__(
+        mcs, name: str, bases: Tuple[Any], namespace: Dict[str, Any]
+    ) -> "MetaUseCase":
         new_class_dict = {}
         if "execute" not in namespace:
             raise NotImplementedError(
                 "Petisco UseCase must implement an execute method"
             )
 
         for attributeName, attribute in namespace.items():
             if isinstance(attribute, FunctionType) and attribute.__name__ == "execute":
                 attribute = wrapper(attribute)
             new_class_dict[attributeName] = attribute
         return type.__new__(mcs, name, bases, new_class_dict)
 
     @abstractmethod
-    def execute(self, *args, **kwargs) -> Result[Any, Error]:
+    def execute(self, *args: Any, **kwargs: Any) -> AnyResult:
         return NotImplementedMethodError
 
 
 class UseCase(metaclass=MetaUseCase):
     @abstractmethod
-    def execute(self, *args, **kwargs) -> Result[Any, Error]:
+    def execute(self, *args: Any, **kwargs: Any) -> AnyResult:
         return NotImplementedMethodError
```

### Comparing `petisco-1.9.9/petisco/base/application/middleware/notifier_middleware.py` & `petisco-2.0.0rc0/petisco/base/application/middleware/notifier_middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-from meiga import Result
+from meiga import AnyResult
 
 from petisco import __version__
 from petisco.base.application.application_info import ApplicationInfo
 from petisco.base.application.dependency_injection.container import Container
 from petisco.base.application.middleware.middleware import Middleware
+from petisco.base.application.notifier.notifier import Notifier
 from petisco.base.application.notifier.notifier_exception_message import (
     NotifierExceptionMessage,
 )
 from petisco.base.application.notifier.notifier_message import NotifierMessage
 from petisco.base.domain.errors.critical_error import CriticalError
 from petisco.base.domain.errors.unknown_error import UnknownError
 
 
 class NotifierMiddleware(Middleware):
-    def __init__(self, wrapped_class_name, wrapped_class_input_arguments):
-        super().__init__(wrapped_class_name, wrapped_class_input_arguments)
-        self.notifier = Container.get("notifier")
+    """
+    Middleware Implementation to notify critical and unknown errors.
 
-    def before(self):
+    This Middleware will check result and notify if necessary using Container.get(Notifier) set dependency.
+    """
+
+    def __init__(self) -> None:
+        self.notifier = Container.get(Notifier)
+
+    def before(self) -> None:
         pass
 
-    def after(self, result: Result):
+    def after(self, result: AnyResult) -> None:
         if result.is_failure:
             error = result.value
 
             meta = {
                 "petisco": __version__,
                 "application_name": ApplicationInfo().name,
                 "application_version": ApplicationInfo().version,
```

### Comparing `petisco-1.9.9/petisco/base/application/notifier/notifier.py` & `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from abc import abstractmethod
+from typing import Dict, List, Union
 
 from petisco.base.application.notifier.notifier_exception_message import (
     NotifierExceptionMessage,
 )
 from petisco.base.application.notifier.notifier_message import NotifierMessage
 from petisco.base.misc.interface import Interface
 
 
-class Notifier(Interface):
+class SlackNotifierMessageConverter(Interface):
     @abstractmethod
-    def publish(self, notifier_message: NotifierMessage):
-        raise NotImplementedError
-
-    @abstractmethod
-    def publish_exception(self, notifier_exception_message: NotifierExceptionMessage):
+    def convert(
+        self, notifier_message: Union[NotifierMessage, NotifierExceptionMessage]
+    ) -> List[Dict]:
+        """
+        Should return a list of blocks. See: https://api.slack.com/reference/block-kit/blocks
+        """
         raise NotImplementedError
```

### Comparing `petisco-1.9.9/petisco/base/application/patterns/crud_repository.py` & `petisco-2.0.0rc0/petisco/base/application/patterns/crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/base/application/patterns/inmemory_crud_repository.py` & `petisco-2.0.0rc0/petisco/base/application/patterns/inmemory_crud_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AggregateAlreadyExistError,
 )
 from petisco.base.domain.errors.defaults.not_found import AggregateNotFoundError
 from petisco.base.domain.model.uuid import Uuid
 
 
 class InmemoryCrudRepository(CrudRepository[AggregateRootType]):
-    def __init__(self):
+    def __init__(self) -> None:
         self._data: Dict[Uuid, Any] = dict()
 
     @meiga
     def save(self, aggregate_root: AggregateRootType) -> BoolResult:
         if aggregate_root.aggregate_id in self._data:
             return Failure(AggregateAlreadyExistError(aggregate_root.aggregate_id))
         self._data[aggregate_root.aggregate_id] = aggregate_root
```

### Comparing `petisco-1.9.9/petisco/base/application/use_case/use_case.py` & `petisco-2.0.0rc0/petisco/base/application/use_case/meta_use_case.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,89 @@
 from abc import ABC, abstractmethod
 from functools import wraps
+from inspect import iscoroutinefunction, signature
 from types import FunctionType
-from typing import Any
+from typing import Any, Callable, Dict, Tuple
 
 import elasticapm
-from meiga import Error, Failure, NotImplementedMethodError, Result
+from meiga import AnyResult, Error, Failure, NotImplementedMethodError
 from meiga.on_failure_exception import OnFailureException
 
 from petisco.base.application.use_case.use_case_uncontrolled_error import (
     UseCaseUncontrolledError,
 )
 
 
-def wrapper(method, wrapped_class_name):
+def use_case_wrapper(
+    method: Callable[..., AnyResult], wrapped_class_name: str
+) -> Callable[..., AnyResult]:
     @wraps(method)
-    def wrapped(*args, **kwargs):
+    def wrapped(*args: Any, **kwargs: Any) -> AnyResult:
         try:
             return method(*args, **kwargs)
         except OnFailureException as exception:
             return exception.result
         except Error as error:
             return Failure(error)
         except Exception as exception:
+            arguments = signature(method).bind(*args, **kwargs).arguments
+            arguments.pop("self")
             uncontrolled_error = UseCaseUncontrolledError.from_exception(
-                exception=exception, arguments=args, class_name=wrapped_class_name
+                exception=exception, arguments=arguments, class_name=wrapped_class_name
+            )
+            client = elasticapm.get_client()
+            if client:
+                client.capture_exception()
+
+            return Failure(uncontrolled_error)
+
+    return wrapped
+
+
+def async_use_case_wrapper(
+    method: Callable[..., AnyResult], wrapped_class_name: str
+) -> Callable[..., AnyResult]:
+    @wraps(method)
+    async def wrapped(*args: Any, **kwargs: Any) -> AnyResult:
+        try:
+            return await method(*args, **kwargs)
+        except OnFailureException as exception:
+            return exception.result
+        except Error as error:
+            return Failure(error)
+        except Exception as exception:
+            arguments = signature(method).bind(*args, **kwargs).arguments
+            arguments.pop("self")
+            uncontrolled_error = UseCaseUncontrolledError.from_exception(
+                exception=exception, arguments=arguments, class_name=wrapped_class_name
             )
             client = elasticapm.get_client()
             if client:
                 client.capture_exception()
 
             return Failure(uncontrolled_error)
 
     return wrapped
 
 
 class MetaUseCase(type, ABC):
-    def __new__(mcs, name, bases, namespace):
+    def __new__(
+        mcs, name: str, bases: Tuple[Any], namespace: Dict[str, Any]
+    ) -> "MetaUseCase":
         new_class_dict = {}
         if "execute" not in namespace:
             raise NotImplementedError(
-                "Petisco UseCase must implement an execute method"
+                "Petisco UseCase or AsyncUseCase must implement an execute method"
             )
 
         for attributeName, attribute in namespace.items():
             if isinstance(attribute, FunctionType) and attribute.__name__ == "execute":
-                attribute = wrapper(attribute, name)
+                if iscoroutinefunction(attribute):
+                    attribute = async_use_case_wrapper(attribute, name)
+                else:
+                    attribute = use_case_wrapper(attribute, name)
             new_class_dict[attributeName] = attribute
         return type.__new__(mcs, name, bases, new_class_dict)
 
     @abstractmethod
-    def execute(self, *args, **kwargs) -> Result[Any, Error]:
-        return NotImplementedMethodError
-
-
-class UseCase(metaclass=MetaUseCase):
-    @abstractmethod
-    def execute(self, *args, **kwargs) -> Result[Any, Error]:
+    def execute(self, *args: Any, **kwargs: Any) -> AnyResult:
         return NotImplementedMethodError
```

### Comparing `petisco-1.9.9/petisco/base/domain/errors/default_http_error_map.py` & `petisco-2.0.0rc0/petisco/base/domain/errors/default_http_error_map.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/base/domain/errors/defaults/already_exists.py` & `petisco-2.0.0rc0/petisco/base/domain/errors/defaults/already_exists.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/base/domain/errors/defaults/not_found.py` & `petisco-2.0.0rc0/petisco/base/domain/errors/defaults/not_found.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Union
 
 from petisco.base.domain.errors.domain_error import DomainError
 from petisco.base.domain.model.uuid import Uuid
 
 
 class NotFound(DomainError):
     ...
@@ -22,11 +22,11 @@
         repository_str = f" (repository: {repository_name})" if repository_name else ""
         message = f"Aggregate{aggregate_id_str} not found{repository_str}"
         uuid_value = aggregate_id.value if aggregate_id else None
         super().__init__(uuid_value=uuid_value, additional_info={"message": message})
 
 
 class AggregatesNotFoundError(DomainError):
-    def __init__(self, repository_name: str = None):
+    def __init__(self, repository_name: Union[str, None] = None):
         repository_str = f" (repository: {repository_name})" if repository_name else ""
         message = f"Aggregates not found{repository_str}]"
         super().__init__(additional_info={"message": message})
```

### Comparing `petisco-1.9.9/petisco/base/domain/errors/domain_error.py` & `petisco-2.0.0rc0/petisco/base/domain/errors/domain_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-from typing import Dict
+from typing import Dict, Optional
 
 from meiga import Error
 
 
 class DomainError(Error):
-    def __init__(self, uuid_value: str = None, additional_info: Dict[str, str] = None):
+    """
+    A base class to define Domain Errors
+    """
+
+    def __init__(
+        self,
+        uuid_value: Optional[str] = None,
+        additional_info: Optional[Dict[str, str]] = None,
+    ):
         self.uuid_value = uuid_value
         self.additional_info = additional_info
         self._additional_detail = ""
         self._specific_detail = "DomainError"
         self._set_detail()
 
-    def _set_detail(self):
+    def _set_detail(self) -> None:
         if self.uuid_value:
             self._additional_detail += f" ({self.uuid_value})"
 
         if self.additional_info:
             self._additional_detail += f" [{self.additional_info}]"
 
     @classmethod
-    def get_specify_detail(cls):
+    def get_specify_detail(cls) -> str:
         return cls.__name__
 
     def detail(self) -> str:
         return f"{self.get_specify_detail()}{self._additional_detail}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.get_specify_detail()}{self._additional_detail}"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.get_specify_detail()}{self._additional_detail}"
```

### Comparing `petisco-1.9.9/petisco/base/domain/errors/unknown_error.py` & `petisco-2.0.0rc0/petisco/base/domain/errors/unknown_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 import sys
 import traceback
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from meiga import Error
 
 
 class UnknownError(Error):
+    """
+    A base class to define unknown errors.
+
+    If UnknownError is caught and uses NotifierMiddleware in your operations (Controllers or Subscribers), when
+    you UseCase fails the system will notify the issue.
+    """
+
     def __init__(
         self,
         exception: Exception,
-        input_parameters=None,
-        executor=None,
-        traceback=None,
-        filename=None,
-        lineno=None,
-        filter_parameters: List[str] = None,
-        meta: Dict = None,
-    ):
+        input_parameters: Any = None,
+        executor: Any = None,
+        traceback: Any = None,
+        filename: Any = None,
+        lineno: Any = None,
+        filter_parameters: Union[List[str], None] = None,
+        meta: Union[Dict[str, Any], None] = None,
+    ) -> None:
         self.message = f"{exception.__class__.__name__}: {str(exception)}"
         self.input_parameters = self._sanitize_input_params(input_parameters)
         self._filter_input_parameters(filter_parameters)
         self.exception = exception
         self.executor = executor
         self.traceback = traceback
         self.filename = filename
         self.lineno = lineno
         self.meta = meta if meta else {}
 
-    def _sanitize_input_params(self, input_parameters):
+    def _sanitize_input_params(self, input_parameters: Any) -> Any:
         if isinstance(input_parameters, tuple):
             return {
                 f"param_{i + 1}": param if not isinstance(param, bytes) else "bytes"
                 for i, param in enumerate(input_parameters)
             }
         elif isinstance(input_parameters, dict):
             return {
                 k: v if not isinstance(v, bytes) else "bytes"
                 for k, v in input_parameters.items()
             }
         else:
             return None
 
-    def _filter_input_parameters(self, filter_parameters: List[str] = None):
+    def _filter_input_parameters(
+        self, filter_parameters: Union[List[str], None] = None
+    ) -> None:
         if filter_parameters:
             self.input_parameters = {
                 k: v
                 for k, v in self.input_parameters.items()
                 if k not in filter_parameters
             }
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         executor_str = f" ({self.executor})" if self.executor else ""
         traceback_str = f"\n{self.traceback}" if self.traceback else ""
         input_parameters_str = (
             f"\nInput Parameters: {str(self.input_parameters)}"
             if self.input_parameters
             else ""
         )
@@ -63,19 +72,19 @@
 
     @classmethod
     def from_exception(
         cls,
         exception: Exception,
         arguments: Any,
         class_name: Optional[str] = None,
-    ):
+    ) -> "UnknownError":
         _, _, tb = sys.exc_info()
-        tb = traceback.extract_tb(tb)[-1]
-        filename = tb.filename if tb and hasattr(tb, "filename") else None
-        lineno = tb.lineno if tb and hasattr(tb, "lineno") else None
+        tb = traceback.extract_tb(tb)[-1]  # type: ignore
+        filename = tb.filename if tb and hasattr(tb, "filename") else None  # type: ignore
+        lineno = tb.lineno if tb and hasattr(tb, "lineno") else None  # type: ignore
 
         unknown_error = cls(
             exception=exception,
             input_parameters=arguments,
             executor=class_name,
             traceback=traceback.format_exc(),
             filename=filename,
```

### Comparing `petisco-1.9.9/petisco/base/domain/message/command.py` & `petisco-2.0.0rc0/petisco/base/domain/message/domain_event.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,42 @@
+from __future__ import annotations
+
 import json
-from typing import Dict, Optional, Type, Union
+from typing import Any, TypeVar
 
 from petisco.base.domain.message.message import Message
 
+T = TypeVar("T", bound="DomainEvent")
+
 
-class Command(Message):
-    def __init__(self, **kwargs):
-        self._set_data()
-        self._set_attributes(**kwargs)
-        self.type = "command"
+class DomainEvent(Message):
+    """
+    A base class to model your domain events.
+    Define your Domain Events to express what happened in your domain.
+    """
+
+    def __init__(self, **data: Any) -> None:
+        super().__init__()
+        self._set_attributes(**data)
+        self._message_type = "domain_event"
 
     @staticmethod
-    def from_dict(message_data: Dict, target_type: Optional[Type] = None):
-        target_type = Command if target_type is None else target_type
+    def from_dict(
+        message_data: dict[str, Any],
+        target_type: type[T] | None = None,
+    ) -> T:
+        target_type = DomainEvent if target_type is None else target_type
         data = message_data.get("data")
-        command = target_type()
-        command._set_data(**data)
-        return command
+        domain_event = target_type()
+        domain_event._set_data(**data)  # type: ignore
+        return domain_event
 
     @staticmethod
-    def from_json(message_json: Union[str, bytes], target_type: Optional[Type] = None):
+    def from_json(
+        message_json: str | bytes,
+        target_type: type[T] | None = None,
+    ) -> T:
         event_dict = json.loads(message_json)
-        return Command.from_dict(event_dict, target_type)
+        return DomainEvent.from_dict(event_dict, target_type)
 
-    def __repr__(self):
-        return self.to_str(class_name="Command", type="domain_event")
+    def __repr__(self) -> str:
+        return self.to_str(class_name="DomainEvent", type="domain_event")
```

### Comparing `petisco-1.9.9/petisco/base/domain/message/command_bus.py` & `petisco-2.0.0rc0/petisco/base/domain/message/command_bus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 
 from petisco.base.domain.message.command import Command
 from petisco.base.domain.message.message_bus import MessageBus
 
 
-class CommandBus(MessageBus):
+class CommandBus(MessageBus[Command]):
+    """
+    A base class to implement an infrastructure-based bus to dispatch commands.
+    """
+
     @abstractmethod
-    def dispatch(self, command: Command):
+    def dispatch(self, command: Command | list[Command]) -> None:
+        """
+        Dispatch one Command or a list of commands
+
+        Dispatch several commands could be a code smell but some use case could require this feature.
+        """
         raise NotImplementedError
 
-    def publish(self, command: Command):
+    def publish(self, command: Command | list[Command]) -> None:
         self.dispatch(command)
 
-    def retry_publish_only_on_store_queue(self, command: Command):
-        pass
-
-    def _check_is_command(self, command: Command):
+    def _check_is_command(self, command: Command) -> None:
         if not command or not issubclass(command.__class__, Command):
-            raise TypeError("CommandBus only publishes DomainEvent objects")
+            raise TypeError(f"{self.__class__.__name__} only publishes Command objects")
 
     @abstractmethod
-    def close(self):
+    def close(self) -> None:
         raise NotImplementedError
```

### Comparing `petisco-1.9.9/petisco/base/domain/message/domain_event_bus.py` & `petisco-2.0.0rc0/petisco/base/domain/message/domain_event_bus.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 
 from petisco.base.domain.message.domain_event import DomainEvent
 from petisco.base.domain.message.message_bus import MessageBus
 
 
-class DomainEventBus(MessageBus):
-    @abstractmethod
-    def publish(self, domain_event: DomainEvent):
-        raise NotImplementedError
-
-    @abstractmethod
-    def retry_publish_only_on_store_queue(self, domain_event: DomainEvent):
-        raise NotImplementedError
+class DomainEventBus(MessageBus[DomainEvent]):
+    """
+    A base class to implement an infrastructure-based bus to publish events.
+    """
 
     @abstractmethod
-    def retry_publish(
-        self,
-        domain_event: DomainEvent,
-        retry_routing_key: str,
-        retry_exchange_name: str = None,
-    ):
+    def publish(self, domain_event: DomainEvent | list[DomainEvent]) -> None:
+        """
+        Publish a DomainEvent or a list of DomainEvents
+        """
         raise NotImplementedError
 
-    def _check_is_domain_event(self, domain_event: DomainEvent):
+    def _check_is_domain_event(
+        self, domain_event: DomainEvent | list[DomainEvent]
+    ) -> None:
         if not domain_event or not issubclass(domain_event.__class__, DomainEvent):
-            raise TypeError("DomainEventBus only publishes DomainEvent objects")
+            raise TypeError(
+                f"{self.__class__.__name__} only publishes DomainEvent objects"
+            )
 
     @abstractmethod
-    def close(self):
+    def close(self) -> None:
         raise NotImplementedError
```

### Comparing `petisco-1.9.9/petisco/base/domain/message/message_bus.py` & `petisco-2.0.0rc0/petisco/base/domain/message/message_bus.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,63 @@
+from __future__ import annotations
+
 import copy
 from abc import ABC, abstractmethod
-from typing import Dict, List
+from typing import Any, Dict, Generic, TypeVar
 
 from petisco.base.domain.message.message import Message
 
+TypeMessage = TypeVar("TypeMessage", bound=Message)
+
+
+class MessageBus(ABC, Generic[TypeMessage]):
+    """
+    A base class to implement an infrastructure-based bus to publish or dispatch messages.
+    """
 
-class MessageBus(ABC):
     @classmethod
-    def __repr__(cls):
+    def __repr__(cls) -> str:
         return cls.__name__
 
     @classmethod
-    def info(cls) -> Dict:
+    def info(cls) -> dict[str, str]:
         return {"name": cls.__name__}
 
-    def _set_additional_meta(self, meta: Dict):
+    def _set_additional_meta(self, meta: dict[str, Any]) -> None:
         self.additional_meta = meta
 
-    def with_meta(self, meta: Dict):
+    def with_meta(self, meta: dict[str, Any]) -> MessageBus[Message]:
         if not isinstance(meta, Dict):
             raise TypeError("MessageBus.with_meta() expect a dict")
-        event_bus = copy.copy(self)
-        event_bus._set_additional_meta(meta)
-        return event_bus
+        message_bus = copy.copy(self)
+        message_bus._set_additional_meta(meta)
+        return message_bus  # type: ignore
 
-    def get_configured_meta(self) -> Dict:
-        configured_meta = {}
+    def get_configured_meta(self) -> dict[str, Any]:
+        configured_meta: dict[str, Any] = {}
         if hasattr(self, "additional_meta"):
             configured_meta = {**configured_meta, **self.additional_meta}
         return configured_meta
 
     @abstractmethod
-    def publish(self, message: Message):
+    def publish(self, message: TypeMessage | list[TypeMessage]) -> None:
+        """
+        Publish a message or a list of messages
+        """
         raise NotImplementedError
 
-    @abstractmethod
-    def retry_publish_only_on_store_queue(self, message: Message):
-        raise NotImplementedError
+    def _check_input(
+        self, message: TypeMessage | list[TypeMessage]
+    ) -> list[TypeMessage]:  # noqa
+        if isinstance(message, list):
+            messages = message
+        else:
+            messages = [message]
+        return messages
 
     @abstractmethod
-    def close(self):
+    def close(self) -> None:
         raise NotImplementedError
 
-    def _check_is_message(self, message: Message):
+    def _check_is_message(self, message: TypeMessage) -> None:
         if not message or not issubclass(message.__class__, Message):
             raise TypeError("MessageBus only publishes Message objects")
-
-    def publish_list(self, messages: List[Message]):
-        for message in messages:
-            self.publish(message)
-
-    def retry_publish_list_only_on_store_queue(self, messages: List[Message]):
-        for message in messages:
-            self.retry_publish_only_on_store_queue(message)
```

### Comparing `petisco-1.9.9/petisco/base/domain/message/message_subscriber.py` & `petisco-2.0.0rc0/petisco/base/domain/message/message_subscriber.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+from __future__ import annotations
+
 import re
 from abc import abstractmethod
 from types import FunctionType
-from typing import List, Type
+from typing import Any
 
 from meiga import BoolResult
 
+from petisco.base.application.middleware.middleware import Middleware
 from petisco.base.domain.message.command_bus import CommandBus
 from petisco.base.domain.message.domain_event_bus import DomainEventBus
 from petisco.base.domain.message.message import Message
+from petisco.base.domain.message.message_bus import TypeMessage
 from petisco.base.domain.message.message_subscriber_info import MessageSubscriberInfo
-from petisco.base.domain.message.not_implemented_message_bus import (
-    NotImplementedMessageBus,
+from petisco.base.domain.message.not_implemented_command_bus import (
+    NotImplementedCommandBus,
+)
+from petisco.base.domain.message.not_implemented_domain_event_bus import (
+    NotImplementedDomainEventBus,
 )
 from petisco.base.misc.interface import Interface
 from petisco.base.misc.result_mapper import ResultMapper
 from petisco.base.misc.wrapper import wrapper
 
 
 class MetaMessageSubscriber(type, Interface):
-    domain_event_bus: DomainEventBus = NotImplementedMessageBus()
-    command_bus: CommandBus = NotImplementedMessageBus()
-    middlewares: List = {}
-
-    def __new__(mcs, name, bases, namespace):
+    domain_event_bus: DomainEventBus = NotImplementedDomainEventBus()
+    command_bus: CommandBus = NotImplementedCommandBus()
+    middlewares: list[Middleware] = []
+
+    def __new__(
+        mcs, name: str, bases: tuple[Any, ...], namespace: dict[str, Any]
+    ) -> MetaMessageSubscriber:
         config = namespace.get("Config")
 
         if "handle" not in namespace:
             raise NotImplementedError(
                 "Petisco MessageSubscriber must implement an handle method"
             )
 
@@ -37,45 +46,45 @@
             if isinstance(attribute, FunctionType) and attribute.__name__ == "handle":
                 attribute = wrapper(attribute, name, config, mapper)
             new_namespace[attributeName] = attribute
 
         return super().__new__(mcs, name, bases, new_namespace)
 
     @abstractmethod
-    def subscribed_to(self) -> List[Type[Message]]:
+    def subscribed_to(self) -> list[type[Message]]:
         raise NotImplementedError()
 
     @abstractmethod
     def handle(self, message: Message) -> BoolResult:
         raise NotImplementedError()
 
 
 class MessageSubscriber(metaclass=MetaMessageSubscriber):
     @abstractmethod
-    def subscribed_to(self) -> List[Type[Message]]:
+    def subscribed_to(self) -> Any:
         raise NotImplementedError()
 
     @abstractmethod
-    def handle(self, message: Message) -> BoolResult:
+    def handle(self, message: TypeMessage) -> BoolResult:
         raise NotImplementedError()
 
     @classmethod
-    def __repr__(cls):
-        subscriptions = cls.subscribed_to(cls)
+    def __repr__(cls) -> str:
+        subscriptions = cls.subscribed_to(cls)  # type: ignore
         if not isinstance(subscriptions, list):
             subscriptions = [subscriptions]
         return f"{cls.__name__}: subscribed_to {[class_type.__name__ for class_type in subscriptions]}"
 
-    def set_domain_event_bus(self, domain_event_bus: DomainEventBus):
+    def set_domain_event_bus(self, domain_event_bus: DomainEventBus) -> None:
         self.domain_event_bus = domain_event_bus
 
-    def set_command_bus(self, command_bus: CommandBus):
+    def set_command_bus(self, command_bus: CommandBus) -> None:
         self.command_bus = command_bus
 
     def get_subscriber_name(self) -> str:
         return re.sub(r"(?<!^)(?=[A-Z])", "_", self.__class__.__name__).lower()
 
-    def get_message_subscribers_info(self) -> List[MessageSubscriberInfo]:
+    def get_message_subscribers_info(self) -> list[MessageSubscriberInfo]:
         subscribers_info = []
         for class_type in self.subscribed_to():
             subscribers_info.append(MessageSubscriberInfo.from_class_type(class_type))
         return subscribers_info
```

### Comparing `petisco-1.9.9/petisco/base/domain/message/not_implemented_domain_event_bus.py` & `petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_domain_event_bus.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from __future__ import annotations
+
 from petisco.base.domain.message.domain_event import DomainEvent
 from petisco.base.domain.message.domain_event_bus import DomainEventBus
 
 
 class NotImplementedDomainEventBus(DomainEventBus):
-    def publish(self, domain_event: DomainEvent):
-        self._check_is_domain_event(domain_event)
-        meta = self.get_configured_meta()
-        _ = domain_event.update_meta(meta)
-
-    def retry_publish_only_on_store_queue(self, domain_event: DomainEvent):
-        self._check_is_domain_event(domain_event)
-        meta = self.get_configured_meta()
-        _ = domain_event.update_meta(meta)
+    def publish(self, domain_event: DomainEvent | list[DomainEvent]) -> None:
+        domain_events = (
+            [domain_event] if isinstance(domain_event, DomainEvent) else domain_event
+        )
+        for domain_event in domain_events:
+            self._check_is_domain_event(domain_event)
+            meta = self.get_configured_meta()
+            _ = domain_event.update_meta(meta)
 
     def retry_publish(
         self,
         domain_event: DomainEvent,
         retry_routing_key: str,
-        retry_exchange_name: str = None,
-    ):
+        retry_exchange_name: str | None = None,
+    ) -> None:
         self._check_is_domain_event(domain_event)
         meta = self.get_configured_meta()
         _ = domain_event.update_meta(meta)
 
-    def close(self):
+    def close(self) -> None:
         pass
```

### Comparing `petisco-1.9.9/petisco/base/domain/message/not_implemented_message_comsumer.py` & `petisco-2.0.0rc0/petisco/base/domain/message/not_implemented_message_comsumer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-from typing import Callable, List, Type
+from __future__ import annotations
+
+from typing import Any, NoReturn
 
 from petisco.base.domain.message.message_consumer import MessageConsumer
 from petisco.base.domain.message.message_subscriber import MessageSubscriber
 
 
-class NotImplementedMessageConsumer(MessageConsumer):
-    def start(self):
-        pass
-
-    def add_subscribers(self, subscribers: List[MessageSubscriber]):
+class NotImplementedMessageConsumer(MessageConsumer[Any]):
+    def start(self) -> NoReturn:
         pass
 
-    def add_subscriber_on_dead_letter(self, subscriber: Type[MessageSubscriber]):
+    def add_subscribers(self, subscribers: list[MessageSubscriber]) -> None:
         pass
 
-    def add_handler_on_store(self, handler: Callable):
+    def add_subscriber_on_dead_letter(
+        self, subscriber: type[MessageSubscriber]
+    ) -> None:
         pass
 
-    def add_subscriber_on_queue(self, queue_name: str, handler: Callable):
+    def add_subscriber_on_queue(
+        self,
+        queue_name: str,
+        subscriber: type[MessageSubscriber],
+        is_store: bool = False,
+        message_type_expected: str = "message",
+    ) -> None:
         pass
 
-    def unsubscribe_subscriber_on_queue(self, queue_name: str):
+    def unsubscribe_subscriber_on_queue(self, queue_name: str) -> None:
         pass
 
-    def resume_subscriber_on_queue(self, queue_name: str):
+    def resume_subscriber_on_queue(self, queue_name: str) -> None:
         pass
 
-    def stop(self):
+    def stop(self) -> None:
         pass
```

### Comparing `petisco-1.9.9/petisco/base/domain/model/value_object.py` & `petisco-2.0.0rc0/petisco/base/domain/model/uuid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-from typing import Any
+from uuid import uuid4
 
+import validators
 from pydantic import validator
-from pydantic.main import BaseModel
 
-from petisco.base.domain.errors.defaults.invalid_value_object import InvalidValueObject
+from petisco.base.domain.errors.defaults.invalid_uuid import InvalidUuid
+from petisco.base.domain.model.value_object import ValueObject
 
 
-class ValueObject(BaseModel):
-    value: Any
+class Uuid(ValueObject):
+    """
+    A base class to define Uuid
 
-    def __init__(self, value: Any, **data) -> None:
-        super().__init__(value=value, **data)
+    Use it to identify domain entities
+    """
 
-    def dict(self, **kwargs):
-        return self.value
-
-    def __setattr__(self, name, value):
-        raise TypeError("ValueObject objects are immutable")
-
-    def __hash__(self):
-        return hash(self.value)
-
-    @classmethod
-    def from_value(cls, value):
-        return cls(value=value)
+    value: str
 
     @validator("value")
-    def validate_value(cls, value):
-        if value is None:
-            raise InvalidValueObject()
+    def validate_value(cls, value: str) -> str:
+        if value is None or not validators.uuid(value):
+            raise InvalidUuid(uuid_value=value)
         return value
+
+    @classmethod
+    def v4(cls) -> "Uuid":
+        return cls(value=str(uuid4()))
```

### Comparing `petisco-1.9.9/petisco/base/domain/persistence/fake_database.py` & `petisco-2.0.0rc0/petisco/base/domain/persistence/legacy_fake_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import List
+from typing import Any, List
 
-from petisco.base.domain.persistence.interface_database import Database
+from petisco.base.domain.persistence.legacy_database import LegacyDatabase
 from petisco.base.domain.persistence.persistence_models import PersistenceModels
 
 
-class FakeDatabase(Database):
+class LegacyFakeDatabase(LegacyDatabase):
     def __init__(self, name: str, model_filename: str):
         models = PersistenceModels.from_filename(model_filename).get_models_names()
         super().__init__(name, models=models)
 
-    def create(self):
+    def create(self) -> None:
         pass
 
-    def delete(self):
+    def delete(self) -> None:
         pass
 
-    def clear_data(self):
+    def clear_data(self) -> None:
         pass
 
-    def get_model(self, model_name: str):
+    def get_model(self, model_name: str) -> Any:
         model = self.models.get(model_name)
         if not model:
             raise IndexError(
                 f'Model "{model_name}" is not available for "{self.name}" database'
             )
         return model
```

### Comparing `petisco-1.9.9/petisco/base/domain/persistence/interface_database.py` & `petisco-2.0.0rc0/petisco/base/domain/persistence/legacy_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from abc import ABC, abstractmethod
-from typing import Dict, List
+from typing import Any, Dict, List, Union
 
 
-class Database(ABC):
-    def __init__(self, name: str, models: Dict = None):
+class LegacyDatabase(ABC):
+    def __init__(self, name: str, models: Union[Dict[str, Any], None] = None):
         self.name = name
         self.models = models if models else {}
 
-    def info(self) -> Dict:
-        _info = {"name": self.name}
+    def info(self) -> Dict[str, Any]:
+        _info: Dict[str, Any] = {"name": self.name}
         if self.models:
             _info["models"] = self.models
         return _info
 
     @abstractmethod
-    def create(self):
+    def create(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def delete(self):
+    def delete(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def clear_data(self):
+    def clear_data(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def get_model(self, model_name: str):
+    def get_model(self, model_name: str) -> Any:
         raise NotImplementedError
 
     @abstractmethod
     def get_model_names(self) -> List[str]:
         raise NotImplementedError
```

### Comparing `petisco-1.9.9/petisco/base/domain/persistence/persistence.py` & `petisco-2.0.0rc0/petisco/base/domain/persistence/persistence.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 import inspect
 from dataclasses import dataclass
-from typing import Callable, List
+from typing import Any, Callable, Dict, List, Union
 
 from loguru import logger
 
-from petisco.base.domain.persistence.interface_database import Database
+from petisco.base.domain.persistence.legacy_database import LegacyDatabase
 from petisco.base.misc.singleton import Singleton
 
 
 @dataclass
 class Persistence(metaclass=Singleton):
-    def __init__(self):
-        self._databases = {}
+    def __init__(self) -> None:
+        self._databases: Dict[str, Any] = {}
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Persistence: {str(self.get_info())}"
 
-    def get_info(self):
+    def get_info(self) -> Dict[str, Any]:
         return {name: database.info() for name, database in self._databases.items()}
 
     @staticmethod
-    def info():
+    def info() -> Dict[str, Any]:
         return Persistence.get_instance().get_info()
 
     @staticmethod
-    def get_instance():
+    def get_instance() -> "Persistence":
         try:
             return Persistence()
         except Exception as e:  # noqa E722
             frame_info = inspect.stack()[1]
             raise ImportError(
                 f"Persistence must be configured. If not, you cannot obtain models\n"
                 f"Following code must be executed after Persistence initialization:\n"
                 f"\tfilename: {frame_info.filename}\n"
                 f"\tlineno: {frame_info.lineno}\n"
                 f"\tfunction: {frame_info.function}\n"
                 f"\tcode_context: {frame_info.code_context}\n\n"
             )
 
-    def add(self, database: Database, skip_if_exist: bool = False):
+    def add(self, database: LegacyDatabase, skip_if_exist: bool = False) -> None:
         if database.name in self._databases:
             if skip_if_exist is False:
                 raise NameError(
                     f"Database {database.name} is already added to Persistence"
                 )
         else:
             self._databases[database.name] = database
 
-    def remove(self, database_name: str, skip_if_not_exist: bool = False):
+    def remove(self, database_name: str, skip_if_not_exist: bool = False) -> None:
         if database_name in self._databases:
             self._databases[database_name].delete()
             del self._databases[database_name]
         else:
             if skip_if_not_exist is False:
                 raise IndexError(
                     f"Database cannot be removed. {database_name} not exists"
                 )
 
-    def create(self):
+    def create(self) -> None:
         for database in self._databases.values():
             database.create()
 
-    def delete(self):
+    def delete(self) -> None:
         for database in self._databases.values():
             database.delete()
 
-    def clear_data(self, database_name: str = None):
+    def clear_data(self, database_name: Union[str, None] = None) -> None:
         databases = self._databases
         if database_name is not None:
             if database_name not in self._databases:
                 raise IndexError(
                     f"Database cannot clear the data. {database_name} not exists"
                 )
             databases = [self._databases.get(database_name)]
         for database in databases.values():
             database.clear_data()
 
     @staticmethod
-    def exist():
+    def exist() -> bool:
         databases = Persistence.get_instance()._databases
         if len(databases) < 1:
             return False
         else:
             return True
 
     @staticmethod
-    def is_available(database_name: str = None):
-        def log_warning(message: str):
+    def is_available(database_name: Union[str, None] = None) -> bool:
+        def log_warning(message: str) -> None:
             logger.debug(message)
 
         databases = Persistence.get_instance()._databases
         if database_name is not None:
             if database_name not in databases:
                 raise IndexError(
                     f"Database cannot return is_available. {database_name} not exists"
@@ -102,26 +102,26 @@
         for database_name, database in databases.items():
             if not database.is_available():
                 log_warning(f"Database {database_name} is not available")
                 return False
         return True
 
     @staticmethod
-    def get_base(database_name: str) -> List[str]:
+    def get_base(database_name: str) -> Any:
         database = Persistence.get_instance()._databases.get(database_name)
         if not database:
             raise IndexError(f"Database name ({database_name}) not exists.")
 
         if not hasattr(database, "get_base"):
             raise IndexError(f"Database ({database_name}) has not get_base method. ")
 
         return database.get_base()
 
     @staticmethod
-    def get_databases() -> List[Database]:
+    def get_databases() -> List[LegacyDatabase]:
         return list(Persistence.get_instance()._databases.values())
 
     @staticmethod
     def get_available_databases() -> List[str]:
         return list(Persistence.get_instance()._databases.keys())
 
     @staticmethod
@@ -129,33 +129,33 @@
         database = Persistence.get_instance()._databases.get(database_name)
         if not database:
             raise IndexError(f"Database name ({database_name}) not exists.")
 
         return list(database.get_model_names())
 
     @staticmethod
-    def get_model(database_name: str, model_name: str):
+    def get_model(database_name: str, model_name: str) -> Any:
         database = Persistence.get_instance()._databases.get(database_name)
         if not database:
             raise IndexError(f"Database name ({database_name}) not exists.")
         return database.get_model(model_name)
 
     @staticmethod
-    def get_session(database_name: str):
+    def get_session(database_name: str) -> Any:
         database = Persistence.get_instance()._databases.get(database_name)
         if not database:
             raise IndexError(f"Database name ({database_name}) not exists.")
 
         if not hasattr(database, "get_session"):
             raise IndexError(f"Database ({database_name}) has not get_session method. ")
 
         return database.get_session()
 
     @staticmethod
-    def get_session_scope(database_name: str) -> Callable:
+    def get_session_scope(database_name: str) -> Callable[..., Any]:
         database = Persistence.get_instance()._databases.get(database_name)
         if not database:
             raise IndexError(f"Database name ({database_name}) not exists.")
 
         if not hasattr(database, "get_session_scope"):
             raise IndexError(
                 f"Database ({database_name}) has not get_session_scope method. "
```

### Comparing `petisco-1.9.9/petisco/base/domain/persistence/persistence_models.py` & `petisco-2.0.0rc0/petisco/base/domain/persistence/persistence_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 import importlib
 import os
 import sys
 import traceback
 from typing import Any, Dict
 
 import yaml
-from yaml.parser import ParserError, ScannerError
+from yaml.parser import ParserError
+from yaml.scanner import ScannerError
 
 
 class PersistenceModels:
-    def __init__(self, models: Dict[str, Any]):
+    def __init__(self, models: Dict[str, Any]) -> None:
         self.models = models
-        self.imported_models = {}
+        self.imported_models: Dict[str, Any] = {}
 
     @staticmethod
-    def from_filename(filename: str):
+    def from_filename(filename: str) -> "PersistenceModels":
         if not os.path.isfile(filename):
             raise FileNotFoundError(f"PersistenceModels ({filename} not found)")
         try:
             with open(filename) as file:
                 petisco_dict = yaml.load(file, Loader=yaml.FullLoader)
                 models = petisco_dict.get("models")
                 return PersistenceModels(models)
         except (ParserError, ScannerError) as e:
             message = f"Error loading {filename} file: {repr(e.__class__)} {e} | {traceback.format_exc()}"
             raise RuntimeError(message)
 
-    def get_models_names(self):
+    def get_models_names(self) -> Dict[str, Any]:
         return self.models
 
-    def import_models(self):
+    def import_models(self) -> None:
         self.imported_models = self.import_database_models()
 
         # self.imported_models = {}
         # for name, model_string in self.models.items():
         #     mod_name, model_name = model_string.rsplit(".", 1)
         #     mod = importlib.import_module(mod_name)
         #     self.imported_models[name] = getattr(mod, model_name)
 
-    def import_database_models(self):
-        def _is_class_in_sqlalchemy_tables(class_model_name: str):
+    def import_database_models(self) -> Dict[str, Any]:
+        def _is_class_in_sqlalchemy_tables(class_model_name: str) -> bool:
             # We need this to filter deletion in case of Model dependencies.
             # For instance, ClientConfigModel imports ClientModel on class model definition
             # It throws the following error:
             #  sqlalchemy.exc.InvalidRequestError: Table 'ClientConfig' is already defined for this MetaData instance.
             #  Specify 'extend_existing=True' to redefine options and columns on an existing Table object.
-            # As a workaround, we only delete the module if it not exist in SQLAlchemy tables.
+            # As a workaround, we only delete the module if it not exists in SQLAlchemy tables.
 
             from petisco.base.domain.persistence.persistence import Persistence
 
             is_in_tables = False
             for database in Persistence.get_databases():
                 if not hasattr(database, "get_base"):
                     continue
@@ -57,32 +58,34 @@
                 if not Base:
                     continue
                 is_in_tables = class_model_name.replace("Model", "") in list(
                     Base.metadata.tables.keys()
                 )
             return is_in_tables
 
-        def _delete_module_if_already_imported(module_name: str, class_model_name: str):
+        def _delete_module_if_already_imported(
+            module_name: str, class_model_name: str
+        ) -> None:
             # Important. SqlAlchemy needs models to be imported
             # Base = Persistence.get_base("petisco")
             # If module is already imported and Base has not tables, Tables won't be imported.
             # This, usually happens when start the application (e.g end2end tests)
             # e.g len(Base.metadata.tables) == 0
             # With this function we ensure that model can be imported to help SqlAlchemy loading models if is not imported yet
             if module_name in sys.modules and not _is_class_in_sqlalchemy_tables(
                 class_model_name
             ):
                 del sys.modules[module_name]
 
-        def _import_database_models_func():
+        def _import_database_models_func() -> Dict[str, Any]:
             imported_models = {}
             for name, model_string in self.models.items():
                 module_name, class_model_name = model_string.rsplit(".", 1)
                 _delete_module_if_already_imported(module_name, class_model_name)
                 module_name = importlib.import_module(module_name, class_model_name)
                 imported_models[name] = getattr(module_name, class_model_name)
             return imported_models
 
         return _import_database_models_func()
 
-    def get_imported_models(self):
+    def get_imported_models(self) -> Dict[str, Any]:
         return self.imported_models
```

### Comparing `petisco-1.9.9/petisco/base/misc/builder.py` & `petisco-2.0.0rc0/petisco/base/misc/builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,39 @@
-from typing import Any
+from typing import Any, Generic, Type, TypeVar
 
+T = TypeVar("T")
 
-class Builder:
-    def __init__(self, klass: Any, is_builder: bool = False, *args, **kwargs):
+
+class Builder(Generic[T]):
+    """
+    Data structure that defines the creation of an instance from its arguments.
+    """
+
+    def __init__(
+        self,
+        klass: Type[T],
+        name_constructor: str = None,
+        is_builder: bool = False,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         self.klass = klass
         self.args = args
         self.kwargs = kwargs
+        self.name_constructor = name_constructor
         self.is_builder = is_builder
 
-    def build(self):
+    def build(self) -> T:
         try:
-            if self.is_builder:
-                instance = self.klass.build(*self.args, **self.kwargs)
+            if self.name_constructor:
+                constructor = getattr(self.klass, self.name_constructor)
+                instance: T = constructor(*self.args, **self.kwargs)
+            elif self.is_builder:
+                instance: T = self.klass.build(*self.args, **self.kwargs)
             else:
-                instance = self.klass(*self.args, **self.kwargs)
+                instance: T = self.klass(*self.args, **self.kwargs)
         except Exception as exc:
             raise RuntimeError(
                 f"Error instantiating {self.klass.__name__}\n{repr(exc)}"
             )
 
         return instance
```

### Comparing `petisco-1.9.9/petisco/cli/petisco.py` & `petisco-2.0.0rc0/petisco/cli/petisco.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import argparse
 import os
 from datetime import datetime
+from typing import Any
 
-from petisco import Uuid, __version__
+from petisco import __version__
+from petisco.base.domain.model.uuid import Uuid
 
 
-def has_args(args):
+def has_args(args: Any) -> bool:
     is_active = False
     for arg in vars(args):
         is_active = is_active or getattr(args, arg)
     return is_active
 
 
-def rename_template(original_name: str, replacement: str):
+def rename_template(original_name: str, replacement: str) -> None:
 
     for dname, _, _ in os.walk("."):
         if original_name in dname:
             os.rename(dname, dname.replace(original_name, replacement))
 
     blacklist = [".git/", ".idea"]
     for dname, dirs, files in os.walk("."):
@@ -34,15 +36,15 @@
                 s = s.replace(original_name, replacement)
                 with open(fpath, "w") as f:
                     f.write(s)
             except Exception:
                 pass
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         prog="petisco 🍪",
         description="petisco is a framework for helping Python developers to build clean Applications",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument(
         "-v", "--version", action="store_true", help="show petisco version number."
```

### Comparing `petisco-1.9.9/petisco/cli/petisco_rabbitmq.py` & `petisco-2.0.0rc0/petisco/cli/petisco_rabbitmq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import argparse
 import logging
 from time import sleep
-from typing import List, Type
+from typing import Any, List, Type, cast
 
 from meiga import BoolResult, isFailure, isSuccess
 
 from petisco import (
     AllMessageSubscriber,
     DomainEvent,
     Message,
     MessageSubscriber,
     __version__,
 )
-from petisco.extra.rabbitmq import RabbitMqConnector, RabbitMqMessageConsumer
-from petisco.legacy import LoggingBasedLogger
+from petisco.extra.logger import Logger, LoggingBasedLogger
+from petisco.extra.rabbitmq.application.message.consumer.rabbitmq_message_consumer import (
+    RabbitMqMessageConsumer,
+)
+from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 
 ORGANIZATION = "alice"
 RETRY_TTL = 5000  # default
 MAX_RETRIES = 5  # default
 
 
-def has_args(args):
+def has_args(args: Any) -> bool:
     is_active = False
     for arg in vars(args):
         is_active = is_active or getattr(args, arg)
     return is_active
 
 
-def get_logger():
-    def logging_config():
+def get_logger() -> Logger:
+    def logging_config() -> None:
         logging.getLogger("pika").setLevel(logging.WARNING)
 
     logger = LoggingBasedLogger("example", config=logging_config)
     return logger
 
 
 class MyDomainEvent(DomainEvent):
@@ -44,15 +47,15 @@
         return [MyDomainEvent]
 
     def handle(self, message: Message) -> BoolResult:
         print(f"> It will unack the message: {message.dict()}\n")
         return isFailure
 
 
-def get_args():
+def get_args() -> Any:
     parser = argparse.ArgumentParser(
         prog="petisco-rabbitmq 🍪",
         description="petisco-rabbitmq helps us on rabbitmq iteration",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument("-rq", "--requeue", action="store_true", help="requeue")
     parser.add_argument(
@@ -125,15 +128,15 @@
     if not has_args(args):
         parser.print_help()
         return None
 
     return args
 
 
-def main():
+def main() -> None:
     args = get_args()
 
     if not args:
         return
 
     if args.requeue:
 
@@ -169,14 +172,16 @@
         )
 
         class RequeueOnMessage(AllMessageSubscriber):
             def handle(self, message: Message) -> BoolResult:
                 if args.wait_to_requeue:
                     sleep(args.wait_sec)
 
+                message = cast(DomainEvent, message)
+
                 self.domain_event_bus.retry_publish(
                     message, args.retry_routing_key, args.retry_exchange_name
                 )
 
                 return isSuccess
 
         consumer.add_subscriber_on_queue(
```

### Comparing `petisco-1.9.9/petisco/extra/elastic/elastic_connection.py` & `petisco-2.0.0rc0/petisco/extra/elastic/elastic_connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import os
+from typing import Dict, List, Optional, Tuple, Union
 
 
 class ElasticConnection:
     def __init__(
         self,
-        username: str = None,
-        password: str = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
         host: str = "http://localhost",
         port: str = "9200",
     ):
         self.username = username
         self.password = password
         self.host = host
         self.port = port
 
     @property
-    def http_auth(self):
+    def http_auth(self) -> Union[Tuple[str, str], None]:
         http_auth = None
         if self.username and self.password:
             http_auth = (self.username, self.password)
         return http_auth
 
     @staticmethod
-    def create(username: str, password: str, host: str, port: str):
+    def create(
+        username: str, password: str, host: str, port: str
+    ) -> "ElasticConnection":
         return ElasticConnection(username, password, host, port)
 
     @staticmethod
-    def create_local():
+    def create_local() -> "ElasticConnection":
         return ElasticConnection(host="http://localhost")
 
     @staticmethod
-    def from_environ():
+    def from_environ() -> "ElasticConnection":
         return ElasticConnection.create(
             os.getenv("ELASTIC_USERNAME", ""),
             os.getenv("ELASTIC_PASSWORD", ""),
             os.getenv("ELASTIC_HOST", "http://localhost"),
             os.getenv("ELASTIC_PORT", "9200"),
         )
 
-    def to_elastic_format(self):
+    def to_elastic_format(self) -> Union[List[str], List[Dict[str, str]]]:
         if self.host.startswith("http"):
             return [f"{self.host}:{self.port}"]
         else:
             return [{"host": self.host, "port": self.port}]
```

### Comparing `petisco-1.9.9/petisco/extra/elastic/elastic_database.py` & `petisco-2.0.0rc0/petisco/extra/elastic/legacy_elastic_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import Callable, List
+from typing import Any, Callable, List
 
-from petisco.base.domain.persistence.interface_database import Database
+from petisco.base.domain.persistence.legacy_database import LegacyDatabase
 from petisco.extra.elastic.elastic_connection import ElasticConnection
-from petisco.extra.elastic.elastic_session_scope_provider import (
-    elastic_session_scope_provider,
-)
+from petisco.extra.elastic.elastic_database import elastic_session_scope_provider
 
 
-class ElasticDatabase(Database):
+class LegacyElasticDatabase(LegacyDatabase):
     @staticmethod
-    def local_connection_checker():
-        return ElasticDatabase(name="test", connection=ElasticConnection.create_local())
+    def local_connection_checker() -> "LegacyElasticDatabase":
+        return LegacyElasticDatabase(
+            name="test", connection=ElasticConnection.create_local()
+        )
 
-    def __init__(self, name: str, connection: ElasticConnection):
+    def __init__(self, name: str, connection: ElasticConnection) -> None:
         if not connection or not isinstance(connection, ElasticConnection):
             raise ConnectionError(
                 "ElasticDatabase needs a valid ElasticConnection connection"
             )
         self.connection = connection
         super().__init__(name)
 
-    def create(self):
+    def create(self) -> None:
         from elasticsearch import Elasticsearch
 
         self.session = Elasticsearch(
             self.connection.to_elastic_format(), http_auth=self.connection.http_auth
         )
 
-    def delete(self):
+    def delete(self) -> None:
         pass
 
-    def clear_data(self):
+    def clear_data(self) -> None:
         pass
 
-    def is_available(self):
+    def is_available(self) -> bool:
         try:
             return self.get_session().ping()
         except Exception:  # noqa E722
             return False
 
-    def get_base(self):
+    def get_base(self) -> None:
         return None
 
-    def get_model(self, model_name: str):
+    def get_model(self, model_name: str) -> Any:
         return None
 
     def get_model_names(self) -> List[str]:
-        return None
+        return []
 
-    def get_session(self):
+    def get_session(self) -> Any:
         return self.session
 
     def get_session_scope(self) -> Callable:
         return elastic_session_scope_provider(self.get_session())
```

### Comparing `petisco-1.9.9/petisco/extra/elastic/elastic_is_running_locally.py` & `petisco-2.0.0rc0/petisco/extra/elastic/elastic_is_running_locally.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from petisco.base.domain.persistence.persistence import Persistence
-from petisco.extra.elastic.elastic_database import ElasticDatabase
+from petisco.extra.elastic.legacy_elastic_database import LegacyElasticDatabase
 
 
 def elastic_is_running_locally() -> bool:
     try:
-        database = ElasticDatabase.local_connection_checker()
+        database = LegacyElasticDatabase.local_connection_checker()
         Persistence().add(database)
         Persistence().create()
         is_running_locally = Persistence.is_available(database.name)
     except:  # noqa: E722
         is_running_locally = False
     Persistence().remove("test", skip_if_not_exist=True)
     return is_running_locally
```

### Comparing `petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_controller.py` & `petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from abc import abstractmethod
-from typing import Any
+from typing import Any, Dict
 
-from meiga import Error, NotImplementedMethodError, Result
+from meiga import AnyResult, NotImplementedMethodError
 
 from petisco.base.application.controller.controller import Controller
+from petisco.base.misc.result_mapper import ResultMapper
 from petisco.extra.fastapi.controller.fastapi_result_mapper import FastAPIResultMapper
 
 
 class FastAPIController(Controller):
     @staticmethod
-    def get_default_mapper():
+    def get_default_mapper() -> ResultMapper:
         return FastAPIResultMapper.default()
 
     @staticmethod
-    def get_config_mapper(config):
+    def get_config_mapper(config: Dict[str, Any]) -> ResultMapper:
         return FastAPIResultMapper.from_config(config)
 
     @abstractmethod
-    def execute(self, *args, **kwargs) -> Result[Any, Error]:
+    def execute(self, *args: Any, **kwargs: Any) -> AnyResult:
         return NotImplementedMethodError
```

### Comparing `petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_failure_handler.py` & `petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_failure_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from typing import NoReturn
+
 import elasticapm
 from fastapi import HTTPException
 from loguru import logger
-from meiga import Result
+from meiga import AnyResult
 
 from petisco import DEFAULT_HTTP_ERROR_MAP
 from petisco.base.application.controller.error_map import ErrorMap
 from petisco.base.application.controller.http_error import (
     DEFAULT_HTTP_ERROR_DETAIL,
     HttpError,
 )
 from petisco.base.domain.errors.domain_error import DomainError
 from petisco.base.domain.errors.unknown_error import UnknownError
 
 
-def fastapi_failure_handler(result: Result, error_map: ErrorMap):
+def fastapi_failure_handler(result: AnyResult, error_map: ErrorMap) -> NoReturn:
     domain_error = result.value
     error_type = type(domain_error)
     http_error = error_map.get(error_type, HttpError())
 
     elasticapm.set_custom_context({"http_response": str(http_error)})
 
     internal_error_message = None
@@ -43,14 +45,15 @@
         )
     else:
         logger.warning(
             f"fastapi_failure_handler: {domain_error.__class__.__name__} is not a DomainError (warning "
             f"mapping error)"
         )
 
+    assert isinstance(http_error.status_code, int)
     http_exception = HTTPException(
         status_code=http_error.status_code, detail=detail, headers=http_error.headers
     )
 
     if (
         isinstance(domain_error, DomainError)
         and type(domain_error) not in DEFAULT_HTTP_ERROR_MAP.keys()
```

### Comparing `petisco-1.9.9/petisco/extra/fastapi/controller/fastapi_result_mapper.py` & `petisco-2.0.0rc0/petisco/extra/fastapi/controller/fastapi_result_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+from typing import Any, Dict
+
 from petisco.base.domain.errors.default_http_error_map import DEFAULT_HTTP_ERROR_MAP
 from petisco.base.misc.result_mapper import ResultMapper
 from petisco.extra.fastapi.controller.fastapi_failure_handler import (
     fastapi_failure_handler,
 )
 from petisco.extra.fastapi.controller.fastapi_success_handler import (
     fastapi_success_handler,
 )
 
 
 class FastAPIResultMapper:
     @staticmethod
-    def default():
+    def default() -> ResultMapper:
         return ResultMapper(
             error_map=DEFAULT_HTTP_ERROR_MAP,
             success_handler=fastapi_success_handler,
             failure_handler=fastapi_failure_handler,
         )
 
     @staticmethod
-    def from_config(config):
+    def from_config(config: Dict[str, Any]) -> ResultMapper:
         error_map = getattr(config, "error_map", DEFAULT_HTTP_ERROR_MAP)
         error_map = {**DEFAULT_HTTP_ERROR_MAP, **error_map}
         return ResultMapper(
             error_map=error_map,
             success_handler=getattr(config, "success_handler", fastapi_success_handler),
-            failure_handler=fastapi_failure_handler,
+            failure_handler=getattr(config, "failure_handler", fastapi_failure_handler),
         )
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/__init__.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import random
 from time import sleep
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from pika.adapters.blocking_connection import BlockingChannel
 from pika.spec import Basic
 
 from petisco.base.domain.message.chaos.message_chaos import MessageChaos
 
 MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK_KEY = "MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK"
@@ -40,59 +40,67 @@
             Routing keys where chaos will not be applied
         """
         self._set_percentage_simulate_nack(percentage_simulate_nack)
         self._set_delay_before_even_handler_second(delay_before_event_handler_second)
         self._set_percentage_simulate_failures(percentage_simulate_failures)
         self._set_protected_routing_keys(protected_routing_keys)
 
-    def _set_percentage_simulate_nack(self, percentage_simulate_nack):
+    def _set_percentage_simulate_nack(
+        self, percentage_simulate_nack: Optional[Union[float, str]]
+    ) -> None:
         if percentage_simulate_nack is None:
             percentage_simulate_nack = os.environ.get(
                 MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK_KEY
             )
         self.percentage_simulate_nack = self._float(percentage_simulate_nack)
 
-    def _set_delay_before_even_handler_second(self, delay_before_even_handler_second):
+    def _set_delay_before_even_handler_second(
+        self, delay_before_even_handler_second: Optional[Union[float, str]]
+    ) -> None:
         if delay_before_even_handler_second is None:
             delay_before_even_handler_second = os.environ.get(
                 MESSAGE_CHAOS_DELAY_BEFORE_EVENT_HANDLER_SECONDS_KEY
             )
         self.delay_before_even_handler_second = self._float(
             delay_before_even_handler_second
         )
 
-    def _set_percentage_simulate_failures(self, percentage_simulate_failures):
+    def _set_percentage_simulate_failures(
+        self, percentage_simulate_failures: Optional[Union[float, str]]
+    ) -> None:
         if percentage_simulate_failures is None:
             percentage_simulate_failures = os.environ.get(
                 MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES_KEY
             )
         self.percentage_simulate_failures = self._float(percentage_simulate_failures)
 
-    def _set_protected_routing_keys(self, protected_routing_keys):
+    def _set_protected_routing_keys(
+        self, protected_routing_keys: Optional[Union[List[str], str]]
+    ) -> None:
         if protected_routing_keys is None:
             protected_routing_keys = os.environ.get(
                 MESSAGE_CHAOS_PROTECTED_ROUTING_KEYS_KEY
             )
         self.protected_routing_keys = self._list(protected_routing_keys)
 
-    def _float(self, value):
+    def _float(self, value: Optional[Union[float, str]]) -> Union[float, None]:
         return float(value) if value is not None else None
 
-    def _list(self, value):
+    def _list(self, value: Optional[Union[List[str], str]]) -> Union[List[str], None]:
         if value is None:
             return None
 
         if isinstance(value, str):
             value = list(value.split(","))
         return value
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"RabbitMqEventChaos: {self.info()}"
 
-    def info(self) -> Dict:
+    def info(self) -> Dict[str, Any]:
         return {
             MESSAGE_CHAOS_PERCENTAGE_SIMULATE_NACK_KEY: self.percentage_simulate_nack,
             MESSAGE_CHAOS_DELAY_BEFORE_EVENT_HANDLER_SECONDS_KEY: self.delay_before_even_handler_second,
             MESSAGE_CHAOS_PERCENTAGE_SIMULATE_FAILURES_KEY: self.percentage_simulate_failures,
             MESSAGE_CHAOS_PROTECTED_ROUTING_KEYS_KEY: self.protected_routing_keys,
         }
 
@@ -124,12 +132,12 @@
             return (
                 True
                 if self.protected_routing_keys is None
                 or routing_key not in self.protected_routing_keys
                 else False
             )
 
-    def delay(self):
+    def delay(self) -> None:
         if self.delay_before_even_handler_second is None:
             pass
         else:
             sleep(self.delay_before_even_handler_second)
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,86 @@
-from typing import List
+from typing import List, Union
 
 from petisco.base.domain.message.message_configurer import MessageConfigurer
 from petisco.base.domain.message.message_subscriber import MessageSubscriber
 from petisco.extra.rabbitmq.application.message.configurer.rabbitmq_message_store_configurer import (
     RabbitMqMessageStoreConfigurer,
 )
 from petisco.extra.rabbitmq.application.message.configurer.rabbitmq_message_subscribers_configurer import (
     RabbitMqMessageSubcribersConfigurer,
 )
+from petisco.extra.rabbitmq.application.message.consumer.rabbitmq_consumer_connector import (
+    RabbitMqConsumerConnector,
+)
 from petisco.extra.rabbitmq.shared.queue_config import QueueConfig
 from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 
 
 class RabbitMqMessageConfigurer(MessageConfigurer):
+    """
+    A class to configure RabbitMQ infrastructure.
+    This class configures exchanges, queue bindings and routing keys from defined MessageSubscribers.
+    """
+
     def __init__(
         self,
         organization: str,
         service: str,
-        connector: RabbitMqConnector = RabbitMqConnector(),
+        connector: Union[
+            RabbitMqConnector, RabbitMqConsumerConnector
+        ] = RabbitMqConnector(),
         queue_config: QueueConfig = QueueConfig.default(),
         use_store_queues: bool = True,
-    ):
+    ) -> None:
         self._use_store_queues = use_store_queues
         self.subscribers_configurer = RabbitMqMessageSubcribersConfigurer(
             organization, service, connector, queue_config
         )
         self.store_configurer = RabbitMqMessageStoreConfigurer(
             organization, service, connector, queue_config
         )
 
-    def configure(self):
+    def configure(self) -> None:
+        """
+        Define exchanges, queue bindings and routing key with empty subscribers.
+        """
         self.configure_subscribers([])
 
     def configure_subscribers(
         self,
         subscribers: List[MessageSubscriber],
         clear_subscriber_before: bool = False,
         clear_store_before: bool = False,
-    ):
+    ) -> None:
+        """
+        Define exchanges, queue bindings and routing keys from given subscribers.
+        """
         if subscribers is None:
             subscribers = []
 
         if clear_subscriber_before:
             self.subscribers_configurer.clear_subscribers(subscribers)
         if clear_store_before and self._use_store_queues:
             self.store_configurer.clear()
 
         self.subscribers_configurer.execute(subscribers)
         if self._use_store_queues:
             self.store_configurer.execute()
 
-    def clear_subscribers(self, subscribers: List[MessageSubscriber]):
+    def clear_subscribers(self, subscribers: List[MessageSubscriber]) -> None:
+        """
+        Clear configured subscribers.
+        """
         if subscribers is None:
             subscribers = []
 
         self.subscribers_configurer.clear_subscribers(subscribers)
         if self._use_store_queues:
             self.store_configurer.clear()
 
-    def clear(self):
+    def clear(self) -> None:
+        """
+        Clear all configured subscribers and store configuration.
+        """
         self.subscribers_configurer.clear()
         if self._use_store_queues:
             self.store_configurer.clear()
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from typing import Union
+
+from petisco.extra.rabbitmq.application.message.consumer.rabbitmq_consumer_connector import (
+    RabbitMqConsumerConnector,
+)
 from petisco.extra.rabbitmq.shared.queue_config import QueueConfig
 from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 from petisco.extra.rabbitmq.shared.rabbitmq_declarer import RabbitMqDeclarer
 from petisco.extra.rabbitmq.shared.rabbitmq_exchange_name_formatter import (
     RabbitMqExchangeNameFormatter,
 )
 
 
 class RabbitMqMessageStoreConfigurer:
     def __init__(
         self,
         organization: str,
         service: str,
-        connector: RabbitMqConnector,
+        connector: Union[RabbitMqConnector, RabbitMqConsumerConnector],
         queue_config: QueueConfig,
-    ):
+    ) -> None:
         self._connector = connector
         self._exchange_name = f"{organization}.{service}"
         self._retry_exchange_name = RabbitMqExchangeNameFormatter.retry(
             self._exchange_name
         )
         self._dead_letter_exchange_name = RabbitMqExchangeNameFormatter.dead_letter(
             self._exchange_name
@@ -26,51 +31,51 @@
         self._common_dead_letter_exchange_name = f"dead_letter.{organization}.store"
 
         self.rabbitmq = RabbitMqDeclarer(
             connector=self._connector, channel_name=self._exchange_name
         )
         self.queue_config = queue_config
 
-    def execute(self):
+    def execute(self) -> None:
         self._configure_exchanges()
         self._declare_queues(
             self._exchange_name,
             self._retry_exchange_name,
             self._dead_letter_exchange_name,
         )
 
-    def clear(self):
+    def clear(self) -> None:
         self._delete_exchange()
         self._delete_queues()
 
-    def _configure_exchanges(self):
+    def _configure_exchanges(self) -> None:
         self.rabbitmq.declare_exchange(self._exchange_name)
         self.rabbitmq.declare_exchange(self._retry_exchange_name)
         self.rabbitmq.declare_exchange(self._dead_letter_exchange_name)
         self.rabbitmq.declare_exchange(self._common_retry_exchange_name)
         self.rabbitmq.declare_exchange(self._common_dead_letter_exchange_name)
 
-    def _delete_exchange(self):
+    def _delete_exchange(self) -> None:
         self.rabbitmq.delete_exchange(self._exchange_name)
         self.rabbitmq.delete_exchange(self._retry_exchange_name)
         self.rabbitmq.delete_exchange(self._dead_letter_exchange_name)
         self.rabbitmq.delete_exchange(self._common_retry_exchange_name)
         self.rabbitmq.delete_exchange(self._common_dead_letter_exchange_name)
 
-    def _delete_queues(self):
+    def _delete_queues(self) -> None:
         self.rabbitmq.delete_queue("store")
         self.rabbitmq.delete_queue("retry.store")
         self.rabbitmq.delete_queue("dead_letter.store")
 
     def _declare_queues(
         self,
         exchange_name: str,
         retry_exchange_name: str,
         dead_letter_exchange_name: str,
-    ):
+    ) -> None:
         self.rabbitmq.declare_queue(
             queue_name="store",
             dead_letter_exchange=self._common_dead_letter_exchange_name,
             dead_letter_routing_key="dead_letter.store",
             message_ttl=self.queue_config.get_main_ttl("store"),
         )
         self.rabbitmq.declare_queue(
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from typing import List, Type
+from typing import Any, List, Type, Union
 
 from petisco.base.domain.message.message_subscriber import MessageSubscriber
+from petisco.extra.rabbitmq.application.message.consumer.rabbitmq_consumer_connector import (
+    RabbitMqConsumerConnector,
+)
 from petisco.extra.rabbitmq.application.message.formatter.rabbitmq_message_subscriber_queue_name_formatter import (
     RabbitMqMessageSubscriberQueueNameFormatter,
 )
 from petisco.extra.rabbitmq.shared.queue_config import QueueConfig
 from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 from petisco.extra.rabbitmq.shared.rabbitmq_declarer import RabbitMqDeclarer
 from petisco.extra.rabbitmq.shared.rabbitmq_exchange_name_formatter import (
@@ -13,60 +16,60 @@
 
 
 class RabbitMqMessageSubcribersConfigurer:
     def __init__(
         self,
         organization: str,
         service: str,
-        connector: RabbitMqConnector,
+        connector: Union[RabbitMqConnector, RabbitMqConsumerConnector],
         queue_config: QueueConfig,
-    ):
+    ) -> None:
         self._connector = connector
         self._exchange_name = f"{organization}.{service}"
         self._retry_exchange_name = RabbitMqExchangeNameFormatter.retry(
             self._exchange_name
         )
         self._dead_letter_exchange_name = RabbitMqExchangeNameFormatter.dead_letter(
             self._exchange_name
         )
         self.rabbitmq = RabbitMqDeclarer(
             connector=self._connector, channel_name=self._exchange_name
         )
-        self._configured_subscribers = []
+        self._configured_subscribers: List[Any] = []
         self.queue_config = queue_config
 
-    def execute(self, subscribers):
+    def execute(self, subscribers) -> None:
         self._configure_exchanges()
         self._declare_queues(
             self._exchange_name,
             self._retry_exchange_name,
             self._dead_letter_exchange_name,
             subscribers,
         )
         self._configured_subscribers += subscribers
 
-    def clear_subscribers(self, subscribers):
+    def clear_subscribers(self, subscribers) -> None:
         self._configured_subscribers += subscribers
         self.clear()
 
-    def clear(self):
+    def clear(self) -> None:
         self._delete_exchange()
         self._delete_queues()
 
-    def _configure_exchanges(self):
+    def _configure_exchanges(self) -> None:
         self.rabbitmq.declare_exchange(self._exchange_name)
         self.rabbitmq.declare_exchange(self._retry_exchange_name)
         self.rabbitmq.declare_exchange(self._dead_letter_exchange_name)
 
-    def _delete_exchange(self):
+    def _delete_exchange(self) -> None:
         self.rabbitmq.delete_exchange(self._exchange_name)
         self.rabbitmq.delete_exchange(self._retry_exchange_name)
         self.rabbitmq.delete_exchange(self._dead_letter_exchange_name)
 
-    def _delete_queues(self):
+    def _delete_queues(self) -> None:
         for SubscriberClass in self._configured_subscribers:
 
             subscriber = SubscriberClass()
             for subscriber_info in subscriber.get_message_subscribers_info():
 
                 if subscriber_info.message_type == "message":
                     # if subscriber_info is subscribed to message it will be consuming from store queue
@@ -96,15 +99,15 @@
 
     def _declare_queues(
         self,
         exchange_name: str,
         retry_exchange_name: str,
         dead_letter_exchange_name: str,
         subscribers: List[Type[MessageSubscriber]],
-    ):
+    ) -> None:
 
         for SubscriberClass in subscribers:
             subscriber = SubscriberClass()
             for subscriber_info in subscriber.get_message_subscribers_info():
                 if subscriber_info.message_type == "message":
                     # if subscriber_info is subscribed to message it will be consuming from store queue
                     break
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from typing import Callable, Optional
+from typing import Any, Callable, Optional
 
-from meiga import Result
+from meiga import AnyResult
 from pika import BasicProperties
 from pika.spec import Basic
 
 from petisco.base.domain.message.consumer_derived_action import ConsumerDerivedAction
-from petisco.legacy.logger.interface_logger import DEBUG, ILogger
-from petisco.legacy.logger.log_message import LogMessage
-from petisco.legacy.logger.not_implemented_logger import NotImplementedLogger
+from petisco.extra.logger.log_message import LogMessage
+from petisco.extra.logger.logger import DEBUG, Logger
+from petisco.extra.logger.not_implemented_logger import NotImplementedLogger
 
 
 class RabbitMqMessageConsumerLogger:
-    def __init__(self, logger: Optional[ILogger] = NotImplementedLogger()):
+    def __init__(self, logger: Optional[Logger] = NotImplementedLogger()) -> None:
         self.logger = logger
 
-    def _get_base_message(self, handler: Callable):
+    def _get_base_message(self, handler: Callable[..., Any]) -> LogMessage:
         return LogMessage(
             layer="rabbitmq_message_consumer", operation=f"{handler.__name__}"
         )
 
-    def _get_event_handler_name(self, handler: Callable):
+    def _get_event_handler_name(self, handler: Callable[..., Any]) -> str:
         handler_name = getattr(handler, "__name__", repr(handler))
         handler_module = getattr(handler, "__module__") + "."
         return f"{handler_module}{handler_name}"
 
     def log_nack_simulation(
         self,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
-        handler: Callable,
-    ):
+        handler: Callable[..., Any],
+    ) -> None:
         self._log_simulation(method, properties, body, handler, "nack simulated")
 
     def log_failure_simulation(
         self,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
-        handler: Callable,
-    ):
+        handler: Callable[..., Any],
+    ) -> None:
         self._log_simulation(method, properties, body, handler, "failure simulated")
 
     def _log_simulation(
         self,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
-        handler: Callable,
+        handler: Callable[..., Any],
         chaos_action: str,
-    ):
+    ) -> None:
         log_message = self._get_base_message(handler)
         event_handler_name = self._get_event_handler_name(handler)
         message = {
             "body": body,
             "properties": properties,
             "method": method,
             "event_handler": event_handler_name,
@@ -62,17 +62,17 @@
         self.logger.log(DEBUG, log_message.set_message(message))
 
     def log_parser_error(
         self,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
-        handler: Callable,
+        handler: Callable[..., Any],
         exception: Exception,
-    ):
+    ) -> None:
         log_message = self._get_base_message(handler)
         event_handler_name = self._get_event_handler_name(handler)
         message = {
             "body": body,
             "properties": properties,
             "method": method,
             "event_handler": event_handler_name,
@@ -81,19 +81,19 @@
         self.logger.log(DEBUG, log_message.set_message(message))
 
     def log(
         self,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
-        handler: Callable,
+        handler: Callable[..., Any],
         log_activity: str = None,
-        result: Result = None,
+        result: AnyResult = None,
         derived_action: ConsumerDerivedAction() = None,
-    ):
+    ) -> None:
         log_message = self._get_base_message(handler)
         event_handler_name = self._get_event_handler_name(handler)
 
         message = {
             "body": body,
             "properties": properties,
             "method": method,
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import Callable, Dict
+from typing import Any, Callable, Dict
 
-from meiga import Result
+from meiga import AnyResult
 from pika import BasicProperties
 from pika.spec import Basic
 
 
 class RabbitMqEventConsumerPrinter:
     def __init__(self, verbose: bool = False):
         self.verbose = verbose
 
     def print_received_message(
         self, method: Basic.Deliver, properties: BasicProperties, body: bytes
-    ):
+    ) -> None:
         if self.verbose:
             print(
                 "\n#####################################################################################################################"
             )
-            print(" [x] Received %r" % (body,))
-            print(" [x] Properties %r" % (properties,))
-            print(" [x] method %r" % (method,))
+            print(f" [x] Received {body!r}")
+            print(f" [x] Properties {properties!r}")
+            print(f" [x] method {method!r}")
 
-    def print_separator(self):
+    def print_separator(self) -> None:
         if self.verbose:
             print(
                 "#####################################################################################################################\n"
             )
 
-    def print_context(self, handler: Callable, result: Result):
+    def print_context(self, handler: Callable[..., Any], result: AnyResult) -> None:
         if self.verbose:
             handler_name = getattr(handler, "__name__", repr(handler))
             handler_module = getattr(handler, "__module__") + "."
 
             print(f" [x] event_handler: {handler_module}{handler_name}")
             print(f" [x] result from event_handler: {result}")
 
-    def print_action(self, action_name: str):
+    def print_action(self, action_name: str) -> None:
         if self.verbose:
             print(f" [>] {action_name}")
 
     def print_send_message_to(
-        self, exchange_name: str, routing_key: str, headers: Dict
-    ):
+        self, exchange_name: str, routing_key: str, headers: Dict[str, Any]
+    ) -> None:
         if self.verbose:
             print(f" [>] send: [{exchange_name} |{routing_key}] -> {headers}")
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import os
 import threading
 import traceback
 from dataclasses import dataclass
 from time import sleep
-from typing import Callable, List, Optional, Type
+from typing import Any, Callable, Dict, List, NoReturn, Optional, Type, Union
 
+from loguru import logger
 from meiga import Failure
 from pika import BasicProperties
 from pika.adapters.blocking_connection import BlockingChannel
+from pika.exceptions import ConnectionClosedByBroker
 from pika.spec import Basic
 
 from petisco.base.domain.message.chaos.message_chaos import MessageChaos
 from petisco.base.domain.message.chaos.message_chaos_error import MessageChaosError
 from petisco.base.domain.message.chaos.not_implemented_message_chaos import (
     NotImplementedMessageChaos,
 )
@@ -19,14 +22,16 @@
 from petisco.base.domain.message.domain_event import DomainEvent
 from petisco.base.domain.message.message import Message
 from petisco.base.domain.message.message_consumer import MessageConsumer
 from petisco.base.domain.message.message_handler_returns_none_error import (
     MessageHandlerReturnsNoneError,
 )
 from petisco.base.domain.message.message_subscriber import MessageSubscriber
+from petisco.extra.logger.logger import Logger
+from petisco.extra.logger.not_implemented_logger import NotImplementedLogger
 from petisco.extra.rabbitmq.application.message.bus.rabbitmq_command_bus import (
     RabbitMqCommandBus,
 )
 from petisco.extra.rabbitmq.application.message.bus.rabbitmq_domain_event_bus import (
     RabbitMqDomainEventBus,
 )
 from petisco.extra.rabbitmq.application.message.consumer.rabbitmq_consumer_connector import (
@@ -41,62 +46,109 @@
 from petisco.extra.rabbitmq.application.message.formatter.rabbitmq_message_subscriber_queue_name_formatter import (
     RabbitMqMessageSubscriberQueueNameFormatter,
 )
 from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 from petisco.extra.rabbitmq.shared.rabbitmq_exchange_name_formatter import (
     RabbitMqExchangeNameFormatter,
 )
-from petisco.legacy.logger.interface_logger import ILogger
-from petisco.legacy.logger.not_implemented_logger import NotImplementedLogger
+
+MAX_ATTEMPTS_TO_RECONNECT = int(
+    os.getenv("PETISCO_RABBITMQ_MAX_ATTEMPTS_TO_RECONNECT_CONSUMER", "20")
+)
+WAIT_SECONDS_TO_RECONNECT = int(
+    os.getenv("PETISCO_RABBITMQ_WAIT_SECONDS_TO_RECONNECT_CONSUMER", "5")
+)
 
 
 @dataclass
 class SubscriberItem:
     queue_name: str
     subscriber: MessageSubscriber
     consumer_tag: str
     is_store: bool = False
 
 
 class RabbitMqMessageConsumer(MessageConsumer):
+    """
+    A RabbitMQ consumer to link received messages from rabbitmq with defined subscribers.
+    """
+
     def __init__(
         self,
         organization: str,
         service: str,
         max_retries: int,
         connector: RabbitMqConnector = RabbitMqConnector(),
         verbose: bool = False,
         chaos: MessageChaos = NotImplementedMessageChaos(),
-        logger: Optional[ILogger] = NotImplementedLogger(),
-    ):
+        logger: Optional[Logger] = NotImplementedLogger(),
+        rabbitmq_key_prefix: str = "consumer",
+    ) -> None:
         self.connector = connector
         self.organization = organization
         self.service = service
         self.exchange_name = f"{organization}.{service}"
-        self.rabbitmq_key = f"consumer-{self.exchange_name}"
+        self.rabbitmq_key = f"{rabbitmq_key_prefix}-{self.exchange_name}"
         self._fallback_store_exchange_name = f"retry.{organization}.store"
         self.max_retries = max_retries
         self._channel = self.connector.get_channel(self.rabbitmq_key)
         self.printer = RabbitMqEventConsumerPrinter(verbose)
         self.consumer_logger = RabbitMqMessageConsumerLogger(logger)
         self.chaos = chaos
-        self.subscribers = {}
+        self.subscribers: Dict[str, SubscriberItem] = {}
+        self._thread: Union[threading.Thread, None] = None
 
-    def start(self):
+    def start(self) -> NoReturn:
+        """
+        Start the process of consuming messages from RabbitMQ and pass to subscriber.
+        """
         if not self._channel:
             raise RuntimeError(
                 "RabbitMqMessageConsumer: cannot start consuming event without any subscriber defined."
             )
         self._thread = threading.Thread(target=self._start)
         self._thread.start()
 
-    def _start(self):
-        self._channel.start_consuming()
+    def _start(self) -> None:
+        try:
+            self._channel.start_consuming()
+        except ConnectionClosedByBroker:
+            self._re_connect(attempt=1)
+
+    def _re_connect(self, attempt: int):
+        if attempt >= MAX_ATTEMPTS_TO_RECONNECT:
+            raise ConnectionError(
+                f"Impossible to reconnect consumer '{self.rabbitmq_key}' after {attempt} attempts"
+            )
+
+        logger.info(
+            f"Trying to reconnect consumer '{self.rabbitmq_key}' (attempt {attempt})"
+        )
+
+        try:
+            self._channel = self.connector.get_channel(self.rabbitmq_key)
+        except ConnectionError:
+            sleep(WAIT_SECONDS_TO_RECONNECT)
+            attempt += 1
+            self._re_connect(attempt=attempt)
+        else:
+            subscribers = [
+                item.subscriber.__class__ for item in self.subscribers.values()
+            ]
+            self.add_subscribers(subscribers)
+            self.start()
+            logger.info(
+                f"Consumer '{self.rabbitmq_key}' reconnected after {attempt} attempts"
+            )
+
+    def add_subscribers(self, subscribers: List[Type[MessageSubscriber]]) -> None:
+        """
+        Add defined subscribers to be connected with main queues.
+        """
 
-    def add_subscribers(self, subscribers: List[Type[MessageSubscriber]]):
         for SubscriberClass in subscribers:
 
             subscriber: MessageSubscriber = SubscriberClass()
 
             for subscriber_info in subscriber.get_message_subscribers_info():
 
                 if subscriber_info.message_type == "message":
@@ -109,37 +161,39 @@
                     )
                     self._add_subscriber_instance_on_queue(
                         queue_name=f"{queue_name}.{subscriber.get_subscriber_name()}",
                         subscriber=subscriber,
                         message_type_expected=subscriber_info.message_type,
                     )
 
-    def add_subscriber_on_dead_letter(self, subscriber: Type[MessageSubscriber]):
+    def add_subscriber_on_dead_letter(
+        self, subscriber: Type[MessageSubscriber]
+    ) -> None:
+        """
+        Add defined subscribers to be connected with the correspondent dead letter.
+        """
         instance_subscriber: MessageSubscriber = subscriber()
         for subscriber_info in instance_subscriber.get_message_subscribers_info():
 
             queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format_dead_letter(
                 subscriber_info, exchange_name=self.exchange_name
             )
             self._add_subscriber_instance_on_queue(
                 queue_name=f"{queue_name}.{instance_subscriber.get_subscriber_name()}",
                 subscriber=instance_subscriber,
                 message_type_expected=subscriber_info.message_type,
             )
 
-    # def add_handler_on_store(self, handler: Callable):
-    #     self.add_handler_on_queue("store", handler, is_store=True)
-
     def _add_subscriber_instance_on_queue(
         self,
         queue_name: str,
         subscriber: MessageSubscriber,
         is_store: bool = False,
         message_type_expected: str = "message",
-    ):
+    ) -> None:
         consumer_tag = self._channel.basic_consume(
             queue=queue_name,
             on_message_callback=self.consumer(
                 subscriber, is_store, message_type_expected
             ),
         )
         self.subscribers[queue_name] = SubscriberItem(
@@ -148,35 +202,38 @@
 
     def add_subscriber_on_queue(
         self,
         queue_name: str,
         subscriber: Type[MessageSubscriber],
         is_store: bool = False,
         message_type_expected: str = "message",
-    ):
-        subscriber: MessageSubscriber = subscriber()
-        return self._add_subscriber_instance_on_queue(
+    ) -> None:
+        """
+        Add defined subscribers to be connected with a specific queue name.
+        """
+        subscriber_instance: MessageSubscriber = subscriber()
+        self._add_subscriber_instance_on_queue(
             queue_name=queue_name,
-            subscriber=subscriber,
+            subscriber=subscriber_instance,
             is_store=is_store,
             message_type_expected=message_type_expected,
         )
 
     def consumer(
         self,
         subscriber: MessageSubscriber,
         is_store: bool = False,
         message_type_expected: str = "message",
-    ) -> Callable:
+    ) -> Callable[..., None]:
         def rabbitmq_consumer(
             ch: BlockingChannel,
             method: Basic.Deliver,
             properties: BasicProperties,
             body: bytes,
-        ):
+        ) -> None:
             self.printer.print_received_message(method, properties, body)
 
             if self.chaos.nack_simulation(ch, method):
                 self.consumer_logger.log_nack_simulation(
                     method, properties, body, subscriber.handle
                 )
                 return
@@ -255,34 +312,35 @@
     def handle_consumption_error(
         self,
         ch: BlockingChannel,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
         is_store: bool,
-    ):
+    ) -> ConsumerDerivedAction:
 
         if self.has_been_redelivered_too_much(properties):
             derived_action = self.send_to_dead_letter(ch, method, properties, body)
         else:
             derived_action = self.send_to_retry(ch, method, properties, body, is_store)
 
         ch.basic_ack(delivery_tag=method.delivery_tag)
 
         return derived_action
 
-    def has_been_redelivered_too_much(self, properties: BasicProperties):
+    def has_been_redelivered_too_much(self, properties: BasicProperties) -> bool:
         if not properties.headers or "redelivery_count" not in properties.headers:
             if self.max_retries < 1:
                 return True
             return False
         else:
-            return properties.headers.get("redelivery_count") >= self.max_retries
+            redelivery_count: int = properties.headers.get("redelivery_count")
+            return bool(redelivery_count >= self.max_retries)
 
-    def _get_routing_key(self, routing_key: str, prefix: str):
+    def _get_routing_key(self, routing_key: str, prefix: str) -> str:
         if routing_key.startswith("retry."):
             routing_key = routing_key.replace("retry.", prefix, 1)
         elif routing_key.startswith("dead_letter."):
             routing_key = routing_key.replace("dead_letter.", prefix, 1)
         else:
             routing_key = f"{prefix}{routing_key}"
         return routing_key
@@ -290,26 +348,27 @@
     def send_to_retry(
         self,
         ch: BlockingChannel,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
         is_store: bool = False,
-    ):
+    ) -> ConsumerDerivedAction:
         self.printer.print_action("send_to_retry")
         exchange_name = RabbitMqExchangeNameFormatter.retry(self.exchange_name)
 
         routing_key = method.routing_key
         if properties.headers:
             routing_key = properties.headers.get("queue", routing_key)
 
         if is_store:
             routing_key = "store"
             exchange_name = self._fallback_store_exchange_name
 
+        assert isinstance(routing_key, str)
         routing_key = self._get_routing_key(routing_key, "retry.")
 
         updated_headers = self.send_message_to(
             exchange_name, ch, routing_key, properties, body
         )
         return ConsumerDerivedAction(
             action="send_to_retry",
@@ -320,17 +379,18 @@
 
     def send_to_dead_letter(
         self,
         ch: BlockingChannel,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
-    ):
+    ) -> ConsumerDerivedAction:
         self.printer.print_action("send_to_dead_letter")
         exchange_name = RabbitMqExchangeNameFormatter.dead_letter(self.exchange_name)
+        assert isinstance(method.routing_key, str)
         routing_key = self._get_routing_key(method.routing_key, "dead_letter.")
         updated_headers = self.send_message_to(
             exchange_name, ch, routing_key, properties, body
         )
         return ConsumerDerivedAction(
             action="send_to_dead_letter",
             exchange_name=exchange_name,
@@ -341,105 +401,105 @@
     def send_message_to(
         self,
         exchange_name: str,
         ch: BlockingChannel,
         routing_key: str,
         properties: BasicProperties,
         body: bytes,
-    ):
+    ) -> Dict[str, Any]:
         if properties.headers:
             redelivery_count = properties.headers.get("redelivery_count", 0)
             properties.headers["redelivery_count"] = redelivery_count + 1
         else:
             properties.headers = {"redelivery_count": 1}
 
         self.printer.print_send_message_to(
-            exchange_name, routing_key, properties.headers
+            exchange_name, routing_key, dict(properties.headers)
         )
 
         ch.basic_publish(
             exchange=exchange_name,
             routing_key=routing_key,
             body=body,
             properties=properties,
         )
 
-        return properties.headers
+        return dict(properties.headers)
 
-    def stop(self):
-        def _log_stop_exception(e: Exception):
-            from petisco.legacy import ERROR, LogMessage, Petisco
-
-            logger = Petisco.get_logger()
-            log_message = LogMessage(
-                layer="petisco", operation="RabbitMQEventSubscriber"
-            )
-            message = f"Error stopping RabbitMQEventSubscriber: {repr(e.__class__)} {e} | {traceback.format_exc()}"
-            logger.log(ERROR, log_message.set_message(message))
+    def stop(self) -> None:
+        """
+        Stop the process of consuming messages from RabbitMQ.
+        """
+
+        def _log_stop_exception(e: Exception) -> None:
+            message = f"Error stopping RabbitMQMessageConsumer: {repr(e.__class__)} {e} | {traceback.format_exc()}"
+            logger.error(message)
 
         if self._thread and self._thread.is_alive():
             self._unsubscribe_all()
             try:
                 self._thread.join()
                 self._thread = None
             except Exception as e:
                 _log_stop_exception(e)
 
-    def _unsubscribe_all(self):
-        def _stop_consuming_consumer_channel():
+    def _unsubscribe_all(self) -> None:
+        def _stop_consuming_consumer_channel() -> None:
             try:
                 self._channel.stop_consuming()
                 self._channel.cancel()
             except ValueError:
                 pass
 
-        def _await_for_stop_consuming_consumer_channel():
+        def _await_for_stop_consuming_consumer_channel() -> None:
             sleep(2.0)
 
         self.connector.get_connection(self.rabbitmq_key).call_later(
             0, _stop_consuming_consumer_channel
         )
 
         _await_for_stop_consuming_consumer_channel()
 
-    def unsubscribe_subscriber_on_queue(self, queue_name: str):
-        subscriber_item: SubscriberItem = self.subscribers.get(queue_name)
+    def unsubscribe_subscriber_on_queue(self, queue_name: str) -> None:
+        subscriber_item = self.subscribers.get(queue_name)
         if subscriber_item is None:
             raise IndexError(
                 f"Cannot unsubscribe an nonexistent queue ({queue_name}). Please, check configured consumers ({list(self.subscribers.keys())})"
             )
 
-        def _unsubscribe_handler_on_queue():
+        def _unsubscribe_handler_on_queue() -> None:
+            assert isinstance(subscriber_item, SubscriberItem)
             self._channel.basic_cancel(consumer_tag=subscriber_item.consumer_tag)
 
         self._do_it_in_consumer_thread(_unsubscribe_handler_on_queue)
 
-    def resume_subscriber_on_queue(self, queue_name: str):
-        subscriber_item: SubscriberItem = self.subscribers.get(queue_name)
+    def resume_subscriber_on_queue(self, queue_name: str) -> None:
+        subscriber_item = self.subscribers.get(queue_name)
         if subscriber_item is None:
             raise IndexError(
                 f"Cannot resume an nonexistent queue ({queue_name}). Please, check configured consumers ({list(self.subscribers.keys())})"
             )
 
-        def _resume_handler_on_queue():
+        def _resume_handler_on_queue() -> None:
+            assert isinstance(subscriber_item, SubscriberItem)
             subscriber_item.consumer_tag = self._channel.basic_consume(
                 queue=subscriber_item.queue_name,
                 on_message_callback=self.consumer(
                     subscriber_item.subscriber, subscriber_item.is_store
                 ),
             )
 
         self._do_it_in_consumer_thread(_resume_handler_on_queue)
 
-    def _do_it_in_consumer_thread(self, action: Callable):
-        def _execute_action():
+    def _do_it_in_consumer_thread(self, action: Callable[..., None]) -> None:
+        def _execute_action() -> None:
             try:
                 action()
             except ValueError:
                 pass
 
-        def _await_for_thread():
+        def _await_for_thread() -> None:
             sleep(2.0)
 
         self.connector.get_connection(self.rabbitmq_key).call_later(0, _execute_action)
 
         _await_for_thread()
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,35 @@
+from typing import Union
+
+from pika import BasicProperties
+from pika.adapters.blocking_connection import BlockingChannel
+
 from petisco.base.domain.message.message import Message
+from petisco.extra.rabbitmq.application.message.formatter.rabbitmq_message_queue_name_formatter import (
+    RabbitMqMessageQueueNameFormatter,
+)
+
+
+class RabbitMqMessagePublisher:
+    def __init__(self, exchange_name: str) -> None:
+        self._exchange_name = exchange_name
+        self._properties = BasicProperties(delivery_mode=2)  # PERSISTENT_TEXT_PLAIN
+
+    def execute(
+        self,
+        channel: BlockingChannel,
+        message: Message,
+        routing_key: Union[str, None] = None,
+    ) -> None:
 
+        if routing_key is None:
+            routing_key = RabbitMqMessageQueueNameFormatter.format(
+                message, exchange_name=self._exchange_name
+            )
 
-class RabbitMqMessageQueueNameFormatter:
-    @staticmethod
-    def format(message: Message, exchange_name: str = None) -> str:
-        message_name = message.name.replace(".", "_")
-        message_type = message.type if message.type != "domain_event" else "event"
-        message_format = f"{message.version}.{message_type}.{message_name}"
-        return f"{exchange_name}.{message_format}" if exchange_name else message_name
-
-    @staticmethod
-    def format_retry(message: Message, exchange_name: str = None) -> str:
-        queue_name = RabbitMqMessageQueueNameFormatter.format(message, exchange_name)
-        return f"retry.{queue_name}"
-
-    @staticmethod
-    def format_dead_letter(message: Message, exchange_name: str = None) -> str:
-        queue_name = RabbitMqMessageQueueNameFormatter.format(message, exchange_name)
-        return f"dead_letter.{queue_name}"
+        channel.confirm_delivery()
+        channel.basic_publish(
+            exchange=self._exchange_name,
+            routing_key=routing_key,
+            body=message.json().encode(),
+            properties=self._properties,
+        )
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/dependencies.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/dependencies.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import List
 
 from petisco.base.application.dependency_injection.dependency import Dependency
+from petisco.base.domain.message.command_bus import CommandBus
+from petisco.base.domain.message.domain_event_bus import DomainEventBus
+from petisco.base.domain.message.message_configurer import MessageConfigurer
+from petisco.base.domain.message.message_consumer import MessageConsumer
 from petisco.base.domain.message.not_implemented_command_bus import (
     NotImplementedCommandBus,
 )
 from petisco.base.domain.message.not_implemented_domain_event_bus import (
     NotImplementedDomainEventBus,
 )
 from petisco.base.domain.message.not_implemented_message_comsumer import (
@@ -16,31 +20,31 @@
 from petisco.base.misc.builder import Builder
 
 
 def get_default_message_dependencies() -> List[Dependency]:
 
     return [
         Dependency(
-            name="domain_event_bus",
-            default_builder=Builder(NotImplementedDomainEventBus),
+            DomainEventBus,
+            builders={"default": Builder(NotImplementedDomainEventBus)},
             envar_modifier="PETISCO_DOMAIN_EVENT_BUS_TYPE",
         ),
         Dependency(
-            name="command_bus",
-            default_builder=Builder(NotImplementedCommandBus),
+            CommandBus,
+            builders={"default": Builder(NotImplementedCommandBus)},
             envar_modifier="PETISCO_COMMAND_BUS_TYPE",
         ),
         Dependency(
-            name="message_configurer",
-            default_builder=Builder(NotImplementedMessageConfigurer),
+            MessageConfigurer,
+            builders={"default": Builder(NotImplementedMessageConfigurer)},
             envar_modifier="PETISCO_MESSAGE_CONFIGURER_TYPE",
         ),
         Dependency(
-            name="message_consumer",
-            default_builder=Builder(NotImplementedMessageConsumer),
+            MessageConsumer,
+            builders={"default": Builder(NotImplementedMessageConsumer)},
             envar_modifier="PETISCO_MESSAGE_CONSUMER_TYPE",
         ),
     ]
 
 
 def get_rabbitmq_message_dependencies(
     organization: str, service: str, max_retries: int = 5
@@ -56,44 +60,52 @@
     )
     from petisco.extra.rabbitmq.application.message.consumer.rabbitmq_message_consumer import (
         RabbitMqMessageConsumer,
     )
 
     return [
         Dependency(
-            name="domain_event_bus",
-            default_builder=Builder(
-                RabbitMqDomainEventBus, organization=organization, service=service
-            ),
+            DomainEventBus,
+            builders={
+                "default": Builder(
+                    RabbitMqDomainEventBus, organization=organization, service=service
+                ),
+                "not_implemented": Builder(NotImplementedDomainEventBus),
+            },
             envar_modifier="PETISCO_DOMAIN_EVENT_BUS_TYPE",
-            builders={"not_implemented": Builder(NotImplementedDomainEventBus)},
         ),
         Dependency(
-            name="command_bus",
-            default_builder=Builder(
-                RabbitMqCommandBus, organization=organization, service=service
-            ),
+            CommandBus,
+            builders={
+                "default": Builder(
+                    RabbitMqCommandBus, organization=organization, service=service
+                ),
+                "not_implemented": Builder(NotImplementedCommandBus),
+            },
             envar_modifier="PETISCO_COMMAND_BUS_TYPE",
-            builders={"not_implemented": Builder(NotImplementedCommandBus)},
         ),
         Dependency(
-            name="message_configurer",
-            default_builder=Builder(
-                RabbitMqMessageConfigurer,
-                organization=organization,
-                service=service,
-            ),
+            MessageConfigurer,
+            builders={
+                "default": Builder(
+                    RabbitMqMessageConfigurer,
+                    organization=organization,
+                    service=service,
+                ),
+                "not_implemented": Builder(NotImplementedMessageConfigurer),
+            },
             envar_modifier="PETISCO_MESSAGE_CONFIGURER_TYPE",
-            builders={"not_implemented": Builder(NotImplementedMessageConfigurer)},
         ),
         Dependency(
-            name="message_consumer",
-            default_builder=Builder(
-                RabbitMqMessageConsumer,
-                organization=organization,
-                service=service,
-                max_retries=max_retries,
-            ),
+            MessageConsumer,
+            builders={
+                "default": Builder(
+                    RabbitMqMessageConsumer,
+                    organization=organization,
+                    service=service,
+                    max_retries=max_retries,
+                ),
+                "not_implemented": Builder(NotImplementedMessageConsumer),
+            },
             envar_modifier="PETISCO_MESSAGE_CONSUMER_TYPE",
-            builders={"not_implemented": Builder(NotImplementedMessageConsumer)},
         ),
     ]
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from distutils.util import strtobool
-from typing import List, NoReturn
+from typing import List, Optional
 
 from petisco.base.application.application_configurer import ApplicationConfigurer
 from petisco.base.application.dependency_injection.container import Container
+from petisco.base.domain.message.message_configurer import MessageConfigurer
 from petisco.base.domain.message.message_subscriber import MessageSubscriber
 
 MAX_RETRIES = 5
 
 CLEAR_SUBSCRIBER_BEFORE = strtobool(
     os.getenv("PETISCO_RABBITMQ_CONFIGURER_CLEAR_SUBSCRIBER_BEFORE", "false")
 )
@@ -16,20 +17,20 @@
 )
 
 
 class RabbitMqMessageApplicationConfigurer(ApplicationConfigurer):
     def __init__(
         self,
         execute_after_dependencies: bool = True,
-        subscribers: List[MessageSubscriber] = None,
+        subscribers: Optional[List[MessageSubscriber]] = None,
     ):
         self.execute_after_dependencies = execute_after_dependencies
         self.subscribers = subscribers
         super().__init__(execute_after_dependencies)
 
-    def execute(self, testing: bool = False) -> NoReturn:
-        configurer = Container.get("message_configurer")
+    def execute(self, testing: bool = False) -> None:
+        configurer = Container.get(MessageConfigurer)
         configurer.configure_subscribers(
             self.subscribers,
             clear_subscriber_before=CLEAR_SUBSCRIBER_BEFORE,
             clear_store_before=CLEAR_STORE_BEFORE,
         )
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/shared/queue_config.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/queue_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,61 @@
-from typing import Dict
+from typing import Any, Dict, Union
 
 from petisco.extra.rabbitmq.shared.specific_queue_config import SpecificQueueConfig
 
 
 class QueueConfig:
     @staticmethod
     def from_dict(
-        specific_queue_configs_dict: dict, default_retry_ttl: int, default_main_ttl: int
-    ):
+        specific_queue_configs_dict: Dict[str, Any],
+        default_retry_ttl: int,
+        default_main_ttl: int,
+    ) -> "QueueConfig":
         specific_queue_configs = {}
         for key, config_dict in specific_queue_configs_dict.items():
             specific_queue_configs[key] = SpecificQueueConfig.from_dict(
                 config_dict, default_retry_ttl, default_main_ttl
             )
 
         return QueueConfig(
             default_retry_ttl=default_retry_ttl,
             default_main_ttl=default_main_ttl,
             specific_queue_configs=specific_queue_configs,
         )
 
     @staticmethod
-    def default(default_retry_ttl: int = 5000, default_main_ttl: int = 5000):
+    def default(
+        default_retry_ttl: int = 5000, default_main_ttl: int = 5000
+    ) -> "QueueConfig":
         return QueueConfig(
             default_retry_ttl=default_retry_ttl,
             default_main_ttl=default_main_ttl,
             specific_queue_configs={},
         )
 
     def __init__(
         self,
         default_retry_ttl: int,
         default_main_ttl: int,
         specific_queue_configs: Dict[str, SpecificQueueConfig],
-    ):
+    ) -> None:
         self.default_retry_ttl = default_retry_ttl
         self.default_main_ttl = default_main_ttl
         self.specific_queue_configs = specific_queue_configs
 
-    def info(self) -> dict:
+    def info(self) -> Dict[str, Any]:
         return {
             name: specific_config.info()
             for name, specific_config in self.specific_queue_configs.items()
         }
 
-    def get_retry_ttl(self, queue_name: str):
+    def get_retry_ttl(self, queue_name: str) -> Union[int, None]:
         for queue_config in self.specific_queue_configs.values():
             if queue_config.has_specific_config(queue_name):
                 return queue_config.get_retry_ttl()
         return self.default_retry_ttl
 
-    def get_main_ttl(self, queue_name: str):
+    def get_main_ttl(self, queue_name: str) -> Union[int, None]:
         for queue_config in self.specific_queue_configs.values():
             if queue_config.has_specific_config(queue_name):
                 return queue_config.get_main_ttl()
         return self.default_main_ttl
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_connector.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_connector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,87 @@
 import os
 import time
+from typing import Dict
 
+from loguru import logger
 from pika import BlockingConnection, ConnectionParameters, PlainCredentials
 from pika.adapters.blocking_connection import BlockingChannel
-from pika.exceptions import StreamLostError
+from pika.exceptions import ConnectionClosedByBroker, StreamLostError
 
 from petisco.base.misc.singleton import Singleton
 
 
 class RabbitMqConnector(metaclass=Singleton):
-    def __init__(self):
-        self.heartbeat = os.environ.get("RABBITMQ_HEARTBEAT", 60)
+    """
+    Singleton class to define RabbitMQ connections and some infrastructure configurations.
+    """
+
+    def __init__(self) -> None:
+        self.heartbeat = int(os.environ.get("RABBITMQ_HEARTBEAT", 60))
         self.user = os.environ.get("RABBITMQ_USER", "guest")
         self.password = os.environ.get("RABBITMQ_PASSWORD", "guest")
         self.host = os.environ.get("RABBITMQ_HOST", "localhost")
         self.port = os.environ.get("RABBITMQ_PORT", "5672")
-        self.num_max_retries_connection = os.environ.get(
-            "RABBITMQ_CONNECTION_NUM_MAX_RETRIES", 15
+        self.num_max_retries_connection = int(
+            os.environ.get("RABBITMQ_CONNECTION_NUM_MAX_RETRIES", 15)
         )
-        self.wait_seconds_retry = os.environ.get(
-            "RABBITMQ_CONNECTION_WAIT_SECONDS_RETRY", 1
+        self.wait_seconds_retry = float(
+            os.environ.get("RABBITMQ_CONNECTION_WAIT_SECONDS_RETRY", 1)
         )
-        self.open_connections = {}
+        self.open_connections: Dict[str, BlockingConnection] = dict()
+
+    @staticmethod
+    def ping() -> None:
+        connector = RabbitMqConnector()
+        connector.get_connection(key_connection="ping")
+        connector.close(key_connection="ping")
 
-    def close_all(self):
+    def close_all(self) -> None:
         for key_connection in list(self.open_connections.keys()):
             connection = self.open_connections.pop(key_connection)
             if connection and connection.is_open:
-                connection.close()
+                try:
+                    connection.close()
+                except StreamLostError as exc:
+                    logger.warning(f"close_all: {str(exc)}")
+                except Exception as exc:  # noqa
+                    logger.error(f"close_all: {str(exc)}")
 
-    def close(self, key_connection: str):
+    def close(self, key_connection: str) -> None:
         connection = self.open_connections.pop(key_connection)
         if connection and connection.is_open:
-            connection.close()
+            try:
+                connection.close()
+            except StreamLostError as exc:
+                logger.warning(f"close: {str(exc)}")
+            except Exception as exc:  # noqa
+                logger.error(f"close_all: {str(exc)}")
 
-    def get_connection(self, key_connection: str):
+    def get_connection(self, key_connection: str) -> BlockingConnection:
         connection = self.open_connections.get(key_connection)
 
         if not connection or not connection.is_open:
             connection = self._create_connection(key_connection)
 
         return connection
 
     def get_channel(self, key_connection: str) -> BlockingChannel:
         connection = self.get_connection(key_connection)
         try:
             channel = connection.channel()
         except StreamLostError:
             connection = self.get_connection(key_connection)
             channel = connection.channel()
+        except ConnectionClosedByBroker:
+            del self.open_connections[key_connection]
+            connection = self.get_connection(key_connection)
+            channel = connection.channel()
         return channel
 
-    def _create_connection(self, key_connection: str):
+    def _create_connection(self, key_connection: str) -> BlockingConnection:
 
         connection = self._create_blocking_connection(key_connection)
 
         self._wait_for_open_connection(connection, key_connection)
 
         if not connection.is_open:
             time_elapsed = round(
@@ -64,15 +90,15 @@
             raise ConnectionError(
                 f"RabbitMQConnector: Impossible to obtain a open connection with host {self.host}. "
                 f"Retried {self.num_max_retries_connection} in ~{time_elapsed} seconds"
             )
 
         return connection
 
-    def _create_blocking_connection(self, connection_name: str):
+    def _create_blocking_connection(self, connection_name: str) -> BlockingConnection:
         try:
             connection = BlockingConnection(
                 ConnectionParameters(
                     heartbeat=self.heartbeat,
                     host=self.host,
                     port=int(self.port),
                     credentials=PlainCredentials(
@@ -84,13 +110,15 @@
         except:  # noqa E722
             raise ConnectionError(
                 f"RabbitMQConnector: Impossible to connect to host {self.host}. "
                 f"Review the following envars: [RABBITMQ_USER, RABBITMQ_PASSWORD, RABBITMQ_HOST, RABBITMQ_PORT, RABBITMQ_CONNECTION_NUM_MAX_RETRIES, RABBITMQ_CONNECTION_WAIT_SECONDS_RETRY]"
             )
         return connection
 
-    def _wait_for_open_connection(self, connection, key_connection):
+    def _wait_for_open_connection(
+        self, connection: BlockingConnection, key_connection: str
+    ) -> None:
         for i in range(self.num_max_retries_connection):
             if connection.is_open:
                 self.open_connections[key_connection] = connection
                 break
             time.sleep(self.wait_seconds_retry)
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,69 @@
+from typing import Any, Dict, Union
+
 from petisco.extra.rabbitmq.shared.rabbitmq_connector import RabbitMqConnector
 
 
 class RabbitMqDeclarer:
     def __init__(self, connector: RabbitMqConnector, channel_name: str):
         self._connector = connector
         self._channel_name = channel_name
 
-    def declare_exchange(self, exchange_name: str, exchange_type: str = "topic"):
+    def declare_exchange(
+        self, exchange_name: str, exchange_type: str = "topic"
+    ) -> None:
         channel = self._connector.get_channel(self._channel_name)
         try:
             channel.exchange_declare(
                 exchange=exchange_name, exchange_type=exchange_type, durable=True
             )
         except Exception as error:
             raise TypeError(
                 f"RabbitMQEventPublisher: Cannot create the exchange ({exchange_name})\n{error}"
             )
         channel.close()
 
-    def delete_exchange(self, exchange_name: str):
+    def delete_exchange(self, exchange_name: str) -> None:
         channel = self._connector.get_channel(self._channel_name)
         channel.exchange_delete(exchange_name)
         channel.close()
 
     def declare_queue(
         self,
         queue_name: str,
-        dead_letter_exchange: str = None,
-        dead_letter_routing_key: str = None,
-        message_ttl: int = None,
-    ):
+        dead_letter_exchange: Union[str, None] = None,
+        dead_letter_routing_key: Union[str, None] = None,
+        message_ttl: Union[int, None] = None,
+    ) -> str:
         channel = self._connector.get_channel(self._channel_name)
 
-        queue_arguments = {}
+        queue_arguments: Dict[str, Any] = {}
         if dead_letter_exchange:
             queue_arguments["x-dead-letter-exchange"] = dead_letter_exchange
 
         if dead_letter_routing_key:
             queue_arguments["x-dead-letter-routing-key"] = dead_letter_routing_key
 
         if message_ttl:
             queue_arguments["x-message-ttl"] = message_ttl
 
         result = channel.queue_declare(
             queue=queue_name, arguments=queue_arguments, durable=True
         )
         channel.close()
 
-        return result.method.queue
+        queue_name: str = result.method.queue
+
+        return queue_name
 
-    def bind_queue(self, exchange_name: str, queue_name: str, routing_key: str):
+    def bind_queue(self, exchange_name: str, queue_name: str, routing_key: str) -> None:
         channel = self._connector.get_channel(self._channel_name)
 
         channel.queue_bind(
             exchange=exchange_name, queue=queue_name, routing_key=routing_key
         )
         channel.close()
 
-    def delete_queue(self, queue_name: str):
+    def delete_queue(self, queue_name: str) -> None:
         channel = self._connector.get_channel(self._channel_name)
         channel.queue_delete(queue_name)
         channel.close()
```

### Comparing `petisco-1.9.9/petisco/extra/rabbitmq/shared/specific_queue_config.py` & `petisco-2.0.0rc0/petisco/extra/rabbitmq/shared/specific_queue_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from fnmatch import fnmatch
+from typing import Any, Dict, Union
 
 
 class SpecificQueueConfig:
     @staticmethod
-    def from_dict(kdict: dict, default_retry_ttl: int, default_main_ttl: int):
+    def from_dict(
+        kdict: Dict[str, Any], default_retry_ttl: int, default_main_ttl: int
+    ) -> "SpecificQueueConfig":
         return SpecificQueueConfig(
             wildcard=kdict.get("when_queue_contains", None),
             specific_retry_ttl=kdict.get("use", {}).get("retry_ttl", default_retry_ttl),
             specific_main_ttl=kdict.get("use", {}).get("main_ttl", default_main_ttl),
         )
 
     def __init__(
         self,
         wildcard: str,
-        specific_retry_ttl: int = None,
-        specific_main_ttl: int = None,
-    ):
+        specific_retry_ttl: Union[int, None] = None,
+        specific_main_ttl: Union[int, None] = None,
+    ) -> None:
         self.wildcard = wildcard
         self.specific_retry_ttl = specific_retry_ttl
         self.specific_main_ttl = specific_main_ttl
 
-    def info(self):
+    def info(self) -> Dict[str, Any]:
         return {
             "when_queue_contains": self.wildcard,
             "specific_retry_ttl": self.specific_retry_ttl,
             "specific_main_ttl": self.specific_main_ttl,
         }
 
     def has_specific_config(self, queue_name: str) -> bool:
         return fnmatch(queue_name, self.wildcard)
 
-    def get_retry_ttl(self):
+    def get_retry_ttl(self) -> Union[int, None]:
         return self.specific_retry_ttl
 
-    def get_main_ttl(self):
+    def get_main_ttl(self) -> Union[int, None]:
         return self.specific_main_ttl
```

### Comparing `petisco-1.9.9/petisco/extra/slack/__init__.py` & `petisco-2.0.0rc0/petisco/extra/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from typing import Dict
+from typing import Any, Dict, List
 
 from petisco.base.application.notifier.notifier_message import NotifierMessage
 from petisco.extra.slack.application.notifier.create_text_meta import create_text_meta
 from petisco.extra.slack.application.notifier.slack_notifier_message_converter import (
     SlackNotifierMessageConverter,
 )
 
 
 class BlocksSlackNotifierMessageConverter(SlackNotifierMessageConverter):
-    def __init__(self, slack_accessory: Dict = None):
+    def __init__(self, slack_accessory: Dict = None) -> None:
         self.slack_accessory = slack_accessory
 
-    def convert(self, notifier_message: NotifierMessage):
+    def convert(self, notifier_message: NotifierMessage) -> List[Dict[str, Any]]:
         header_block = self._create_header_block(notifier_message.title)
         message_block = self._create_message_block(notifier_message)
         divider_block = {"type": "divider"}
         return [header_block, message_block, divider_block]
 
-    def _create_header_block(self, title: str):
+    def _create_header_block(self, title: str) -> Dict[str, Any]:
         return {
             "type": "header",
             "text": {
                 "type": "plain_text",
                 "text": title,
                 "emoji": True,
             },
         }
 
-    def _create_message_block(self, notifier_message: NotifierMessage):
+    def _create_message_block(
+        self, notifier_message: NotifierMessage
+    ) -> Dict[str, Any]:
         text_message = ""
         if notifier_message.message:
             text_message += f"{notifier_message.message}"
 
         text_meta = create_text_meta(notifier_message.meta)
         if text_meta:
             text_message += text_meta
```

### Comparing `petisco-1.9.9/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/extra/slack/application/notifier/slack_notifier.py` & `petisco-2.0.0rc0/petisco/extra/slack/application/notifier/slack_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,25 +35,27 @@
         ] = ExceptionBlocksSlackNotifierMessageConverter(),
     ):
         self.channel = channel
         self.converter = converter
         self.exception_converter = exception_converter
         self.client = WebClient(token=token)
 
-    def publish(self, notifier_message: NotifierMessage):
+    def publish(self, notifier_message: NotifierMessage) -> None:
         try:
             self.client.chat_postMessage(
                 channel=self.channel,
                 blocks=self.converter.convert(notifier_message),
                 text=notifier_message.title,
             )
         except SlackApiError as e:
             raise SlackError(e.response["error"])
 
-    def publish_exception(self, notifier_exception_message: NotifierExceptionMessage):
+    def publish_exception(
+        self, notifier_exception_message: NotifierExceptionMessage
+    ) -> None:
         try:
             self.client.chat_postMessage(
                 channel=self.channel,
                 blocks=self.exception_converter.convert(notifier_exception_message),
                 text=notifier_exception_message.title,
             )
         except SlackApiError as e:
```

### Comparing `petisco-1.9.9/petisco/extra/slack/dependencies.py` & `petisco-2.0.0rc0/petisco/extra/slack/dependencies.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from typing import List
 
 from petisco.base.application.dependency_injection.dependency import Dependency
 from petisco.base.application.notifier.not_implemented_notifier import (
     NotImplementedNotifier,
 )
+from petisco.base.application.notifier.notifier import Notifier
 from petisco.base.misc.builder import Builder
 
 
 def get_default_notifier_dependencies() -> List[Dependency]:
 
     return [
         Dependency(
-            name="notifier",
-            default_builder=Builder(NotImplementedNotifier),
+            Notifier,
+            builders={"default": Builder(NotImplementedNotifier)},
             envar_modifier="PETISCO_NOTIFIER_TYPE",
         )
     ]
 
 
 def get_slack_notifier_dependencies(token: str, channel: str) -> List[Dependency]:
     from petisco.extra.slack.application.notifier.slack_notifier import SlackNotifier
 
     return [
         Dependency(
-            name="notifier",
-            default_builder=Builder(SlackNotifier, token=token, channel=channel),
+            Notifier,
+            builders={
+                "default": Builder(SlackNotifier, token=token, channel=channel),
+                "not_implemented": Builder(NotImplementedNotifier),
+            },
             envar_modifier="PETISCO_NOTIFIER_TYPE",
-            builders={"not_implemented": Builder(NotImplementedNotifier)},
         )
     ]
```

### Comparing `petisco-1.9.9/petisco/extra/sqlalchemy/__init__.py` & `petisco-2.0.0rc0/petisco/extra/sqlalchemy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from petisco.extra.sqlalchemy.is_sqlalchemy_available import is_sqlalchemy_available
 
 if is_sqlalchemy_available():
+    from petisco.extra.sqlalchemy.sql.async_sql_database import AsyncSqlDatabase
+    from petisco.extra.sqlalchemy.sql.mysql.legacy_mysql_database import (
+        LegacyMySqlDatabase,
+    )
     from petisco.extra.sqlalchemy.sql.mysql.mysql_connection import MySqlConnection
-    from petisco.extra.sqlalchemy.sql.mysql.mysql_database import MySqlDatabase
+    from petisco.extra.sqlalchemy.sql.sql_database import SqlDatabase
     from petisco.extra.sqlalchemy.sql.sql_executor import SqlExecutor
+    from petisco.extra.sqlalchemy.sql.sqlite.legacy_sqlite_database import (
+        LegacySqliteDatabase,
+    )
     from petisco.extra.sqlalchemy.sql.sqlite.sqlite_connection import SqliteConnection
-    from petisco.extra.sqlalchemy.sql.sqlite.sqlite_database import SqliteDatabase
 
     __all__ = [
         "MySqlConnection",
-        "MySqlDatabase",
+        "LegacyMySqlDatabase",
         "SqliteConnection",
-        "SqliteDatabase",
+        "LegacySqliteDatabase",
         "SqlExecutor",
+        "SqlDatabase",
+        "AsyncSqlDatabase",
     ]
 else:
     __all__ = []
```

### Comparing `petisco-1.9.9/petisco/extra/sqlalchemy/sql/base_sql_repository.py` & `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/base_sql_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any, Union
+
 from meiga import BoolResult, Error, Failure, isSuccess
 
 from petisco import Uuid
 from petisco.base.application.patterns.repository import Repository
 from petisco.base.domain.errors.defaults.already_exists import (
     AggregateAlreadyExistError,
 )
@@ -10,43 +12,43 @@
     AggregatesNotFoundError,
 )
 
 
 class BaseSqlRepository(Repository):
     @classmethod
     def fail_if_aggregate_already_exist(
-        cls, model, aggregate_id: Uuid, result_error: Error = None
+        cls, model: Any, aggregate_id: Uuid, result_error: Union[Error, None] = None
     ) -> BoolResult:
         if model:
             error = (
                 AggregateAlreadyExistError(
                     aggregate_id, cls.__name__, model.__tablename__
                 )
                 if not result_error
                 else result_error
             )
             return Failure(error)
         return isSuccess
 
     @classmethod
     def fail_if_aggregate_not_found(
-        cls, model, aggregate_id: Uuid, result_error: Error = None
+        cls, model: Any, aggregate_id: Uuid, result_error: Union[Error, None] = None
     ) -> BoolResult:
         if not model:
             error = (
                 AggregateNotFoundError(aggregate_id, cls.__name__)
                 if not result_error
                 else result_error
             )
             return Failure(error)
         return isSuccess
 
     @classmethod
     def fail_if_aggregates_not_found(
-        cls, model, result_error: Error = None
+        cls, model: Any, result_error: Union[Error, None] = None
     ) -> BoolResult:
         if not model:
             error = (
                 AggregatesNotFoundError(cls.__name__)
                 if not result_error
                 else result_error
             )
```

### Comparing `petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py` & `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,30 +29,30 @@
         server_name: str = "mysql",
         driver: str = "pymysql",
         user: str = "root",
         password: str = "root",
         host: str = "mysql",
         port: str = "3306",
         database_name: str = MYSQL_DATABASE_DEFAULT,
-    ):
+    ) -> "MySqlConnection":
         url = (
             f"{server_name}+{driver}://{user}:{password}@{host}:{port}/{database_name}"
         )
         return MySqlConnection(
             server_name, driver, user, password, host, port, database_name, url
         )
 
     @staticmethod
-    def create_local(database_name: str = MYSQL_DATABASE_DEFAULT):
+    def create_local(database_name: str = MYSQL_DATABASE_DEFAULT) -> "MySqlConnection":
         return MySqlConnection.create(
             host="localhost", port="3307", database_name=database_name
         )
 
     @staticmethod
-    def from_environ():
+    def from_environ() -> "MySqlConnection":
         return MySqlConnection.create(
             "mysql",
             "pymysql",
             os.getenv("MYSQL_USER", "root"),
             os.getenv("MYSQL_PASSWORD", "root"),
             os.getenv("MYSQL_HOST", "mysql"),
             os.getenv("MYSQL_PORT", "3306"),
```

### Comparing `petisco-1.9.9/petisco/extra/sqlalchemy/sql/mysql/mysql_database.py` & `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-from typing import Callable, List
+import os
+from typing import Any, Callable, List
 
+from sqlalchemy import text
 from sqlalchemy.orm import scoped_session
 
-from petisco.base.domain.persistence.interface_database import Database
+from petisco.base.domain.persistence.legacy_database import LegacyDatabase
 from petisco.base.domain.persistence.persistence_models import PersistenceModels
-from petisco.extra.sqlalchemy.sql.mysql.mysql_connection import MySqlConnection
 from petisco.extra.sqlalchemy.sql.sql_session_scope_provider import (
     sql_session_scope_provider,
 )
+from petisco.extra.sqlalchemy.sql.sqlite.sqlite_connection import SqliteConnection
 
 
-class MySqlDatabase(Database):
-    @staticmethod
-    def local_connection_checker():
-        return MySqlDatabase(
-            name="test", connection=MySqlConnection.create_local("test")
-        )
-
+class LegacySqliteDatabase(LegacyDatabase):
     def __init__(
         self,
         name: str,
-        connection: MySqlConnection,
+        connection: SqliteConnection,
         model_filename: str = None,
         print_sql_statements: bool = False,
         use_scoped_session: bool = True,
         use_future: bool = True,
     ):
-        if not connection or not isinstance(connection, MySqlConnection):
+        if not connection or not isinstance(connection, SqliteConnection):
             raise ConnectionError(
-                "MySqlDatabase needs a valid MySqlConnection connection"
+                "SqliteDatabase needs a valid SqliteConnection connection"
             )
         if model_filename:
             self.persistence_models = PersistenceModels.from_filename(model_filename)
         else:
             self.persistence_models = PersistenceModels(models={})
         self.connection = connection
         self.print_sql_statements = print_sql_statements
         self.use_scoped_session = use_scoped_session
         self.use_future = use_future
-
         super().__init__(name, self.persistence_models.models)
         self._init()
 
     def _init(self):
         from sqlalchemy.ext.declarative import declarative_base
 
         self.base = declarative_base()
@@ -51,51 +46,50 @@
         self.persistence_models.import_models()
         from sqlalchemy import create_engine
         from sqlalchemy.orm import sessionmaker
         from sqlalchemy_utils import create_database, database_exists
 
         engine = create_engine(
             self.connection.url,
-            pool_pre_ping=True,
             json_serializer=lambda obj: obj,
             json_deserializer=lambda obj: obj,
             echo=self.print_sql_statements,
             future=self.use_future,
         )
 
         if not database_exists(engine.url):
             create_database(engine.url)
             self.base.metadata.create_all(engine)
 
         self.session_maker = sessionmaker(bind=engine, future=self.use_future)
 
     def delete(self):
-        pass
-        # os.remove(self.connection.database_name)
+        if os.path.exists(self.connection.database_name):
+            os.remove(self.connection.database_name)
 
     def clear_data(self):
-        # Not available yet to avoid production problems.
-        # This, needs to be well documented.
-        # self.base.metadata.drop_all(self.engine)
-        pass
+        session_scope = self.get_session_scope()
+        with session_scope() as session:
+            for table in reversed(self.base.metadata.sorted_tables):
+                session.execute(table.delete())
 
     def is_available(self):
         try:
             session_scope = self.get_session_scope()
             with session_scope() as session:
-                session.execute("SELECT 1")
+                session.execute(text("SELECT 1"))
                 _is_available = True
         except Exception:  # noqa E722
             _is_available = False
         return _is_available
 
     def get_base(self):
         return self.base
 
-    def get_model(self, model_name: str):
+    def get_model(self, model_name: str) -> Any:
         model = self.persistence_models.get_imported_models().get(model_name)
         if not model:
             raise IndexError(
                 f'Model "{model_name}" is not available for "{self.name}" database'
             )
         return model
```

### Comparing `petisco-1.9.9/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py` & `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from contextlib import contextmanager
-from typing import Callable
+from contextlib import asynccontextmanager
+from typing import AsyncContextManager, Callable
 
+from loguru import logger
 from sqlalchemy.exc import OperationalError
+from sqlalchemy.ext.asyncio import AsyncSession
 
-from petisco.extra.sqlalchemy.sqlalchemy_operational_database_error import (
-    SqlAlchemyOperationalDatabaseError,
-)
 
-
-def sql_session_scope_provider(Session) -> Callable:
-    @contextmanager
-    def session_scope():
-        session = Session()
+def async_sql_session_scope_provider(
+    async_session_factory: Callable[[], AsyncSession]
+) -> Callable[..., AsyncContextManager[AsyncSession]]:
+    @asynccontextmanager
+    async def session_scope() -> AsyncContextManager[AsyncSession]:
+        session = async_session_factory()
         try:
             yield session
-            session.commit()
+            await session.commit()
         except OperationalError as e:
-            print(e)
-            session.rollback()
-            raise SqlAlchemyOperationalDatabaseError
+            logger.error(e)
+            await session.rollback()
+            raise e
         except Exception as e:
-            session.rollback()
+            logger.error(e)
+            await session.rollback()
             raise e
         finally:
-            session.close()
-        Session.remove()
+            await session.close()
+        # await session.delete()
 
     return session_scope
```

### Comparing `petisco-1.9.9/petisco/extra/sqlalchemy/sql/sqlite/sqlite_database.py` & `petisco-2.0.0rc0/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,102 @@
-import os
-from typing import Callable, List
+from typing import Any, Callable, List
 
+from sqlalchemy import text
 from sqlalchemy.orm import scoped_session
 
-from petisco.base.domain.persistence.interface_database import Database
+from petisco.base.domain.persistence.legacy_database import LegacyDatabase
 from petisco.base.domain.persistence.persistence_models import PersistenceModels
+from petisco.extra.sqlalchemy.sql.mysql.mysql_connection import MySqlConnection
 from petisco.extra.sqlalchemy.sql.sql_session_scope_provider import (
     sql_session_scope_provider,
 )
-from petisco.extra.sqlalchemy.sql.sqlite.sqlite_connection import SqliteConnection
 
 
-class SqliteDatabase(Database):
+class LegacyMySqlDatabase(LegacyDatabase):
+    @staticmethod
+    def local_connection_checker() -> "LegacyMySqlDatabase":
+        return LegacyMySqlDatabase(
+            name="test", connection=MySqlConnection.create_local("test")
+        )
+
     def __init__(
         self,
         name: str,
-        connection: SqliteConnection,
+        connection: MySqlConnection,
         model_filename: str = None,
         print_sql_statements: bool = False,
         use_scoped_session: bool = True,
         use_future: bool = True,
     ):
-        if not connection or not isinstance(connection, SqliteConnection):
+        if not connection or not isinstance(connection, MySqlConnection):
             raise ConnectionError(
-                "SqliteDatabase needs a valid SqliteConnection connection"
+                "MySqlDatabase needs a valid MySqlConnection connection"
             )
         if model_filename:
             self.persistence_models = PersistenceModels.from_filename(model_filename)
         else:
             self.persistence_models = PersistenceModels(models={})
         self.connection = connection
         self.print_sql_statements = print_sql_statements
         self.use_scoped_session = use_scoped_session
         self.use_future = use_future
+
         super().__init__(name, self.persistence_models.models)
         self._init()
 
-    def _init(self):
+    def _init(self) -> None:
         from sqlalchemy.ext.declarative import declarative_base
 
         self.base = declarative_base()
 
-    def create(self):
+    def create(self) -> None:
         self.persistence_models.import_models()
         from sqlalchemy import create_engine
         from sqlalchemy.orm import sessionmaker
         from sqlalchemy_utils import create_database, database_exists
 
         engine = create_engine(
             self.connection.url,
+            pool_pre_ping=True,
             json_serializer=lambda obj: obj,
             json_deserializer=lambda obj: obj,
             echo=self.print_sql_statements,
             future=self.use_future,
         )
 
         if not database_exists(engine.url):
             create_database(engine.url)
             self.base.metadata.create_all(engine)
 
         self.session_maker = sessionmaker(bind=engine, future=self.use_future)
 
-    def delete(self):
-        if os.path.exists(self.connection.database_name):
-            os.remove(self.connection.database_name)
-
-    def clear_data(self):
-        session_scope = self.get_session_scope()
-        with session_scope() as session:
-            for table in reversed(self.base.metadata.sorted_tables):
-                session.execute(table.delete())
+    def delete(self) -> None:
+        pass
+        # os.remove(self.connection.database_name)
+
+    def clear_data(self) -> None:
+        # Not available yet to avoid production problems.
+        # This, needs to be well documented.
+        # self.base.metadata.drop_all(self.engine)
+        pass
 
-    def is_available(self):
+    def is_available(self) -> bool:
         try:
             session_scope = self.get_session_scope()
             with session_scope() as session:
-                session.execute("SELECT 1")
+                session.execute(text("SELECT 1"))
                 _is_available = True
         except Exception:  # noqa E722
             _is_available = False
         return _is_available
 
     def get_base(self):
         return self.base
 
-    def get_model(self, model_name: str):
+    def get_model(self, model_name: str) -> Any:
         model = self.persistence_models.get_imported_models().get(model_name)
         if not model:
             raise IndexError(
                 f'Model "{model_name}" is not available for "{self.name}" database'
             )
         return model
```

### Comparing `petisco-1.9.9/petisco/extra/sqlmodel/sqlmodel_crud_repository.py` & `petisco-2.0.0rc0/petisco/extra/sqlmodel/sqlmodel_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-1.9.9/petisco/legacy/logger/logging_based_logger.py` & `petisco-2.0.0rc0/petisco/extra/logger/loguru_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,45 @@
-import logging
 import os
-from typing import Callable
 
-from petisco.legacy.logger.interface_logger import (
+from loguru import logger
+
+from petisco.extra.logger.log_message import LogMessage
+from petisco.extra.logger.logger import (
     CRITICAL,
     DEBUG,
     ERROR,
     FATAL,
     INFO,
     WARN,
     WARNING,
-    ILogger,
+    Logger,
 )
-from petisco.legacy.logger.log_message import LogMessage
-
-CORRESPONDENCES_LOGGING_LEVEL = {
-    "DEBUG": logging.DEBUG,
-    "INFO": logging.INFO,
-    "WARNING": logging.WARNING,
-    "ERROR": logging.ERROR,
-    "CRITICAL": logging.CRITICAL,
-}
 
 
-class LoggingBasedLogger(ILogger):
-    def __init__(
-        self,
-        logger_name: str,
-        format: str = "%(name)s - %(levelname)s - %(message)s",
-        config: Callable = None,
-    ):
+class LoguruLogger(Logger):
+    def __init__(self):
         self.logging_level = os.environ.get("PETISCO_LOGGING_LEVEL", "INFO").upper()
-        logging_level_value = CORRESPONDENCES_LOGGING_LEVEL.get(
-            self.logging_level, logging.INFO
-        )
-        logging.basicConfig(format=format, level=logging_level_value)
-        if config:
-            config()
-        self.logger = logging.getLogger(logger_name)
-        self.logger.setLevel(logging_level_value)
-        self.logger.info(f"Set PETISCO_LOGGING_LEVEL: {self.logging_level}")
+        logger.info(f"Set PETISCO_LOGGING_LEVEL: {self.logging_level}")
 
     def log(self, logging_level, log_message: LogMessage):
         message = log_message.to_dict()
         if logging_level == INFO:
             message["meta"]["level"] = "info"
-            self.logger.info(message)
+            logger.info(message)
         elif logging_level == DEBUG:
             message["meta"]["level"] = "debug"
-            self.logger.debug(message)
+            logger.debug(message)
         elif logging_level == CRITICAL:
             message["meta"]["level"] = "critical"
-            self.logger.critical(message)
+            logger.critical(message)
         elif logging_level == FATAL:
             message["meta"]["level"] = "fatal"
-            self.logger.fatal(message)
+            logger.error(message)
         elif logging_level == ERROR:
             message["meta"]["level"] = "error"
-            self.logger.error(message)
+            logger.error(message)
         elif logging_level == WARN:
             message["meta"]["level"] = "warning"
-            self.logger.warn(message)
+            logger.warning(message)
         elif logging_level == WARNING:
             message["meta"]["level"] = "warning"
-            self.logger.warning(message)
+            logger.warning(message)
```

### Comparing `petisco-1.9.9/petisco/public_api.py` & `petisco-2.0.0rc0/petisco/public_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-# coding=utf-8
-# Copyright (C) 2021+ Alice, Vigo, Spain
-
 """Public API of Alice Petisco Framework"""
-from typing import List, Type
-
 from petisco.base.application.application import Application
 from petisco.base.application.application_configurer import ApplicationConfigurer
+from petisco.base.application.controller.async_controller import AsyncController
 from petisco.base.application.controller.controller import Controller
 from petisco.base.application.controller.error_map import ErrorMap
+from petisco.base.application.controller.handlers import (
+    custom_message_handler,
+    unwrap_result_handler,
+)
 from petisco.base.application.controller.http_error import HttpError
 from petisco.base.application.dependency_injection.container import Container
 from petisco.base.application.dependency_injection.dependency import Dependency
-from petisco.base.application.dependency_injection.injector import (  # deprecated
-    Injector,
-)
 from petisco.base.application.middleware.middleware import Middleware
 from petisco.base.application.middleware.notifier_middleware import NotifierMiddleware
 from petisco.base.application.middleware.print_middleware import PrintMiddleware
 from petisco.base.application.notifier.not_implemented_notifier import (
     NotImplementedNotifier,
 )
 from petisco.base.application.notifier.notifier import Notifier
 from petisco.base.application.notifier.notifier_exception_message import (
     NotifierExceptionMessage,
 )
 from petisco.base.application.notifier.notifier_message import NotifierMessage
 from petisco.base.application.patterns.app_service import AppService
+from petisco.base.application.patterns.async_app_service import AsyncAppService
 from petisco.base.application.patterns.crud_repository import CrudRepository
 from petisco.base.application.patterns.inmemory_crud_repository import (
     InmemoryCrudRepository,
 )
 from petisco.base.application.patterns.repository import Repository
+from petisco.base.application.use_case.async_use_case import AsyncUseCase
 from petisco.base.application.use_case.use_case import UseCase
 from petisco.base.application.use_case.use_case_uncontrolled_error import (
     UseCaseUncontrolledError,
 )
 from petisco.base.domain.errors.critical_error import CriticalError
 from petisco.base.domain.errors.default_http_error_map import DEFAULT_HTTP_ERROR_MAP
 from petisco.base.domain.errors.defaults.already_exists import (
@@ -80,32 +79,41 @@
 )
 from petisco.base.domain.message.not_implemented_message_configurer import (
     NotImplementedMessageConfigurer,
 )
 from petisco.base.domain.model.aggregate_root import AggregateRoot
 from petisco.base.domain.model.uuid import Uuid
 from petisco.base.domain.model.value_object import ValueObject
+from petisco.base.domain.persistence.database import Database
+from petisco.base.domain.persistence.databases import Databases
 from petisco.base.domain.persistence.persistence import Persistence
 from petisco.base.domain.persistence.persistence_models import PersistenceModels
+from petisco.base.domain.persistence.sql_base import SqlBase
 from petisco.base.misc.builder import Builder
 from petisco.base.misc.interface import Interface
 from petisco.base.misc.result_mapper import ResultMapper
+from petisco.base.misc.singleton import Singleton
 from petisco.base.testing.assert_http import assert_http
 
-base = [
+__all__ = [
+    # base
     "Controller",
+    "AsyncController",
+    "unwrap_result_handler",
+    "custom_message_handler",
     "ResultMapper",
     "Middleware",
     "NotifierMiddleware",
     "Notifier",
     "NotifierMessage",
     "NotifierExceptionMessage",
     "NotImplementedNotifier",
     "PrintMiddleware",
     "UseCase",
+    "AsyncUseCase",
     "UseCaseUncontrolledError",
     "assert_http",
     "Dependency",
     "Container",
     "Message",
     "DomainEvent",
     "Command",
@@ -124,24 +132,27 @@
     "Uuid",
     "Interface",
     "DomainEventSubscriber",
     "CommandSubscriber",
     "AllMessageSubscriber",
     "Persistence",
     "PersistenceModels",
+    "Databases",
+    "Database",
+    "SqlBase",
     "Repository",
     "CrudRepository",
     "InmemoryCrudRepository",
     "AppService",
+    "AsyncAppService",
     "Application",
     "ApplicationConfigurer",
     "Builder",
-]
-
-errors = [
+    "Singleton",
+    # error
     "DEFAULT_HTTP_ERROR_MAP",
     "DomainError",
     "CriticalError",
     "NotFound",
     "AlreadyExists",
     "AggregateNotFoundError",
     "AggregatesNotFoundError",
@@ -153,13 +164,7 @@
     "UserAlreadyExists",
     "NotAllowed",
     "InvalidUuid",
     "InvalidValueObject",
     "HttpError",
     "ErrorMap",
 ]
-
-
-deprecated = ["Injector"]
-modules: List[str] = []
-
-__all__ = base + errors + deprecated + modules
```

### Comparing `petisco-1.9.9/petisco.egg-info/SOURCES.txt` & `petisco-2.0.0rc0/petisco.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,53 +2,60 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 petisco/VERSION
 petisco/__init__.py
 petisco/public_api.py
+petisco/py.typed
 petisco.egg-info/PKG-INFO
 petisco.egg-info/SOURCES.txt
 petisco.egg-info/dependency_links.txt
 petisco.egg-info/entry_points.txt
 petisco.egg-info/not-zip-safe
 petisco.egg-info/requires.txt
 petisco.egg-info/top_level.txt
 petisco/base/__init__.py
 petisco/base/application/__init__.py
 petisco/base/application/application.py
 petisco/base/application/application_configurer.py
 petisco/base/application/application_info.py
+petisco/base/application/chaos/__init__.py
+petisco/base/application/chaos/chaos_config.py
+petisco/base/application/chaos/check_chaos.py
 petisco/base/application/controller/__init__.py
+petisco/base/application/controller/async_controller.py
 petisco/base/application/controller/controller.py
-petisco/base/application/controller/controller_executor_wrapper.py
 petisco/base/application/controller/error_map.py
+petisco/base/application/controller/handlers.py
 petisco/base/application/controller/http_error.py
+petisco/base/application/controller/meta_controller.py
 petisco/base/application/dependency_injection/__init__.py
 petisco/base/application/dependency_injection/container.py
 petisco/base/application/dependency_injection/dependency.py
-petisco/base/application/dependency_injection/injector.py
 petisco/base/application/handlers/__init__.py
 petisco/base/application/handlers/message_handler.py
-petisco/base/application/handlers/use_case_uncontrolled_error.py
 petisco/base/application/middleware/__init__.py
 petisco/base/application/middleware/middleware.py
 petisco/base/application/middleware/notifier_middleware.py
 petisco/base/application/middleware/print_middleware.py
 petisco/base/application/notifier/__init__.py
 petisco/base/application/notifier/not_implemented_notifier.py
 petisco/base/application/notifier/notifier.py
 petisco/base/application/notifier/notifier_exception_message.py
 petisco/base/application/notifier/notifier_message.py
 petisco/base/application/patterns/__init__.py
 petisco/base/application/patterns/app_service.py
+petisco/base/application/patterns/async_app_service.py
 petisco/base/application/patterns/crud_repository.py
 petisco/base/application/patterns/inmemory_crud_repository.py
 petisco/base/application/patterns/repository.py
 petisco/base/application/use_case/__init__.py
+petisco/base/application/use_case/async_use_case.py
+petisco/base/application/use_case/meta_use_case.py
 petisco/base/application/use_case/use_case.py
 petisco/base/application/use_case/use_case_uncontrolled_error.py
 petisco/base/domain/__init__.py
 petisco/base/domain/errors/__init__.py
 petisco/base/domain/errors/critical_error.py
 petisco/base/domain/errors/default_http_error_map.py
 petisco/base/domain/errors/domain_error.py
@@ -85,115 +92,135 @@
 petisco/base/domain/message/chaos/message_chaos_error.py
 petisco/base/domain/message/chaos/not_implemented_message_chaos.py
 petisco/base/domain/model/__init__.py
 petisco/base/domain/model/aggregate_root.py
 petisco/base/domain/model/uuid.py
 petisco/base/domain/model/value_object.py
 petisco/base/domain/persistence/__init__.py
+petisco/base/domain/persistence/async_database.py
+petisco/base/domain/persistence/async_fake_database.py
+petisco/base/domain/persistence/database.py
+petisco/base/domain/persistence/databases.py
 petisco/base/domain/persistence/fake_database.py
-petisco/base/domain/persistence/interface_database.py
+petisco/base/domain/persistence/legacy_database.py
+petisco/base/domain/persistence/legacy_fake_database.py
 petisco/base/domain/persistence/persistence.py
 petisco/base/domain/persistence/persistence_models.py
+petisco/base/domain/persistence/sql_base.py
 petisco/base/misc/__init__.py
+petisco/base/misc/async_wrapper.py
 petisco/base/misc/builder.py
 petisco/base/misc/interface.py
 petisco/base/misc/result_mapper.py
 petisco/base/misc/singleton.py
 petisco/base/misc/wrapper.py
 petisco/base/testing/__init__.py
 petisco/base/testing/assert_http.py
 petisco/cli/__init__.py
 petisco/cli/petisco.py
+petisco/cli/petisco_dev.py
 petisco/cli/petisco_rabbitmq.py
 petisco/extra/__init__.py
 petisco/extra/elastic/__init__.py
-petisco/extra/elastic/elastic_apm_monitoring_app_service.py
+petisco/extra/elastic/async_elastic_database.py
 petisco/extra/elastic/elastic_connection.py
 petisco/extra/elastic/elastic_database.py
 petisco/extra/elastic/elastic_is_running_locally.py
-petisco/extra/elastic/elastic_operational_database_error.py
-petisco/extra/elastic/elastic_session_scope_provider.py
 petisco/extra/elastic/is_elastic_available.py
+petisco/extra/elastic/legacy_elastic_database.py
+petisco/extra/elastic_apm/__init__.py
+petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
+petisco/extra/elastic_apm/is_elastic_apm_available.py
 petisco/extra/fastapi/__init__.py
 petisco/extra/fastapi/is_fastapi_available.py
 petisco/extra/fastapi/application/__init__.py
 petisco/extra/fastapi/application/fastapi_application.py
 petisco/extra/fastapi/controller/__init__.py
+petisco/extra/fastapi/controller/as_fastapi.py
 petisco/extra/fastapi/controller/fastapi_controller.py
 petisco/extra/fastapi/controller/fastapi_default_response.py
 petisco/extra/fastapi/controller/fastapi_failure_handler.py
 petisco/extra/fastapi/controller/fastapi_result_mapper.py
 petisco/extra/fastapi/controller/fastapi_success_handler.py
 petisco/extra/fastapi/testing/__init__.py
 petisco/extra/fastapi/testing/assert_http_exception.py
+petisco/extra/logger/__init__.py
+petisco/extra/logger/log_message.py
+petisco/extra/logger/logger.py
+petisco/extra/logger/logging_based_logger.py
+petisco/extra/logger/loguru_logger.py
+petisco/extra/logger/not_implemented_logger.py
 petisco/extra/rabbitmq/__init__.py
 petisco/extra/rabbitmq/dependencies.py
 petisco/extra/rabbitmq/is_pika_available.py
 petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
 petisco/extra/rabbitmq/application/__init__.py
 petisco/extra/rabbitmq/application/chaos/__init__.py
 petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
 petisco/extra/rabbitmq/application/message/__init__.py
 petisco/extra/rabbitmq/application/message/bus/__init__.py
 petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
 petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
 petisco/extra/rabbitmq/application/message/configurer/__init__.py
 petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
 petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
 petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
 petisco/extra/rabbitmq/application/message/consumer/__init__.py
 petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
-petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_domain_event_bus.py
 petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
 petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
 petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
 petisco/extra/rabbitmq/application/message/formatter/__init__.py
 petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
 petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
 petisco/extra/rabbitmq/shared/__init__.py
 petisco/extra/rabbitmq/shared/queue_config.py
 petisco/extra/rabbitmq/shared/rabbitmq_connector.py
-petisco/extra/rabbitmq/shared/rabbitmq_consumer_connector.py
 petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
 petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
 petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
 petisco/extra/rabbitmq/shared/specific_queue_config.py
+petisco/extra/redis/__init__.py
+petisco/extra/redis/is_redis_available.py
+petisco/extra/redis/application/__init__.py
+petisco/extra/redis/application/message/__init__.py
+petisco/extra/redis/application/message/bus/__init__.py
+petisco/extra/redis/application/message/bus/redis_command_bus.py
+petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
+petisco/extra/redis/application/message/bus/redis_message_bus.py
 petisco/extra/slack/__init__.py
 petisco/extra/slack/dependencies.py
 petisco/extra/slack/is_slack_available.py
 petisco/extra/slack/application/__init__.py
 petisco/extra/slack/application/notifier/__init__.py
 petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
 petisco/extra/slack/application/notifier/create_text_meta.py
 petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
 petisco/extra/slack/application/notifier/slack_notifier.py
 petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
 petisco/extra/sqlalchemy/__init__.py
 petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-petisco/extra/sqlalchemy/sqlalchemy_operational_database_error.py
 petisco/extra/sqlalchemy/sql/__init__.py
+petisco/extra/sqlalchemy/sql/async_sql_database.py
+petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
 petisco/extra/sqlalchemy/sql/base_sql_repository.py
 petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+petisco/extra/sqlalchemy/sql/sql_database.py
 petisco/extra/sqlalchemy/sql/sql_executor.py
 petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
 petisco/extra/sqlalchemy/sql/mysql/__init__.py
+petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
 petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
-petisco/extra/sqlalchemy/sql/mysql/mysql_database.py
 petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
 petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
-petisco/extra/sqlalchemy/sql/sqlite/sqlite_database.py
 petisco/extra/sqlmodel/__init__.py
 petisco/extra/sqlmodel/is_sqlmodel_available.py
 petisco/extra/sqlmodel/sqlmodel_crud_repository.py
 petisco/extra/threading/__init__.py
 petisco/extra/threading/pool_executor.py
-petisco/legacy/__init__.py
-petisco/legacy/logger/__init__.py
-petisco/legacy/logger/interface_logger.py
-petisco/legacy/logger/log_message.py
-petisco/legacy/logger/logging_based_logger.py
-petisco/legacy/logger/not_implemented_logger.py
 requirements/requirements.txt
 tests/__init__.py
 tests/conftest.py
 tests/fixtures.py
 tests/modules/__init__.py
```

### Comparing `petisco-1.9.9/tests/fixtures.py` & `petisco-2.0.0rc0/tests/fixtures.py`

 * *Files identical despite different names*

