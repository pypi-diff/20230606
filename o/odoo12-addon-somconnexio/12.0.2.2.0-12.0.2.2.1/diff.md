# Comparing `tmp/odoo12-addon-somconnexio-12.0.2.2.0.tar.gz` & `tmp/odoo12-addon-somconnexio-12.0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo12-addon-somconnexio-12.0.2.2.0.tar", last modified: Wed May 24 09:28:26 2023, max compression
+gzip compressed data, was "dist/odoo12-addon-somconnexio-12.0.2.2.1.tar", last modified: Tue Jun  6 09:29:33 2023, max compression
```

## Comparing `odoo12-addon-somconnexio-12.0.2.2.0.tar` & `odoo12-addon-somconnexio-12.0.2.2.1.tar`

### file list

```diff
@@ -1,596 +1,596 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/
--rw-r--r--   0 root         (0) root         (0)     4972 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4507 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/README.md
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9643 2023-05-24 09:00:20.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5170 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/http.py
--rw-rw-rw-   0 root         (0) root         (0)     3458 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/public_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/correos_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/correos_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/correos_services/shipment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/
--rw-rw-rw-   0 root         (0) root         (0)    46993 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account.account.template-sc.csv
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_chart_template_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     2954 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_group.xml
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_journal.xml
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_payment_mode.xml
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_payment_term.xml
--rw-rw-rw-   0 root         (0) root         (0)     1730 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_tax.xml
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_tax_group.xml
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/analytic_account.xml
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/base_automation.xml
--rw-rw-rw-   0 root         (0) root         (0)     2241 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/company.xml
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml
--rw-rw-rw-   0 root         (0) root         (0)     3786 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/contract_terminate_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)      947 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/crm_stage_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      658 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml
--rw-rw-rw-   0 root         (0) root         (0)     1238 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/discovery_channel.xml
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/fiber_signal_type_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/hr_attendance_place.xml
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/ir_config_pararameter.xml
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/ir_sequence.xml
--rw-rw-rw-   0 root         (0) root         (0)    13962 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/mail_activity_type.xml
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/mail_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     3266 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/mis_report.xml
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/partner_action_tag_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/partner_priority.xml
--rw-rw-rw-   0 root         (0) root         (0)    13582 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/previous_provider_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_attribute.xml
--rw-rw-rw-   0 root         (0) root         (0)     7767 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_attribute_value.xml
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_categories.xml
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml
--rw-rw-rw-   0 root         (0) root         (0)    10349 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_pack_line.xml
--rw-rw-rw-   0 root         (0) root         (0)    40646 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_product.xml
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml
--rw-rw-rw-   0 root         (0) root         (0)    11160 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_template_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/res.partner.bank.xml
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/res.users.xml
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/res_bank_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/service_technology.xml
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/service_technology_service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/share_type.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/demo/
--rw-rw-rw-   0 root         (0) root         (0)     6259 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/demo/partner.xml
--rw-rw-rw-   0 root         (0) root         (0)    13717 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/demo/pricelist.xml
--rw-rw-rw-   0 root         (0) root         (0)     2346 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/demo/subscription_requests.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/helpers/date.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/helpers/language.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/i18n/
--rw-rw-rw-   0 root         (0) root         (0)   320073 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/i18n/ca_ES.po
--rw-rw-rw-   0 root         (0) root         (0)   329543 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/i18n/es.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/contract_line_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/contract_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/crm_lead_listener.py
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/partner_bank_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1355 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/partner_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8/pre-clean-mail-tracking-value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8.11/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8.11/post-create-copy-contract-service-info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/post-migrate-change-address.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.13/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.2/
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.9/
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-recompute-is-from-pack.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py
--rw-rw-rw-   0 root         (0) root         (0)     1260 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1191 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.1.8/pre-assign-imd-manual-created-activity-types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-05-24 09:00:20.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/erppeek/
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/erppeek/README.md
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/erppeek/erppeek.ini
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/erppeek/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     1043 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/
--rw-rw-rw-   0 root         (0) root         (0)     1838 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_asset.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_banking_mandate.py
--rw-rw-rw-   0 root         (0) root         (0)     6377 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_invoice.py
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_invoice_line.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_journal.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_move.py
--rw-rw-rw-   0 root         (0) root         (0)     3769 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_payment_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_tax.py
--rw-rw-rw-   0 root         (0) root         (0)    21169 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/aged_partner_balance.py
--rw-rw-rw-   0 root         (0) root         (0)     7108 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py
--rw-rw-rw-   0 root         (0) root         (0)    37812 2023-05-24 09:00:20.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/broadband.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_terminate_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_terminate_user_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/coop_agreement.py
--rw-rw-rw-   0 root         (0) root         (0)    21856 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)    11230 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/discovery_channel.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/fiber_signal_type.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/hr_attendance.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/hr_attendance_place.py
--rw-rw-rw-   0 root         (0) root         (0)     3864 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/hr_employee.py
--rw-rw-rw-   0 root         (0) root         (0)     4417 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/ir_model_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/ir_server_action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/broadband.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/l10n_es_aeat_report.py
--rw-rw-rw-   0 root         (0) root         (0)     3881 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/mail_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/mail_thread.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/mass_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/opencell_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/operation_request.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/operation_request_terminate_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/partner_action_tag.py
--rw-rw-rw-   0 root         (0) root         (0)     2816 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/partner_otrs_view.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/payment_return.py
--rw-rw-rw-   0 root         (0) root         (0)     3407 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/payment_return_line.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/previous_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_attribute_value.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_category_technology_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_pack_line.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_pricelist.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_product.py
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_template.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/res_company.py
--rw-rw-rw-   0 root         (0) root         (0)    22511 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/res_partner_bank.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/service_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/service_technology.py
--rw-rw-rw-   0 root         (0) root         (0)     2509 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/stock_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/stock_production_lot.py
--rw-rw-rw-   0 root         (0) root         (0)    12471 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/subscription_request.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/utm_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/access.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     5121 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/customer.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/opencell_resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/opencell_types/
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/opencell_types/address.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/opencell_types/custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/opencell_types/description.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/services.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/customer_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/opencell_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/subscription_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/router_4G_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/account_asset_report_xls.py
--rw-rw-rw-   0 root         (0) root         (0)    20209 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/aged_partner_balance.xml
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1398 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1969 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     3799 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/report_paperformat.xml
--rw-rw-rw-   0 root         (0) root         (0)     8425 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     3036 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/security/
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/security/ir.model.access.csv
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/security/res_groups.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5557 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/account_invoice_process.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/account_invoice_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/account_payment_group_process.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/bank_from_iban_getter.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/change_partner_emails.py
--rw-rw-rw-   0 root         (0) root         (0)     5468 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_change_tariff_process.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_change_tariff_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    10363 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_contract_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_email_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_iban_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_iban_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2809 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_one_shot_process.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_one_shot_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/adsl.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/ba.py
--rw-rw-rw-   0 root         (0) root         (0)    13704 2023-05-24 08:16:37.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10651 2023-05-24 08:16:37.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/fiber.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/router4g.py
--rw-rw-rw-   0 root         (0) root         (0)     8974 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/crm_lead_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/discovery_channel_service.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/get_activation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/hashids_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/partner_email_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/partner_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     8806 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/product_catalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/provider_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5730 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/res_partner_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21971 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/subscription_request_service.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/vat_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/somoffice/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/somoffice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/somoffice/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/somoffice/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/
--rw-rw-rw-   0 root         (0) root         (0)     9682 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/activities.png
--rw-rw-rw-   0 root         (0) root         (0)    12957 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/broadband_contract.png
--rw-rw-rw-   0 root         (0) root         (0)    13548 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/broadband_lead_lines.png
--rw-rw-rw-   0 root         (0) root         (0)     6550 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/emails.png
--rw-rw-rw-   0 root         (0) root         (0)    15486 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/mobile_contract.png
--rw-rw-rw-   0 root         (0) root         (0)    15574 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/mobile_lead_lines.png
--rw-rw-rw-   0 root         (0) root         (0)    15844 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/packs.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/img/
--rw-rw-rw-   0 root         (0) root         (0)    17014 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/img/sc-image.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/my_attendances.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/xml/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/xml/activity.xml
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/xml/attendance.xml
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/xml/contract_email.xml
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/xml/mail_chatter_buttons.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/common_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/correos_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/correos_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7677 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/correos_services/test_shipment.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     6137 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10823 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     5866 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     3491 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     7360 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_invoice.py
--rw-rw-rw-   0 root         (0) root         (0)     3598 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     3854 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_payment_order.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py
--rw-rw-rw-   0 root         (0) root         (0)    33841 2023-05-23 10:45:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_contract.py
--rw-rw-rw-   0 root         (0) root         (0)     5657 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_coop_agreement.py
--rw-rw-rw-   0 root         (0) root         (0)    85607 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)     9390 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_mail_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     5484 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_mass_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)     6492 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     9187 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_payment_return.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_previous_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    28217 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_product_product.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_product_template.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_production_lot.py
--rw-rw-rw-   0 root         (0) root         (0)    46314 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_server_action.py
--rw-rw-rw-   0 root         (0) root         (0)    10862 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_service_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)     4876 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_stock_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)    26854 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_subscription_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_address.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_customer.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15080 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10511 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     6230 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)    15234 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7743 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5744 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)    10104 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     6530 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     4644 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/sc_test_case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-05-19 08:39:08.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    25341 2023-05-24 08:16:37.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)     9744 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/
--rw-rw-rw-   0 root         (0) root         (0)    71869 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py
--rw-rw-rw-   0 root         (0) root         (0)     6513 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    16973 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    24404 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    43501 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7531 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py
--rw-rw-rw-   0 root         (0) root         (0)    15498 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2980 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    12908 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)    13013 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py
--rw-rw-rw-   0 root         (0) root         (0)    34346 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_get_activation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_hashids_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1501 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py
--rw-rw-rw-   0 root         (0) root         (0)     6003 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)    16662 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_provider_service.py
--rw-rw-rw-   0 root         (0) root         (0)    18948 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_res_partner_service.py
--rw-rw-rw-   0 root         (0) root         (0)     8798 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/somoffice/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/somoffice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/somoffice/test_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:26:48.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9061 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9357 2023-05-19 11:58:28.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     5693 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2552 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    21666 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4007 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     5504 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     9940 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    13855 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     3322 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    30774 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4421 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1648 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py
--rw-rw-rw-   0 root         (0) root         (0)     7011 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_asset_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_invoice_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_move.xml
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_move_line.xml
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_payment_order_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_tax_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/act_account_move_to_account_move_line_open.xml
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/aeat_report_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2690 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/broadband_isp_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    25337 2023-05-24 09:00:20.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/contract_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1117 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/coop_agreement_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/crm_lead.xml
--rw-rw-rw-   0 root         (0) root         (0)    15207 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/crm_lead_line.xml
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/data_range_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/hr_attendance.xml
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/ir_action_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     9621 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mail_activity_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mass_mailing_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/menus.xml
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mis_budget_item_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mobile_isp_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-22 14:24:02.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/open_boards_activities.xml
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/operation_request.xml
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/orange_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/partner_action_tag_views.xml
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/payment_return_import_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/payment_return_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/previous_provider_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_attribute_views.xml
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_pricelist_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_product_view.xml
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_template_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/res_company_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    13562 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/res_partner_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/service_technology_service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/stock_move_line_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/stock_production_lot.xml
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/subscription_request_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/templates_js.xml
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/
--rw-rw-rw-   0 root         (0) root         (0)     1170 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_payment_line_create/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_payment_line_create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_address_change/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_address_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8088 2023-05-19 11:58:28.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py
--rw-rw-rw-   0 root         (0) root         (0)     4084 2023-05-19 11:58:28.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_compensation/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_compensation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py
--rw-rw-rw-   0 root         (0) root         (0)     3492 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_holder_change/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_holder_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12025 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3782 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2088 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4572 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2134 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_tariff_change/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_tariff_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5592 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py
--rw-rw-rw-   0 root         (0) root         (0)     2684 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_terminate/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_terminate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11844 2023-05-19 15:08:31.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)    10758 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     1810 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_leads_validate/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_leads_validate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/import_payment_group/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/import_payment_group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/mail_compose_message/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/mail_compose_message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_email_change/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_email_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_confirm/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_confirm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/product_publish/
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/product_publish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/test_mailing/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/test_mailing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-19 08:39:09.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4972 2023-05-24 09:28:25.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    32533 2023-05-24 09:28:25.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:28:25.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:28:25.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2998 2023-05-24 09:28:25.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-24 09:28:25.000000 odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:28:26.000000 odoo12-addon-somconnexio-12.0.2.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5934 2023-05-23 11:17:52.000000 odoo12-addon-somconnexio-12.0.2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4507 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9643 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5170 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     3458 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/public_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/correos_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/correos_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/correos_services/shipment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/
+-rw-rw-rw-   0 root         (0) root         (0)    46993 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account.account.template-sc.csv
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_chart_template_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_group.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_journal.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_payment_mode.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_payment_term.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_tax.xml
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_tax_group.xml
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/analytic_account.xml
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/base_automation.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2241 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/company.xml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/contract_terminate_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/crm_stage_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/discovery_channel.xml
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/fiber_signal_type_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/hr_attendance_place.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/ir_config_pararameter.xml
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/ir_sequence.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13962 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/mail_activity_type.xml
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/mail_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/mis_report.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/partner_action_tag_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/partner_priority.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13582 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/previous_provider_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_attribute.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7767 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_attribute_value.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_categories.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7830 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)    10349 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_pack_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)    40646 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_product.xml
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)    11160 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_template_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/res.partner.bank.xml
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/res.users.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/res_bank_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/service_technology.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/service_technology_service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/share_type.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/demo/
+-rw-rw-rw-   0 root         (0) root         (0)     6259 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/demo/partner.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13717 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/demo/pricelist.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/demo/subscription_requests.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/helpers/date.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/helpers/language.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)   320073 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/i18n/ca_ES.po
+-rw-rw-rw-   0 root         (0) root         (0)   329543 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/i18n/es.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/contract_line_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/contract_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/crm_lead_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/partner_bank_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/partner_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8/pre-clean-mail-tracking-value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8.11/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8.11/post-create-copy-contract-service-info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/post-migrate-change-address.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.13/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-recompute-is-from-pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.1.8/pre-assign-imd-manual-created-activity-types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/erppeek/
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/erppeek/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/erppeek/erppeek.ini
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/erppeek/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1043 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_asset.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_banking_mandate.py
+-rw-rw-rw-   0 root         (0) root         (0)     6377 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_invoice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_invoice_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_move.py
+-rw-rw-rw-   0 root         (0) root         (0)     3769 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_payment_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_tax.py
+-rw-rw-rw-   0 root         (0) root         (0)    21169 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/aged_partner_balance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7108 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py
+-rw-rw-rw-   0 root         (0) root         (0)    39338 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/broadband.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_terminate_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_terminate_user_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/coop_agreement.py
+-rw-rw-rw-   0 root         (0) root         (0)    21856 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)    11230 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/discovery_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/fiber_signal_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/hr_attendance.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/hr_attendance_place.py
+-rw-rw-rw-   0 root         (0) root         (0)     3864 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/hr_employee.py
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/ir_model_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/ir_server_action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/broadband.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/l10n_es_aeat_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     3881 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/mail_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/mail_thread.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/mass_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/opencell_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/operation_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/operation_request_terminate_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/partner_action_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/partner_otrs_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/payment_return.py
+-rw-rw-rw-   0 root         (0) root         (0)     3407 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/payment_return_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/previous_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_attribute_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_category_technology_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_pack_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_pricelist.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_product.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/res_company.py
+-rw-rw-rw-   0 root         (0) root         (0)    22511 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/res_partner_bank.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/service_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/service_technology.py
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/stock_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/stock_production_lot.py
+-rw-rw-rw-   0 root         (0) root         (0)    12471 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/subscription_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/utm_source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/access.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     5121 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/opencell_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/opencell_types/
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/opencell_types/address.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/opencell_types/custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/opencell_types/description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/customer_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/opencell_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/subscription_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/router_4G_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/account_asset_report_xls.py
+-rw-rw-rw-   0 root         (0) root         (0)    20209 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/aged_partner_balance.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1969 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/report_paperformat.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8425 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/security/
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/security/ir.model.access.csv
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/security/res_groups.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5557 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/account_invoice_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/account_invoice_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/account_payment_group_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/bank_from_iban_getter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/change_partner_emails.py
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_change_tariff_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_change_tariff_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    10363 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_contract_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_email_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_iban_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_iban_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_one_shot_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_one_shot_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/adsl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/ba.py
+-rw-rw-rw-   0 root         (0) root         (0)    13704 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10651 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/fiber.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/router4g.py
+-rw-rw-rw-   0 root         (0) root         (0)     8974 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/crm_lead_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/discovery_channel_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/get_activation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/hashids_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/partner_email_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/partner_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     8806 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/product_catalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/provider_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5730 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/res_partner_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21971 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/subscription_request_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/vat_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/somoffice/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/somoffice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/somoffice/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/somoffice/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/
+-rw-rw-rw-   0 root         (0) root         (0)     9682 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/activities.png
+-rw-rw-rw-   0 root         (0) root         (0)    12957 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/broadband_contract.png
+-rw-rw-rw-   0 root         (0) root         (0)    13548 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/broadband_lead_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)     6550 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/emails.png
+-rw-rw-rw-   0 root         (0) root         (0)    15486 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/mobile_contract.png
+-rw-rw-rw-   0 root         (0) root         (0)    15574 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/mobile_lead_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)    15844 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/packs.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)    17014 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/img/sc-image.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/my_attendances.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/xml/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/xml/activity.xml
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/xml/attendance.xml
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/xml/contract_email.xml
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/xml/mail_chatter_buttons.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/common_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/correos_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/correos_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7677 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/correos_services/test_shipment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     6137 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10823 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     5866 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     3491 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7360 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_invoice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3598 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     3854 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_payment_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    33841 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     5657 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_coop_agreement.py
+-rw-rw-rw-   0 root         (0) root         (0)    85607 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)     9390 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_mail_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5484 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_mass_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6492 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9187 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_payment_return.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_previous_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    28217 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_product_product.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_product_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_production_lot.py
+-rw-rw-rw-   0 root         (0) root         (0)    46314 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_server_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    10862 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_service_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4876 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_stock_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)    26854 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_subscription_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_address.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15080 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10511 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     6230 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    15234 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7743 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5744 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10104 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     4644 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/sc_test_case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    25341 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     9744 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/
+-rw-rw-rw-   0 root         (0) root         (0)    71869 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     6513 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    16973 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    24404 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    43501 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7531 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py
+-rw-rw-rw-   0 root         (0) root         (0)    15498 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    12908 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    13013 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    34346 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_get_activation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_hashids_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py
+-rw-rw-rw-   0 root         (0) root         (0)     6003 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    16662 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_provider_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    18948 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_res_partner_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     8798 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/somoffice/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/somoffice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/somoffice/test_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9061 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9357 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     5693 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2552 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    21666 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4007 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     5504 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     9940 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13855 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12968 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    30774 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4421 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     7011 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_asset_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_invoice_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_move.xml
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_move_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_payment_order_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_tax_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/act_account_move_to_account_move_line_open.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/aeat_report_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/broadband_isp_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    25408 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/contract_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/coop_agreement_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/crm_lead.xml
+-rw-rw-rw-   0 root         (0) root         (0)    15207 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/crm_lead_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/data_range_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/hr_attendance.xml
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/ir_action_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     9621 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mail_activity_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mass_mailing_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/menus.xml
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mis_budget_item_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mobile_isp_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/open_boards_activities.xml
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/operation_request.xml
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/orange_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/partner_action_tag_views.xml
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/payment_return_import_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/payment_return_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/previous_provider_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_attribute_views.xml
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_pricelist_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_product_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_template_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/res_company_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13562 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/res_partner_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/service_technology_service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/stock_move_line_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/stock_production_lot.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/subscription_request_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/templates_js.xml
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)     1170 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_invoice_confirm/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_invoice_confirm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_payment_line_create/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_payment_line_create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_address_change/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_address_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8088 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     4084 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_compensation/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_compensation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3492 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_force_oc_integration/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_force_oc_integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_holder_change/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_holder_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12025 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3782 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change_force/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change_force/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_invoice_payment/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_invoice_payment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4572 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_one_shot_request/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_one_shot_request/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_tariff_change/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_tariff_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2684 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_terminate/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_terminate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_lead_from_partner/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_lead_from_partner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11844 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10758 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_subscription_from_partner/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_subscription_from_partner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_remesa/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_remesa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_leads_validate/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_leads_validate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/import_payment_group/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/import_payment_group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/invoice_claim_1_send/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/invoice_claim_1_send/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/mail_compose_message/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/mail_compose_message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_email_change/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_email_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_confirm/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_confirm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/product_publish/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/product_publish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/product_publish/product_publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/test_mailing/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/test_mailing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    32533 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 09:29:33.000000 odoo12-addon-somconnexio-12.0.2.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5934 2023-06-06 09:04:25.000000 odoo12-addon-somconnexio-12.0.2.2.1/setup.py
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/PKG-INFO` & `odoo12-addon-somconnexio-12.0.2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-somconnexio
-Version: 12.0.2.2.0
+Version: 12.0.2.2.1
 Summary: Odoo Som Connexió customizations
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/README.md` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/README.md`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/__manifest__.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "name": "Odoo Som Connexió customizations",
-    "version": "12.0.2.2.0",
+    "version": "12.0.2.2.1",
     "depends": [
         "account_asset_management",
         "account_banking_sepa_credit_transfer",
         "account_banking_sepa_direct_debit",
         "account_cancel",
         "account_chart_update",
         "account_due_list",
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/controllers.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/controllers.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/http.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/http.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/controllers/public_controller.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/controllers/public_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/correos_services/shipment.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/correos_services/shipment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account.account.template-sc.csv` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account.account.template-sc.csv`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_chart_template_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_chart_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_group.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_group.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_journal.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_journal.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_payment_mode.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_payment_mode.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_payment_term.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_payment_term.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/account_tax.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/account_tax.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/analytic_account.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/base_automation.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/base_automation.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/company.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/company.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/contract_terminate_reason.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/contract_terminate_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/crm_stage_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/crm_stage_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/discovery_channel.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/discovery_channel.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/fiber_signal_type_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/fiber_signal_type_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/hr_attendance_place.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/hr_attendance_place.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/ir_config_pararameter.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/ir_config_pararameter.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/ir_sequence.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/ir_sequence.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/mail_activity_type.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/mail_activity_type.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/mis_report.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/mis_report.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/partner_action_tag_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/partner_action_tag_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/partner_priority.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/partner_priority.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/previous_provider_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/previous_provider_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_attribute.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_attribute.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_attribute_value.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_attribute_value.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_categories.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_categories.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_pack_line.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_pack_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_product.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_product.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/product_template_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/product_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/res_bank_data.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/res_bank_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/service_technology.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/service_technology.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/service_technology_service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/service_technology_service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/data/share_type.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/data/share_type.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/demo/partner.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/demo/partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/demo/pricelist.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/demo/pricelist.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/demo/subscription_requests.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/demo/subscription_requests.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/hooks.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/hooks.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/i18n/ca_ES.po` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/i18n/ca_ES.po`

 * *Files 0% similar despite different names*

```diff
@@ -1464,15 +1464,15 @@
 #: model:ir.model.fields,field_description:easy_my_coop.field_share_line__share_short_name
 #: model:ir.model.fields,field_description:easy_my_coop.field_subscription_register__share_short_name
 #: model:ir.model.fields,field_description:easy_my_coop.field_subscription_request__share_short_name
 msgid "Share type name"
 msgstr "Nom del tipus d'acció"
 
 #. module: somconnexio
-#: model:ir.model.fields,field_description:somconnexio.field_contract_contract__shared_bonds_contract_ids
+#: model:ir.model.fields,field_description:somconnexio.field_contract_contract__sharing_bond_contract_ids
 msgid "Shared Bond Mobile Contracts"
 msgstr "Contractes mòbil compartint dades"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__shared_bond_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__shared_bond_id
 msgid "Shared bond ID"
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/i18n/es.po` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/i18n/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -6236,15 +6236,15 @@
 
 #. module: somconnexio
 #: selection:res.partner,type:0
 msgid "Shipping address"
 msgstr "Dirección de envío"
 
 #. module: somconnexio
-#: model:ir.model.fields,field_description:somconnexio.field_contract_contract__shared_bonds_contract_ids
+#: model:ir.model.fields,field_description:somconnexio.field_contract_contract__sharing_bond_contract_ids
 msgid "Shared Bond Mobile Contracts"
 msgstr "Contratos móvil compartiendo datos"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__shared_bond_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__shared_bond_id
 msgid "Shared bond ID"
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/contract_line_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/contract_line_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/contract_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/contract_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/crm_lead_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/crm_lead_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/partner_bank_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/partner_bank_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/listeners/partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/listeners/partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/erppeek/README.md` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/erppeek/README.md`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/__init__.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_asset.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_asset.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_banking_mandate.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_banking_mandate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_invoice.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_invoice.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_invoice_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_invoice_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_move_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_payment_order.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_payment_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/aged_partner_balance.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/aged_partner_balance.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,21 +272,21 @@
         string="Number of pack contracts",
     )
     children_pack_contract_ids = fields.One2many(
         comodel_name='contract.contract',
         inverse_name='parent_pack_contract_id',
         string="Mobile contracts of pack",
     )
-    shared_bonds_contract_ids = fields.Many2many(
+    sharing_bond_contract_ids = fields.Many2many(
         comodel_name='contract.contract',
         relation="sharing_data_contracts",
         column1="id",
         column2="contract_id",
         string="Shared Bond Mobile Contracts",
-        compute='_compute_shared_bonds_contract_ids',
+        compute='_compute_sharing_bond_contract_ids',
         store=True,
     )
     shared_bond_id = fields.Char(
         'Shared bond ID',
         related='mobile_contract_service_info_id.shared_bond_id',
     )
 
@@ -298,40 +298,77 @@
         return res
 
     @api.depends("number_contracts_in_pack")
     def _compute_is_pack(self):
         for contract in self:
             contract.is_pack = bool(contract.number_contracts_in_pack)
 
-    @api.depends("children_pack_contract_ids", "parent_pack_contract_id")
+    @api.depends("children_pack_contract_ids", "parent_pack_contract_id",
+                 "sharing_bond_contract_ids")
     def _compute_number_contract_in_pack(self):
         for contract in self:
-            pack_contract_ids = [contract.id]
+            pack_contract_ids = []
             if contract.parent_pack_contract_id:
                 pack_contract_ids.append(contract.parent_pack_contract_id.id)
             if contract.children_pack_contract_ids:
                 pack_contract_ids.extend(contract.children_pack_contract_ids.ids)
+            if contract.sharing_bond_contract_ids:
+                pack_contract_ids.extend(contract.sharing_bond_contract_ids.ids)
+
+            if contract.id not in pack_contract_ids:
+                pack_contract_ids.append(contract.id)
 
             contract.number_contracts_in_pack = (
                 len(pack_contract_ids) if len(pack_contract_ids) > 1 else 0
             )
 
-    @api.depends("shared_bond_id", "shared_bonds_contract_ids.shared_bond_id")
-    def _compute_shared_bonds_contract_ids(self):
+    @api.depends("shared_bond_id")
+    def _compute_sharing_bond_contract_ids(self):
+        """
+        We use direct SQL commits here to ensure that Many2Many relation of
+        sharing_bond_contract_ids is stored in DB following both directions
+        ex:
+            id, contract_id
+             X,           Y
+             Y,           X
+
+        It will also be recomputed every time we edit the shared_bond_id
+        """
+
         for contract in self:
-            contracts_with_shared_bonds = (
-                self.env["contract.contract"].search(
-                    [
+            # DELETE from DB table sharing_data_contracts all instances with contract.id
+            self.env.cr.execute(
+                "DELETE FROM sharing_data_contracts WHERE id = %s or contract_id = %s",
+                (contract.id, contract.id)
+            )
+            if contract.shared_bond_id:
+                contracts_with_shared_bond = (
+                    self.env["contract.contract"].search([
                         ("is_terminated", "=", False),
+                        (
+                            "service_technology_id",
+                            "=",
+                            self.env.ref("somconnexio.service_technology_mobile").id,
+                        ),
                         ("shared_bond_id", "=", contract.shared_bond_id),
-                    ]
+
+                    ])
                 )
-            )
-            for c in contracts_with_shared_bonds:
-                c.shared_bonds_contract_ids = contracts_with_shared_bonds
+
+                # Assign matching contracts according to their "shared_bond_id"
+                contract.sharing_bond_contract_ids = [
+                    (6, 0, contracts_with_shared_bond.ids)
+                ]
+
+                # INSERT to DB table sharing_data_contracts missing relation
+                for sharing_contract_id in contracts_with_shared_bond.ids:
+                    self.env.cr.execute(
+                        "INSERT INTO sharing_data_contracts VALUES (%s, %s)",
+                        (sharing_contract_id, contract.id)
+                    )
 
     def _compute_mail_activity_count(self):
         for contract in self:
             count = self.env['mail.activity'].search_count([
                 ('res_id', '=', contract.id),
                 ('res_model', '=', 'contract.contract')
             ])
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/base.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/broadband.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/broadband.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/contract_info/mobile.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/contract_info/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/coop_agreement.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/coop_agreement.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/crm_lead.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/hr_employee.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/hr_employee.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/ir_model_data.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/ir_model_data.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/ir_server_action.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/ir_server_action.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/base.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/broadband.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/broadband.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/isp_info/mobile.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/isp_info/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/l10n_es_aeat_report.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/l10n_es_aeat_report.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/mail_activity.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/mail_activity.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/mass_mailing.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/mass_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/opencell_configuration.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/opencell_configuration.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/partner_action_tag.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/partner_action_tag.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/partner_otrs_view.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/partner_otrs_view.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/payment_return.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/payment_return.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/payment_return_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/payment_return_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_product.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_product.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/product_template.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/product_template.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/res_company.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/res_company.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/res_partner.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/stock_move_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/stock_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/stock_production_lot.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/stock_production_lot.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/models/subscription_request.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/customer.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/customer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/services.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/services.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_models/subscription.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_models/subscription.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/customer_update_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/customer_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/opencell_services/subscription_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/opencell_services/subscription_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/account_asset_report_xls.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/account_asset_report_xls.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/aged_partner_balance.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/aged_partner_balance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/report_paperformat.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/report_paperformat.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/security/ir.model.access.csv` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/__init__.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/account_invoice_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/account_invoice_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/account_payment_group_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/account_payment_group_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/bank_from_iban_getter.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/bank_from_iban_getter.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/change_partner_emails.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/change_partner_emails.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_change_tariff_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_change_tariff_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_contract_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_contract_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_email_change_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_email_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_iban_change_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_iban_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_one_shot_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_one_shot_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/adsl.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/adsl.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/ba.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/ba.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/base.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/fiber.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/fiber.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/mobile.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/contract_process/router4g.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/contract_process/router4g.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/crm_lead_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/discovery_channel_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/discovery_channel_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/get_activation_date.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/get_activation_date.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/partner_email_change_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/partner_email_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/product_catalog_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/product_catalog_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/provider_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/provider_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/res_partner_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/res_partner_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/schemas.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/schemas.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/services/subscription_request_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/services/subscription_request_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/somoffice/user.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/somoffice/user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/activities.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/activities.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/broadband_contract.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/broadband_contract.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/broadband_lead_lines.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/broadband_lead_lines.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/emails.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/emails.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/mobile_contract.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/mobile_contract.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/mobile_lead_lines.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/mobile_lead_lines.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/description/packs.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/description/packs.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/img/sc-image.png` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/img/sc-image.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/js/my_attendances.js` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/js/my_attendances.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/static/src/xml/attendance.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/static/src/xml/attendance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/__init__.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/common_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/common_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/correos_services/test_shipment.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/correos_services/test_shipment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/factories.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/factories.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/helpers.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_invoice.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_invoice.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_move_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_payment_order.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_payment_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_contract.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,15 +654,15 @@
         contract = self.Contract.create(vals_contract)
         self.assertEquals(contract.parent_pack_contract_id, parent_contract)
         self.assertEquals(parent_contract.children_pack_contract_ids, contract)
         self.assertEquals(parent_contract.number_contracts_in_pack, 2)
         self.assertTrue(contract.is_pack)
         self.assertTrue(parent_contract.is_pack)
 
-    def test_shared_bonds_contract_ids(self, *args):
+    def test_sharing_bond_contract_ids(self, *args):
         partner_id = self.partner.id
         shared_bond_id = 'ABCDEFGHI'
 
         ba_vals_contract = {
             'name': 'Test Contract Broadband',
             'partner_id': partner_id,
             'service_partner_id': self.service_partner.id,
@@ -707,33 +707,33 @@
         self.assertEquals(fiber_contract.children_pack_contract_ids, mbl_1_contract)
         self.assertEquals(fiber_contract.number_contracts_in_pack, 2)
 
         # Create second mobile contract sharing data with the first one
         mbl_vals_contract['mobile_contract_service_info_id'] = msci.copy().id
         mbl_2_contract = self.Contract.create(mbl_vals_contract)
 
-        self.assertTrue(mbl_2_contract.shared_bonds_contract_ids)
+        self.assertTrue(mbl_2_contract.sharing_bond_contract_ids)
         self.assertEquals(
-            mbl_2_contract.shared_bonds_contract_ids.ids,
+            mbl_2_contract.sharing_bond_contract_ids.ids,
             [mbl_1_contract.id, mbl_2_contract.id]
         )
         self.assertEquals(
             fiber_contract.children_pack_contract_ids.ids,
             [mbl_1_contract.id, mbl_2_contract.id]
         )
         self.assertEquals(fiber_contract.number_contracts_in_pack, 3)
 
         # Create third mobile contract sharing data with the other two
         mbl_vals_contract['mobile_contract_service_info_id'] = msci.copy().id
         mbl_3_contract = self.Contract.create(mbl_vals_contract)
 
-        self.assertTrue(mbl_3_contract.shared_bonds_contract_ids)
-        self.assertEquals(len(mbl_3_contract.shared_bonds_contract_ids), 3)
+        self.assertTrue(mbl_3_contract.sharing_bond_contract_ids)
+        self.assertEquals(len(mbl_3_contract.sharing_bond_contract_ids), 3)
         self.assertEquals(
-            mbl_3_contract.shared_bonds_contract_ids.ids,
+            mbl_3_contract.sharing_bond_contract_ids.ids,
             [mbl_1_contract.id, mbl_2_contract.id, mbl_3_contract.id]
         )
         self.assertEquals(
             fiber_contract.children_pack_contract_ids.ids,
             [mbl_1_contract.id, mbl_2_contract.id, mbl_3_contract.id]
         )
         self.assertEquals(fiber_contract.number_contracts_in_pack, 4)
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_coop_agreement.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_coop_agreement.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_crm_lead.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_mail_activity.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_mail_activity.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_mass_mailing.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_mass_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_payment_return.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_payment_return.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_previous_provider.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_previous_provider.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_product_product.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_product_product.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_product_template.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_product_template.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_production_lot.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_production_lot.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_server_action.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_server_action.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_service_supplier.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_service_supplier.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_stock_move_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_stock_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/models/test_subscription_request.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/models/test_subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_address.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_address.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_customer.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_customer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/sc_test_case.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/sc_test_case.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_get_activation_date.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_get_activation_date.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_provider_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_provider_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_res_partner_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_res_partner_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/somoffice/test_user.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/somoffice/test_user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_asset_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_asset_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_invoice_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_invoice_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_move.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_move.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_move_line.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_move_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/account_payment_order_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/account_payment_order_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/aeat_report_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/aeat_report_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/broadband_isp_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/broadband_isp_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/contract_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/contract_view.xml`

 * *Files 0% similar despite different names*

#### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/contract_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/contract_view.xml`

```diff
@@ -343,17 +343,19 @@
     <field name="name">Pack contracts</field>
     <field name="res_model">contract.contract</field>
     <field name="view_type">form</field>
     <field name="view_mode">tree,form</field>
     <field name="domain">[
         '|',
         '|',
+        '|',
         ('id', 'in', [active_id]),
         ('parent_pack_contract_id', 'in', [active_id]),
         ('children_pack_contract_ids', 'in', [active_id]),
+        ('sharing_bond_contract_ids', 'in', [active_id]),
       ]</field>
   </record>
   <record id="act_contract_contract_pack_related_contracts_view_tree" model="ir.actions.act_window.view">
     <field name="sequence">0</field>
     <field name="view_mode">tree</field>
     <field name="view_id" ref="contract_contract_pack_related_contracts_tree"/>
     <field name="act_window_id" ref="act_contract_contract_pack_related_contracts"/>
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/coop_agreement_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/coop_agreement_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/crm_lead.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/crm_lead.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/crm_lead_line.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/crm_lead_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/hr_attendance.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/hr_attendance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/ir_action_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/ir_action_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mail_activity_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mail_activity_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/menus.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/menus.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mis_budget_item_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mis_budget_item_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mobile_isp_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mobile_isp_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/open_boards_activities.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/open_boards_activities.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/operation_request.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/operation_request.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/partner_action_tag_views.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/partner_action_tag_views.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/payment_return_import_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/payment_return_import_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/payment_return_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/payment_return_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/previous_provider_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/previous_provider_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_attribute_views.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_attribute_views.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_pricelist_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_pricelist_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/product_product_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/product_product_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/res_company_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/res_company_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/res_partner_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/service_technology_service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/service_technology_service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/stock_move_line_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/stock_move_line_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/subscription_request_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/subscription_request_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/templates_js.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/templates_js.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/__init__.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/product_publish/product_publish.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/PKG-INFO` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-somconnexio
-Version: 12.0.2.2.0
+Version: 12.0.2.2.1
 Summary: Odoo Som Connexió customizations
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/SOURCES.txt` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/odoo12_addon_somconnexio.egg-info/requires.txt` & `odoo12-addon-somconnexio-12.0.2.2.1/odoo12_addon_somconnexio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.0/setup.py` & `odoo12-addon-somconnexio-12.0.2.2.1/setup.py`

 * *Files identical despite different names*

