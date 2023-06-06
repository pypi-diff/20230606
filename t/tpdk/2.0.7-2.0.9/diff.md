# Comparing `tmp/tpdk-2.0.7.tar.gz` & `tmp/tpdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpdk-2.0.7.tar", last modified: Mon Jun  5 15:35:17 2023, max compression
+gzip compressed data, was "tpdk-2.0.9.tar", last modified: Tue Jun  6 13:55:00 2023, max compression
```

## Comparing `tpdk-2.0.7.tar` & `tpdk-2.0.9.tar`

### file list

```diff
@@ -1,209 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.973115 tpdk-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-05 15:35:17.977115 tpdk-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20037 2023-06-05 15:35:09.000000 tpdk-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-05 15:35:09.000000 tpdk-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:35:17.977115 tpdk-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-05 15:35:09.000000 tpdk-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.961115 tpdk-2.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_ai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_ai_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_branding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evaluation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evaluation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence_read_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_media_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_independent_write_seller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_update_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_write_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_independent_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_persona_auth_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_persona_external_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_post_auth_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_read_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_update_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_resolution_center_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_safe_checkout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_transaction_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_transaction_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_transaction_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_unprocessable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_unprocessable_entity_violations_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_email_validation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_post_register_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_support_read_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_write_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_history_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_history_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_subscription_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_subscription_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.961115 tpdk-2.0.7/tpdk/
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.965115 tpdk-2.0.7/tpdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/ai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/branding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30230 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50992 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/persona_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   107228 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/resolution_center_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   158178 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/safe_checkout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41484 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.973115 tpdk-2.0.7/tpdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/ai_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evaluation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evaluation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence_read_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/media_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/notification_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/notification_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_independent_write_seller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_update_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_write_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel_write.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_independent_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_persona_auth_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_persona_external_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_post_auth_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_read_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_update_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/transaction_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/transaction_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/transaction_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/unprocessable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/unprocessable_entity_violations_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_email_validation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_post_register_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_support_read_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_write_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_history_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_history_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_subscription_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_subscription_write.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.961115 tpdk-2.0.7/tpdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:55:00.737979 tpdk-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-06 13:55:00.737979 tpdk-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20059 2023-06-06 13:54:52.000000 tpdk-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-06 13:54:52.000000 tpdk-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 13:55:00.741979 tpdk-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-06 13:54:52.000000 tpdk-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:55:00.717979 tpdk-2.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_address_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_address_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_address_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_address_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_ai_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_dispute_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_dispute_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_dispute_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_dispute_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_dispute_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_evaluation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_evaluation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_evidence_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_evidence_read_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_evidence_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_media_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_metadata_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_metadata_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_metadata_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_metadata_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_notification_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_notification_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer_independent_write_seller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_offer_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_organization_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_organization_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_organization_update_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_organization_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_organization_write_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_parcel_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_parcel_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_parcel_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_auth_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_external_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_independent_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_post_auth_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_read_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_token_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_update_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_persona_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_resolution_center_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_safe_checkout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_transaction_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_transaction_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_transaction_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_unprocessable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_unprocessable_entity_violations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user_email_validation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user_post_register_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user_support_read_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_user_write_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_webhook_history_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_webhook_history_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_webhook_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_webhook_subscription_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-06 13:54:52.000000 tpdk-2.0.9/test/test_webhook_subscription_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:55:00.717979 tpdk-2.0.9/tpdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:55:00.721979 tpdk-2.0.9/tpdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30230 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51146 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/persona_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107228 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/resolution_center_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158178 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/safe_checkout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41127 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41484 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api/webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:55:00.737979 tpdk-2.0.9/tpdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/address_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/address_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/address_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/address_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/ai_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/dispute_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/dispute_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/dispute_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/dispute_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/dispute_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/evaluation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/evaluation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/evidence_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/evidence_read_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/evidence_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/media_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/metadata_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/metadata_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/metadata_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/metadata_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/notification_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/notification_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer_independent_write_seller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/offer_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/organization_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/organization_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/organization_update_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/organization_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/organization_write_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/parcel_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/parcel_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/parcel_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_auth_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_external_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_independent_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_post_auth_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_read_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_token_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_update_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/persona_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/transaction_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/transaction_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/transaction_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/unprocessable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/unprocessable_entity_violations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user_email_validation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user_post_register_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user_support_read_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/user_write_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/webhook_history_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/webhook_history_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/webhook_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/webhook_subscription_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/models/webhook_subscription_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-06-06 13:54:52.000000 tpdk-2.0.9/tpdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:55:00.721979 tpdk-2.0.9/tpdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-06 13:55:00.000000 tpdk-2.0.9/tpdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-06 13:55:00.000000 tpdk-2.0.9/tpdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:55:00.000000 tpdk-2.0.9/tpdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 13:55:00.000000 tpdk-2.0.9/tpdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 13:55:00.000000 tpdk-2.0.9/tpdk.egg-info/top_level.txt
```

### Comparing `tpdk-2.0.7/README.md` & `tpdk-2.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tpdk
 Our API suite for the **Resolution Center** and the **Safe Checkout** features.
 Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.7
-- Package version: 2.0.7
+- API version: 2.0.9
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://tripartie.com](https://tripartie.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -218,24 +218,25 @@
  - [OrganizationWriteBillingAddress](docs/OrganizationWriteBillingAddress.md)
  - [Parcel](docs/Parcel.md)
  - [ParcelIndependentWrite](docs/ParcelIndependentWrite.md)
  - [ParcelRead](docs/ParcelRead.md)
  - [ParcelWrite](docs/ParcelWrite.md)
  - [Persona](docs/Persona.md)
  - [PersonaAddress](docs/PersonaAddress.md)
+ - [PersonaAuthReturn](docs/PersonaAuthReturn.md)
  - [PersonaCollectionRead](docs/PersonaCollectionRead.md)
+ - [PersonaExternalAuth](docs/PersonaExternalAuth.md)
  - [PersonaIndependentWrite](docs/PersonaIndependentWrite.md)
  - [PersonaIndependentWriteAddress](docs/PersonaIndependentWriteAddress.md)
- - [PersonaPersonaAuthReturn](docs/PersonaPersonaAuthReturn.md)
- - [PersonaPersonaExternalAuth](docs/PersonaPersonaExternalAuth.md)
  - [PersonaPostAuthRead](docs/PersonaPostAuthRead.md)
  - [PersonaRead](docs/PersonaRead.md)
  - [PersonaReadAddress](docs/PersonaReadAddress.md)
  - [PersonaRegister](docs/PersonaRegister.md)
  - [PersonaToken](docs/PersonaToken.md)
+ - [PersonaTokenWrite](docs/PersonaTokenWrite.md)
  - [PersonaUpdate](docs/PersonaUpdate.md)
  - [PersonaUpdateAddress](docs/PersonaUpdateAddress.md)
  - [PersonaWrite](docs/PersonaWrite.md)
  - [PersonaWriteAddress](docs/PersonaWriteAddress.md)
  - [TransactionCollectionRead](docs/TransactionCollectionRead.md)
  - [TransactionIndependentWrite](docs/TransactionIndependentWrite.md)
  - [TransactionRead](docs/TransactionRead.md)
```

### Comparing `tpdk-2.0.7/pyproject.toml` & `tpdk-2.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tpdk"
-version = "2.0.7"
+version = "2.0.9"
 description = "Tripartie"
 authors = ["Tripartie SAS <noc@tripartie.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/tripartie/tpdk"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Tripartie"]
```

### Comparing `tpdk-2.0.7/setup.py` & `tpdk-2.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "tpdk"
-VERSION = "2.0.7"
+VERSION = "2.0.9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `tpdk-2.0.7/test/test_address.py` & `tpdk-2.0.9/test/test_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_address_independent_write.py` & `tpdk-2.0.9/test/test_address_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_address_read.py` & `tpdk-2.0.9/test/test_address_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_address_update.py` & `tpdk-2.0.9/test/test_address_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_address_write.py` & `tpdk-2.0.9/test/test_address_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_ai_api.py` & `tpdk-2.0.9/test/test_ai_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_ai_hint.py` & `tpdk-2.0.9/test/test_ai_hint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_api_client.py` & `tpdk-2.0.9/test/test_api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_branding_api.py` & `tpdk-2.0.9/test/test_branding_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_dispute.py` & `tpdk-2.0.9/test/test_dispute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_dispute_collection_read.py` & `tpdk-2.0.9/test/test_dispute_collection_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_dispute_independent_write.py` & `tpdk-2.0.9/test/test_dispute_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_dispute_post_creation_read.py` & `tpdk-2.0.9/test/test_dispute_post_creation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_dispute_read.py` & `tpdk-2.0.9/test/test_dispute_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_dispute_update.py` & `tpdk-2.0.9/test/test_dispute_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_dispute_write.py` & `tpdk-2.0.9/test/test_dispute_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_evaluation_read.py` & `tpdk-2.0.9/test/test_evaluation_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_evaluation_write.py` & `tpdk-2.0.9/test/test_evaluation_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_evidence.py` & `tpdk-2.0.9/test/test_evidence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_evidence_read.py` & `tpdk-2.0.9/test/test_evidence_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_evidence_read_media.py` & `tpdk-2.0.9/test/test_evidence_read_media.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_evidence_write.py` & `tpdk-2.0.9/test/test_evidence_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_media.py` & `tpdk-2.0.9/test/test_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_media_read.py` & `tpdk-2.0.9/test/test_media_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_message.py` & `tpdk-2.0.9/test/test_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_metadata.py` & `tpdk-2.0.9/test/test_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_metadata_independent_write.py` & `tpdk-2.0.9/test/test_metadata_independent_write.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_metadata_read.py` & `tpdk-2.0.9/test/test_metadata_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_metadata_update.py` & `tpdk-2.0.9/test/test_metadata_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_metadata_write.py` & `tpdk-2.0.9/test/test_metadata_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_notification.py` & `tpdk-2.0.9/test/test_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_notification_api.py` & `tpdk-2.0.9/test/test_notification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_notification_read.py` & `tpdk-2.0.9/test/test_notification_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_notification_update.py` & `tpdk-2.0.9/test/test_notification_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer.py` & `tpdk-2.0.9/test/test_offer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer_collection_read.py` & `tpdk-2.0.9/test/test_offer_collection_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer_independent_write.py` & `tpdk-2.0.9/test/test_offer_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer_independent_write_seller.py` & `tpdk-2.0.9/test/test_offer_independent_write_seller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer_post_creation_read.py` & `tpdk-2.0.9/test/test_offer_post_creation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer_read.py` & `tpdk-2.0.9/test/test_offer_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer_update.py` & `tpdk-2.0.9/test/test_offer_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_offer_write.py` & `tpdk-2.0.9/test/test_offer_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_organization_read.py` & `tpdk-2.0.9/test/test_organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_organization_support_read.py` & `tpdk-2.0.9/test/test_organization_support_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_organization_update.py` & `tpdk-2.0.9/test/test_organization_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_organization_update_billing_address.py` & `tpdk-2.0.9/test/test_organization_update_billing_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_organization_write.py` & `tpdk-2.0.9/test/test_organization_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_organization_write_billing_address.py` & `tpdk-2.0.9/test/test_organization_write_billing_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_parcel.py` & `tpdk-2.0.9/test/test_parcel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_parcel_independent_write.py` & `tpdk-2.0.9/test/test_parcel_independent_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_parcel_read.py` & `tpdk-2.0.9/test/test_parcel_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_parcel_write.py` & `tpdk-2.0.9/test/test_parcel_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona.py` & `tpdk-2.0.9/test/test_persona.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_address.py` & `tpdk-2.0.9/test/test_persona_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_api.py` & `tpdk-2.0.9/test/test_persona_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_collection_read.py` & `tpdk-2.0.9/test/test_persona_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_independent_write.py` & `tpdk-2.0.9/test/test_persona_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_independent_write_address.py` & `tpdk-2.0.9/test/test_persona_independent_write_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_persona_auth_return.py` & `tpdk-2.0.9/test/test_persona_auth_return.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import tpdk
-from tpdk.models.persona_persona_auth_return import PersonaPersonaAuthReturn  # noqa: E501
+from tpdk.models.persona_auth_return import PersonaAuthReturn  # noqa: E501
 from tpdk.rest import ApiException
 
-class TestPersonaPersonaAuthReturn(unittest.TestCase):
-    """PersonaPersonaAuthReturn unit test stubs"""
+class TestPersonaAuthReturn(unittest.TestCase):
+    """PersonaAuthReturn unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PersonaPersonaAuthReturn
+        """Test PersonaAuthReturn
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PersonaPersonaAuthReturn`
+        # uncomment below to create an instance of `PersonaAuthReturn`
         """
-        model = tpdk.models.persona_persona_auth_return.PersonaPersonaAuthReturn()  # noqa: E501
+        model = tpdk.models.persona_auth_return.PersonaAuthReturn()  # noqa: E501
         if include_optional :
-            return PersonaPersonaAuthReturn(
+            return PersonaAuthReturn(
                 auth_url = 'https://next.tripartie.app/?d=01ARZ3NDEKTSV4RRFFQ69G5FAV&t=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MTIzNDU2Nzg5LCJuYW1lIjoiSm9zZXBoIn0.OpOSSw7e485LOP5PrzScxHb7SR6sAOMRckfFwi4rp7o', 
                 expire_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
-            return PersonaPersonaAuthReturn(
+            return PersonaAuthReturn(
         )
         """
 
-    def testPersonaPersonaAuthReturn(self):
-        """Test PersonaPersonaAuthReturn"""
+    def testPersonaAuthReturn(self):
+        """Test PersonaAuthReturn"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tpdk-2.0.7/test/test_persona_persona_external_auth.py` & `tpdk-2.0.9/test/test_persona_register.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import tpdk
-from tpdk.models.persona_persona_external_auth import PersonaPersonaExternalAuth  # noqa: E501
+from tpdk.models.persona_register import PersonaRegister  # noqa: E501
 from tpdk.rest import ApiException
 
-class TestPersonaPersonaExternalAuth(unittest.TestCase):
-    """PersonaPersonaExternalAuth unit test stubs"""
+class TestPersonaRegister(unittest.TestCase):
+    """PersonaRegister unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PersonaPersonaExternalAuth
+        """Test PersonaRegister
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PersonaPersonaExternalAuth`
+        # uncomment below to create an instance of `PersonaRegister`
         """
-        model = tpdk.models.persona_persona_external_auth.PersonaPersonaExternalAuth()  # noqa: E501
+        model = tpdk.models.persona_register.PersonaRegister()  # noqa: E501
         if include_optional :
-            return PersonaPersonaExternalAuth(
+            return PersonaRegister(
                 captcha = '', 
-                target_url = 'https://next.tripartie.app/?d=01ARZ3NDEKTSV4RRFFQ69G5FAV', 
                 plain_password = 'secr$t', 
+                first_name = 'John', 
+                last_name = 'Doe', 
+                gender = 'RATHER_NOT_SAY', 
+                date_of_birth = datetime.datetime.strptime('1975-12-30', '%Y-%m-%d').date(), 
+                language = 'FR', 
                 email = 'john.doe@gmail.com', 
                 mobile_phone_number = '+33700000000'
             )
         else :
-            return PersonaPersonaExternalAuth(
+            return PersonaRegister(
         )
         """
 
-    def testPersonaPersonaExternalAuth(self):
-        """Test PersonaPersonaExternalAuth"""
+    def testPersonaRegister(self):
+        """Test PersonaRegister"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tpdk-2.0.7/test/test_persona_post_auth_read.py` & `tpdk-2.0.9/test/test_persona_post_auth_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_read.py` & `tpdk-2.0.9/test/test_persona_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_read_address.py` & `tpdk-2.0.9/test/test_persona_read_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_register.py` & `tpdk-2.0.9/test/test_user_write.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import tpdk
-from tpdk.models.persona_register import PersonaRegister  # noqa: E501
+from tpdk.models.user_write import UserWrite  # noqa: E501
 from tpdk.rest import ApiException
 
-class TestPersonaRegister(unittest.TestCase):
-    """PersonaRegister unit test stubs"""
+class TestUserWrite(unittest.TestCase):
+    """UserWrite unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PersonaRegister
+        """Test UserWrite
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PersonaRegister`
+        # uncomment below to create an instance of `UserWrite`
         """
-        model = tpdk.models.persona_register.PersonaRegister()  # noqa: E501
+        model = tpdk.models.user_write.UserWrite()  # noqa: E501
         if include_optional :
-            return PersonaRegister(
+            return UserWrite(
                 captcha = '', 
+                first_name = 'Jacob', 
+                last_name = 'TAHRI', 
+                public_name = 'Nickname', 
+                role_in_company = 'Accounting Dpt', 
+                birthday = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                email = '', 
                 plain_password = 'secr$t', 
-                first_name = 'John', 
-                last_name = 'Doe', 
-                gender = 'RATHER_NOT_SAY', 
-                date_of_birth = datetime.datetime.strptime('1975-12-30', '%Y-%m-%d').date(), 
-                language = 'FR', 
-                email = 'john.doe@gmail.com', 
-                mobile_phone_number = '+33700000000'
+                intl_phone_number = '+33700000000', 
+                origin_country = 'FRA', 
+                preferred_language = 'FR', 
+                consent_mail_notification = True, 
+                consent_mail_ads = True, 
+                organization = None
             )
         else :
-            return PersonaRegister(
+            return UserWrite(
+                first_name = 'Jacob',
+                last_name = 'TAHRI',
+                public_name = 'Nickname',
+                role_in_company = 'Accounting Dpt',
+                email = '',
+                plain_password = 'secr$t',
+                origin_country = 'FRA',
+                preferred_language = 'FR',
         )
         """
 
-    def testPersonaRegister(self):
-        """Test PersonaRegister"""
+    def testUserWrite(self):
+        """Test UserWrite"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tpdk-2.0.7/test/test_persona_token.py` & `tpdk-2.0.9/test/test_persona_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_update.py` & `tpdk-2.0.9/test/test_persona_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_update_address.py` & `tpdk-2.0.9/test/test_persona_update_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_write.py` & `tpdk-2.0.9/test/test_persona_write.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_persona_write_address.py` & `tpdk-2.0.9/test/test_persona_write_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_resolution_center_api.py` & `tpdk-2.0.9/test/test_resolution_center_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_safe_checkout_api.py` & `tpdk-2.0.9/test/test_safe_checkout_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_transaction_collection_read.py` & `tpdk-2.0.9/test/test_transaction_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_transaction_independent_write.py` & `tpdk-2.0.9/test/test_transaction_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_transaction_read.py` & `tpdk-2.0.9/test/test_transaction_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_unprocessable_entity.py` & `tpdk-2.0.9/test/test_unprocessable_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_unprocessable_entity_violations_inner.py` & `tpdk-2.0.9/test/test_unprocessable_entity_violations_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_user.py` & `tpdk-2.0.9/test/test_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_user_api.py` & `tpdk-2.0.9/test/test_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_user_email_validation_write.py` & `tpdk-2.0.9/test/test_user_email_validation_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_user_post_register_read.py` & `tpdk-2.0.9/test/test_user_post_register_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_user_support_read.py` & `tpdk-2.0.9/test/test_user_support_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_user_support_read_organization.py` & `tpdk-2.0.9/test/test_user_support_read_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_user_write.py` & `tpdk-2.0.9/test/test_view.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,64 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import tpdk
-from tpdk.models.user_write import UserWrite  # noqa: E501
+from tpdk.models.view import View  # noqa: E501
 from tpdk.rest import ApiException
 
-class TestUserWrite(unittest.TestCase):
-    """UserWrite unit test stubs"""
+class TestView(unittest.TestCase):
+    """View unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UserWrite
+        """Test View
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UserWrite`
+        # uncomment below to create an instance of `View`
         """
-        model = tpdk.models.user_write.UserWrite()  # noqa: E501
+        model = tpdk.models.view.View()  # noqa: E501
         if include_optional :
-            return UserWrite(
-                captcha = '', 
-                first_name = 'Jacob', 
-                last_name = 'TAHRI', 
-                public_name = 'Nickname', 
-                role_in_company = 'Accounting Dpt', 
-                birthday = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                email = '', 
-                plain_password = 'secr$t', 
-                intl_phone_number = '+33700000000', 
-                origin_country = 'FRA', 
-                preferred_language = 'FR', 
-                consent_mail_notification = True, 
-                consent_mail_ads = True, 
-                organization = None
+            return View(
+                id = 56, 
+                ip_address = '', 
+                offer = '', 
+                dispute = '', 
+                persona = '', 
+                user = '', 
+                hit_count = 1, 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
-            return UserWrite(
-                first_name = 'Jacob',
-                last_name = 'TAHRI',
-                public_name = 'Nickname',
-                role_in_company = 'Accounting Dpt',
-                email = '',
-                plain_password = 'secr$t',
-                origin_country = 'FRA',
-                preferred_language = 'FR',
+            return View(
+                ip_address = '',
+                hit_count = 1,
         )
         """
 
-    def testUserWrite(self):
-        """Test UserWrite"""
+    def testView(self):
+        """Test View"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tpdk-2.0.7/test/test_user_write_organization.py` & `tpdk-2.0.9/test/test_user_write_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_view.py` & `tpdk-2.0.9/test/test_webhook_history_read.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import tpdk
-from tpdk.models.view import View  # noqa: E501
+from tpdk.models.webhook_history_read import WebhookHistoryRead  # noqa: E501
 from tpdk.rest import ApiException
 
-class TestView(unittest.TestCase):
-    """View unit test stubs"""
+class TestWebhookHistoryRead(unittest.TestCase):
+    """WebhookHistoryRead unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test View
+        """Test WebhookHistoryRead
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `View`
+        # uncomment below to create an instance of `WebhookHistoryRead`
         """
-        model = tpdk.models.view.View()  # noqa: E501
+        model = tpdk.models.webhook_history_read.WebhookHistoryRead()  # noqa: E501
         if include_optional :
-            return View(
-                id = 56, 
-                ip_address = '', 
-                offer = '', 
-                dispute = '', 
-                persona = '', 
-                user = '', 
-                hit_count = 1, 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+            return WebhookHistoryRead(
+                event = 'dispute.opened', 
+                url = '', 
+                response_code = 56, 
+                response_body = '', 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                attempted_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                retry_count = 56
             )
         else :
-            return View(
-                ip_address = '',
-                hit_count = 1,
+            return WebhookHistoryRead(
+                event = 'dispute.opened',
+                url = '',
+                response_code = 56,
+                response_body = '',
+                retry_count = 56,
         )
         """
 
-    def testView(self):
-        """Test View"""
+    def testWebhookHistoryRead(self):
+        """Test WebhookHistoryRead"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tpdk-2.0.7/test/test_webhook.py` & `tpdk-2.0.9/test/test_webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_webhook_api.py` & `tpdk-2.0.9/test/test_webhook_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_webhook_history_collection_read.py` & `tpdk-2.0.9/test/test_webhook_history_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_webhook_object.py` & `tpdk-2.0.9/test/test_webhook_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_webhook_subscription_read.py` & `tpdk-2.0.9/test/test_webhook_subscription_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/test/test_webhook_subscription_write.py` & `tpdk-2.0.9/test/test_webhook_subscription_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/__init__.py` & `tpdk-2.0.9/tpdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.9"
 
 # import apis into sdk package
 from tpdk.api.ai_api import AIApi
 from tpdk.api.branding_api import BrandingApi
 from tpdk.api.notification_api import NotificationApi
 from tpdk.api.persona_api import PersonaApi
 from tpdk.api.resolution_center_api import ResolutionCenterApi
@@ -86,24 +86,25 @@
 from tpdk.models.organization_write_billing_address import OrganizationWriteBillingAddress
 from tpdk.models.parcel import Parcel
 from tpdk.models.parcel_independent_write import ParcelIndependentWrite
 from tpdk.models.parcel_read import ParcelRead
 from tpdk.models.parcel_write import ParcelWrite
 from tpdk.models.persona import Persona
 from tpdk.models.persona_address import PersonaAddress
+from tpdk.models.persona_auth_return import PersonaAuthReturn
 from tpdk.models.persona_collection_read import PersonaCollectionRead
+from tpdk.models.persona_external_auth import PersonaExternalAuth
 from tpdk.models.persona_independent_write import PersonaIndependentWrite
 from tpdk.models.persona_independent_write_address import PersonaIndependentWriteAddress
-from tpdk.models.persona_persona_auth_return import PersonaPersonaAuthReturn
-from tpdk.models.persona_persona_external_auth import PersonaPersonaExternalAuth
 from tpdk.models.persona_post_auth_read import PersonaPostAuthRead
 from tpdk.models.persona_read import PersonaRead
 from tpdk.models.persona_read_address import PersonaReadAddress
 from tpdk.models.persona_register import PersonaRegister
 from tpdk.models.persona_token import PersonaToken
+from tpdk.models.persona_token_write import PersonaTokenWrite
 from tpdk.models.persona_update import PersonaUpdate
 from tpdk.models.persona_update_address import PersonaUpdateAddress
 from tpdk.models.persona_write import PersonaWrite
 from tpdk.models.persona_write_address import PersonaWriteAddress
 from tpdk.models.transaction_collection_read import TransactionCollectionRead
 from tpdk.models.transaction_independent_write import TransactionIndependentWrite
 from tpdk.models.transaction_read import TransactionRead
```

### Comparing `tpdk-2.0.7/tpdk/api/ai_api.py` & `tpdk-2.0.9/tpdk/api/ai_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/api/branding_api.py` & `tpdk-2.0.9/tpdk/api/branding_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/api/notification_api.py` & `tpdk-2.0.9/tpdk/api/notification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/api/persona_api.py` & `tpdk-2.0.9/tpdk/api/persona_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -23,14 +23,15 @@
 from pydantic import Field, StrictInt, StrictStr, conlist
 
 from typing import List, Optional
 
 from tpdk.models.persona_collection_read import PersonaCollectionRead
 from tpdk.models.persona_post_auth_read import PersonaPostAuthRead
 from tpdk.models.persona_read import PersonaRead
+from tpdk.models.persona_token_write import PersonaTokenWrite
 from tpdk.models.persona_update import PersonaUpdate
 from tpdk.models.persona_write import PersonaWrite
 
 from tpdk.api_client import ApiClient
 from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
@@ -746,59 +747,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def api_personas_idtoken_post(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_write : Annotated[PersonaWrite, Field(..., description="The new Persona resource")], **kwargs) -> PersonaPostAuthRead:  # noqa: E501
+    def api_personas_idtoken_post(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_token_write : Annotated[PersonaTokenWrite, Field(..., description="The new Persona resource")], **kwargs) -> PersonaPostAuthRead:  # noqa: E501
         """Issue authenticated URL for single end-user  # noqa: E501
 
         Without this, your users may be required to pass a MFA challenge even if they are already logged-in from your website. Pass the URL you wish your user access, either a Dispute or Safe-checkout resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personas_idtoken_post(id, persona_write, async_req=True)
+        >>> thread = api.api_personas_idtoken_post(id, persona_token_write, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
-        :param persona_write: The new Persona resource (required)
-        :type persona_write: PersonaWrite
+        :param persona_token_write: The new Persona resource (required)
+        :type persona_token_write: PersonaTokenWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: PersonaPostAuthRead
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the api_personas_idtoken_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.api_personas_idtoken_post_with_http_info(id, persona_write, **kwargs)  # noqa: E501
+        return self.api_personas_idtoken_post_with_http_info(id, persona_token_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_idtoken_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_write : Annotated[PersonaWrite, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
+    def api_personas_idtoken_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_token_write : Annotated[PersonaTokenWrite, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Issue authenticated URL for single end-user  # noqa: E501
 
         Without this, your users may be required to pass a MFA challenge even if they are already logged-in from your website. Pass the URL you wish your user access, either a Dispute or Safe-checkout resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personas_idtoken_post_with_http_info(id, persona_write, async_req=True)
+        >>> thread = api.api_personas_idtoken_post_with_http_info(id, persona_token_write, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
-        :param persona_write: The new Persona resource (required)
-        :type persona_write: PersonaWrite
+        :param persona_token_write: The new Persona resource (required)
+        :type persona_token_write: PersonaTokenWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -820,15 +821,15 @@
         :rtype: tuple(PersonaPostAuthRead, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'persona_write'
+            'persona_token_write'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -861,16 +862,16 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['persona_write'] is not None:
-            _body_params = _params['persona_write']
+        if _params['persona_token_write'] is not None:
+            _body_params = _params['persona_token_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
```

### Comparing `tpdk-2.0.7/tpdk/api/resolution_center_api.py` & `tpdk-2.0.9/tpdk/api/resolution_center_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/api/safe_checkout_api.py` & `tpdk-2.0.9/tpdk/api/safe_checkout_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/api/user_api.py` & `tpdk-2.0.9/tpdk/api/user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -20,16 +20,16 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from tpdk.models.persona_persona_auth_return import PersonaPersonaAuthReturn
-from tpdk.models.persona_persona_external_auth import PersonaPersonaExternalAuth
+from tpdk.models.persona_auth_return import PersonaAuthReturn
+from tpdk.models.persona_external_auth import PersonaExternalAuth
 from tpdk.models.persona_read import PersonaRead
 from tpdk.models.persona_register import PersonaRegister
 from tpdk.models.user import User
 from tpdk.models.user_email_validation_write import UserEmailValidationWrite
 from tpdk.models.user_post_register_read import UserPostRegisterRead
 from tpdk.models.user_support_read import UserSupportRead
 from tpdk.models.user_write import UserWrite
@@ -51,55 +51,55 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def api_personasauthentication_post(self, persona_persona_external_auth : Annotated[PersonaPersonaExternalAuth, Field(..., description="The new Persona resource")], **kwargs) -> PersonaPersonaAuthReturn:  # noqa: E501
+    def api_personasauthentication_post(self, persona_external_auth : Annotated[PersonaExternalAuth, Field(..., description="The new Persona resource")], **kwargs) -> PersonaAuthReturn:  # noqa: E501
         """Persona Authentication  # noqa: E501
 
         Main route for Persona (Organization customers) to authenticate themselves. Public access, captcha protected and MFA mandatory.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personasauthentication_post(persona_persona_external_auth, async_req=True)
+        >>> thread = api.api_personasauthentication_post(persona_external_auth, async_req=True)
         >>> result = thread.get()
 
-        :param persona_persona_external_auth: The new Persona resource (required)
-        :type persona_persona_external_auth: PersonaPersonaExternalAuth
+        :param persona_external_auth: The new Persona resource (required)
+        :type persona_external_auth: PersonaExternalAuth
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PersonaPersonaAuthReturn
+        :rtype: PersonaAuthReturn
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the api_personasauthentication_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.api_personasauthentication_post_with_http_info(persona_persona_external_auth, **kwargs)  # noqa: E501
+        return self.api_personasauthentication_post_with_http_info(persona_external_auth, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personasauthentication_post_with_http_info(self, persona_persona_external_auth : Annotated[PersonaPersonaExternalAuth, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
+    def api_personasauthentication_post_with_http_info(self, persona_external_auth : Annotated[PersonaExternalAuth, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Persona Authentication  # noqa: E501
 
         Main route for Persona (Organization customers) to authenticate themselves. Public access, captcha protected and MFA mandatory.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personasauthentication_post_with_http_info(persona_persona_external_auth, async_req=True)
+        >>> thread = api.api_personasauthentication_post_with_http_info(persona_external_auth, async_req=True)
         >>> result = thread.get()
 
-        :param persona_persona_external_auth: The new Persona resource (required)
-        :type persona_persona_external_auth: PersonaPersonaExternalAuth
+        :param persona_external_auth: The new Persona resource (required)
+        :type persona_external_auth: PersonaExternalAuth
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -114,21 +114,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PersonaPersonaAuthReturn, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PersonaAuthReturn, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'persona_persona_external_auth'
+            'persona_external_auth'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -158,16 +158,16 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['persona_persona_external_auth'] is not None:
-            _body_params = _params['persona_persona_external_auth']
+        if _params['persona_external_auth'] is not None:
+            _body_params = _params['persona_external_auth']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -176,15 +176,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
-            '201': "PersonaPersonaAuthReturn",
+            '201': "PersonaAuthReturn",
             '400': None,
             '422': None,
         }
 
         return self.api_client.call_api(
             '/personas/authentication', 'POST',
             _path_params,
```

### Comparing `tpdk-2.0.7/tpdk/api/webhook_api.py` & `tpdk-2.0.9/tpdk/api/webhook_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/api_client.py` & `tpdk-2.0.9/tpdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.7/python'
+        self.user_agent = 'OpenAPI-Generator/2.0.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tpdk-2.0.7/tpdk/api_response.py` & `tpdk-2.0.9/tpdk/api_response.py`

 * *Files identical despite different names*

### Comparing `tpdk-2.0.7/tpdk/configuration.py` & `tpdk-2.0.9/tpdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -412,16 +412,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.7\n"\
-               "SDK Package Version: 2.0.7".\
+               "Version of the API: 2.0.9\n"\
+               "SDK Package Version: 2.0.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tpdk-2.0.7/tpdk/exceptions.py` & `tpdk-2.0.9/tpdk/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/__init__.py` & `tpdk-2.0.9/tpdk/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -62,24 +62,25 @@
 from tpdk.models.organization_write_billing_address import OrganizationWriteBillingAddress
 from tpdk.models.parcel import Parcel
 from tpdk.models.parcel_independent_write import ParcelIndependentWrite
 from tpdk.models.parcel_read import ParcelRead
 from tpdk.models.parcel_write import ParcelWrite
 from tpdk.models.persona import Persona
 from tpdk.models.persona_address import PersonaAddress
+from tpdk.models.persona_auth_return import PersonaAuthReturn
 from tpdk.models.persona_collection_read import PersonaCollectionRead
+from tpdk.models.persona_external_auth import PersonaExternalAuth
 from tpdk.models.persona_independent_write import PersonaIndependentWrite
 from tpdk.models.persona_independent_write_address import PersonaIndependentWriteAddress
-from tpdk.models.persona_persona_auth_return import PersonaPersonaAuthReturn
-from tpdk.models.persona_persona_external_auth import PersonaPersonaExternalAuth
 from tpdk.models.persona_post_auth_read import PersonaPostAuthRead
 from tpdk.models.persona_read import PersonaRead
 from tpdk.models.persona_read_address import PersonaReadAddress
 from tpdk.models.persona_register import PersonaRegister
 from tpdk.models.persona_token import PersonaToken
+from tpdk.models.persona_token_write import PersonaTokenWrite
 from tpdk.models.persona_update import PersonaUpdate
 from tpdk.models.persona_update_address import PersonaUpdateAddress
 from tpdk.models.persona_write import PersonaWrite
 from tpdk.models.persona_write_address import PersonaWriteAddress
 from tpdk.models.transaction_collection_read import TransactionCollectionRead
 from tpdk.models.transaction_independent_write import TransactionIndependentWrite
 from tpdk.models.transaction_read import TransactionRead
```

### Comparing `tpdk-2.0.7/tpdk/models/address.py` & `tpdk-2.0.9/tpdk/models/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/address_independent_write.py` & `tpdk-2.0.9/tpdk/models/address_independent_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/address_read.py` & `tpdk-2.0.9/tpdk/models/address_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/address_update.py` & `tpdk-2.0.9/tpdk/models/address_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/address_write.py` & `tpdk-2.0.9/tpdk/models/address_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/ai_hint.py` & `tpdk-2.0.9/tpdk/models/ai_hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/api_client.py` & `tpdk-2.0.9/tpdk/models/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/dispute.py` & `tpdk-2.0.9/tpdk/models/dispute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/dispute_collection_read.py` & `tpdk-2.0.9/tpdk/models/dispute_collection_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/dispute_independent_write.py` & `tpdk-2.0.9/tpdk/models/dispute_independent_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/dispute_post_creation_read.py` & `tpdk-2.0.9/tpdk/models/dispute_post_creation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/dispute_read.py` & `tpdk-2.0.9/tpdk/models/dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/dispute_update.py` & `tpdk-2.0.9/tpdk/models/dispute_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/dispute_write.py` & `tpdk-2.0.9/tpdk/models/dispute_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/evaluation_read.py` & `tpdk-2.0.9/tpdk/models/evaluation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/evaluation_write.py` & `tpdk-2.0.9/tpdk/models/evaluation_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/evidence.py` & `tpdk-2.0.9/tpdk/models/evidence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/evidence_read.py` & `tpdk-2.0.9/tpdk/models/evidence_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/evidence_read_media.py` & `tpdk-2.0.9/tpdk/models/evidence_read_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/evidence_write.py` & `tpdk-2.0.9/tpdk/models/evidence_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/media.py` & `tpdk-2.0.9/tpdk/models/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/media_read.py` & `tpdk-2.0.9/tpdk/models/media_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/message.py` & `tpdk-2.0.9/tpdk/models/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/metadata.py` & `tpdk-2.0.9/tpdk/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/metadata_independent_write.py` & `tpdk-2.0.9/tpdk/models/metadata_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/metadata_read.py` & `tpdk-2.0.9/tpdk/models/metadata_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/metadata_update.py` & `tpdk-2.0.9/tpdk/models/metadata_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/metadata_write.py` & `tpdk-2.0.9/tpdk/models/metadata_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/notification.py` & `tpdk-2.0.9/tpdk/models/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/notification_read.py` & `tpdk-2.0.9/tpdk/models/notification_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/notification_update.py` & `tpdk-2.0.9/tpdk/models/notification_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer.py` & `tpdk-2.0.9/tpdk/models/offer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer_collection_read.py` & `tpdk-2.0.9/tpdk/models/offer_collection_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer_independent_write.py` & `tpdk-2.0.9/tpdk/models/offer_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer_independent_write_seller.py` & `tpdk-2.0.9/tpdk/models/offer_independent_write_seller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer_post_creation_read.py` & `tpdk-2.0.9/tpdk/models/offer_post_creation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer_read.py` & `tpdk-2.0.9/tpdk/models/offer_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer_update.py` & `tpdk-2.0.9/tpdk/models/offer_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/offer_write.py` & `tpdk-2.0.9/tpdk/models/offer_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/organization_read.py` & `tpdk-2.0.9/tpdk/models/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/organization_support_read.py` & `tpdk-2.0.9/tpdk/models/organization_support_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/organization_update.py` & `tpdk-2.0.9/tpdk/models/organization_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/organization_update_billing_address.py` & `tpdk-2.0.9/tpdk/models/organization_update_billing_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/organization_write.py` & `tpdk-2.0.9/tpdk/models/organization_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/organization_write_billing_address.py` & `tpdk-2.0.9/tpdk/models/organization_write_billing_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/parcel.py` & `tpdk-2.0.9/tpdk/models/parcel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/parcel_independent_write.py` & `tpdk-2.0.9/tpdk/models/parcel_independent_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/parcel_read.py` & `tpdk-2.0.9/tpdk/models/parcel_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/parcel_write.py` & `tpdk-2.0.9/tpdk/models/parcel_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona.py` & `tpdk-2.0.9/tpdk/models/persona.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_address.py` & `tpdk-2.0.9/tpdk/models/persona_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_collection_read.py` & `tpdk-2.0.9/tpdk/models/persona_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_independent_write.py` & `tpdk-2.0.9/tpdk/models/persona_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_independent_write_address.py` & `tpdk-2.0.9/tpdk/models/persona_independent_write_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_persona_auth_return.py` & `tpdk-2.0.9/tpdk/models/persona_auth_return.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,15 +18,15 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class PersonaPersonaAuthReturn(BaseModel):
+class PersonaAuthReturn(BaseModel):
     """
     
     """
     auth_url: Optional[StrictStr] = Field(None, alias="authUrl", description="Url that is able to bypass MFA for a single user. Please note that this should not be shared between the complainant and the seller or anyone external to them.")
     expire_at: Optional[datetime] = Field(None, alias="expireAt", description="This authenticated-URL cannot be renewed, you will have to re-create one each time. Typically valid for a single hour.")
     __properties = ["authUrl", "expireAt"]
 
@@ -40,16 +40,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PersonaPersonaAuthReturn:
-        """Create an instance of PersonaPersonaAuthReturn from a JSON string"""
+    def from_json(cls, json_str: str) -> PersonaAuthReturn:
+        """Create an instance of PersonaAuthReturn from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -63,21 +63,21 @@
         # and __fields_set__ contains the field
         if self.expire_at is None and "expire_at" in self.__fields_set__:
             _dict['expireAt'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PersonaPersonaAuthReturn:
-        """Create an instance of PersonaPersonaAuthReturn from a dict"""
+    def from_dict(cls, obj: dict) -> PersonaAuthReturn:
+        """Create an instance of PersonaAuthReturn from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PersonaPersonaAuthReturn.parse_obj(obj)
+            return PersonaAuthReturn.parse_obj(obj)
 
-        _obj = PersonaPersonaAuthReturn.parse_obj({
+        _obj = PersonaAuthReturn.parse_obj({
             "auth_url": obj.get("authUrl"),
             "expire_at": obj.get("expireAt")
         })
         return _obj
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_persona_external_auth.py` & `tpdk-2.0.9/tpdk/models/persona_external_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,15 +18,15 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class PersonaPersonaExternalAuth(BaseModel):
+class PersonaExternalAuth(BaseModel):
     """
     
     """
     captcha: Optional[StrictStr] = None
     target_url: Optional[StrictStr] = Field(None, alias="targetUrl", description="The URL you wish that Persona to go to without additional MFA. The URL MUST concern that Persona.")
     plain_password: Optional[StrictStr] = Field(None, alias="plainPassword")
     email: Optional[StrictStr] = None
@@ -43,16 +43,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PersonaPersonaExternalAuth:
-        """Create an instance of PersonaPersonaExternalAuth from a JSON string"""
+    def from_json(cls, json_str: str) -> PersonaExternalAuth:
+        """Create an instance of PersonaExternalAuth from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -81,23 +81,23 @@
         # and __fields_set__ contains the field
         if self.mobile_phone_number is None and "mobile_phone_number" in self.__fields_set__:
             _dict['mobilePhoneNumber'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PersonaPersonaExternalAuth:
-        """Create an instance of PersonaPersonaExternalAuth from a dict"""
+    def from_dict(cls, obj: dict) -> PersonaExternalAuth:
+        """Create an instance of PersonaExternalAuth from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PersonaPersonaExternalAuth.parse_obj(obj)
+            return PersonaExternalAuth.parse_obj(obj)
 
-        _obj = PersonaPersonaExternalAuth.parse_obj({
+        _obj = PersonaExternalAuth.parse_obj({
             "captcha": obj.get("captcha"),
             "target_url": obj.get("targetUrl"),
             "plain_password": obj.get("plainPassword"),
             "email": obj.get("email"),
             "mobile_phone_number": obj.get("mobilePhoneNumber")
         })
         return _obj
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_post_auth_read.py` & `tpdk-2.0.9/tpdk/models/persona_post_auth_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_read.py` & `tpdk-2.0.9/tpdk/models/persona_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_read_address.py` & `tpdk-2.0.9/tpdk/models/persona_read_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_register.py` & `tpdk-2.0.9/tpdk/models/persona_register.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_token.py` & `tpdk-2.0.9/tpdk/models/persona_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_update.py` & `tpdk-2.0.9/tpdk/models/persona_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_update_address.py` & `tpdk-2.0.9/tpdk/models/persona_update_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_write.py` & `tpdk-2.0.9/tpdk/models/persona_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/persona_write_address.py` & `tpdk-2.0.9/tpdk/models/persona_write_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/transaction_collection_read.py` & `tpdk-2.0.9/tpdk/models/transaction_collection_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/transaction_independent_write.py` & `tpdk-2.0.9/tpdk/models/transaction_independent_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/transaction_read.py` & `tpdk-2.0.9/tpdk/models/transaction_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/unprocessable_entity.py` & `tpdk-2.0.9/tpdk/models/unprocessable_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/unprocessable_entity_violations_inner.py` & `tpdk-2.0.9/tpdk/models/unprocessable_entity_violations_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user.py` & `tpdk-2.0.9/tpdk/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user_api.py` & `tpdk-2.0.9/tpdk/models/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user_email_validation_write.py` & `tpdk-2.0.9/tpdk/models/user_email_validation_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user_post_register_read.py` & `tpdk-2.0.9/tpdk/models/user_post_register_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user_support_read.py` & `tpdk-2.0.9/tpdk/models/user_support_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user_support_read_organization.py` & `tpdk-2.0.9/tpdk/models/user_support_read_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user_write.py` & `tpdk-2.0.9/tpdk/models/user_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/user_write_organization.py` & `tpdk-2.0.9/tpdk/models/user_write_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/view.py` & `tpdk-2.0.9/tpdk/models/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/webhook.py` & `tpdk-2.0.9/tpdk/models/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/webhook_history_collection_read.py` & `tpdk-2.0.9/tpdk/models/webhook_history_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/webhook_history_read.py` & `tpdk-2.0.9/tpdk/models/webhook_history_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/webhook_object.py` & `tpdk-2.0.9/tpdk/models/webhook_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/webhook_subscription_read.py` & `tpdk-2.0.9/tpdk/models/webhook_subscription_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/models/webhook_subscription_write.py` & `tpdk-2.0.9/tpdk/models/webhook_subscription_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk/rest.py` & `tpdk-2.0.9/tpdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.7
+    The version of the OpenAPI document: 2.0.9
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.7/tpdk.egg-info/SOURCES.txt` & `tpdk-2.0.9/tpdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,24 +53,25 @@
 test/test_parcel.py
 test/test_parcel_independent_write.py
 test/test_parcel_read.py
 test/test_parcel_write.py
 test/test_persona.py
 test/test_persona_address.py
 test/test_persona_api.py
+test/test_persona_auth_return.py
 test/test_persona_collection_read.py
+test/test_persona_external_auth.py
 test/test_persona_independent_write.py
 test/test_persona_independent_write_address.py
-test/test_persona_persona_auth_return.py
-test/test_persona_persona_external_auth.py
 test/test_persona_post_auth_read.py
 test/test_persona_read.py
 test/test_persona_read_address.py
 test/test_persona_register.py
 test/test_persona_token.py
+test/test_persona_token_write.py
 test/test_persona_update.py
 test/test_persona_update_address.py
 test/test_persona_write.py
 test/test_persona_write_address.py
 test/test_resolution_center_api.py
 test/test_safe_checkout_api.py
 test/test_transaction_collection_read.py
@@ -162,24 +163,25 @@
 tpdk/models/organization_write_billing_address.py
 tpdk/models/parcel.py
 tpdk/models/parcel_independent_write.py
 tpdk/models/parcel_read.py
 tpdk/models/parcel_write.py
 tpdk/models/persona.py
 tpdk/models/persona_address.py
+tpdk/models/persona_auth_return.py
 tpdk/models/persona_collection_read.py
+tpdk/models/persona_external_auth.py
 tpdk/models/persona_independent_write.py
 tpdk/models/persona_independent_write_address.py
-tpdk/models/persona_persona_auth_return.py
-tpdk/models/persona_persona_external_auth.py
 tpdk/models/persona_post_auth_read.py
 tpdk/models/persona_read.py
 tpdk/models/persona_read_address.py
 tpdk/models/persona_register.py
 tpdk/models/persona_token.py
+tpdk/models/persona_token_write.py
 tpdk/models/persona_update.py
 tpdk/models/persona_update_address.py
 tpdk/models/persona_write.py
 tpdk/models/persona_write_address.py
 tpdk/models/transaction_collection_read.py
 tpdk/models/transaction_independent_write.py
 tpdk/models/transaction_read.py
```

