# Comparing `tmp/splunk_add_on_ucc_framework-6.0.0b1.tar.gz` & `tmp/splunk_add_on_ucc_framework-6.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splunk_add_on_ucc_framework-6.0.0b1.tar", max compression
+gzip compressed data, was "splunk_add_on_ucc_framework-6.0.0b2.tar", max compression
```

## Comparing `splunk_add_on_ucc_framework-6.0.0b1.tar` & `splunk_add_on_ucc_framework-6.0.0b2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    11357 2021-07-22 11:49:58.215733 splunk_add_on_ucc_framework-6.0.0b1/LICENSE
--rw-r--r--   0        0        0    87299 2021-07-22 11:50:54.740371 splunk_add_on_ucc_framework-6.0.0b1/NOTICE
--rw-r--r--   0        0        0     3825 2021-07-22 11:49:58.215733 splunk_add_on_ucc_framework-6.0.0b1/README.md
--rw-r--r--   0        0        0     2783 2021-07-22 11:51:28.152755 splunk_add_on_ucc_framework-6.0.0b1/pyproject.toml
--rw-r--r--   0        0        0  2054438 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/THIRDPARTY
--rw-r--r--   0        0        0        6 2021-07-12 13:25:08.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/VERSION
--rw-r--r--   0        0        0    30553 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/__init__.py
--rw-r--r--   0        0        0      615 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/__init__.py
--rw-r--r--   0        0        0      615 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/__init__.py
--rw-r--r--   0        0        0     2285 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/builder_constant.py
--rw-r--r--   0        0        0     9434 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/conf_parser.py
--rw-r--r--   0        0        0     5846 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/logger.py
--rw-r--r--   0        0        0      615 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/__init__.py
--rw-r--r--   0        0        0     4176 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/event_writer.py
--rw-r--r--   0        0        0     1198 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/memory_event_writer.py
--rw-r--r--   0        0        0     4797 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_aggregator.py
--rw-r--r--   0        0        0      710 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_exception.py
--rw-r--r--   0        0        0     3545 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_util.py
--rw-r--r--   0        0        0     4570 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/monitor.py
--rw-r--r--   0        0        0     4539 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/number_metric_collector.py
--rw-r--r--   0        0        0     2381 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/app_manifest.py
--rw-r--r--   0        0        0     8991 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/arf_dir_templates/modular_alert_package/${product_id}/appserver/static/alerticon.png
--rw-r--r--   0        0        0      441 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/arf_dir_templates/modular_alert_package.settings
--rw-r--r--   0        0        0     2702 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/global_config_validator.py
--rw-r--r--   0        0        0      615 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/__init__.py
--rw-r--r--   0        0        0     5732 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/__init__.py
--rw-r--r--   0        0        0     2263 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_base.py
--rw-r--r--   0        0        0       76 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_conf_default_settings.json
--rw-r--r--   0        0        0     9970 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_conf_gen.py
--rw-r--r--   0        0        0     1585 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_exceptions.py
--rw-r--r--   0        0        0    11686 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_helper.py
--rw-r--r--   0        0        0     5269 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_html_gen.py
--rw-r--r--   0        0        0     4455 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_merge.py
--rw-r--r--   0        0        0     7973 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_py_gen.py
--rw-r--r--   0        0        0     1226 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_template.py
--rw-r--r--   0        0        0     1225 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_consts.py
--rw-r--r--   0        0        0     2435 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action.py.template
--rw-r--r--   0        0        0     3674 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action_helper.py.template
--rw-r--r--   0        0        0      932 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.spec.template
--rw-r--r--   0        0        0     1003 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.template
--rw-r--r--   0        0        0      897 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/basecontrol.html
--rw-r--r--   0        0        0      501 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/checkbox.html
--rw-r--r--   0        0        0      254 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/default.html
--rw-r--r--   0        0        0      304 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/default2.html
--rw-r--r--   0        0        0      282 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/default3.html
--rw-r--r--   0        0        0      370 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/dropdownlist.html
--rw-r--r--   0        0        0      480 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/dropdownlist_splunk_search.html
--rw-r--r--   0        0        0      553 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/helper.html
--rw-r--r--   0        0        0      664 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/radio.html
--rw-r--r--   0        0        0      307 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/text.html
--rw-r--r--   0        0        0      308 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/eventtypes.conf.template
--rw-r--r--   0        0        0       97 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/mod_alert.html.template
--rw-r--r--   0        0        0       97 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/mod_alert2.html.template
--rw-r--r--   0        0        0      233 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/tags.conf.template
--rw-r--r--   0        0        0     5290 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/cim_actions.py
--rw-r--r--   0        0        0     3696 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/normalize.py
--rw-r--r--   0        0        0  3516411 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.js
--rw-r--r--   0        0        0    68658 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.licenses.txt
--rw-r--r--   0        0        0   341162 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.js
--rw-r--r--   0        0        0    68658 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.licenses.txt
--rw-r--r--   0        0        0    86519 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.js
--rw-r--r--   0        0        0    68658 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.licenses.txt
--rw-r--r--   0        0        0    20299 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/4.js
--rw-r--r--   0        0        0    40407 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/5.js
--rw-r--r--   0        0        0  4473190 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.js
--rw-r--r--   0        0        0   123225 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.licenses.txt
--rw-r--r--   0        0        0     1021 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/redirect_page.js
--rw-r--r--   0        0        0     1518 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/templates/base.html
--rw-r--r--   0        0        0     1546 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/templates/redirect.html
--rw-r--r--   0        0        0      468 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/app.conf
--rw-r--r--   0        0        0      726 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/nav/default.xml
--rw-r--r--   0        0        0      757 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/views/configuration.xml
--rw-r--r--   0        0        0      750 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/views/inputs.xml
--rw-r--r--   0        0        0      769 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/views/redirect.xml
--rw-r--r--   0        0        0    27971 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/schema/schema.json
--rw-r--r--   0        0        0     3656 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/start_alert_build.py
--rw-r--r--   0        0        0       93 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/templates/README.md
--rw-r--r--   0        0        0     1476 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/templates/input.template
--rw-r--r--   0        0        0     4697 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/templates/input_with_helper.template
--rw-r--r--   0        0        0     5917 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/templates/oauth.template
--rw-r--r--   0        0        0     2151 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/__init__.py
--rw-r--r--   0        0        0     4154 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/builder.py
--rw-r--r--   0        0        0      615 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/__init__.py
--rw-r--r--   0        0        0     4690 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/base.py
--rw-r--r--   0        0        0     2238 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/datainput.py
--rw-r--r--   0        0        0     1509 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/field.py
--rw-r--r--   0        0        0     2075 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/multiple_model.py
--rw-r--r--   0        0        0     1446 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/oauth_model.py
--rw-r--r--   0        0        0     1988 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/single_model.py
--rw-r--r--   0        0        0    15342 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/global_config.py
--rw-r--r--   0        0        0     2621 2021-07-22 11:49:58.219733 splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/rest_conf.py
--rw-r--r--   0        0        0     6260 2021-07-22 11:51:29.527143 splunk_add_on_ucc_framework-6.0.0b1/setup.py
--rw-r--r--   0        0        0     4806 2021-07-22 11:51:29.527895 splunk_add_on_ucc_framework-6.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/LICENSE
+-rw-r--r--   0        0        0    87299 2021-08-14 14:43:27.699183 splunk_add_on_ucc_framework-6.0.0b2/NOTICE
+-rw-r--r--   0        0        0     3825 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/README.md
+-rw-r--r--   0        0        0     2783 2021-08-14 14:44:03.439670 splunk_add_on_ucc_framework-6.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0  2054438 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/THIRDPARTY
+-rw-r--r--   0        0        0        6 2021-07-12 13:25:08.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/VERSION
+-rw-r--r--   0        0        0    30560 2021-08-14 14:44:03.435670 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/__init__.py
+-rw-r--r--   0        0        0      615 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/__init__.py
+-rw-r--r--   0        0        0      615 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/__init__.py
+-rw-r--r--   0        0        0     2285 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/builder_constant.py
+-rw-r--r--   0        0        0     9434 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/conf_parser.py
+-rw-r--r--   0        0        0     5846 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/logger.py
+-rw-r--r--   0        0        0      615 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/__init__.py
+-rw-r--r--   0        0        0     4176 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/event_writer.py
+-rw-r--r--   0        0        0     1198 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/memory_event_writer.py
+-rw-r--r--   0        0        0     4797 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_aggregator.py
+-rw-r--r--   0        0        0      710 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_exception.py
+-rw-r--r--   0        0        0     3545 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_util.py
+-rw-r--r--   0        0        0     4570 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/monitor.py
+-rw-r--r--   0        0        0     4539 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/number_metric_collector.py
+-rw-r--r--   0        0        0     2381 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/app_manifest.py
+-rw-r--r--   0        0        0     8991 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/arf_dir_templates/modular_alert_package/${product_id}/appserver/static/alerticon.png
+-rw-r--r--   0        0        0      441 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/arf_dir_templates/modular_alert_package.settings
+-rw-r--r--   0        0        0     2702 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/global_config_validator.py
+-rw-r--r--   0        0        0      615 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/__init__.py
+-rw-r--r--   0        0        0     5732 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/__init__.py
+-rw-r--r--   0        0        0     2263 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_base.py
+-rw-r--r--   0        0        0       76 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_conf_default_settings.json
+-rw-r--r--   0        0        0     9970 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_conf_gen.py
+-rw-r--r--   0        0        0     1585 2021-08-14 14:42:33.538435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_exceptions.py
+-rw-r--r--   0        0        0    11686 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_helper.py
+-rw-r--r--   0        0        0     5269 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_html_gen.py
+-rw-r--r--   0        0        0     4455 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_merge.py
+-rw-r--r--   0        0        0     7973 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_py_gen.py
+-rw-r--r--   0        0        0     1226 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_template.py
+-rw-r--r--   0        0        0     1225 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_consts.py
+-rw-r--r--   0        0        0     2435 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action.py.template
+-rw-r--r--   0        0        0     3674 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action_helper.py.template
+-rw-r--r--   0        0        0      932 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.spec.template
+-rw-r--r--   0        0        0     1003 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.template
+-rw-r--r--   0        0        0      897 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/basecontrol.html
+-rw-r--r--   0        0        0      501 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/checkbox.html
+-rw-r--r--   0        0        0      254 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/default.html
+-rw-r--r--   0        0        0      304 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/default2.html
+-rw-r--r--   0        0        0      282 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/default3.html
+-rw-r--r--   0        0        0      370 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/dropdownlist.html
+-rw-r--r--   0        0        0      480 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/dropdownlist_splunk_search.html
+-rw-r--r--   0        0        0      553 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/helper.html
+-rw-r--r--   0        0        0      664 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/radio.html
+-rw-r--r--   0        0        0      307 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/text.html
+-rw-r--r--   0        0        0      308 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/eventtypes.conf.template
+-rw-r--r--   0        0        0       97 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/mod_alert.html.template
+-rw-r--r--   0        0        0       97 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/mod_alert2.html.template
+-rw-r--r--   0        0        0      233 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/tags.conf.template
+-rw-r--r--   0        0        0     5290 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/cim_actions.py
+-rw-r--r--   0        0        0     3696 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/normalize.py
+-rw-r--r--   0        0        0  3516411 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.js
+-rw-r--r--   0        0        0    68658 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.licenses.txt
+-rw-r--r--   0        0        0   341162 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.js
+-rw-r--r--   0        0        0    68658 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.licenses.txt
+-rw-r--r--   0        0        0    86519 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.js
+-rw-r--r--   0        0        0    68658 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.licenses.txt
+-rw-r--r--   0        0        0    20299 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/4.js
+-rw-r--r--   0        0        0    40407 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/5.js
+-rw-r--r--   0        0        0  4473190 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.js
+-rw-r--r--   0        0        0   123225 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.licenses.txt
+-rw-r--r--   0        0        0     1021 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/redirect_page.js
+-rw-r--r--   0        0        0     1518 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/templates/base.html
+-rw-r--r--   0        0        0     1546 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/templates/redirect.html
+-rw-r--r--   0        0        0      468 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/app.conf
+-rw-r--r--   0        0        0      726 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/nav/default.xml
+-rw-r--r--   0        0        0      757 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/views/configuration.xml
+-rw-r--r--   0        0        0      750 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/views/inputs.xml
+-rw-r--r--   0        0        0      769 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/views/redirect.xml
+-rw-r--r--   0        0        0    27971 2021-07-12 13:24:48.000000 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/schema/schema.json
+-rw-r--r--   0        0        0     3656 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/start_alert_build.py
+-rw-r--r--   0        0        0       93 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/templates/README.md
+-rw-r--r--   0        0        0     1476 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/templates/input.template
+-rw-r--r--   0        0        0     4697 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/templates/input_with_helper.template
+-rw-r--r--   0        0        0     5917 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/templates/oauth.template
+-rw-r--r--   0        0        0     2127 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/__init__.py
+-rw-r--r--   0        0        0     4154 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/builder.py
+-rw-r--r--   0        0        0      615 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/__init__.py
+-rw-r--r--   0        0        0     4690 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/base.py
+-rw-r--r--   0        0        0     2238 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/datainput.py
+-rw-r--r--   0        0        0     1509 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/field.py
+-rw-r--r--   0        0        0     2075 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/multiple_model.py
+-rw-r--r--   0        0        0     1446 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/oauth_model.py
+-rw-r--r--   0        0        0     1988 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/single_model.py
+-rw-r--r--   0        0        0    15342 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/global_config.py
+-rw-r--r--   0        0        0     2621 2021-08-14 14:42:33.542435 splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/rest_conf.py
+-rw-r--r--   0        0        0     6260 2021-08-14 14:44:04.645872 splunk_add_on_ucc_framework-6.0.0b2/setup.py
+-rw-r--r--   0        0        0     4806 2021-08-14 14:44:04.646546 splunk_add_on_ucc_framework-6.0.0b2/PKG-INFO
```

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/LICENSE` & `splunk_add_on_ucc_framework-6.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/NOTICE` & `splunk_add_on_ucc_framework-6.0.0b2/NOTICE`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/README.md` & `splunk_add_on_ucc_framework-6.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/pyproject.toml` & `splunk_add_on_ucc_framework-6.0.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "splunk_add_on_ucc_framework"
-version = "6.0.0-beta.1"
+version = "6.0.0-beta.2"
 description = "Splunk Add-on SDK formerly UCC is a build and code generation framework"
 authors = ["rfaircloth-splunk <rfaircloth@splunk.com>"]
 include = [
 "splunk_add_on_ucc_framework/schema",
 "splunk_add_on_ucc_framework/THIRDPARTY.npm",
 "splunk_add_on_ucc_framework/package",
 "splunk_add_on_ucc_framework/package/locale",
```

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/THIRDPARTY` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/THIRDPARTY`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "5.0.0"
+__version__ = "6.0.0-beta.2"
 
 import argparse
 import configparser
 import glob
 import json
 import logging
 import os
```

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/builder_constant.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/builder_constant.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/conf_parser.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/conf_parser.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/logger.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/logger.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/event_writer.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/event_writer.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/memory_event_writer.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/memory_event_writer.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_aggregator.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_aggregator.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_exception.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_exception.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_util.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/metric_util.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/monitor.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/monitor.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/number_metric_collector.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/alert_utils/alert_utils_common/metric_collector/number_metric_collector.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/app_manifest.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/app_manifest.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/arf_dir_templates/modular_alert_package/${product_id}/appserver/static/alerticon.png` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/arf_dir_templates/modular_alert_package/${product_id}/appserver/static/alerticon.png`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/global_config_validator.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/global_config_validator.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_base.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_base.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_conf_gen.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_conf_gen.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_exceptions.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_exceptions.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_helper.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_helper.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_html_gen.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_html_gen.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_merge.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_merge.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_py_gen.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_py_gen.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_template.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/alert_actions_template.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_consts.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_consts.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action.py.template` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action.py.template`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action_helper.py.template` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_action_helper.py.template`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.spec.template` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.spec.template`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.template` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/alert_actions.conf.template`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/basecontrol.html` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/basecontrol.html`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/helper.html` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/helper.html`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/radio.html` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/arf_template/default_html_theme/radio.html`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/modular_alert_builder/build_core/cim_actions.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/modular_alert_builder/build_core/cim_actions.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/normalize.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/normalize.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.js` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.js`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.licenses.txt` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/0.licenses.txt`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.js` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.js`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.licenses.txt` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/1.licenses.txt`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.js` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.js`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.licenses.txt` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/3.licenses.txt`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/4.js` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/4.js`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/5.js` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/5.js`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.js` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.js`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.licenses.txt` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/entry_page.licenses.txt`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/static/js/build/redirect_page.js` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/static/js/build/redirect_page.js`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/templates/base.html` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/templates/base.html`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/appserver/templates/redirect.html` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/appserver/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/nav/default.xml` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/nav/default.xml`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/views/configuration.xml` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/views/configuration.xml`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/views/inputs.xml` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/views/inputs.xml`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/package/default/data/ui/views/redirect.xml` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/package/default/data/ui/views/redirect.xml`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/schema/schema.json` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/schema/schema.json`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/start_alert_build.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/start_alert_build.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/templates/input.template` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/templates/input.template`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/templates/input_with_helper.template` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/templates/input_with_helper.template`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/templates/oauth.template` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/templates/oauth.template`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 __all__ = [
     "RestBuilder",
     "RestBuilderError",
     "RestHandlerClass",
     "build",
 ]
 
-__version__ = "0.0.0"
-
-
 RestHandlerClass = collections.namedtuple(
     "RestHandlerClass",
     ("module", "name"),
 )
 
 
 def build(schema, handler, output_path, j2_env, post_process=None, *args, **kwargs):
```

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/builder.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/builder.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/__init__.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/base.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/base.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/datainput.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/datainput.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/field.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/field.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/multiple_model.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/multiple_model.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/oauth_model.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/oauth_model.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/single_model.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/endpoint/single_model.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/global_config.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/global_config.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/splunk_add_on_ucc_framework/uccrestbuilder/rest_conf.py` & `splunk_add_on_ucc_framework-6.0.0b2/splunk_add_on_ucc_framework/uccrestbuilder/rest_conf.py`

 * *Files identical despite different names*

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/setup.py` & `splunk_add_on_ucc_framework-6.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 entry_points = \
 {'console_scripts': ['install-libs = '
                      'splunk_add_on_ucc_framework:install_requirements',
                      'ucc-gen = splunk_add_on_ucc_framework:main']}
 
 setup_kwargs = {
     'name': 'splunk-add-on-ucc-framework',
-    'version': '6.0.0b1',
+    'version': '6.0.0b2',
     'description': 'Splunk Add-on SDK formerly UCC is a build and code generation framework',
     'long_description': '# SPDX-FileCopyrightText: 2020 Splunk Inc.\n\n# splunk-add-on-ucc-framework\n\n![PyPI](https://img.shields.io/pypi/v/splunk-add-on-ucc-framework)\n![Python](https://img.shields.io/pypi/pyversions/splunk-add-on-ucc-framework.svg)\n\nA framework to generate UI based Splunk Add-ons. It includes UI, Rest handler, Modular input, Oauth, Alert action templates.\n\n> Note: after UCC 5.2 Python 2 specific libraries are not supported anymore.\n> This means if the add-on has `package/lib/py2/requirements.txt` they will \n> not be installed while running `ucc-gen` command. Therefore modular inputs \n> that are supposed to run on Python 2 will not be supported by UCC. \n\n## What is UCC?\n\nUCC stands for  Universal Configuration Console. It is a service for generating Splunk Add-ons which is easily customizable and flexible.\nUCC provides basic UI template for creating Addon\'s UI. It is helpful to control the activity by using hooks and other functionalities.\n\n\n## Features\n\n- Generate UCC based addons for your Splunk Technology Add-ons\n\n## UCC 5\n\nUCC 5 has potentially breaking changes to add-ons using hook extension in the UX. Previously such hooks were limited to un-optimized js files placed in the package.\nAdd-ons may now package such extensions with webpack.\n\n## Requirements\n\n- Addon package and globalConfig.json file\n\n> Note: You may refer the globalConfig.json file [here](https://github.com/splunk/addonfactory-ucc-generator/blob/master/tests/data/globalConfig.json)\n\n\n## Installation\n\n"splunk-add-on-ucc-framework" can be installed via `pip` from `PyPI`:\n\n```bash\n$ pip3 install splunk-add-on-ucc-framework\n```\n\n## pre-commit\n\nPlease visit `pre-commit` quick start [section](https://pre-commit.com/#quick-start).\n\n## How to use\n\nTo build the UCC based addon follow the below steps:\n\n1. Install the `splunk-add-on-ucc-framework` via `pip3`.\n2. Run the `ucc-gen` command.\n3. Make sure that `package` folder and `globalConfig.json` file are present in the addon folder.\n4. The final addon package will be generated, in the `output` folder.\n\n\n## Workflow\n\nBy the running the `ucc-gen` command, the following steps are executed:\n1. Cleaning out the `output` folder.\n2. Retrieve the package ID of addon.\n3. Copy UCC template directory under `output/<package_ID>` directory.\n4. Copy `globalConfig.json` file to `output/<package_ID>/appserver/static/js/build` directory.\n5. Collect and install Addon\'s requirements into `output/<package_ID>/lib` directory of addon\'s package.\n6. For the addon\'s requirements, packages are installed according to following table:\n\n    | File Name            | Description                         | Output directory in UCC build |\n    |----------------------|-------------------------------------|-------------------------------|\n    | lib/requirements.txt     | Python3 compatible packages | output/<package_ID>/lib   |\n\n7. Replace tokens in views.\n8. Copy addon\'s `package/*` to `output/<package_ID>/*` directory.\n9. If an addon requires some additional configurations in packaging than implement the steps in additional_packaging.py\n\n## Params\n\nsplunk-add-on-ucc-framework supports the following params:\n\n| Name       | Description                                                                                              |\n|------------|----------------------------------------------------------------------------------------------------------|\n| source     | Folder containing the app.manifest and app source                                                        |\n| config     | Path to the configuration file, Defaults to GlobalConfig.json in the parent directory of source provided |\n| ta-version | Optional override Current version of TA, Default version is version specified in globalConfig.json a Splunkbase compatible version of SEMVER will be used by default                         |\n',
     'author': 'rfaircloth-splunk',
     'author_email': 'rfaircloth@splunk.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/splunk/splunk-add-on-sdk-python/',
```

### Comparing `splunk_add_on_ucc_framework-6.0.0b1/PKG-INFO` & `splunk_add_on_ucc_framework-6.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splunk-add-on-ucc-framework
-Version: 6.0.0b1
+Version: 6.0.0b2
 Summary: Splunk Add-on SDK formerly UCC is a build and code generation framework
 Home-page: https://github.com/splunk/splunk-add-on-sdk-python/
 Keywords: splunk
 Author: rfaircloth-splunk
 Author-email: rfaircloth@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

