# Comparing `tmp/huntflow_api_client-0.0.8.tar.gz` & `tmp/huntflow_api_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_api_client-0.0.8.tar", last modified: Wed May 31 12:47:16 2023, max compression
+gzip compressed data, was "huntflow_api_client-0.0.9.tar", last modified: Thu Jun  1 10:57:55 2023, max compression
```

## Comparing `huntflow_api_client-0.0.8.tar` & `huntflow_api_client-0.0.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1065 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/LICENSE
--rw-r--r--   0        0        0      488 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/README.md
--rw-r--r--   0        0        0       76 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/__init__.py
--rw-r--r--   0        0        0     5578 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/api.py
--rw-r--r--   0        0        0     1372 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/__init__.py
--rw-r--r--   0        0        0     1760 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/account_vacancy_request.py
--rw-r--r--   0        0        0     1434 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/accounts.py
--rw-r--r--   0        0        0     2903 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/applicant_on_vacancy.py
--rw-r--r--   0        0        0      730 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0     8554 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/applicants.py
--rw-r--r--   0        0        0      941 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/base.py
--rw-r--r--   0        0        0     2651 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/coworkers.py
--rw-r--r--   0        0        0      743 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/delayed_tasks.py
--rw-r--r--   0        0        0     3002 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/dictionaries.py
--rw-r--r--   0        0        0     2554 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/divisions.py
--rw-r--r--   0        0        0     6720 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/production_calendars.py
--rw-r--r--   0        0        0      713 2023-05-31 12:46:57.912334 huntflow_api_client-0.0.8/huntflow_api_client/entities/rejection_reason.py
--rw-r--r--   0        0        0     2456 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/entities/tags.py
--rw-r--r--   0        0        0     9379 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/entities/vacancies.py
--rw-r--r--   0        0        0     2918 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/entities/vacancy_requests.py
--rw-r--r--   0        0        0     1789 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/entities/webhooks.py
--rw-r--r--   0        0        0      553 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/errors/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/errors/errors.py
--rw-r--r--   0        0        0     3732 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/errors/handlers.py
--rw-r--r--   0        0        0      361 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/errors/response_hooks.py
--rw-r--r--   0        0        0        0 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/__init__.py
--rw-r--r--   0        0        0     6501 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/common.py
--rw-r--r--   0        0        0     2394 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/consts.py
--rw-r--r--   0        0        0        0 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/__init__.py
--rw-r--r--   0        0        0     3614 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/applicant_on_vacancy.py
--rw-r--r--   0        0        0     6196 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/applicants.py
--rw-r--r--   0        0        0     1492 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/dictionaries.py
--rw-r--r--   0        0        0      691 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/divisions.py
--rw-r--r--   0        0        0      921 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/production_calendars.py
--rw-r--r--   0        0        0      259 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/tags.py
--rw-r--r--   0        0        0     3123 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/vacancies.py
--rw-r--r--   0        0        0     1407 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/vacancy_requests.py
--rw-r--r--   0        0        0      482 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/request/webhooks.py
--rw-r--r--   0        0        0        0 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/__init__.py
--rw-r--r--   0        0        0     2102 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/account_vacancy_request.py
--rw-r--r--   0        0        0     1595 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/accounts.py
--rw-r--r--   0        0        0     1054 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/applicant_on_vacancy.py
--rw-r--r--   0        0        0      773 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0    12930 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/applicants.py
--rw-r--r--   0        0        0     1262 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/coworkers.py
--rw-r--r--   0        0        0     1299 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/delayed_tasks.py
--rw-r--r--   0        0        0     2261 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/dictionaries.py
--rw-r--r--   0        0        0     1507 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/divisions.py
--rw-r--r--   0        0        0      330 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/offers.py
--rw-r--r--   0        0        0     1525 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/production_calendars.py
--rw-r--r--   0        0        0      476 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/rejection_reason.py
--rw-r--r--   0        0        0      781 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/survey.py
--rw-r--r--   0        0        0      241 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/tags.py
--rw-r--r--   0        0        0     6182 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/vacancies.py
--rw-r--r--   0        0        0     2901 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/vacancy_requests.py
--rw-r--r--   0        0        0      719 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/models/response/webhooks.py
--rw-r--r--   0        0        0       53 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/tokens/__init__.py
--rw-r--r--   0        0        0     1871 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/tokens/locker.py
--rw-r--r--   0        0        0     5186 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/tokens/proxy.py
--rw-r--r--   0        0        0      730 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/tokens/storage.py
--rw-r--r--   0        0        0      548 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/huntflow_api_client/tokens/token.py
--rw-r--r--   0        0        0     1597 2023-05-31 12:47:16.398106 huntflow_api_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     4744 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/api.py
--rw-r--r--   0        0        0       79 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0      176 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/fixtures/server.py
--rw-r--r--   0        0        0      856 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/fixtures/tokens.py
--rw-r--r--   0        0        0        0 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/__init__.py
--rw-r--r--   0        0        0     3161 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_account_divisions.py
--rw-r--r--   0        0        0     2590 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_account_tags.py
--rw-r--r--   0        0        0     3782 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_account_vacancy_request.py
--rw-r--r--   0        0        0     2279 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_accounts.py
--rw-r--r--   0        0        0     3614 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_applicant_on_vacancy.py
--rw-r--r--   0        0        0     1214 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_applicant_on_vacancy_statuses.py
--rw-r--r--   0        0        0    16778 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_applicants.py
--rw-r--r--   0        0        0     2815 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_coworkers.py
--rw-r--r--   0        0        0     1323 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_delayed_tasks.py
--rw-r--r--   0        0        0     4417 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_dictionaries.py
--rw-r--r--   0        0        0     7692 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_production_calendar.py
--rw-r--r--   0        0        0     1039 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_rejection_reasons.py
--rw-r--r--   0        0        0    14337 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_vacancies.py
--rw-r--r--   0        0        0     4266 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_vacancy_request.py
--rw-r--r--   0        0        0     2534 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_entities/test_webhooks.py
--rw-r--r--   0        0        0        0 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_errors/__init__.py
--rw-r--r--   0        0        0     8007 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_errors/test_error_handlers.py
--rw-r--r--   0        0        0        0 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_tokens/__init__.py
--rw-r--r--   0        0        0     5630 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_tokens/test_access_token.py
--rw-r--r--   0        0        0     1973 2023-05-31 12:46:57.916335 huntflow_api_client-0.0.8/tests/test_tokens/test_huntflow_token_proxy.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-01 10:57:43.667030 huntflow_api_client-0.0.9/LICENSE
+-rw-r--r--   0        0        0      488 2023-06-01 10:57:43.667030 huntflow_api_client-0.0.9/README.md
+-rw-r--r--   0        0        0       76 2023-06-01 10:57:43.667030 huntflow_api_client-0.0.9/huntflow_api_client/__init__.py
+-rw-r--r--   0        0        0     5578 2023-06-01 10:57:43.667030 huntflow_api_client-0.0.9/huntflow_api_client/api.py
+-rw-r--r--   0        0        0     1372 2023-06-01 10:57:43.667030 huntflow_api_client-0.0.9/huntflow_api_client/entities/__init__.py
+-rw-r--r--   0        0        0     1760 2023-06-01 10:57:43.667030 huntflow_api_client-0.0.9/huntflow_api_client/entities/account_vacancy_request.py
+-rw-r--r--   0        0        0     1434 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/accounts.py
+-rw-r--r--   0        0        0     2903 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      730 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0     8554 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/applicants.py
+-rw-r--r--   0        0        0      941 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/base.py
+-rw-r--r--   0        0        0     2651 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/coworkers.py
+-rw-r--r--   0        0        0      743 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/delayed_tasks.py
+-rw-r--r--   0        0        0     3002 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/dictionaries.py
+-rw-r--r--   0        0        0     2554 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/divisions.py
+-rw-r--r--   0        0        0     6720 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/production_calendars.py
+-rw-r--r--   0        0        0      713 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/rejection_reason.py
+-rw-r--r--   0        0        0     2456 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/tags.py
+-rw-r--r--   0        0        0     9379 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/vacancies.py
+-rw-r--r--   0        0        0     2918 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/vacancy_requests.py
+-rw-r--r--   0        0        0     1789 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/entities/webhooks.py
+-rw-r--r--   0        0        0      553 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/errors/__init__.py
+-rw-r--r--   0        0        0     1128 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/errors/errors.py
+-rw-r--r--   0        0        0     3732 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/errors/handlers.py
+-rw-r--r--   0        0        0      361 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/errors/response_hooks.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/__init__.py
+-rw-r--r--   0        0        0     6501 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/common.py
+-rw-r--r--   0        0        0     2394 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/consts.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/__init__.py
+-rw-r--r--   0        0        0     3614 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/applicant_on_vacancy.py
+-rw-r--r--   0        0        0     6196 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/applicants.py
+-rw-r--r--   0        0        0     1492 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/dictionaries.py
+-rw-r--r--   0        0        0      691 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/divisions.py
+-rw-r--r--   0        0        0      921 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/production_calendars.py
+-rw-r--r--   0        0        0      259 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/tags.py
+-rw-r--r--   0        0        0     3123 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/vacancies.py
+-rw-r--r--   0        0        0     1407 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/vacancy_requests.py
+-rw-r--r--   0        0        0      482 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/request/webhooks.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/__init__.py
+-rw-r--r--   0        0        0     2102 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/account_vacancy_request.py
+-rw-r--r--   0        0        0     1595 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/accounts.py
+-rw-r--r--   0        0        0     1054 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      773 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0    12930 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/applicants.py
+-rw-r--r--   0        0        0     1262 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/coworkers.py
+-rw-r--r--   0        0        0     1299 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/delayed_tasks.py
+-rw-r--r--   0        0        0     2261 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/dictionaries.py
+-rw-r--r--   0        0        0     1507 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/divisions.py
+-rw-r--r--   0        0        0      330 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/offers.py
+-rw-r--r--   0        0        0     1525 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/production_calendars.py
+-rw-r--r--   0        0        0      476 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/rejection_reason.py
+-rw-r--r--   0        0        0      781 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/survey.py
+-rw-r--r--   0        0        0      241 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/tags.py
+-rw-r--r--   0        0        0     6182 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/vacancies.py
+-rw-r--r--   0        0        0     2901 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/vacancy_requests.py
+-rw-r--r--   0        0        0      719 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/models/response/webhooks.py
+-rw-r--r--   0        0        0       53 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/tokens/__init__.py
+-rw-r--r--   0        0        0     1871 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/tokens/locker.py
+-rw-r--r--   0        0        0     5186 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/tokens/proxy.py
+-rw-r--r--   0        0        0      730 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/tokens/storage.py
+-rw-r--r--   0        0        0      548 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/huntflow_api_client/tokens/token.py
+-rw-r--r--   0        0        0     1597 2023-06-01 10:57:55.631297 huntflow_api_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     4744 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/api.py
+-rw-r--r--   0        0        0       79 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0      176 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/fixtures/server.py
+-rw-r--r--   0        0        0      856 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/fixtures/tokens.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/__init__.py
+-rw-r--r--   0        0        0     3161 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_account_divisions.py
+-rw-r--r--   0        0        0     2590 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_account_tags.py
+-rw-r--r--   0        0        0     3782 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_account_vacancy_request.py
+-rw-r--r--   0        0        0     2279 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_accounts.py
+-rw-r--r--   0        0        0     3614 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_applicant_on_vacancy.py
+-rw-r--r--   0        0        0     1214 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_applicant_on_vacancy_statuses.py
+-rw-r--r--   0        0        0    16900 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_applicants.py
+-rw-r--r--   0        0        0     2815 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_coworkers.py
+-rw-r--r--   0        0        0     1323 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_delayed_tasks.py
+-rw-r--r--   0        0        0     4417 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_dictionaries.py
+-rw-r--r--   0        0        0     7692 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_production_calendar.py
+-rw-r--r--   0        0        0     1039 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_rejection_reasons.py
+-rw-r--r--   0        0        0    14337 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_vacancies.py
+-rw-r--r--   0        0        0     4266 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_vacancy_request.py
+-rw-r--r--   0        0        0     2534 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_entities/test_webhooks.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_errors/__init__.py
+-rw-r--r--   0        0        0     8007 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_errors/test_error_handlers.py
+-rw-r--r--   0        0        0        0 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_tokens/__init__.py
+-rw-r--r--   0        0        0     5630 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_tokens/test_access_token.py
+-rw-r--r--   0        0        0     1973 2023-06-01 10:57:43.671030 huntflow_api_client-0.0.9/tests/test_tokens/test_huntflow_token_proxy.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.9/PKG-INFO
```

### Comparing `huntflow_api_client-0.0.8/LICENSE` & `huntflow_api_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/api.py` & `huntflow_api_client-0.0.9/huntflow_api_client/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/__init__.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/account_vacancy_request.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/accounts.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/applicant_on_vacancy.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/applicant_on_vacancy_status.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/applicants.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/base.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/base.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/coworkers.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/delayed_tasks.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/dictionaries.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/divisions.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/production_calendars.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/rejection_reason.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/rejection_reason.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/tags.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/vacancies.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/vacancy_requests.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/entities/webhooks.py` & `huntflow_api_client-0.0.9/huntflow_api_client/entities/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/errors/__init__.py` & `huntflow_api_client-0.0.9/huntflow_api_client/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/errors/errors.py` & `huntflow_api_client-0.0.9/huntflow_api_client/errors/errors.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/errors/handlers.py` & `huntflow_api_client-0.0.9/huntflow_api_client/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/common.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/common.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/consts.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/consts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/request/applicant_on_vacancy.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/request/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/request/applicants.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/request/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/request/dictionaries.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/request/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/request/divisions.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/request/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/request/production_calendars.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/request/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/request/vacancies.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/request/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/request/vacancy_requests.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/request/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/account_vacancy_request.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/accounts.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/applicant_on_vacancy.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/applicant_on_vacancy_status.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/applicants.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/applicants.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     email: Union[EmailStr, str, None] = Field(
         None,
         description="Email address",
     )
     tags: List[ApplicantTag] = Field(..., description="List of tags")
     links: List[ApplicantLink] = Field(..., description="Applicant's vacancies")
     external: Optional[List[ApplicantResume]] = Field(None, description="Applicant's resume")
-    agreement: Optional[AgreementStateEnum] = Field(
+    agreement: Optional[ApplicantAgreement] = Field(
         None,
         description="Agreement's state of applicant to personal data processing",
     )
     doubles: List[ApplicantDouble] = Field(..., description="List of duplicates")
     social: List[ApplicantSocial] = Field(..., description="List of applicant's social accounts")
 
 
@@ -112,15 +112,15 @@
     )
     birthday: Optional[date] = Field(None, description="Date of birth")
     files: Optional[List[PositiveInt]] = Field(
         None,
         description="Upload files<br>The list of file's ID attached to the applicant",
     )
     doubles: List[ApplicantDouble] = Field(..., description="List of duplicates")
-    agreement: Optional[AgreementStateEnum] = Field(
+    agreement: Optional[ApplicantAgreement] = Field(
         None,
         description="Agreement's state of applicant to personal data processing",
     )
     external: List[ApplicantResume] = Field(..., description="Applicant's resume")
     social: List[ApplicantSocial] = Field(..., description="List of applicant's social accounts")
```

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/coworkers.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/delayed_tasks.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/dictionaries.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/divisions.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/production_calendars.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/survey.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/survey.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/vacancies.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/vacancy_requests.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/models/response/webhooks.py` & `huntflow_api_client-0.0.9/huntflow_api_client/models/response/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/tokens/locker.py` & `huntflow_api_client-0.0.9/huntflow_api_client/tokens/locker.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/tokens/proxy.py` & `huntflow_api_client-0.0.9/huntflow_api_client/tokens/proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/tokens/storage.py` & `huntflow_api_client-0.0.9/huntflow_api_client/tokens/storage.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/huntflow_api_client/tokens/token.py` & `huntflow_api_client-0.0.9/huntflow_api_client/tokens/token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/pyproject.toml` & `huntflow_api_client-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "huntflow-api-client"
-version = "0.0.8"
+version = "0.0.9"
 description = "Huntflow API Client for Python"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "httpx>=0.23.3",
     "email-validator>=1.3.1",
```

### Comparing `huntflow_api_client-0.0.8/tests/api.py` & `huntflow_api_client-0.0.9/tests/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/fixtures/tokens.py` & `huntflow_api_client-0.0.9/tests/fixtures/tokens.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_account_divisions.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_account_divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_account_tags.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_account_tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_account_vacancy_request.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_accounts.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_applicant_on_vacancy.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_applicant_on_vacancy_statuses.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_applicant_on_vacancy_statuses.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_applicants.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_applicants.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 {
                     "id": 1,
                     "auth_type": "NATIVE",
                     "account_source": None,
                     "updated": "2023-05-10T10:46:39+03:00",
                 },
             ],
-            "agreement": None,
+            "agreement": {"state": None, "decision_date": None},
             "doubles": [],
             "social": [],
         },
     ],
 }
 APPLICANT_GET_RESPONSE: Dict[str, Any] = {
     "first_name": "John",
@@ -129,15 +129,15 @@
         {
             "id": 1,
             "auth_type": "Auth",
             "account_source": 10,
             "updated": "2020-01-01T00:00:00+03:00",
         },
     ],
-    "agreement": "declined",
+    "agreement": {"state": None, "decision_date": None},
     "doubles": [{"double": 8}],
     "social": [
         {
             "id": 1,
             "social_type": "TELEGRAM",
             "value": "TelegramUsername",
             "verified": False,
@@ -179,15 +179,15 @@
     "company": "Google Inc.",
     "photo": 1,
     "id": 19,
     "created": "2020-01-01T00:00:00+03:00",
     "birthday": "2020-01-01",
     "files": [1, 2, 3],
     "doubles": [{"double": 8}],
-    "agreement": "sent",
+    "agreement": {"state": None, "decision_date": None},
     "external": [
         {
             "id": 1,
             "auth_type": "Auth",
             "account_source": 10,
             "updated": "2020-01-01T00:00:00+03:00",
         },
@@ -233,15 +233,15 @@
         {
             "id": 1,
             "auth_type": "Auth",
             "account_source": 10,
             "updated": "2020-01-01T00:00:00+03:00",
         },
     ],
-    "agreement": "declined",
+    "agreement": {"state": None, "decision_date": None},
     "doubles": [{"double": 8}],
     "social": [
         {
             "id": 1,
             "social_type": "TELEGRAM",
             "value": "TelegramUsername",
             "verified": False,
```

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_coworkers.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_delayed_tasks.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_dictionaries.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_production_calendar.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_production_calendar.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_rejection_reasons.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_rejection_reasons.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_vacancies.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_vacancy_request.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_entities/test_webhooks.py` & `huntflow_api_client-0.0.9/tests/test_entities/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_errors/test_error_handlers.py` & `huntflow_api_client-0.0.9/tests/test_errors/test_error_handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_tokens/test_access_token.py` & `huntflow_api_client-0.0.9/tests/test_tokens/test_access_token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/tests/test_tokens/test_huntflow_token_proxy.py` & `huntflow_api_client-0.0.9/tests/test_tokens/test_huntflow_token_proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.8/PKG-INFO` & `huntflow_api_client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-api-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Huntflow API Client for Python
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

