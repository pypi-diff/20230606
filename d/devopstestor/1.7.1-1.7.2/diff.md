# Comparing `tmp/devopstestor-1.7.1.tar.gz` & `tmp/devopstestor-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstestor-1.7.1.tar", last modified: Mon Jun  5 10:46:39 2023, max compression
+gzip compressed data, was "devopstestor-1.7.2.tar", last modified: Tue Jun  6 09:47:01 2023, max compression
```

## Comparing `devopstestor-1.7.1.tar` & `devopstestor-1.7.2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.419587 devopstestor-1.7.1/
--rw-rw-rw-   0 root         (0) root         (0)    22958 2023-06-05 10:46:29.000000 devopstestor-1.7.1/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-05 10:46:29.000000 devopstestor-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      708 2023-06-05 10:46:39.418587 devopstestor-1.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-05 10:46:29.000000 devopstestor-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.399587 devopstestor-1.7.1/devopstestor/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.401587 devopstestor-1.7.1/devopstestor/config/
--rw-rw-rw-   0 root         (0) root         (0)     2837 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/core.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.401587 devopstestor-1.7.1/devopstestor/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.402587 devopstestor-1.7.1/devopstestor/src/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_machine_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_report.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.404587 devopstestor-1.7.1/devopstestor/src/core/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/devopstestor_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/devopstestor_server.py
--rw-rw-rw-   0 root         (0) root         (0)     8433 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/global_config_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8219 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/machines_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/ordonnanceur.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/report_render_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/source_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/testcase_executor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.406587 devopstestor-1.7.1/devopstestor/src/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2619 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/json_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/log_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.407587 devopstestor-1.7.1/devopstestor/src/machine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/debug_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7573 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/docker_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/local_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7560 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/vagrant_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.408587 devopstestor-1.7.1/devopstestor/src/provisionner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/empty_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/logstash_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     8768 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/minion_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/systemd_provisionner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.409587 devopstestor-1.7.1/devopstestor/src/reporting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/campaign_report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/deployment_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_elk_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.410587 devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
--rw-rw-rw-   0 root         (0) root         (0)     7258 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_text_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/scenario_report.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/testcase_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/verifier_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.411587 devopstestor-1.7.1/devopstestor/src/scenarios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/logstash.py
--rw-rw-rw-   0 root         (0) root         (0)     6385 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/mock_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.411587 devopstestor-1.7.1/devopstestor/src/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/copytemplate_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/dirlink_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/git_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.413587 devopstestor-1.7.1/devopstestor/src/testcase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/scenario_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/testcase_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/tests_cases_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.396587 devopstestor-1.7.1/devopstestor/testconf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.397587 devopstestor-1.7.1/devopstestor/testconf/verifiers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/service/
--rw-rw-rw-   0 root         (0) root         (0)     4529 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/service/http_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/http_logger/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.415587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.415587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.416587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.416587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/packages/
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.417587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.417587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/users/
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.418587 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.418587 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6214 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/verififier_luncher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.400587 devopstestor-1.7.1/devopstestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      708 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4372 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 10:46:39.419587 devopstestor-1.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-05 10:46:29.000000 devopstestor-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.016860 devopstestor-1.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2023-06-06 09:46:49.000000 devopstestor-1.7.2/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-06 09:46:49.000000 devopstestor-1.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-06 09:47:01.016860 devopstestor-1.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-06 09:46:49.000000 devopstestor-1.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:00.999861 devopstestor-1.7.2/devopstestor/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.002861 devopstestor-1.7.2/devopstestor/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2837 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/config/core.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.002861 devopstestor-1.7.2/devopstestor/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.003861 devopstestor-1.7.2/devopstestor/src/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/abstract/abstract_machine_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/abstract/abstract_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/abstract/abstract_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/abstract/abstract_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.004860 devopstestor-1.7.2/devopstestor/src/core/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/devopstestor_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/devopstestor_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8427 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/global_config_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8219 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/machines_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/ordonnanceur.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/report_render_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/source_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/core/testcase_executor_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.005860 devopstestor-1.7.2/devopstestor/src/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/lib/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/lib/json_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/lib/log_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.006860 devopstestor-1.7.2/devopstestor/src/machine/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/machine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/machine/debug_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7567 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/machine/docker_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/machine/local_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/machine/vagrant_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.007861 devopstestor-1.7.2/devopstestor/src/provisionner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/provisionner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/provisionner/empty_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/provisionner/logstash_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     8768 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/provisionner/minion_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/provisionner/systemd_provisionner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.008860 devopstestor-1.7.2/devopstestor/src/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/campaign_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/deployment_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/report_elk_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.009860 devopstestor-1.7.2/devopstestor/src/reporting/report_html_renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/report_html_renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/report_text_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/scenario_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/testcase_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/reporting/verifier_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.010860 devopstestor-1.7.2/devopstestor/src/scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/scenarios/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/scenarios/logstash.py
+-rw-rw-rw-   0 root         (0) root         (0)     6385 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/scenarios/mock_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/scenarios/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.011860 devopstestor-1.7.2/devopstestor/src/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/sources/copytemplate_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/sources/dirlink_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/sources/git_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.011860 devopstestor-1.7.2/devopstestor/src/testcase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/testcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/testcase/scenario_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/testcase/test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/testcase/testcase_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/src/testcase/tests_cases_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:00.996861 devopstestor-1.7.2/devopstestor/testconf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:00.998861 devopstestor-1.7.2/devopstestor/testconf/verifiers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.012860 devopstestor-1.7.2/devopstestor/testconf/verifiers/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.012860 devopstestor-1.7.2/devopstestor/testconf/verifiers/service/
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/service/http_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.013860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.013860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/http_logger/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.013860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.013860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.014860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.014860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/packages/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.015860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.015860 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/users/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.015860 devopstestor-1.7.2/devopstestor/testconf/verifiers/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.015860 devopstestor-1.7.2/devopstestor/testconf/verifiers/utils/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/utils/logstash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6214 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-06-06 09:46:49.000000 devopstestor-1.7.2/devopstestor/testconf/verifiers/utils/verififier_luncher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:47:01.000861 devopstestor-1.7.2/devopstestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-06 09:47:00.000000 devopstestor-1.7.2/devopstestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-06-06 09:47:00.000000 devopstestor-1.7.2/devopstestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:47:00.000000 devopstestor-1.7.2/devopstestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-06 09:47:00.000000 devopstestor-1.7.2/devopstestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 09:47:00.000000 devopstestor-1.7.2/devopstestor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 09:47:01.016860 devopstestor-1.7.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-06 09:46:49.000000 devopstestor-1.7.2/setup.py
```

### Comparing `devopstestor-1.7.1/LICENCE` & `devopstestor-1.7.2/LICENCE`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/PKG-INFO` & `devopstestor-1.7.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.7.1
+Version: 1.7.2
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.7.1/devopstestor/config/arguments.yml` & `devopstestor-1.7.2/devopstestor/config/arguments.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/config/machine.yml` & `devopstestor-1.7.2/devopstestor/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/config/report.yml` & `devopstestor-1.7.2/devopstestor/config/report.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/config/source_manager.yml` & `devopstestor-1.7.2/devopstestor/config/source_manager.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/config/testcase.yml` & `devopstestor-1.7.2/devopstestor/config/testcase.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/abstract/abstract_machine_controller.py` & `devopstestor-1.7.2/devopstestor/src/abstract/abstract_machine_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/abstract/abstract_provisionner.py` & `devopstestor-1.7.2/devopstestor/src/abstract/abstract_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/abstract/abstract_report.py` & `devopstestor-1.7.2/devopstestor/src/abstract/abstract_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/abstract/abstract_source_accessor.py` & `devopstestor-1.7.2/devopstestor/src/abstract/abstract_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/devopstestor.py` & `devopstestor-1.7.2/devopstestor/src/core/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/devopstestor_client.py` & `devopstestor-1.7.2/devopstestor/src/core/devopstestor_client.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/devopstestor_server.py` & `devopstestor-1.7.2/devopstestor/src/core/devopstestor_server.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/global_config_factory.py` & `devopstestor-1.7.2/devopstestor/src/core/global_config_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         :return: un objet Config avec tous les elements
         """
         base_config = base_config.clone()
         base_config.set('lib_path', lib_path, force=True)
         base_config.set('client_path', client_path, force=True)
 
         log.debut('Chargement des configurations')
-        env_conf_dir_params = [get_global_path(global_config=base_config, relative_path=lpath) for lpath in os.environ['DEVOPSTESTOR_OTHER_CONF_DIRS'].split(':')] if os.getenv('DEVOPSTESTOR_OTHER_CONF_DIRS', '') != '' else []
+        env_conf_dir_params = [get_global_path(global_config=base_config, in_path=lpath) for lpath in os.environ['DEVOPSTESTOR_OTHER_CONF_DIRS'].split(':')] if os.getenv('DEVOPSTESTOR_OTHER_CONF_DIRS', '') != '' else []
         for path in [os.path.join(lib_path, 'config'), os.path.join(client_path, 'config')] + env_conf_dir_params:
             for file in os.listdir(path):
                 file_path = path + "/" + file
                 node_name = Path(file).stem
                 if node_name in base_config.config:
                     # La config cote lib sert de valeur par defaut
                     base_config.config[node_name] = copy_merge_recursive_dict(defaut=base_config.config[node_name], source=yaml.load(open(file_path), Loader=yaml.Loader))
```

### Comparing `devopstestor-1.7.1/devopstestor/src/core/machines_factory.py` & `devopstestor-1.7.2/devopstestor/src/core/machines_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/ordonnanceur.py` & `devopstestor-1.7.2/devopstestor/src/core/ordonnanceur.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/report_render_manager.py` & `devopstestor-1.7.2/devopstestor/src/core/report_render_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/source_manager.py` & `devopstestor-1.7.2/devopstestor/src/core/source_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/core/testcase_executor_factory.py` & `devopstestor-1.7.2/devopstestor/src/core/testcase_executor_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/lib/config.py` & `devopstestor-1.7.2/devopstestor/src/lib/config.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/lib/core_utils.py` & `devopstestor-1.7.2/devopstestor/src/lib/core_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/lib/json_utils.py` & `devopstestor-1.7.2/devopstestor/src/lib/json_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/lib/log_manager.py` & `devopstestor-1.7.2/devopstestor/src/lib/log_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/lib/utils.py` & `devopstestor-1.7.2/devopstestor/src/lib/utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/machine/debug_controller.py` & `devopstestor-1.7.2/devopstestor/src/machine/debug_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/machine/docker_controller.py` & `devopstestor-1.7.2/devopstestor/src/machine/docker_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     @staticmethod
     def _build_image(machine_configuration, global_config):
         logger.debut('build', 'Debut build image')
         client = docker.from_env()
         dockerfile_path = get_global_path(
             global_config=global_config,
-            relative_path=machine_configuration.get('dockerfile_path')
+            in_path=machine_configuration.get('dockerfile_path')
         )
         context_path = os.path.dirname(dockerfile_path)
         filename = os.path.basename(dockerfile_path)
         tag = machine_configuration.get('docker_run_args::image')
         logger.info('Build config', context_path=context_path, filename=filename, tag=tag)
         (image, logs) = client.images.build(
             tag=tag,
```

### Comparing `devopstestor-1.7.1/devopstestor/src/machine/local_controller.py` & `devopstestor-1.7.2/devopstestor/src/machine/local_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/machine/vagrant_controller.py` & `devopstestor-1.7.2/devopstestor/src/machine/vagrant_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def create_machine(self, global_config:Config, machine_configuration:Config, machine_name:str, source_manager:SourceManager, resume_machine=False):
         """
         Initialise et lance la VM
         """
         vagrant_orig_path = get_global_path(
             global_config=global_config, 
-            relative_path=machine_configuration.get('vagrant_dir')
+            in_path=machine_configuration.get('vagrant_dir')
         )
         machine_name = machine_name.replace('testauto_','')
 
         # Clone de la configuration dans un dossier a part
         # En effet, plusieurs instance de la VM doivent pouvoir etre cree
         self.vagrant_working_path = os.path.join(vagrant_orig_path, ".testauto_vms", machine_name)
 
@@ -77,15 +77,15 @@
         """
         Retourne True si la machine est deja existante
         """
         # calcul du chemin vers le vagrant file de la VM
         vagrant_dir = os.path.join(
             get_global_path(
                 global_config=self.global_config, 
-                relative_path=machine_configuration.get('vagrant_dir')
+                in_path=machine_configuration.get('vagrant_dir')
             ), 
             ".testauto_vms", 
             machine_name.replace('testauto_','')
         )
         if not os.path.isdir(vagrant_dir):
             # Si pas de conf, on considere que la VM est down
             return False
```

### Comparing `devopstestor-1.7.1/devopstestor/src/provisionner/empty_provisionner.py` & `devopstestor-1.7.2/devopstestor/src/provisionner/empty_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/provisionner/logstash_provisionner.py` & `devopstestor-1.7.2/devopstestor/src/provisionner/logstash_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/provisionner/minion_provisionner.py` & `devopstestor-1.7.2/devopstestor/src/provisionner/minion_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/provisionner/systemd_provisionner.py` & `devopstestor-1.7.2/devopstestor/src/provisionner/systemd_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/reporting/report_elk_renderer.py` & `devopstestor-1.7.2/devopstestor/src/reporting/report_elk_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/__init__.py` & `devopstestor-1.7.2/devopstestor/src/reporting/report_html_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja` & `devopstestor-1.7.2/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/reporting/report_text_renderer.py` & `devopstestor-1.7.2/devopstestor/src/reporting/report_text_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/reporting/scenario_report.py` & `devopstestor-1.7.2/devopstestor/src/reporting/scenario_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/reporting/testcase_report.py` & `devopstestor-1.7.2/devopstestor/src/reporting/testcase_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/reporting/verifier_report.py` & `devopstestor-1.7.2/devopstestor/src/reporting/verifier_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/scenarios/devopstestor.py` & `devopstestor-1.7.2/devopstestor/src/scenarios/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/scenarios/logstash.py` & `devopstestor-1.7.2/devopstestor/src/scenarios/logstash.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/scenarios/mock_utils.py` & `devopstestor-1.7.2/devopstestor/src/scenarios/mock_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/scenarios/systemd.py` & `devopstestor-1.7.2/devopstestor/src/scenarios/systemd.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/sources/copytemplate_source_accessor.py` & `devopstestor-1.7.2/devopstestor/src/sources/copytemplate_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/sources/dirlink_source_accessor.py` & `devopstestor-1.7.2/devopstestor/src/sources/dirlink_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/sources/git_source_accessor.py` & `devopstestor-1.7.2/devopstestor/src/sources/git_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/testcase/scenario_executor.py` & `devopstestor-1.7.2/devopstestor/src/testcase/scenario_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/testcase/test_case.py` & `devopstestor-1.7.2/devopstestor/src/testcase/test_case.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/testcase/testcase_executor.py` & `devopstestor-1.7.2/devopstestor/src/testcase/testcase_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/src/testcase/tests_cases_loader.py` & `devopstestor-1.7.2/devopstestor/src/testcase/tests_cases_loader.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/context_fixtures.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/service/http_logger.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/service/http_logger.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/verififier_luncher.py` & `devopstestor-1.7.2/devopstestor/testconf/verifiers/utils/verififier_luncher.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/devopstestor.egg-info/PKG-INFO` & `devopstestor-1.7.2/devopstestor.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.7.1
+Version: 1.7.2
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.7.1/devopstestor.egg-info/SOURCES.txt` & `devopstestor-1.7.2/devopstestor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7.1/setup.py` & `devopstestor-1.7.2/setup.py`

 * *Files identical despite different names*

