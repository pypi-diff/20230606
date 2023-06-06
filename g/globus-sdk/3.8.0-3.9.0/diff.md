# Comparing `tmp/globus-sdk-3.8.0.tar.gz` & `tmp/globus-sdk-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-sdk-3.8.0.tar", last modified: Wed May  4 17:50:53 2022, max compression
+gzip compressed data, was "globus-sdk-3.9.0.tar", last modified: Thu Jun  2 17:31:34 2022, max compression
```

## Comparing `globus-sdk-3.8.0.tar` & `globus-sdk-3.9.0.tar`

### file list

```diff
@@ -1,156 +1,169 @@
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.830352 globus-sdk-3.8.0/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      580 2021-12-20 21:34:23.000000 globus-sdk-3.8.0/COPYING
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11358 2022-04-15 14:40:51.000000 globus-sdk-3.8.0/LICENSE
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       67 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/MANIFEST.in
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3003 2022-05-04 17:50:53.830352 globus-sdk-3.8.0/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2211 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/README.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      693 2022-05-04 17:50:53.830352 globus-sdk-3.8.0/setup.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3046 2022-03-16 23:33:19.000000 globus-sdk-3.8.0/setup.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.790353 globus-sdk-3.8.0/src/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.798353 globus-sdk-3.8.0/src/globus_sdk/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3014 2022-05-03 12:14:27.000000 globus-sdk-3.8.0/src/globus_sdk/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5139 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/_sphinxext.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.798353 globus-sdk-3.8.0/src/globus_sdk/_testing/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      390 2022-03-11 16:34:53.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.802353 globus-sdk-3.8.0/src/globus_sdk/_testing/data/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.802353 globus-sdk-3.8.0/src/globus_sdk/_testing/data/auth/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/auth/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      413 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/auth/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2029 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/auth/get_identities.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      374 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/auth/oauth2_userinfo.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.806352 globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      730 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      379 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/delete_group.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      354 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/get_group.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5785 2022-03-16 15:21:13.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/get_my_groups.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.810352 globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-03-02 21:06:59.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      896 2022-03-02 21:06:59.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/create_role.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      919 2022-03-02 21:06:59.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/delete_role.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1404 2022-03-02 21:06:59.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/get_role_list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1054 2022-03-02 21:06:59.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/post_search.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1031 2022-03-02 21:06:59.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/search.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.814352 globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      361 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/create_job.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      363 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/delete_job.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4315 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/get_job.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      366 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/list_jobs.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      527 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/update_job.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      221 2022-03-11 16:34:53.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/helpers.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3209 2022-05-03 12:14:27.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/models.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2705 2022-03-04 03:46:52.000000 globus-sdk-3.8.0/src/globus_sdk/_testing/registry.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.814352 globus-sdk-3.8.0/src/globus_sdk/authorizers/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      543 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/authorizers/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      872 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/authorizers/access_token.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1739 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/authorizers/base.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      920 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/authorizers/basic.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4232 2022-05-04 17:47:38.000000 globus-sdk-3.8.0/src/globus_sdk/authorizers/client_credentials.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3968 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/authorizers/refresh_token.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7063 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/authorizers/renewing.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11212 2022-04-21 16:51:58.000000 globus-sdk-3.8.0/src/globus_sdk/client.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.814352 globus-sdk-3.8.0/src/globus_sdk/config/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      297 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/config/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2885 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/config/env_vars.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4394 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/config/environments.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.818352 globus-sdk-3.8.0/src/globus_sdk/exc/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      695 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/exc/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7458 2022-04-21 16:51:58.000000 globus-sdk-3.8.0/src/globus_sdk/exc/api.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      427 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/exc/base.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1505 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/exc/convert.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3910 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/exc/err_info.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.818352 globus-sdk-3.8.0/src/globus_sdk/local_endpoint/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      168 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/local_endpoint/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.818352 globus-sdk-3.8.0/src/globus_sdk/local_endpoint/personal/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      191 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/local_endpoint/personal/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7211 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/local_endpoint/personal/endpoint.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3078 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/local_endpoint/personal/owner_info.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.818352 globus-sdk-3.8.0/src/globus_sdk/paging/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      526 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/paging/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6442 2022-04-06 17:49:09.000000 globus-sdk-3.8.0/src/globus_sdk/paging/base.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      971 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/paging/last_key.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2307 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/paging/limit_offset.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1808 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/paging/marker.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1221 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/paging/next_token.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2810 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/paging/table.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/py.typed
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7330 2022-04-21 16:51:58.000000 globus-sdk-3.8.0/src/globus_sdk/response.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10884 2022-05-04 17:47:38.000000 globus-sdk-3.8.0/src/globus_sdk/scopes.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.818352 globus-sdk-3.8.0/src/globus_sdk/services/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.818352 globus-sdk-3.8.0/src/globus_sdk/services/auth/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      592 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.822352 globus-sdk-3.8.0/src/globus_sdk/services/auth/client/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      213 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/client/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    20965 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/client/base.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9375 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/client/confidential_client.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5240 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/client/native_client.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      312 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/errors.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.822352 globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      280 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5800 2022-05-04 17:47:38.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/authorization_code.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2351 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/base.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9113 2022-05-04 17:47:38.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/native_app.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9158 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/identity_map.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      222 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/oauth2_constants.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.822352 globus-sdk-3.8.0/src/globus_sdk/services/auth/response/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      218 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/response/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      272 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/response/identities.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9265 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/auth/response/oauth.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.822352 globus-sdk-3.8.0/src/globus_sdk/services/gcs/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      470 2022-05-03 12:14:27.000000 globus-sdk-3.8.0/src/globus_sdk/services/gcs/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11889 2022-05-03 12:14:27.000000 globus-sdk-3.8.0/src/globus_sdk/services/gcs/client.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    19171 2022-05-03 12:14:27.000000 globus-sdk-3.8.0/src/globus_sdk/services/gcs/data.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1134 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/gcs/errors.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3399 2022-02-10 15:01:31.000000 globus-sdk-3.8.0/src/globus_sdk/services/gcs/response.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.822352 globus-sdk-3.8.0/src/globus_sdk/services/groups/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      497 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/groups/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10372 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/services/groups/client.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6364 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/groups/data.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      124 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/groups/errors.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5867 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/groups/manager.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.826352 globus-sdk-3.8.0/src/globus_sdk/services/search/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      199 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/search/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    20217 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/search/client.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10375 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/search/data.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      777 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/search/errors.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.826352 globus-sdk-3.8.0/src/globus_sdk/services/timer/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      164 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/services/timer/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3534 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/services/timer/client.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6034 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/services/timer/data.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2271 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/services/timer/errors.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.826352 globus-sdk-3.8.0/src/globus_sdk/services/transfer/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      363 2022-03-03 17:30:12.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    93258 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/client.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.826352 globus-sdk-3.8.0/src/globus_sdk/services/transfer/data/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      348 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/data/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6001 2022-02-10 17:42:30.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/data/delete_data.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    14310 2022-04-08 04:42:54.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/data/transfer_data.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      825 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/errors.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.826352 globus-sdk-3.8.0/src/globus_sdk/services/transfer/response/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      176 2022-03-03 17:30:12.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/response/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6155 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/response/activation.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      532 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/response/iterable.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      936 2022-03-02 19:59:28.000000 globus-sdk-3.8.0/src/globus_sdk/services/transfer/transport.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.830352 globus-sdk-3.8.0/src/globus_sdk/tokenstorage/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      293 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/tokenstorage/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2148 2022-03-10 18:27:59.000000 globus-sdk-3.8.0/src/globus_sdk/tokenstorage/base.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4694 2022-03-02 16:11:20.000000 globus-sdk-3.8.0/src/globus_sdk/tokenstorage/file_adapters.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10306 2022-03-02 23:13:41.000000 globus-sdk-3.8.0/src/globus_sdk/tokenstorage/sqlite_adapter.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.830352 globus-sdk-3.8.0/src/globus_sdk/transport/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      518 2022-03-16 23:33:19.000000 globus-sdk-3.8.0/src/globus_sdk/transport/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2084 2022-02-07 21:41:35.000000 globus-sdk-3.8.0/src/globus_sdk/transport/encoders.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    17441 2022-04-21 16:51:58.000000 globus-sdk-3.8.0/src/globus_sdk/transport/requests.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4998 2022-05-03 12:17:38.000000 globus-sdk-3.8.0/src/globus_sdk/transport/retry.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      154 2022-04-25 15:48:36.000000 globus-sdk-3.8.0/src/globus_sdk/types.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6049 2022-05-03 12:14:27.000000 globus-sdk-3.8.0/src/globus_sdk/utils.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      136 2022-05-04 17:48:03.000000 globus-sdk-3.8.0/src/globus_sdk/version.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-05-04 17:50:53.798353 globus-sdk-3.8.0/src/globus_sdk.egg-info/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3003 2022-05-04 17:50:53.000000 globus-sdk-3.8.0/src/globus_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4992 2022-05-04 17:50:53.000000 globus-sdk-3.8.0/src/globus_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2022-05-04 17:50:53.000000 globus-sdk-3.8.0/src/globus_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      358 2022-05-04 17:50:53.000000 globus-sdk-3.8.0/src/globus_sdk.egg-info/requires.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       11 2022-05-04 17:50:53.000000 globus-sdk-3.8.0/src/globus_sdk.egg-info/top_level.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2481 2022-04-29 20:34:09.000000 globus-sdk-3.8.0/tox.ini
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      580 2021-12-20 21:34:23.000000 globus-sdk-3.9.0/COPYING
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11358 2022-04-15 14:40:51.000000 globus-sdk-3.9.0/LICENSE
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       67 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/MANIFEST.in
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2966 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2211 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/README.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      693 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/setup.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3046 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/setup.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.872232 globus-sdk-3.9.0/src/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.876232 globus-sdk-3.9.0/src/globus_sdk/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8410 2022-06-02 17:31:14.000000 globus-sdk-3.9.0/src/globus_sdk/__init__.py
+-rwxrwxr-x   0 sirosen  (10000) sirosen  (10000)     5318 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/_generate_init.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5139 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/_sphinxext.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.876232 globus-sdk-3.9.0/src/globus_sdk/_testing/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      390 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.880231 globus-sdk-3.9.0/src/globus_sdk/_testing/data/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.880231 globus-sdk-3.9.0/src/globus_sdk/_testing/data/auth/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/auth/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      413 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/auth/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2029 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/auth/get_identities.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      374 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/auth/oauth2_userinfo.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.880231 globus-sdk-3.9.0/src/globus_sdk/_testing/data/globus_connect_server/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/globus_connect_server/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1744 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/globus_connect_server/create_storage_gateway.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      654 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/globus_connect_server/delete_storage_gateway.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1743 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/globus_connect_server/get_storage_gateway.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2566 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/globus_connect_server/get_storage_gateway_list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1767 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/globus_connect_server/update_storage_gateway.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.880231 globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      730 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      379 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/delete_group.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      354 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/get_group.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5785 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/get_my_groups.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.880231 globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      896 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/create_role.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      919 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/delete_role.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1404 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/get_role_list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1054 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/post_search.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1031 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/search.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.880231 globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      361 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/create_job.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      363 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/delete_job.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4315 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/get_job.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      366 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/list_jobs.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      527 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/update_job.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      259 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/helpers.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3442 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/models.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2705 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/_testing/registry.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      154 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/_types.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/authorizers/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      543 2022-05-12 17:30:09.000000 globus-sdk-3.9.0/src/globus_sdk/authorizers/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      872 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/authorizers/access_token.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1739 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/authorizers/base.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      920 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/authorizers/basic.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4278 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/authorizers/client_credentials.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4013 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/authorizers/refresh_token.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7107 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/authorizers/renewing.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11212 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/client.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/config/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      297 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/config/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2885 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/config/env_vars.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4394 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/config/environments.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/exc/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      695 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/exc/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7458 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/exc/api.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      427 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/exc/base.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1505 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/exc/convert.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3910 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/exc/err_info.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/local_endpoint/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      168 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/local_endpoint/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/local_endpoint/personal/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      191 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/local_endpoint/personal/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7211 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/local_endpoint/personal/endpoint.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3078 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/local_endpoint/personal/owner_info.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/paging/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      526 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/paging/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6442 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/paging/base.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      971 2022-05-12 16:51:31.000000 globus-sdk-3.9.0/src/globus_sdk/paging/last_key.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2307 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/paging/limit_offset.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1808 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/paging/marker.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1221 2022-02-10 17:42:30.000000 globus-sdk-3.9.0/src/globus_sdk/paging/next_token.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2810 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/paging/table.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/py.typed
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8168 2022-06-01 22:17:13.000000 globus-sdk-3.9.0/src/globus_sdk/response.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11808 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/scopes.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/services/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.884231 globus-sdk-3.9.0/src/globus_sdk/services/auth/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      592 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.888231 globus-sdk-3.9.0/src/globus_sdk/services/auth/client/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      213 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/client/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    20966 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/client/base.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9375 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/client/confidential_client.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5240 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/client/native_client.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      301 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/errors.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.888231 globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      280 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5800 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/authorization_code.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2351 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/base.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9113 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/native_app.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9158 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/identity_map.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      222 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/oauth2_constants.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.888231 globus-sdk-3.9.0/src/globus_sdk/services/auth/response/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      218 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/response/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      272 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/response/identities.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9265 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/auth/response/oauth.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.888231 globus-sdk-3.9.0/src/globus_sdk/services/gcs/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1348 2022-06-01 22:17:13.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    17180 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/client.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.888231 globus-sdk-3.9.0/src/globus_sdk/services/gcs/data/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1183 2022-06-01 22:17:13.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/data/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1018 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/data/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    16263 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/data/collection.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1511 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/data/role.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    24908 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/data/storage_gateway.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1134 2022-05-16 14:57:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/errors.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3399 2022-02-10 15:01:31.000000 globus-sdk-3.9.0/src/globus_sdk/services/gcs/response.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.888231 globus-sdk-3.9.0/src/globus_sdk/services/groups/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      497 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/groups/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10414 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/groups/client.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6365 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/groups/data.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      124 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/groups/errors.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5868 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/groups/manager.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.888231 globus-sdk-3.9.0/src/globus_sdk/services/search/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      199 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/search/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    20218 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/search/client.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10375 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/search/data.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      777 2022-05-16 14:57:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/search/errors.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/src/globus_sdk/services/timer/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      164 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/timer/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3535 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/timer/client.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6034 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/timer/data.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2271 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/timer/errors.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/src/globus_sdk/services/transfer/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      363 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    93259 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/client.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/src/globus_sdk/services/transfer/data/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      348 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/data/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6274 2022-06-02 17:29:24.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/data/delete_data.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    16692 2022-06-02 17:29:24.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/data/transfer_data.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      825 2022-05-16 14:57:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/errors.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/src/globus_sdk/services/transfer/response/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      176 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/response/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6155 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/response/activation.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      532 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/response/iterable.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      936 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/services/transfer/transport.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/src/globus_sdk/tokenstorage/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      293 2022-02-07 21:41:35.000000 globus-sdk-3.9.0/src/globus_sdk/tokenstorage/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2148 2022-06-02 17:29:31.000000 globus-sdk-3.9.0/src/globus_sdk/tokenstorage/base.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4694 2022-06-02 17:29:31.000000 globus-sdk-3.9.0/src/globus_sdk/tokenstorage/file_adapters.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10306 2022-06-02 17:29:31.000000 globus-sdk-3.9.0/src/globus_sdk/tokenstorage/sqlite_adapter.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.892231 globus-sdk-3.9.0/src/globus_sdk/transport/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      518 2022-03-16 23:33:19.000000 globus-sdk-3.9.0/src/globus_sdk/transport/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2084 2022-05-16 14:57:35.000000 globus-sdk-3.9.0/src/globus_sdk/transport/encoders.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    17441 2022-05-27 22:28:48.000000 globus-sdk-3.9.0/src/globus_sdk/transport/requests.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4998 2022-05-27 16:35:28.000000 globus-sdk-3.9.0/src/globus_sdk/transport/retry.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6769 2022-06-01 22:17:13.000000 globus-sdk-3.9.0/src/globus_sdk/utils.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      136 2022-06-02 17:29:38.000000 globus-sdk-3.9.0/src/globus_sdk/version.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-06-02 17:31:34.876232 globus-sdk-3.9.0/src/globus_sdk.egg-info/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2966 2022-06-02 17:31:34.000000 globus-sdk-3.9.0/src/globus_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5666 2022-06-02 17:31:34.000000 globus-sdk-3.9.0/src/globus_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2022-06-02 17:31:34.000000 globus-sdk-3.9.0/src/globus_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      358 2022-06-02 17:31:34.000000 globus-sdk-3.9.0/src/globus_sdk.egg-info/requires.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       11 2022-06-02 17:31:34.000000 globus-sdk-3.9.0/src/globus_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2811 2022-06-01 23:14:34.000000 globus-sdk-3.9.0/tox.ini
```

### Comparing `globus-sdk-3.8.0/COPYING` & `globus-sdk-3.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/LICENSE` & `globus-sdk-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/PKG-INFO` & `globus-sdk-3.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: globus-sdk
-Version: 3.8.0
+Version: 3.9.0
 Summary: Globus SDK for Python
 Home-page: https://github.com/globus/globus-sdk-python
 Author: Globus Team
 Author-email: support@globus.org
-License: UNKNOWN
 Keywords: globus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -86,9 +84,7 @@
 
 Links
 -----
 | Full Documentation: http://globus-sdk-python.readthedocs.io/
 | Source Code: https://github.com/globus/globus-sdk-python
 | API Documentation: https://docs.globus.org/api/
 | Release History + Changelog: https://github.com/globus/globus-sdk-python/releases
-
-
```

### Comparing `globus-sdk-3.8.0/README.rst` & `globus-sdk-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/setup.cfg` & `globus-sdk-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/setup.py` & `globus-sdk-3.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path
 import re
 
 from setuptools import find_packages, setup
 
 MYPY_REQUIREMENTS = [
-    "mypy==0.940",
+    "mypy==0.960",
     "types-docutils",
     "types-jwt",
     "types-requests",
     "typing-extensions",
 ]
 LINT_REQUIREMENTS = [
     "flake8<5",
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_sphinxext.py` & `globus-sdk-3.9.0/src/globus_sdk/_sphinxext.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/auth/get_identities.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/auth/get_identities.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/_common.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/_common.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/groups/get_my_groups.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/groups/get_my_groups.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/create_role.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/create_role.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/delete_role.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/delete_role.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/get_role_list.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/get_role_list.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/post_search.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/post_search.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/search/search.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/search/search.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/get_job.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/get_job.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/data/timer/update_job.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/data/timer/update_job.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/models.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,18 @@
         self.service = service
         self.path = path
         if service:
             self.full_url = slash_join(self._url_map[service], path)
         else:
             self.full_url = path
 
-        self.method = method
+        # convert the method to uppercase so that specifying `method="post"` will match
+        # correctly -- method matching is case sensitive but we don't need to expose the
+        # possibility of a non-uppercase method
+        self.method = method.upper()
         self.json = json
         self.body = body
 
         if headers is None:
             headers = {"Content-Type": "application/json"}
         self.headers = headers
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/_testing/registry.py` & `globus-sdk-3.9.0/src/globus_sdk/_testing/registry.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/authorizers/__init__.py` & `globus-sdk-3.9.0/src/globus_sdk/authorizers/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/authorizers/access_token.py` & `globus-sdk-3.9.0/src/globus_sdk/authorizers/access_token.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/authorizers/base.py` & `globus-sdk-3.9.0/src/globus_sdk/authorizers/base.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/authorizers/basic.py` & `globus-sdk-3.9.0/src/globus_sdk/authorizers/basic.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/authorizers/client_credentials.py` & `globus-sdk-3.9.0/src/globus_sdk/authorizers/client_credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
-from typing import Any, Callable, Dict, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
 
 from globus_sdk.scopes import MutableScope, _ScopeCollectionType
-from globus_sdk.services.auth import ConfidentialAppAuthClient, OAuthTokenResponse
+
+if TYPE_CHECKING:
+    from globus_sdk.services.auth import ConfidentialAppAuthClient, OAuthTokenResponse
 
 from .renewing import RenewingAuthorizer
 
 log = logging.getLogger(__name__)
 
 
 class ClientCredentialsAuthorizer(RenewingAuthorizer):
@@ -54,42 +56,42 @@
         ``on_refresh`` callback can be used to update the Access Tokens and
         their expiration times.
     :type on_refresh: callable, optional
     """
 
     def __init__(
         self,
-        confidential_client: ConfidentialAppAuthClient,
+        confidential_client: "ConfidentialAppAuthClient",
         scopes: _ScopeCollectionType,
         *,
         access_token: Optional[str] = None,
         expires_at: Optional[int] = None,
-        on_refresh: Optional[Callable[[OAuthTokenResponse], Any]] = None,
+        on_refresh: Optional[Callable[["OAuthTokenResponse"], Any]] = None,
     ):
 
         # values for _get_token_data
         self.confidential_client = confidential_client
         self.scopes = MutableScope.scopes2str(scopes)
 
         log.info(
             "Setting up ClientCredentialsAuthorizer with confidential_client="
             f"[instance:{id(confidential_client)}] and scopes={self.scopes}"
         )
 
         super().__init__(access_token, expires_at, on_refresh)
 
-    def _get_token_response(self) -> OAuthTokenResponse:
+    def _get_token_response(self) -> "OAuthTokenResponse":
         """
         Make a client credentials grant
         """
         return self.confidential_client.oauth2_client_credentials_tokens(
             requested_scopes=self.scopes
         )
 
-    def _extract_token_data(self, res: OAuthTokenResponse) -> Dict[str, Any]:
+    def _extract_token_data(self, res: "OAuthTokenResponse") -> Dict[str, Any]:
         """
         Get the tokens .by_resource_server,
         Ensure that only one token was gotten, and return that token.
         """
         token_data = res.by_resource_server.values()
         if len(token_data) != 1:
             raise ValueError(
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/authorizers/refresh_token.py` & `globus-sdk-3.9.0/src/globus_sdk/authorizers/refresh_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
-from typing import Any, Callable, Dict, Optional
-
-from globus_sdk.services.auth import AuthClient, OAuthTokenResponse
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
 
 from .renewing import RenewingAuthorizer
 
+if TYPE_CHECKING:
+    from globus_sdk.services.auth import AuthClient, OAuthTokenResponse
+
 log = logging.getLogger(__name__)
 
 
 class RefreshTokenAuthorizer(RenewingAuthorizer):
     r"""
     Implements Authorization using a Refresh Token to periodically fetch
     renewed Access Tokens. It may be initialized with an Access Token, or it
@@ -49,38 +50,38 @@
         their expiration times.
     :type on_refresh: callable, optional
     """
 
     def __init__(
         self,
         refresh_token: str,
-        auth_client: AuthClient,
+        auth_client: "AuthClient",
         *,
         access_token: Optional[str] = None,
         expires_at: Optional[int] = None,
-        on_refresh: Optional[Callable[[OAuthTokenResponse], Any]] = None,
+        on_refresh: Optional[Callable[["OAuthTokenResponse"], Any]] = None,
     ):
         log.info(
             "Setting up RefreshTokenAuthorizer with auth_client="
             f"[instance:{id(auth_client)}]"
         )
 
         # required for _get_token_data
         self.refresh_token = refresh_token
         self.auth_client = auth_client
 
         super().__init__(access_token, expires_at, on_refresh)
 
-    def _get_token_response(self) -> OAuthTokenResponse:
+    def _get_token_response(self) -> "OAuthTokenResponse":
         """
         Make a refresh token grant
         """
         return self.auth_client.oauth2_refresh_token(self.refresh_token)
 
-    def _extract_token_data(self, res: OAuthTokenResponse) -> Dict[str, Any]:
+    def _extract_token_data(self, res: "OAuthTokenResponse") -> Dict[str, Any]:
         """
         Get the tokens .by_resource_server,
         Ensure that only one token was gotten, and return that token.
 
         If the token_data includes a "refresh_token" field, update self.refresh_token to
         that value.
         """
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/authorizers/renewing.py` & `globus-sdk-3.9.0/src/globus_sdk/authorizers/renewing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import abc
 import logging
 import time
-from typing import Any, Callable, Dict, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
 
 from globus_sdk import exc, utils
-from globus_sdk.services.auth import OAuthTokenResponse
 
 from .base import GlobusAuthorizer
 
+if TYPE_CHECKING:
+    from globus_sdk.services.auth import OAuthTokenResponse
+
 log = logging.getLogger(__name__)
 # Provides a buffer for token expiration time to account for
 # possible delays or clock skew.
 EXPIRES_ADJUST_SECONDS = 60
 
 
 class RenewingAuthorizer(GlobusAuthorizer, metaclass=abc.ABCMeta):
@@ -46,15 +48,15 @@
     :type on_refresh: callable, optional
     """
 
     def __init__(
         self,
         access_token: Optional[str] = None,
         expires_at: Optional[int] = None,
-        on_refresh: Optional[Callable[[OAuthTokenResponse], Any]] = None,
+        on_refresh: Optional[Callable[["OAuthTokenResponse"], Any]] = None,
     ):
         self._access_token = None
         self._access_token_hash = None
 
         log.info(
             "Setting up a RenewingAuthorizer. It will use an "
             "auth type of Bearer and can handle 401s."
@@ -92,22 +94,22 @@
     @access_token.setter
     def access_token(self, value: Optional[str]) -> None:
         self._access_token = value
         if value:
             self._access_token_hash = utils.sha256_string(value)
 
     @abc.abstractmethod
-    def _get_token_response(self) -> OAuthTokenResponse:
+    def _get_token_response(self) -> "OAuthTokenResponse":
         """
         Using whatever method the specific authorizer implementing this class
         does, get a new token response.
         """
 
     @abc.abstractmethod
-    def _extract_token_data(self, res: OAuthTokenResponse) -> Dict[str, Any]:
+    def _extract_token_data(self, res: "OAuthTokenResponse") -> Dict[str, Any]:
         """
         Given a token response object, get the first element of
         token_response.by_resource_server
         This method is expected to enforce that by_resource_server is only
         returning one access token, and return a ValueError otherwise.
         """
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/client.py` & `globus-sdk-3.9.0/src/globus_sdk/client.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/config/env_vars.py` & `globus-sdk-3.9.0/src/globus_sdk/config/env_vars.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/config/environments.py` & `globus-sdk-3.9.0/src/globus_sdk/config/environments.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/exc/__init__.py` & `globus-sdk-3.9.0/src/globus_sdk/exc/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/exc/api.py` & `globus-sdk-3.9.0/src/globus_sdk/exc/api.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/exc/convert.py` & `globus-sdk-3.9.0/src/globus_sdk/exc/convert.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/exc/err_info.py` & `globus-sdk-3.9.0/src/globus_sdk/exc/err_info.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/local_endpoint/personal/endpoint.py` & `globus-sdk-3.9.0/src/globus_sdk/local_endpoint/personal/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/local_endpoint/personal/owner_info.py` & `globus-sdk-3.9.0/src/globus_sdk/local_endpoint/personal/owner_info.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/paging/__init__.py` & `globus-sdk-3.9.0/src/globus_sdk/paging/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/paging/base.py` & `globus-sdk-3.9.0/src/globus_sdk/paging/base.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/paging/last_key.py` & `globus-sdk-3.9.0/src/globus_sdk/paging/last_key.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/paging/limit_offset.py` & `globus-sdk-3.9.0/src/globus_sdk/paging/limit_offset.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/paging/marker.py` & `globus-sdk-3.9.0/src/globus_sdk/paging/marker.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/paging/next_token.py` & `globus-sdk-3.9.0/src/globus_sdk/paging/next_token.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/paging/table.py` & `globus-sdk-3.9.0/src/globus_sdk/paging/table.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/response.py` & `globus-sdk-3.9.0/src/globus_sdk/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import collections.abc
 import json
 import logging
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Iterator,
+    List,
     Mapping,
     Optional,
     Union,
     cast,
 )
 
 from requests import Response
@@ -27,15 +29,16 @@
     be used instead.
 
     The most common response data is a JSON dictionary. To make
     handling this type of response as seamless as possible, the
     ``GlobusHTTPResponse`` object implements the immutable mapping protocol for
     dict-style access. This is just an alias for access to the underlying data.
 
-    If ``data`` is not a dictionary, item access will raise ``TypeError``.
+    If the response data is not a dictionary or list, item access will raise
+    ``TypeError``.
 
     >>> print("Response ID": r["id"]) # alias for r.data["id"]
 
     :ivar client: The client instance which made the request
     """
 
     def __init__(
@@ -144,15 +147,15 @@
         if self.data is not None:
             return json.dumps(self.data, indent=2, separators=(",", ": "))
         return self.text
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.text})"
 
-    def __getitem__(self, key: str) -> Any:
+    def __getitem__(self, key: Union[str, int, slice]) -> Any:
         # force evaluation of the data property outside of the upcoming
         # try-catch so that we don't accidentally catch TypeErrors thrown
         # during the getter function itself
         data = self.data
         try:
             return data[key]
         except TypeError as err:
@@ -173,14 +176,20 @@
         """
         ``x in response`` is an alias for ``x in response.data``
         """
         if self.data is None:
             return False
         return item in self.data
 
+    def __bool__(self) -> bool:
+        """
+        ``bool(response)`` is an alias for ``bool(response.data)``
+        """
+        return bool(self.data)
+
 
 class IterableResponse(GlobusHTTPResponse):
     """This response class adds an __iter__ method on an 'iter_key' variable.
     The assumption is that iter produces dicts or dict-like mappings."""
 
     default_iter_key: ClassVar[str]
     iter_key: str
@@ -199,7 +208,25 @@
             )
         iter_key = iter_key if iter_key is not None else self.default_iter_key
         self.iter_key = iter_key
         super().__init__(response, client)
 
     def __iter__(self) -> Iterator[Mapping[Any, Any]]:
         return iter(cast(Mapping[Any, Any], self)[self.iter_key])
+
+
+class ArrayResponse(GlobusHTTPResponse):
+    """This response class adds an ``__iter__`` method which assumes that the top-level
+    data of the response is a JSON array."""
+
+    def __iter__(self) -> Iterator[Any]:
+        return iter(cast(List[Any], self.data))
+
+    def __len__(self) -> int:
+        """
+        ``len(response)`` is an alias for ``len(response.data)``
+        """
+        if not isinstance(self.data, collections.abc.Sequence):
+            raise TypeError(
+                f"Cannot take len() on data when type is '{type(self.data).__name__}'"
+            )
+        return len(self.data)
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/scopes.py` & `globus-sdk-3.9.0/src/globus_sdk/scopes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Iterable, Iterator, List, Union
+from typing import Dict, Iterable, Iterator, List, Tuple, Union
 
 from globus_sdk import utils
 
 # this type alias is meant for internal use, which is why it's named with an underscore
 _ScopeCollectionType = Union[
     str,
     "MutableScope",
@@ -106,14 +106,16 @@
         will set attributes on the instance using the URN scope format.
     :type known_scopes: list of str, optional
     :param known_url_scopes: A list of scope names to pre-populate on this instance.
         This will set attributes on the instance using the URL scope format.
     :type known_url_scopes: list of str, optional
     """
 
+    _classattr_scope_names: List[str] = []
+
     def __init__(
         self,
         resource_server: str,
         *,
         known_scopes: Union[List[str], str, None] = None,
         known_url_scopes: Union[List[str], str, None] = None,
     ) -> None:
@@ -124,19 +126,22 @@
             else []
         )
         self._known_url_scopes = (
             list(utils.safe_strseq_iter(known_url_scopes))
             if known_url_scopes is not None
             else []
         )
+        self._known_scope_names: List[str] = []
         if self._known_scopes:
             for scope_name in self._known_scopes:
+                self._known_scope_names.append(scope_name)
                 setattr(self, scope_name, self.urn_scope_string(scope_name))
         if self._known_url_scopes:
             for scope_name in self._known_url_scopes:
+                self._known_scope_names.append(scope_name)
                 setattr(self, scope_name, self.url_scope_string(scope_name))
 
     # custom __getattr__ instructs `mypy` that unknown attributes of a ScopeBuilder are
     # of type `str`, allowing for dynamic attribute names
     # to test, try creating a module with
     #
     #       from globus_sdk.scopes import TransferScopes
@@ -209,27 +214,40 @@
         MutableScope('urn:globus:auth:scope:transfer.api.globus.org:all')
 
         :param scope: The name of the scope to convert to a MutableScope
         :type scope: str
         """
         return MutableScope(getattr(self, scope))
 
+    def _iter_scopes(self) -> Iterator[Tuple[str, str]]:
+        for name in self._classattr_scope_names:
+            yield (name, getattr(self, name))
+        for name in self._known_scope_names:
+            yield (name, getattr(self, name))
+
+    def __str__(self) -> str:
+        return f"ScopeBuilder[{self.resource_server}]\n" + "\n".join(
+            f"  {k}:\n    {v}" for k, v in self._iter_scopes()
+        )
+
 
 class GCSEndpointScopeBuilder(ScopeBuilder):
     """
     A ScopeBuilder with a named property for the GCS manage_collections scope.
     "manage_collections" is a scope on GCS Endpoints. The resource_server string should
     be the GCS Endpoint ID.
 
     **Examples**
 
     >>> sb = GCSEndpointScopeBuilder("xyz")
     >>> mc_scope = sb.manage_collections
     """
 
+    _classattr_scope_names = ["manage_collections"]
+
     @property
     def manage_collections(self) -> str:
         return self.urn_scope_string("manage_collections")
 
 
 class GCSCollectionScopeBuilder(ScopeBuilder):
     """
@@ -237,22 +255,31 @@
     "data_access" is a scope on GCS Collections. The resource_server string should
     be the GCS Collection ID.
 
     **Examples**
 
     >>> sb = GCSCollectionScopeBuilder("xyz")
     >>> da_scope = sb.data_access
+    >>> https_scope = sb.https
     """
 
+    _classattr_scope_names = ["data_access", "https"]
+
     @property
     def data_access(self) -> str:
         return self.url_scope_string("data_access")
 
+    @property
+    def https(self) -> str:
+        return self.url_scope_string("https")
+
 
 class _AuthScopesBuilder(ScopeBuilder):
+    _classattr_scope_names = ["openid", "email", "profile"]
+
     openid: str = "openid"
     email: str = "email"
     profile: str = "profile"
 
 
 AuthScopes = _AuthScopesBuilder(
     "auth.globus.org",
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/__init__.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/client/base.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/client/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     # pylint can't handle quoted annotations yet:
     # https://github.com/PyCQA/pylint/issues/3299
     from typing import Literal  # pylint: disable=unused-import
 else:
     from typing_extensions import Literal
 
 from globus_sdk import client, exc, utils
+from globus_sdk._types import IntLike, UUIDLike
 from globus_sdk.authorizers import NullAuthorizer
 from globus_sdk.response import GlobusHTTPResponse
 from globus_sdk.scopes import AuthScopes
-from globus_sdk.types import IntLike, UUIDLike
 
 from ..errors import AuthAPIError
 from ..flow_managers import GlobusOAuthFlowManager
 from ..response import GetIdentitiesResponse, OAuthTokenResponse
 
 log = logging.getLogger(__name__)
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/client/confidential_client.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/client/confidential_client.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/client/native_client.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/client/native_client.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/authorization_code.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/authorization_code.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/base.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/base.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/flow_managers/native_app.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/flow_managers/native_app.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/identity_map.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/identity_map.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/auth/response/oauth.py` & `globus-sdk-3.9.0/src/globus_sdk/services/auth/response/oauth.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/gcs/client.py` & `globus-sdk-3.9.0/src/globus_sdk/services/groups/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,321 +1,298 @@
-import uuid
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar, Union
 
-from globus_sdk import client, paging, response, scopes, utils
-from globus_sdk.authorizers import GlobusAuthorizer
-from globus_sdk.types import UUIDLike
-
-from .data import CollectionDocument, GCSRoleDocument
-from .errors import GCSAPIError
-from .response import IterableGCSResponse, UnpackingGCSResponse
+from globus_sdk import client, response, utils
+from globus_sdk._types import UUIDLike
+from globus_sdk.scopes import GroupsScopes
+
+from .data import BatchMembershipActions, GroupPolicies
+from .errors import GroupsAPIError
 
 C = TypeVar("C", bound=Callable[..., Any])
 
 
-def _gcsdoc(message: str, link: str) -> Callable[[C], C]:
+def _groupdoc(message: str, link: str) -> Callable[[C], C]:
     # do not use functools.partial because it doesn't preserve type information
     # see: https://github.com/python/mypy/issues/1484
     def partial(func: C) -> C:
         return utils.doc_api_method(
             message,
             link,
-            external_base_url="https://docs.globus.org/globus-connect-server/v5/api",
+            external_base_url="https://groups.api.globus.org/redoc#operation",
         )(func)
 
     return partial
 
 
-class GCSClient(client.BaseClient):
+class GroupsClient(client.BaseClient):
     """
-    A GCSClient provides communication with the GCS Manager API of a Globus Connect
-    Server instance.
-    For full reference, see the `documentation for the GCS Manager API
-    <https://docs.globus.org/globus-connect-server/v5/api/>`_.
-
-    Unlike other client types, this must be provided with an address for the GCS
-    Manager. All other arguments are the same as those for `~globus_sdk.BaseClient`.
+    Client for the
+    `Globus Groups API <https://docs.globus.org/api/groups/>`_.
 
-    :param gcs_address: The FQDN (DNS name) or HTTPS URL for the GCS Manager API.
-    :type gcs_address: str
+    This provides a relatively low level client to public groups API endpoints.
+    You may also consider looking at the GroupsManager as a simpler interface
+    to more common actions.
 
-    .. automethodlist:: globus_sdk.GCSClient
+    .. automethodlist:: globus_sdk.GroupsClient
     """
 
-    service_name = "globus_connect_server"
-    error_class = GCSAPIError
-
-    def __init__(
-        self,
-        gcs_address: str,
-        *,
-        environment: Optional[str] = None,
-        authorizer: Optional[GlobusAuthorizer] = None,
-        app_name: Optional[str] = None,
-        transport_params: Optional[Dict[str, Any]] = None,
-    ):
-        # check if the provided address was a DNS name or an HTTPS URL
-        # if it was a URL, do not modify, but if it's a DNS name format it accordingly
-        # as a heuristic for this: just check if string starts with "https://" (this is
-        # sufficient to distinguish between the two for valid inputs)
-        if not gcs_address.startswith("https://"):
-            gcs_address = f"https://{gcs_address}/api/"
-        super().__init__(
-            base_url=gcs_address,
-            environment=environment,
-            authorizer=authorizer,
-            app_name=app_name,
-            transport_params=transport_params,
-        )
-
-    @staticmethod
-    def get_gcs_endpoint_scopes(
-        endpoint_id: Union[uuid.UUID, str]
-    ) -> scopes.GCSEndpointScopeBuilder:
-        """Given a GCS Endpoint ID, this helper constructs an object containing the
-        scopes for that Endpoint.
-
-        :param endpoint_id: The ID of the Endpoint
-        :type endpoint_id: UUID or str
-
-        See documentation for :class:`globus_sdk.scopes.GCSEndpointScopeBuilder` for
-        more information.
-        """
-        return scopes.GCSEndpointScopeBuilder(str(endpoint_id))
-
-    @staticmethod
-    def get_gcs_collection_scopes(
-        collection_id: Union[uuid.UUID, str]
-    ) -> scopes.GCSCollectionScopeBuilder:
-        """Given a GCS Collection ID, this helper constructs an object containing the
-        scopes for that Collection.
-
-        :param collection_id: The ID of the Collection
-        :type collection_id: UUID or str
+    base_path = "/v2/"
+    error_class = GroupsAPIError
+    service_name = "groups"
+    scopes = GroupsScopes
+
+    @_groupdoc(
+        "Retrieve your groups and membership",
+        "get_my_groups_and_memberships_v2_groups_my_groups_get",
+    )
+    def get_my_groups(
+        self, *, query_params: Optional[Dict[str, Any]] = None
+    ) -> response.ArrayResponse:
+        """
+        Return a list of groups your identity belongs to.
 
-        See documentation for :class:`globus_sdk.scopes.GCSCollectionScopeBuilder` for
-        more information.
+        :param query_params: Additional passthrough query parameters
+        :type query_params: dict, optional
         """
-        return scopes.GCSCollectionScopeBuilder(str(collection_id))
+        return response.ArrayResponse(
+            self.get("/groups/my_groups", query_params=query_params)
+        )
 
-    @_gcsdoc("List Collections", "openapi_Collections/#ListCollections")
-    def get_collection_list(
+    @_groupdoc("Get Group", "get_group_v2_groups__group_id__get")
+    def get_group(
         self,
+        group_id: UUIDLike,
         *,
-        mapped_collection_id: Optional[UUIDLike] = None,
-        filter: Union[  # pylint: disable=redefined-builtin
-            str, Iterable[str], None
-        ] = None,
-        include: Union[str, Iterable[str], None] = None,
+        include: Union[None, str, Iterable[str]] = None,
         query_params: Optional[Dict[str, Any]] = None,
-    ) -> IterableGCSResponse:
+    ) -> response.GlobusHTTPResponse:
         """
-        ``GET /collections``
+        Get details about a specific group
 
-        :param mapped_collection_id: Filter collections which were created using this
-            mapped collection ID.
-        :type mapped_collection_id: str or UUID
-        :param filter: Filter the returned set to any combination of the following:
-            ``mapped_collections``, ``guest_collections``, ``managed_by_me``,
-            ``created_by_me``.
-        :type filter: str or iterable of str, optional
-        :param include: Names of additional documents to include in the response
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param include: list of additional fields to include (allowed fields are
+            ``memberships``, ``my_memberships``, ``policies``, ``allowed_actions``, and
+            ``child_ids``)
         :type include: str or iterable of str, optional
-        :param query_params: Additional passthrough query parameters
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
-
-        List the Collections on an Endpoint
         """
         if query_params is None:
             query_params = {}
         if include is not None:
-            if isinstance(include, str):
-                include = [include]
-            query_params["include"] = ",".join(include)
-        if mapped_collection_id is not None:
-            query_params["mapped_collection_id"] = mapped_collection_id
-        if filter is not None:
-            if isinstance(filter, str):
-                filter = [filter]
-            query_params["filter"] = ",".join(filter)
-        return IterableGCSResponse(self.get("collections", query_params=query_params))
+            query_params["include"] = ",".join(utils.safe_strseq_iter(include))
+        return self.get(f"/groups/{group_id}", query_params=query_params)
 
-    @_gcsdoc("Get Collection", "openapi_Collections/#getCollection")
-    def get_collection(
-        self,
-        collection_id: UUIDLike,
-        *,
-        query_params: Optional[Dict[str, Any]] = None,
-    ) -> UnpackingGCSResponse:
+    @_groupdoc("Delete a group", "delete_group_v2_groups__group_id__delete")
+    def delete_group(
+        self, group_id: UUIDLike, *, query_params: Optional[Dict[str, Any]] = None
+    ) -> response.GlobusHTTPResponse:
         """
-        ``GET /collections/{collection_id}``
+        Delete a group.
 
-        :param collection_id: The ID of the collection to lookup
-        :type collection_id: str or UUID
-        :param query_params: Additional passthrough query parameters
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
+        """
+        return self.delete(f"/groups/{group_id}", query_params=query_params)
 
-        Lookup a Collection on an Endpoint
+    @_groupdoc("Create a group", "create_group_v2_groups_post")
+    def create_group(
+        self, data: Dict[str, Any], *, query_params: Optional[Dict[str, Any]] = None
+    ) -> response.GlobusHTTPResponse:
         """
-        return UnpackingGCSResponse(
-            self.get(f"/collections/{collection_id}", query_params=query_params),
-            "collection",
-        )
+        Create a group.
 
-    @_gcsdoc("Create Collection", "openapi_Collections/#createCollection")
-    def create_collection(
-        self,
-        collection_data: Union[Dict[str, Any], CollectionDocument],
-    ) -> UnpackingGCSResponse:
+        :param data: the group document to create
+        :type data: dict
+        :param query_params: additional passthrough query parameters
+        :type query_params: dict, optional
         """
-        ``POST /collections``
+        return self.post("/groups", data=data, query_params=query_params)
 
-        Create a collection. This is used to create either a mapped or a guest
-        collection. When created, a ``collection:administrator`` role for that
-        collection will be created using the caller’s identity.
+    @_groupdoc("Update a group", "update_group_v2_groups__group_id__put")
+    def update_group(
+        self,
+        group_id: UUIDLike,
+        data: Dict[str, Any],
+        *,
+        query_params: Optional[Dict[str, Any]] = None,
+    ) -> response.GlobusHTTPResponse:
+        """
+        Update a given group.
 
-        In order to create a guest collection, the caller must have an identity that
-        matches the Storage Gateway policies.
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param data: the group document to use for update
+        :type data: dict
+        :param query_params: additional passthrough query parameters
+        :type query_params: dict, optional
+        """
+        return self.put(f"/groups/{group_id}", data=data, query_params=query_params)
 
-        In order to create a mapped collection, the caller must have an
-        ``endpoint:administrator`` or ``endpoint:owner`` role.
+    @_groupdoc(
+        "Get the policies for the group",
+        "get_policies_v2_groups__group_id__policies_get",
+    )
+    def get_group_policies(
+        self, group_id: UUIDLike, *, query_params: Optional[Dict[str, Any]] = None
+    ) -> response.GlobusHTTPResponse:
+        """
+        Get policies for the given group
 
-        :param collection_data: The collection document for the new collection
-        :type collection_data: dict or CollectionDocument
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param query_params: additional passthrough query parameters
+        :type query_params: dict, optional
         """
-        return UnpackingGCSResponse(
-            self.post("/collections", data=collection_data), "collection"
-        )
+        return self.get(f"/groups/{group_id}/policies", query_params=query_params)
 
-    @_gcsdoc("Update Collection", "openapi_Collections/#patchCollection")
-    def update_collection(
+    @_groupdoc(
+        "Set the policies for the group",
+        "update_policies_v2_groups__group_id__policies_put",
+    )
+    def set_group_policies(
         self,
-        collection_id: UUIDLike,
-        collection_data: Union[Dict[str, Any], CollectionDocument],
+        group_id: UUIDLike,
+        data: Union[Dict[str, Any], GroupPolicies],
         *,
         query_params: Optional[Dict[str, Any]] = None,
-    ) -> UnpackingGCSResponse:
+    ) -> response.GlobusHTTPResponse:
         """
-        ``PATCH /collections/{collection_id}``
+        Set policies for the group.
 
-        :param collection_id: The ID of the collection to update
-        :type collection_id: str or UUID
-        :param collection_data: The collection document for the modified collection
-        :type collection_data: dict or CollectionDocument
-        :param query_params: Additional passthrough query parameters
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param data: the group policy document to set
+        :type data: dict or ``GroupPolicies``
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
         """
-        return UnpackingGCSResponse(
-            self.patch(
-                f"/collections/{collection_id}",
-                data=collection_data,
-                query_params=query_params,
-            ),
-            "collection",
+        return self.put(
+            f"/groups/{group_id}/policies", data=data, query_params=query_params
         )
 
-    @_gcsdoc("Delete Collection", "openapi_Collections/#deleteCollection")
-    def delete_collection(
-        self,
-        collection_id: UUIDLike,
-        *,
-        query_params: Optional[Dict[str, Any]] = None,
+    @_groupdoc(
+        "Get the preferences for your identity set",
+        "get_identity_set_preferences_v2_preferences_get",
+    )
+    def get_identity_preferences(
+        self, *, query_params: Optional[Dict[str, Any]] = None
     ) -> response.GlobusHTTPResponse:
         """
-        ``DELETE /collections/{collection_id}``
+        Get identity preferences.  Currently this only includes whether the
+        user allows themselves to be added to groups.
 
-        :param collection_id: The ID of the collection to delete
-        :type collection_id: str or UUID
-        :param query_params: Additional passthrough query parameters
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
         """
-        return self.delete(f"/collections/{collection_id}", query_params=query_params)
+        return self.get("/preferences", query_params=query_params)
 
-    @_gcsdoc("List Roles", "openapi_Roles/#listRoles")
-    @paging.has_paginator(
-        paging.MarkerPaginator,
-        items_key="data",
+    @_groupdoc(
+        "Set the preferences for your identity set",
+        "put_identity_set_preferences_v2_preferences_put",
     )
-    def get_role_list(
+    def set_identity_preferences(
         self,
-        collection_id: Optional[UUIDLike] = None,
-        include: Optional[str] = None,
+        data: Dict[str, Any],
+        *,
         query_params: Optional[Dict[str, Any]] = None,
-    ) -> IterableGCSResponse:
+    ) -> response.GlobusHTTPResponse:
         """
-        ``GET /roles``
+        Set identity preferences.  Currently this only includes whether the
+        user allows themselves to be added to groups.
 
-        :param collection_id: UUID of a Collection. If given then only roles
-            related to that Collection are returned, otherwise only Endpoint
-            roles are returned.
-        :type collection_id: str or UUID, optional
-        :param include: Pass "all_roles" to request all roles all roles
-            relevant to the resource instead of only those the caller has on
-            the resource
-        :type include: str, optional
-        :param query_params: Additional passthrough query parameters
+        :param data: the identity set preferences document
+        :type data: dict
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
-        """
-        if query_params is None:
-            query_params = {}
-        if include is not None:
-            query_params["include"] = include
-        if collection_id is not None:
-            query_params["collection_id"] = collection_id
 
-        path = "/roles"
-        return IterableGCSResponse(self.get(path, query_params=query_params))
+        **Examples**
 
-    @_gcsdoc("Create Role", "openapi_Roles/#postRole")
-    def create_role(
+        >>> gc = globus_sdk.GroupsClient(...)
+        >>> gc.set_identity_preferences({"allow_add": False})
+        """
+        return self.put("/preferences", data=data, query_params=query_params)
+
+    @_groupdoc(
+        "Get the membership fields for your identity set",
+        "get_membership_fields_v2_groups__group_id__membership_fields_get",
+    )
+    def get_membership_fields(
         self,
-        data: Union[Dict[str, Any], GCSRoleDocument],
+        group_id: UUIDLike,
+        *,
         query_params: Optional[Dict[str, Any]] = None,
-    ) -> UnpackingGCSResponse:
+    ) -> response.GlobusHTTPResponse:
         """
-        POST /roles
+        Get membership fields for your identities.
 
-        :param data: Data in the format of a Role document, it is recommended
-            to use the `RoleDocumment` class to construct this data.
-        :type data: dict
-        :param query_params: Additional passthrough query parameters
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
         """
-        path = "/roles"
-        return UnpackingGCSResponse(
-            self.post(path, data=data, query_params=query_params),
-            "role",
+        return self.get(
+            f"/groups/{group_id}/membership_fields", query_params=query_params
         )
 
-    @_gcsdoc("Get a Role", "openapi_Roles/#getRole")
-    def get_role(
+    @_groupdoc(
+        "Set the membership fields for your identity set",
+        "put_membership_fields_v2_groups__group_id__membership_fields_put",
+    )
+    def set_membership_fields(
         self,
-        role_id: UUIDLike,
+        group_id: UUIDLike,
+        data: Dict[Any, str],
+        *,
         query_params: Optional[Dict[str, Any]] = None,
-    ) -> UnpackingGCSResponse:
+    ) -> response.GlobusHTTPResponse:
         """
-        GET /roles/{role_id}
+        Set membership fields for your identities.
 
-        :param role_id: UUID for the Role to be gotten
-        :type role_id: str or UUID
-        :param query_params: Additional passthrough query parameters
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param data: the membership fields document
+        :type data: dict
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
         """
-        path = f"/roles/{role_id}"
-        return UnpackingGCSResponse(self.get(path, query_params=query_params), "role")
+        return self.put(
+            f"/groups/{group_id}/membership_fields",
+            data=data,
+            query_params=query_params,
+        )
 
-    @_gcsdoc("Delete a Role", "openapi_Roles/#deleteRole")
-    def delete_role(
+    @_groupdoc(
+        "Perform actions on members of the group",
+        "group_membership_post_actions_v2_groups__group_id__post",
+    )
+    def batch_membership_action(
         self,
-        role_id: UUIDLike,
+        group_id: UUIDLike,
+        actions: Union[Dict[str, Any], BatchMembershipActions],
+        *,
         query_params: Optional[Dict[str, Any]] = None,
     ) -> response.GlobusHTTPResponse:
         """
-        DELETE /roles/{role_id}
+        Execute a batch of actions against several group memberships.
 
-        :param role_id: UUID for the Role to be deleted
-        :type role_id: str or UUID
-        :param query_params: Additional passthrough query parameters
+        :param group_id: the ID of the group
+        :type group_id: str or UUID
+        :param actions: the batch of membership actions to perform, modifying, creating,
+            and removing memberships in the group
+        :type actions: dict or BatchMembershipActions
+        :param query_params: additional passthrough query parameters
         :type query_params: dict, optional
+
+        **Examples**
+
+        >>> gc = globus_sdk.GroupsClient(...)
+        >>> group_id = ...
+        >>> batch = globus_sdk.BatchMembershipActions()
+        >>> batch.add_members("ae332d86-d274-11e5-b885-b31714a110e9")
+        >>> batch.invite_members("c699d42e-d274-11e5-bf75-1fc5bf53bb24")
+        >>> gc.batch_membership_action(group_id, batch)
         """
-        path = f"/roles/{role_id}"
-        return self.delete(path, query_params=query_params)
+        return self.post(f"/groups/{group_id}", data=actions, query_params=query_params)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/gcs/data.py` & `globus-sdk-3.9.0/src/globus_sdk/services/gcs/data/collection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import abc
-from typing import Any, Callable, Dict, Iterable, Optional, Tuple
+from typing import Any, Dict, Iterable, Optional, Tuple
 
 from globus_sdk import utils
-from globus_sdk.types import UUIDLike
+from globus_sdk._types import UUIDLike
+
+from ._common import ensure_datatype
 
 #
 # NOTE -- on the organization of arguments in this module --
 #
 # The arguments to each collection type are defined explicitly for good type annotations
 # and documentation.
 # However, it's easy for things to get out of sync or different between the various
@@ -99,14 +101,15 @@
     :param public: If True, the collection will be visible to other Globus users
     :type public: bool, optional
 
     :param additional_fields: Additional data for inclusion in the collection document
     :type additional_fields: dict, optional
     """
 
+    DATATYPE_BASE: str = "collection"
     DATATYPE_VERSION_IMPLICATIONS: Dict[str, Tuple[int, int, int]] = {
         "disable_anonymous_writes": (1, 5, 0),
         "force_verify": (1, 4, 0),
         "sharing_users_allow": (1, 2, 0),
         "sharing_users_deny": (1, 2, 0),
         "enable_https": (1, 1, 0),
         "user_message": (1, 1, 0),
@@ -173,45 +176,14 @@
             self.update(additional_fields)
 
     @property
     @abc.abstractmethod
     def collection_type(self) -> str:
         raise NotImplementedError
 
-    def _deduce_datatype_version(self) -> str:
-        max_deduced_version = (1, 0, 0)
-        for fieldname, version in self.DATATYPE_VERSION_IMPLICATIONS.items():
-            if fieldname not in self:
-                continue
-            if version > max_deduced_version:
-                max_deduced_version = version
-        return ".".join(str(x) for x in max_deduced_version)
-
-    def _ensure_datatype(self) -> None:
-        if "DATA_TYPE" not in self:
-            self["DATA_TYPE"] = f"collection#{self._deduce_datatype_version()}"
-
-    def _set_value(
-        self, key: str, val: Any, callback: Optional[Callable[[Any], Any]] = None
-    ) -> None:
-        if val is not None:
-            self[key] = callback(val) if callback else val
-
-    def _set_optstrs(self, **kwargs: Any) -> None:
-        for k, v in kwargs.items():
-            self._set_value(k, v, callback=str)
-
-    def _set_optstrlists(self, **kwargs: Optional[Iterable[Any]]) -> None:
-        for k, v in kwargs.items():
-            self._set_value(k, v, callback=lambda x: list(utils.safe_strseq_iter(x)))
-
-    def _set_optbools(self, **kwargs: Optional[bool]) -> None:
-        for k, v in kwargs.items():
-            self._set_value(k, v, callback=bool)
-
 
 class MappedCollectionDocument(CollectionDocument):
     """
     An object used to represent a Mapped Collection for creation or update operations.
     The initializer supports all writable fields on Mapped Collections but does not
     include read-only fields like ``id``.
 
@@ -338,15 +310,15 @@
         )
         self._set_optbools(
             allow_guest_collections=allow_guest_collections,
             disable_anonymous_writes=disable_anonymous_writes,
         )
         self._set_value("sharing_restrict_paths", sharing_restrict_paths)
         self._set_value("policies", policies)
-        self._ensure_datatype()
+        ensure_datatype(self)
 
 
 class GuestCollectionDocument(CollectionDocument):
     """
     An object used to represent a Guest Collection for creation or update operations.
     The initializer supports all writable fields on Guest Collections but does not
     include read-only fields like ``id``.
@@ -436,56 +408,8 @@
             # additional fields
             additional_fields=additional_fields,
         )
         self._set_optstrs(
             mapped_collection_id=mapped_collection_id,
             user_credential_id=user_credential_id,
         )
-        self._ensure_datatype()
-
-
-class GCSRoleDocument(utils.PayloadWrapper):
-    """
-    Convenience class for constructing a Role document
-    to use as the `data` parameter to `create_role`
-
-    :param DATA_TYPE: Versioned document type.
-    :type DATA_TYPE: str
-    :param collection: Collection ID for the collection the role will apply to.
-        This value is omitted when creating an endpoint
-        role or when creating role definitions when creating collections.
-    :type collection: str or UUID, optional
-    :param principal: Auth identity or group id URN. Should be in the format
-        urn:globus:auth:[identity|group]:{uuid of identity or group}
-    :type principal: str, optional
-    :param role: Role assigned to the principal. Known values are owner,
-        administrator, access_manager, activity_manager, and activity_monitor
-    :type role: str, optional
-    """
-
-    def _set_value(
-        self, key: str, val: Any, callback: Optional[Callable[[Any], Any]] = None
-    ) -> None:
-        if val is not None:
-            self[key] = callback(val) if callback else val
-
-    def _set_optstrs(self, **kwargs: Any) -> None:
-        for k, v in kwargs.items():
-            self._set_value(k, v, callback=str)
-
-    def __init__(
-        self,
-        DATA_TYPE: str = "role#1.0.0",
-        collection: Optional[UUIDLike] = None,
-        principal: Optional[str] = None,
-        role: Optional[str] = None,
-        additional_fields: Optional[Dict[str, Any]] = None,
-    ) -> None:
-        super().__init__()
-        self._set_optstrs(
-            DATA_TYPE=DATA_TYPE,
-            collection=collection,
-            principal=principal,
-            role=role,
-        )
-        if additional_fields is not None:
-            self.update(additional_fields)
+        ensure_datatype(self)
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/gcs/errors.py` & `globus-sdk-3.9.0/src/globus_sdk/services/gcs/errors.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/gcs/response.py` & `globus-sdk-3.9.0/src/globus_sdk/services/gcs/response.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/groups/data.py` & `globus-sdk-3.9.0/src/globus_sdk/services/groups/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from typing import Any, Iterable, Optional
 
 from globus_sdk import utils
-from globus_sdk.types import UUIDLike
+from globus_sdk._types import UUIDLike
 
 
 class GroupRole(Enum):
     member = "member"
     manager = "manager"
     admin = "admin"
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/groups/manager.py` & `globus-sdk-3.9.0/src/globus_sdk/services/groups/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Iterable, Optional
 
 from globus_sdk import response
-from globus_sdk.types import UUIDLike
+from globus_sdk._types import UUIDLike
 
 from .client import GroupsClient
 from .data import (
     BatchMembershipActions,
     GroupMemberVisibility,
     GroupPolicies,
     GroupRequiredSignupFields,
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/search/client.py` & `globus-sdk-3.9.0/src/globus_sdk/services/search/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, Dict, Optional, Union
 
 from globus_sdk import client, paging, response, utils
+from globus_sdk._types import UUIDLike
 from globus_sdk.scopes import SearchScopes
-from globus_sdk.types import UUIDLike
 
 from .data import SearchQuery, SearchScrollQuery
 from .errors import SearchAPIError
 
 log = logging.getLogger(__name__)
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/search/data.py` & `globus-sdk-3.9.0/src/globus_sdk/services/search/data.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/search/errors.py` & `globus-sdk-3.9.0/src/globus_sdk/services/search/errors.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/timer/client.py` & `globus-sdk-3.9.0/src/globus_sdk/services/timer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, Dict, Optional, Union
 
 from globus_sdk import client, response
+from globus_sdk._types import UUIDLike
 from globus_sdk.scopes import TimerScopes
-from globus_sdk.types import UUIDLike
 
 from .data import TimerJob
 from .errors import TimerAPIError
 
 log = logging.getLogger(__name__)
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/timer/data.py` & `globus-sdk-3.9.0/src/globus_sdk/services/timer/data.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/timer/errors.py` & `globus-sdk-3.9.0/src/globus_sdk/services/timer/errors.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/transfer/client.py` & `globus-sdk-3.9.0/src/globus_sdk/services/transfer/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import time
 import uuid
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, Union
 
 from globus_sdk import client, exc, paging, response, utils
+from globus_sdk._types import DateLike, IntLike, UUIDLike
 from globus_sdk.scopes import TransferScopes
-from globus_sdk.types import DateLike, IntLike, UUIDLike
 
 from .data import DeleteData, TransferData
 from .errors import TransferAPIError
 from .response import ActivationRequirementsResponse, IterableTransferResponse
 from .transport import TransferRequestsTransport
 
 log = logging.getLogger(__name__)
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/transfer/data/delete_data.py` & `globus-sdk-3.9.0/src/globus_sdk/services/transfer/data/delete_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import logging
 from typing import TYPE_CHECKING, Any, Dict, Iterator, Optional, Union
 
 from globus_sdk import utils
-from globus_sdk.types import UUIDLike
+from globus_sdk._types import UUIDLike
 
 if TYPE_CHECKING:
     import globus_sdk
 
 log = logging.getLogger(__name__)
 
 
@@ -43,14 +43,17 @@
     :param deadline: An ISO-8601 timestamp (as a string) or a datetime object which
         defines a deadline for the deletion. At the deadline, even if the data deletion
         is not complete, the job will be canceled. We recommend ensuring that the
         timestamp is in UTC to avoid confusion and ambiguity. Examples of ISO-8601
         timestamps include ``2017-10-12 09:30Z``, ``2017-10-12 12:33:54+00:00``, and
         ``2017-10-12``
     :type deadline: str or datetime, optional
+    :param skip_activation_check: When true, allow submission even if the endpoint
+        isn't currently activated
+    :type skip_activation_check: bool, optional
     :param notify_on_succeeded: Send a notification email when the delete task
         completes with a status of SUCCEEDED.
         [default: ``True``]
     :type notify_on_succeeded: bool, optional
     :param notify_on_failed: Send a notification email when the delete task completes
         with a status of FAILED.
         [default: ``True``]
@@ -86,28 +89,30 @@
         transfer_client: "globus_sdk.TransferClient",
         endpoint: UUIDLike,
         *,
         label: Optional[str] = None,
         submission_id: Optional[UUIDLike] = None,
         recursive: bool = False,
         deadline: Optional[Union[str, datetime.datetime]] = None,
+        skip_activation_check: bool = False,
         notify_on_succeeded: bool = True,
         notify_on_failed: bool = True,
         notify_on_inactive: bool = True,
         additional_fields: Optional[Dict[str, Any]] = None,
     ) -> None:
         super().__init__()
         self["DATA_TYPE"] = "delete"
         self["submission_id"] = (
             str(submission_id)
             if submission_id is not None
             else transfer_client.get_submission_id()["value"]
         )
         self["endpoint"] = str(endpoint)
         self["recursive"] = recursive
+        self["skip_activation_check"] = skip_activation_check
         self["notify_on_succeeded"] = notify_on_succeeded
         self["notify_on_failed"] = notify_on_failed
         self["notify_on_inactive"] = notify_on_inactive
 
         if label is not None:
             self["label"] = label
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/transfer/data/transfer_data.py` & `globus-sdk-3.9.0/src/globus_sdk/services/transfer/data/transfer_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import datetime
 import logging
+import sys
 from typing import TYPE_CHECKING, Any, Dict, Iterator, Optional, Union
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 from globus_sdk import utils
-from globus_sdk.types import UUIDLike
+from globus_sdk._types import UUIDLike
 
 if TYPE_CHECKING:
     import globus_sdk
 
 log = logging.getLogger(__name__)
 
 
@@ -66,14 +72,17 @@
     :param recursive_symlinks: Specify the behavior of recursive directory transfers
         when encountering symlinks. One of ``"ignore"``, ``"keep"``, or ``"copy"``.
         ``"ignore"`` skips symlinks, ``"keep"`` creates symlinks at the destination
         matching the source (without modifying the link path at all), and
         ``"copy"`` follows symlinks on the source, failing if the link is invalid.
         [default: ``"ignore"``]
     :type recursive_symlinks: str
+    :param skip_activation_check: When true, allow submission even if the endpoints
+        aren't currently activated
+    :type skip_activation_check: bool, optional
     :param skip_source_errors: When true, source permission denied and file
         not found errors from the source endpoint will cause the offending
         path to be skipped.
         [default: ``False``]
     :type skip_source_errors: bool, optional
     :param fail_on_quota_errors: When true, quota exceeded errors will cause the
         task to fail.
@@ -151,19 +160,22 @@
         self,
         transfer_client: "globus_sdk.TransferClient",
         source_endpoint: UUIDLike,
         destination_endpoint: UUIDLike,
         *,
         label: Optional[str] = None,
         submission_id: Optional[UUIDLike] = None,
-        sync_level: Union[str, int, None] = None,
+        sync_level: Union[
+            Literal["exists", "size", "mtime", "checksum"], int, None
+        ] = None,
         verify_checksum: bool = False,
         preserve_timestamp: bool = False,
         encrypt_data: bool = False,
         deadline: Optional[Union[datetime.datetime, str]] = None,
+        skip_activation_check: bool = False,
         skip_source_errors: bool = False,
         fail_on_quota_errors: bool = False,
         recursive_symlinks: str = "ignore",
         delete_destination_extra: bool = False,
         notify_on_succeeded: bool = True,
         notify_on_failed: bool = True,
         notify_on_inactive: bool = True,
@@ -177,14 +189,15 @@
         )
         self["source_endpoint"] = str(source_endpoint)
         self["destination_endpoint"] = str(destination_endpoint)
         self["verify_checksum"] = verify_checksum
         self["preserve_timestamp"] = preserve_timestamp
         self["encrypt_data"] = encrypt_data
         self["recursive_symlinks"] = recursive_symlinks
+        self["skip_activation_check"] = skip_activation_check
         self["skip_source_errors"] = skip_source_errors
         self["fail_on_quota_errors"] = fail_on_quota_errors
         self["delete_destination_extra"] = delete_destination_extra
         self["notify_on_succeeded"] = notify_on_succeeded
         self["notify_on_failed"] = notify_on_failed
         self["notify_on_inactive"] = notify_on_inactive
         if label is not None:
@@ -309,14 +322,64 @@
                 self["destination_endpoint"],
                 source_path,
                 destination_path,
             )
         )
         self["DATA"].append(item_data)
 
+    def add_filter_rule(
+        self,
+        name: str,
+        *,
+        method: Literal["exclude"] = "exclude",
+        type: Optional[  # pylint: disable=redefined-builtin
+            Literal["file", "dir"]
+        ] = None,
+    ) -> None:
+        """
+        Add a filter rule to the transfer document.
+
+        These rules specify which items are or are not included when recursively
+        transferring directories.
+
+        Currently, only ``method="exclude"`` (the default) is supported. This means that
+        items matching the ``name`` field will be excluded from the transfer.
+
+        :param name: A pattern to match against item names. Wildcards are supported, as
+            are character groups: ``*`` matches everything, ``?`` matches any single
+            character, ``[]`` matches any single character within the brackets, and
+            ``[!]`` matches any single character not within the brackets.
+        :type name: str
+        :param method: The method to use for filtering. Only the default, ``"exclude"``
+            is supported.
+        :type method: str, optional
+        :param type: The types of items on which to apply this filter rule. Either
+            ``"file"`` or ``"dir"``. If unspecified, the rule applies to both.
+        :type type: str, optional
+
+        Example Usage:
+
+        >>> tdata = TransferData(...)
+        >>> tdata.add_filter_rule("*.tgz", type="file")
+        >>> tdata.add_filter_rule("*.tar.gz", type="file")
+
+        ``tdata`` now describes a transfer which will skip any gzipped tar files with
+        the extensions `.tgz` or `.tar.gz`
+        """
+        if "filter_rules" not in self:
+            self["filter_rules"] = []
+        rule = {
+            "DATA_TYPE": "filter_rule",
+            "method": method,
+            "name": name,
+        }
+        if type is not None:
+            rule["type"] = type
+        self["filter_rules"].append(rule)
+
     def iter_items(self) -> Iterator[Dict[str, Any]]:
         """
         An iterator of items created by ``add_item``.
 
         Each item takes the form of a dictionary.
         """
         yield from iter(self["DATA"])
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/transfer/errors.py` & `globus-sdk-3.9.0/src/globus_sdk/services/transfer/errors.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/transfer/response/activation.py` & `globus-sdk-3.9.0/src/globus_sdk/services/transfer/response/activation.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/transfer/response/iterable.py` & `globus-sdk-3.9.0/src/globus_sdk/services/transfer/response/iterable.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/services/transfer/transport.py` & `globus-sdk-3.9.0/src/globus_sdk/services/transfer/transport.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/tokenstorage/base.py` & `globus-sdk-3.9.0/src/globus_sdk/tokenstorage/base.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/tokenstorage/file_adapters.py` & `globus-sdk-3.9.0/src/globus_sdk/tokenstorage/file_adapters.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/tokenstorage/sqlite_adapter.py` & `globus-sdk-3.9.0/src/globus_sdk/tokenstorage/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/transport/__init__.py` & `globus-sdk-3.9.0/src/globus_sdk/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/transport/encoders.py` & `globus-sdk-3.9.0/src/globus_sdk/transport/encoders.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/transport/requests.py` & `globus-sdk-3.9.0/src/globus_sdk/transport/requests.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/transport/retry.py` & `globus-sdk-3.9.0/src/globus_sdk/transport/retry.py`

 * *Files identical despite different names*

### Comparing `globus-sdk-3.8.0/src/globus_sdk/utils.py` & `globus-sdk-3.9.0/src/globus_sdk/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -117,26 +117,49 @@
 
     Payload types inheriting from this class can be passed directly to the client
     ``post()``, ``put()``, and ``patch()`` methods instead of a dict. These methods will
     recognize a ``PayloadWrapper`` and convert it to a dict for serialization with the
     requested encoder (e.g. as a JSON request body).
     """
 
-    # note: this class doesn't actually define any methods, properties, or attributes
-    # it's just our own flavor of UserDict, which wraps a 'data' dict
-    #
     # use UserDict rather than subclassing dict so that our API is always consistent
     # e.g. `dict.pop` does not invoke `dict.__delitem__`. Overriding `__delitem__` on a
     # dict subclass can lead to inconsistent behavior between usages like these:
     #   x = d["k"]; del d["k"]
     #   x = d.pop("k")
     #
     # UserDict inherits from MutableMapping and only defines the dunder methods, so
     # changing its behavior safely/consistently is simpler
 
+    #
+    # internal helpers for setting non-null values
+    #
+
+    def _set_value(
+        self, key: str, val: Any, callback: Optional[Callable[[Any], Any]] = None
+    ) -> None:
+        if val is not None:
+            self[key] = callback(val) if callback else val
+
+    def _set_optstrs(self, **kwargs: Any) -> None:
+        for k, v in kwargs.items():
+            self._set_value(k, v, callback=str)
+
+    def _set_optstrlists(self, **kwargs: Optional[Iterable[Any]]) -> None:
+        for k, v in kwargs.items():
+            self._set_value(k, v, callback=lambda x: list(safe_strseq_iter(x)))
+
+    def _set_optbools(self, **kwargs: Optional[bool]) -> None:
+        for k, v in kwargs.items():
+            self._set_value(k, v, callback=bool)
+
+    def _set_optints(self, **kwargs: Any) -> None:
+        for k, v in kwargs.items():
+            self._set_value(k, v, callback=int)
+
 
 def in_sphinx_build() -> bool:  # pragma: no cover
     # check if `sphinx-build` was used to invoke
     return os.path.basename(sys.argv[0]) in ["sphinx-build", "sphinx-build.exe"]
 
 
 class _classproperty(Generic[T, R]):
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk.egg-info/PKG-INFO` & `globus-sdk-3.9.0/src/globus_sdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: globus-sdk
-Version: 3.8.0
+Version: 3.9.0
 Summary: Globus SDK for Python
 Home-page: https://github.com/globus/globus-sdk-python
 Author: Globus Team
 Author-email: support@globus.org
-License: UNKNOWN
 Keywords: globus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -86,9 +84,7 @@
 
 Links
 -----
 | Full Documentation: http://globus-sdk-python.readthedocs.io/
 | Source Code: https://github.com/globus/globus-sdk-python
 | API Documentation: https://docs.globus.org/api/
 | Release History + Changelog: https://github.com/globus/globus-sdk-python/releases
-
-
```

### Comparing `globus-sdk-3.8.0/src/globus_sdk.egg-info/SOURCES.txt` & `globus-sdk-3.9.0/src/globus_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 tox.ini
 src/globus_sdk/__init__.py
+src/globus_sdk/_generate_init.py
 src/globus_sdk/_sphinxext.py
+src/globus_sdk/_types.py
 src/globus_sdk/client.py
 src/globus_sdk/py.typed
 src/globus_sdk/response.py
 src/globus_sdk/scopes.py
-src/globus_sdk/types.py
 src/globus_sdk/utils.py
 src/globus_sdk/version.py
 src/globus_sdk.egg-info/PKG-INFO
 src/globus_sdk.egg-info/SOURCES.txt
 src/globus_sdk.egg-info/dependency_links.txt
 src/globus_sdk.egg-info/requires.txt
 src/globus_sdk.egg-info/top_level.txt
@@ -24,14 +25,20 @@
 src/globus_sdk/_testing/models.py
 src/globus_sdk/_testing/registry.py
 src/globus_sdk/_testing/data/__init__.py
 src/globus_sdk/_testing/data/auth/__init__.py
 src/globus_sdk/_testing/data/auth/_common.py
 src/globus_sdk/_testing/data/auth/get_identities.py
 src/globus_sdk/_testing/data/auth/oauth2_userinfo.py
+src/globus_sdk/_testing/data/globus_connect_server/__init__.py
+src/globus_sdk/_testing/data/globus_connect_server/create_storage_gateway.py
+src/globus_sdk/_testing/data/globus_connect_server/delete_storage_gateway.py
+src/globus_sdk/_testing/data/globus_connect_server/get_storage_gateway.py
+src/globus_sdk/_testing/data/globus_connect_server/get_storage_gateway_list.py
+src/globus_sdk/_testing/data/globus_connect_server/update_storage_gateway.py
 src/globus_sdk/_testing/data/groups/__init__.py
 src/globus_sdk/_testing/data/groups/_common.py
 src/globus_sdk/_testing/data/groups/delete_group.py
 src/globus_sdk/_testing/data/groups/get_group.py
 src/globus_sdk/_testing/data/groups/get_my_groups.py
 src/globus_sdk/_testing/data/search/__init__.py
 src/globus_sdk/_testing/data/search/create_role.py
@@ -85,17 +92,21 @@
 src/globus_sdk/services/auth/flow_managers/base.py
 src/globus_sdk/services/auth/flow_managers/native_app.py
 src/globus_sdk/services/auth/response/__init__.py
 src/globus_sdk/services/auth/response/identities.py
 src/globus_sdk/services/auth/response/oauth.py
 src/globus_sdk/services/gcs/__init__.py
 src/globus_sdk/services/gcs/client.py
-src/globus_sdk/services/gcs/data.py
 src/globus_sdk/services/gcs/errors.py
 src/globus_sdk/services/gcs/response.py
+src/globus_sdk/services/gcs/data/__init__.py
+src/globus_sdk/services/gcs/data/_common.py
+src/globus_sdk/services/gcs/data/collection.py
+src/globus_sdk/services/gcs/data/role.py
+src/globus_sdk/services/gcs/data/storage_gateway.py
 src/globus_sdk/services/groups/__init__.py
 src/globus_sdk/services/groups/client.py
 src/globus_sdk/services/groups/data.py
 src/globus_sdk/services/groups/errors.py
 src/globus_sdk/services/groups/manager.py
 src/globus_sdk/services/search/__init__.py
 src/globus_sdk/services/search/client.py
```

### Comparing `globus-sdk-3.8.0/tox.ini` & `globus-sdk-3.9.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,25 @@
 commands = pre-commit run --all-files
 
 [testenv:mypy{,-mindeps}]
 deps = mindeps: typing_extensions==4.0
 commands = mypy src/ {posargs}
 
 [testenv:mypy-test]
-deps = mypy
+deps = mypy==0.960
 commands = mypy --show-error-codes --warn-unused-ignores tests/non-pytest/mypy-ignore-tests/
 
+[testenv:test-lazy-imports]
+# these tests are slow and CPU-bound, so they are run with xdist `-n auto` for speed
+# reassess if we start using xdist for the main testsuite
+deps = pytest-xdist<3
+commands =
+    pytest -n auto tests/non-pytest/lazy-imports/test_for_import_cycles.py
+    pytest tests/unit/test_lazy_imports.py
+
 [testenv:pylint]
 deps = pylint
 commands = pylint src/
 
 [testenv:pyright]
 deps = pyright
 commands = pyright src/ {posargs}
```

