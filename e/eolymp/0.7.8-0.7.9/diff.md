# Comparing `tmp/eolymp-0.7.8.tar.gz` & `tmp/eolymp-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eolymp-0.7.8.tar", last modified: Sun Nov  6 15:45:49 2022, max compression
+gzip compressed data, was "eolymp-0.7.9.tar", last modified: Mon Nov  7 23:52:28 2022, max compression
```

## Comparing `eolymp-0.7.8.tar` & `eolymp-0.7.9.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.869610 eolymp-0.7.8/
--rw-r--r--   0 root         (0) root         (0)      911 2022-11-06 15:45:49.869610 eolymp-0.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2022-11-06 15:45:49.000000 eolymp-0.7.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.829610 eolymp-0.7.8/eolymp/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.829610 eolymp-0.7.8/eolymp/annotations/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2308 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/http_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2402 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/http_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1536 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/ratelimit_pb2.py
--rw-r--r--   0 root         (0) root         (0)      623 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/ratelimit_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1571 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/resource_pb2.py
--rw-r--r--   0 root         (0) root         (0)      720 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/resource_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1462 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/scope_pb2.py
--rw-r--r--   0 root         (0) root         (0)      654 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/scope_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1505 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      607 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/annotations/service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.829610 eolymp-0.7.8/eolymp/apollo/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/apollo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1364 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/apollo/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      820 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/apollo/events_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.837610 eolymp-0.7.8/eolymp/atlas/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36847 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/atlas_http.py
--rw-r--r--   0 root         (0) root         (0)    64866 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/atlas_pb2.py
--rw-r--r--   0 root         (0) root         (0)    42762 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/atlas_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1574 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/attachment_pb2.py
--rw-r--r--   0 root         (0) root         (0)      725 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/attachment_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1590 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/category_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1523 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/category_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     9704 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/change_pb2.py
--rw-r--r--   0 root         (0) root         (0)    12624 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/change_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2641 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2231 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1226 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/feedback_pb2.py
--rw-r--r--   0 root         (0) root         (0)      381 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/feedback_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1143 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/file_pb2.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/file_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1435 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/permission_pb2.py
--rw-r--r--   0 root         (0) root         (0)      898 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/permission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1600 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)      796 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1427 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/score_pb2.py
--rw-r--r--   0 root         (0) root         (0)      953 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1251 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/scoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)      396 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/scoring_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2283 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/solution_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1932 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/solution_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2241 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/statement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1858 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/statement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5199 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7540 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1962 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1714 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1663 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/test_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1090 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/test_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2102 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/testset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1756 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/atlas/testset_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.841610 eolymp-0.7.8/eolymp/cognito/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/access_key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      997 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/access_key_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    10180 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/cognito_http.py
--rw-r--r--   0 root         (0) root         (0)    25450 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/cognito_pb2.py
--rw-r--r--   0 root         (0) root         (0)    19947 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/cognito_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1321 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/entitlement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      451 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/entitlement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1170 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/quota_pb2.py
--rw-r--r--   0 root         (0) root         (0)      482 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/quota_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2264 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2827 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/cognito/user_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.841610 eolymp-0.7.8/eolymp/community/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2705 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2886 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/attribute_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     7060 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/community_http.py
--rw-r--r--   0 root         (0) root         (0)    15341 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/community_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9842 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/community_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1696 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1025 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3271 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/member_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4362 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/community/member_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.841610 eolymp-0.7.8/eolymp/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1489 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/core/http_client.py
--rw-r--r--   0 root         (0) root         (0)     2288 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/core/oauth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.845610 eolymp-0.7.8/eolymp/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1617 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      834 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2978 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/executor_http.py
--rw-r--r--   0 root         (0) root         (0)     8042 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/executor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5724 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/executor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1667 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/interactor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1452 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/interactor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5869 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10559 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/job_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1225 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/language_pb2.py
--rw-r--r--   0 root         (0) root         (0)      565 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/language_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5195 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/report_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7674 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/report_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1290 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/runtime_pb2.py
--rw-r--r--   0 root         (0) root         (0)      752 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/runtime_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2965 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4284 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/status_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3478 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/task_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5824 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/task_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1565 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/usage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1635 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/usage_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1912 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/verifier_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1906 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/executor/verifier_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.845610 eolymp-0.7.8/eolymp/geography/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/country_pb2.py
--rw-r--r--   0 root         (0) root         (0)      549 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/country_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2570 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/geography_http.py
--rw-r--r--   0 root         (0) root         (0)     4943 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/geography_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2558 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/geography_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1252 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/region_pb2.py
--rw-r--r--   0 root         (0) root         (0)      660 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/geography/region_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.849610 eolymp-0.7.8/eolymp/helpdesk/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1489 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/document_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1129 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/document_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1736 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1082 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4451 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/helpdesk_http.py
--rw-r--r--   0 root         (0) root         (0)    10118 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/helpdesk_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7153 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/helpdesk/helpdesk_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.853610 eolymp-0.7.8/eolymp/judge/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2724 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2702 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1844 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/announcement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1105 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/announcement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3801 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/contest_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4548 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/contest_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1777 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/entitlement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      816 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/entitlement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3285 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3207 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    41445 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/judge_http.py
--rw-r--r--   0 root         (0) root         (0)    75528 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/judge_pb2.py
--rw-r--r--   0 root         (0) root         (0)    53016 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/judge_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2865 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/participant_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3253 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/participant_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3389 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4212 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1837 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/reply_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1202 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/reply_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1491 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/result_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1178 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/result_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2362 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/score_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3063 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5019 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6972 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1851 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1426 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2091 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/ticket_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1902 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/judge/ticket_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.857610 eolymp-0.7.8/eolymp/keeper/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/keeper/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1544 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/keeper/blob_pb2.py
--rw-r--r--   0 root         (0) root         (0)      787 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/keeper/blob_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1928 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/keeper/keeper_http.py
--rw-r--r--   0 root         (0) root         (0)     4188 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/keeper/keeper_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1978 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/keeper/keeper_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.857610 eolymp-0.7.8/eolymp/oauth2/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/oauth2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2837 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/oauth2/oauth2_http.py
--rw-r--r--   0 root         (0) root         (0)     7399 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/oauth2/oauth2_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7255 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/oauth2/oauth2_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.857610 eolymp-0.7.8/eolymp/playground/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/playground/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1434 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/playground/playground_http.py
--rw-r--r--   0 root         (0) root         (0)     3659 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/playground/playground_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2131 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/playground/playground_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2337 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/playground/run_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2763 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/playground/run_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.861610 eolymp-0.7.8/eolymp/ranker/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2245 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2299 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1258 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      652 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1165 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/format_pb2.py
--rw-r--r--   0 root         (0) root         (0)      335 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/format_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8378 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/ranker_http.py
--rw-r--r--   0 root         (0) root         (0)    17239 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/ranker_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11000 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/ranker_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3343 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/scoreboard_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5626 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/ranker/scoreboard_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.861610 eolymp-0.7.8/eolymp/resolver/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1003 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/resolver/resolver_http.py
--rw-r--r--   0 root         (0) root         (0)     3800 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/resolver/resolver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3246 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/resolver/resolver_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.861610 eolymp-0.7.8/eolymp/typewriter/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6584 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/block_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9637 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/block_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2640 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/inline_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2997 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/inline_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      896 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/typewriter_http.py
--rw-r--r--   0 root         (0) root         (0)     2363 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/typewriter_pb2.py
--rw-r--r--   0 root         (0) root         (0)      854 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/typewriter/typewriter_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.865610 eolymp-0.7.8/eolymp/universe/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1505 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/idp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1215 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/idp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1446 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/permission_pb2.py
--rw-r--r--   0 root         (0) root         (0)      867 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/permission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3033 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/space_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3792 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/space_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8063 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/universe_http.py
--rw-r--r--   0 root         (0) root         (0)    15591 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/universe_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10057 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/universe/universe_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.865610 eolymp-0.7.8/eolymp/wellknown/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/wellknown/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/wellknown/direction_pb2.py
--rw-r--r--   0 root         (0) root         (0)      331 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/wellknown/direction_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2426 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/wellknown/errors_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2458 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/wellknown/errors_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4481 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/wellknown/expression_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3915 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/wellknown/expression_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.869610 eolymp-0.7.8/eolymp/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1714 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1054 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1579 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/file_pb2.py
--rw-r--r--   0 root         (0) root         (0)      627 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/file_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2415 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/project_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/project_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5307 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/workspace_http.py
--rw-r--r--   0 root         (0) root         (0)    10575 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/workspace_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6521 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp/workspace/workspace_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-06 15:45:49.829610 eolymp-0.7.8/eolymp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      911 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6619 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-11-06 15:45:49.000000 eolymp-0.7.8/eolymp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-06 15:45:49.869610 eolymp-0.7.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      974 2022-11-06 15:45:49.000000 eolymp-0.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.234156 eolymp-0.7.9/
+-rw-r--r--   0 root         (0) root         (0)      911 2022-11-07 23:52:28.234156 eolymp-0.7.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2022-11-07 23:52:27.000000 eolymp-0.7.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.206155 eolymp-0.7.9/eolymp/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.210156 eolymp-0.7.9/eolymp/annotations/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/annotations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/http_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/http_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1536 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/ratelimit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      623 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/ratelimit_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1571 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/resource_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      720 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/resource_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1462 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/scope_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      654 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/scope_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1505 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      607 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/annotations/service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.210156 eolymp-0.7.9/eolymp/apollo/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/apollo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/apollo/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      820 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/apollo/events_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.214156 eolymp-0.7.9/eolymp/atlas/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/atlas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36847 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/atlas_http.py
+-rw-r--r--   0 root         (0) root         (0)    64866 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/atlas_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    42762 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/atlas_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/attachment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      725 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/attachment_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1590 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/category_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/category_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     9704 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/change_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    12624 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/change_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2641 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1226 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/feedback_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      381 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/feedback_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1143 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/file_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/file_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1435 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/permission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      898 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/permission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1600 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      796 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1427 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      953 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1251 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/scoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      396 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/scoring_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2283 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/solution_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/solution_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2241 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/statement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/statement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5199 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7540 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1962 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1663 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/test_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/test_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2102 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/testset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/atlas/testset_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.214156 eolymp-0.7.9/eolymp/cognito/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/cognito/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/access_key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      997 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/access_key_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    10180 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/cognito_http.py
+-rw-r--r--   0 root         (0) root         (0)    25450 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/cognito_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    19947 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/cognito_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1321 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/entitlement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      451 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/entitlement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1170 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/quota_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      482 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/quota_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2264 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/cognito/user_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.218156 eolymp-0.7.9/eolymp/community/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/attribute_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     7939 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/community_http.py
+-rw-r--r--   0 root         (0) root         (0)    17368 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/community_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10655 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/community_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1696 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1591 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/idp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/idp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3271 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/member_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/community/member_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.218156 eolymp-0.7.9/eolymp/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/core/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/core/oauth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.218156 eolymp-0.7.9/eolymp/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      834 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2978 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/executor_http.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/executor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/executor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1667 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/interactor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/interactor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5869 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/job_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1225 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/language_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      565 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/language_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5195 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/report_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7674 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/report_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1290 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/runtime_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      752 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/runtime_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2965 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4284 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/status_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3478 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/task_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5824 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/task_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1565 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/usage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/usage_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1912 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/verifier_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/executor/verifier_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.222156 eolymp-0.7.9/eolymp/geography/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/geography/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/geography/country_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      549 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/geography/country_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2570 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/geography/geography_http.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/geography/geography_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/geography/geography_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1252 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/geography/region_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      660 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/geography/region_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.222156 eolymp-0.7.9/eolymp/helpdesk/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/helpdesk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/helpdesk/document_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/helpdesk/document_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1736 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/helpdesk/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/helpdesk/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4451 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/helpdesk/helpdesk_http.py
+-rw-r--r--   0 root         (0) root         (0)    10118 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/helpdesk/helpdesk_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7153 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/helpdesk/helpdesk_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.226156 eolymp-0.7.9/eolymp/judge/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1844 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/announcement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/announcement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3801 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/contest_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/contest_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1777 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/entitlement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      816 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/entitlement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3285 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    41445 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/judge_http.py
+-rw-r--r--   0 root         (0) root         (0)    75528 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/judge_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    53016 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/judge_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2865 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/participant_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/participant_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3389 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4212 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1837 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/reply_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/reply_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1491 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/result_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/result_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2362 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5019 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6972 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2091 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/ticket_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/judge/ticket_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.226156 eolymp-0.7.9/eolymp/keeper/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/keeper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/keeper/blob_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      787 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/keeper/blob_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1928 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/keeper/keeper_http.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/keeper/keeper_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/keeper/keeper_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.226156 eolymp-0.7.9/eolymp/oauth2/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/oauth2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/oauth2/oauth2_http.py
+-rw-r--r--   0 root         (0) root         (0)     7399 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/oauth2/oauth2_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7255 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/oauth2/oauth2_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.226156 eolymp-0.7.9/eolymp/playground/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/playground/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/playground/playground_http.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/playground/playground_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2131 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/playground/playground_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2337 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/playground/run_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/playground/run_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.230156 eolymp-0.7.9/eolymp/ranker/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/ranker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1258 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      652 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/format_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      335 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/format_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8378 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/ranker_http.py
+-rw-r--r--   0 root         (0) root         (0)    17239 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/ranker_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11000 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/ranker_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3343 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/scoreboard_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5626 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/ranker/scoreboard_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.230156 eolymp-0.7.9/eolymp/resolver/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/resolver/resolver_http.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/resolver/resolver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/resolver/resolver_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.230156 eolymp-0.7.9/eolymp/typewriter/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/typewriter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6584 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/typewriter/block_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9637 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/typewriter/block_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2640 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/typewriter/inline_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/typewriter/inline_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      896 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/typewriter/typewriter_http.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/typewriter/typewriter_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      854 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/typewriter/typewriter_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.230156 eolymp-0.7.9/eolymp/universe/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/universe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/universe/permission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      867 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/universe/permission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3033 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/universe/space_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3792 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/universe/space_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6920 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/universe/universe_http.py
+-rw-r--r--   0 root         (0) root         (0)    13454 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/universe/universe_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9039 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/universe/universe_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.234156 eolymp-0.7.9/eolymp/wellknown/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/wellknown/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/wellknown/direction_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      331 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/wellknown/direction_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2426 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/wellknown/errors_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/wellknown/errors_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4481 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/wellknown/expression_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/wellknown/expression_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.234156 eolymp-0.7.9/eolymp/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1579 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/file_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      627 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/file_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2415 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/project_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/project_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5307 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/workspace_http.py
+-rw-r--r--   0 root         (0) root         (0)    10575 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/workspace_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6521 2022-11-07 23:52:27.000000 eolymp-0.7.9/eolymp/workspace/workspace_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 23:52:28.206155 eolymp-0.7.9/eolymp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      911 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6621 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-11-07 23:52:28.000000 eolymp-0.7.9/eolymp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-07 23:52:28.234156 eolymp-0.7.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      974 2022-11-07 23:52:27.000000 eolymp-0.7.9/setup.py
```

### Comparing `eolymp-0.7.8/PKG-INFO` & `eolymp-0.7.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.7.8
+Version: 0.7.9
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.7.8/README.md` & `eolymp-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/http_pb2.py` & `eolymp-0.7.9/eolymp/annotations/http_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/http_pb2.pyi` & `eolymp-0.7.9/eolymp/annotations/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/ratelimit_pb2.py` & `eolymp-0.7.9/eolymp/annotations/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/ratelimit_pb2.pyi` & `eolymp-0.7.9/eolymp/annotations/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/resource_pb2.py` & `eolymp-0.7.9/eolymp/annotations/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/resource_pb2.pyi` & `eolymp-0.7.9/eolymp/annotations/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/scope_pb2.py` & `eolymp-0.7.9/eolymp/annotations/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/scope_pb2.pyi` & `eolymp-0.7.9/eolymp/annotations/scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/service_pb2.py` & `eolymp-0.7.9/eolymp/annotations/service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/annotations/service_pb2.pyi` & `eolymp-0.7.9/eolymp/annotations/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/apollo/events_pb2.py` & `eolymp-0.7.9/eolymp/apollo/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/apollo/events_pb2.pyi` & `eolymp-0.7.9/eolymp/apollo/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/atlas_http.py` & `eolymp-0.7.9/eolymp/atlas/atlas_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/atlas_pb2.py` & `eolymp-0.7.9/eolymp/atlas/atlas_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/atlas_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/atlas_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/attachment_pb2.py` & `eolymp-0.7.9/eolymp/atlas/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/attachment_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/category_pb2.py` & `eolymp-0.7.9/eolymp/atlas/category_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/category_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/change_pb2.py` & `eolymp-0.7.9/eolymp/atlas/change_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/change_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/change_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/events_pb2.py` & `eolymp-0.7.9/eolymp/atlas/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/events_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/feedback_pb2.py` & `eolymp-0.7.9/eolymp/atlas/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/file_pb2.py` & `eolymp-0.7.9/eolymp/atlas/file_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/permission_pb2.py` & `eolymp-0.7.9/eolymp/atlas/permission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/permission_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/permission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/problem_pb2.py` & `eolymp-0.7.9/eolymp/atlas/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/problem_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/problem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/score_pb2.py` & `eolymp-0.7.9/eolymp/atlas/score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/score_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/scoring_pb2.py` & `eolymp-0.7.9/eolymp/atlas/scoring_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/solution_pb2.py` & `eolymp-0.7.9/eolymp/atlas/solution_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/solution_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/solution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/statement_pb2.py` & `eolymp-0.7.9/eolymp/atlas/statement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/statement_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/statement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/submission_pb2.py` & `eolymp-0.7.9/eolymp/atlas/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/submission_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/template_pb2.py` & `eolymp-0.7.9/eolymp/atlas/template_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/template_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/test_pb2.py` & `eolymp-0.7.9/eolymp/atlas/test_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/test_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/testset_pb2.py` & `eolymp-0.7.9/eolymp/atlas/testset_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/atlas/testset_pb2.pyi` & `eolymp-0.7.9/eolymp/atlas/testset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/access_key_pb2.py` & `eolymp-0.7.9/eolymp/cognito/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/access_key_pb2.pyi` & `eolymp-0.7.9/eolymp/cognito/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/cognito_http.py` & `eolymp-0.7.9/eolymp/cognito/cognito_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/cognito_pb2.py` & `eolymp-0.7.9/eolymp/cognito/cognito_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/cognito_pb2.pyi` & `eolymp-0.7.9/eolymp/cognito/cognito_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/entitlement_pb2.py` & `eolymp-0.7.9/eolymp/cognito/entitlement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/quota_pb2.py` & `eolymp-0.7.9/eolymp/cognito/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/user_pb2.py` & `eolymp-0.7.9/eolymp/cognito/user_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/cognito/user_pb2.pyi` & `eolymp-0.7.9/eolymp/cognito/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/community/attribute_pb2.py` & `eolymp-0.7.9/eolymp/community/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/community/attribute_pb2.pyi` & `eolymp-0.7.9/eolymp/community/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/community/community_http.py` & `eolymp-0.7.9/eolymp/community/community_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,7 +210,33 @@
             url=self.url+path,
             path=path,
             request_data=request,
             response_symbol=_sym_db.GetSymbol("eolymp.community.ListAttributesOutput"),
             **kwargs,
         )
 
+    def DescribeIdentityProvider(self, request, **kwargs):
+        path = "/idp"
+
+        return self.transport.request(
+            name="eolymp.community.Community/DescribeIdentityProvider",
+            method="GET",
+            url=self.url+path,
+            path=path,
+            request_data=request,
+            response_symbol=_sym_db.GetSymbol("eolymp.community.DescribeIdentityProviderOutput"),
+            **kwargs,
+        )
+
+    def ConfigureIdentityProvider(self, request, **kwargs):
+        path = "/idp"
+
+        return self.transport.request(
+            name="eolymp.community.Community/ConfigureIdentityProvider",
+            method="PUT",
+            url=self.url+path,
+            path=path,
+            request_data=request,
+            response_symbol=_sym_db.GetSymbol("eolymp.community.ConfigureIdentityProviderOutput"),
+            **kwargs,
+        )
+
```

### Comparing `eolymp-0.7.8/eolymp/community/community_pb2.py` & `eolymp-0.7.9/eolymp/community/community_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.community import attribute_pb2 as eolymp_dot_community_dot_attribute__pb2
+from eolymp.community import idp_pb2 as eolymp_dot_community_dot_idp__pb2
 from eolymp.community import member_pb2 as eolymp_dot_community_dot_member__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/community/community.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a\x1d\x65olymp/community/member.proto\x1a!eolymp/wellknown/expression.proto\"N\n\x0eJoinSpaceInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x06values\x18\x14 \x03(\x0b\x32\x1e.eolymp.community.Member.Value\"2\n\x0fJoinSpaceOutput\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\x12\x11\n\tmember_id\x18\x01 \x01(\t\"E\n\x13RegisterMemberInput\x12.\n\x06values\x18\x01 \x03(\x0b\x32\x1e.eolymp.community.Member.Value\"\x16\n\x14RegisterMemberOutput\"\x11\n\x0fLeaveSpaceInput\"\x12\n\x10LeaveSpaceOutput\":\n\x0e\x41\x64\x64MemberInput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"2\n\x0f\x41\x64\x64MemberOutput\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\x12\x11\n\tmember_id\x18\x01 \x01(\t\"P\n\x11UpdateMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\x12(\n\x06member\x18\x02 \x01(\x0b\x32\x18.eolymp.community.Member\"\x14\n\x12UpdateMemberOutput\"&\n\x11RemoveMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"\x14\n\x12RemoveMemberOutput\"(\n\x13\x44\x65scribeMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"@\n\x14\x44\x65scribeMemberOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\x17\n\x15IntrospectMemberInput\"B\n\x16IntrospectMemberOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\xba\x02\n\x10ListMembersInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12:\n\x07\x66ilters\x18( \x01(\x0b\x32).eolymp.community.ListMembersInput.Filter\x1a\xcb\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12/\n\x07user_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x32\n\x08\x64isabled\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x30\n\x04name\x18\x04 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\"K\n\x11ListMembersOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\'\n\x05items\x18\x02 \x03(\x0b\x32\x18.eolymp.community.Member\"Z\n\x11\x41\x64\x64\x41ttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\"\n\x12\x41\x64\x64\x41ttributeOutput\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\"]\n\x14UpdateAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\x17\n\x15UpdateAttributeOutput\"-\n\x14RemoveAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"\x17\n\x15RemoveAttributeOutput\"/\n\x16\x44\x65scribeAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"I\n\x17\x44\x65scribeAttributeOutput\x12.\n\tattribute\x18\x01 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\xee\x02\n\x13ListAttributesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.community.ListAttributesInput.Filter\x1a\xf9\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12-\n\x03key\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x06hidden\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x32\n\x08required\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12.\n\x04type\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"Q\n\x14ListAttributesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.community.Attribute2\x8b\x12\n\tCommunity\x12\x94\x01\n\tJoinSpace\x12 .eolymp.community.JoinSpaceInput\x1a!.eolymp.community.JoinSpaceOutput\"B\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:join\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x10\"\x0e/members/_self\x12\x97\x01\n\nLeaveSpace\x12!.eolymp.community.LeaveSpaceInput\x1a\".eolymp.community.LeaveSpaceOutput\"B\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:join\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x10*\x0e/members/_self\x12\xaf\x01\n\x0eRegisterMember\x12%.eolymp.community.RegisterMemberInput\x1a&.eolymp.community.RegisterMemberOutput\"N\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1b\"\x19/members/_self/attributes\x12\x8c\x01\n\x10IntrospectMember\x12\'.eolymp.community.IntrospectMemberInput\x1a(.eolymp.community.IntrospectMemberOutput\"%\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x10\x12\x0e/members/_self\x12\x8f\x01\n\tAddMember\x12 .eolymp.community.AddMemberInput\x1a!.eolymp.community.AddMemberOutput\"=\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\"\x08/members\x12\xa4\x01\n\x0cUpdateMember\x12#.eolymp.community.UpdateMemberInput\x1a$.eolymp.community.UpdateMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\"\x14/members/{member_id}\x12\xa4\x01\n\x0cRemoveMember\x12#.eolymp.community.RemoveMemberInput\x1a$.eolymp.community.RemoveMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16*\x14/members/{member_id}\x12\xa9\x01\n\x0e\x44\x65scribeMember\x12%.eolymp.community.DescribeMemberInput\x1a&.eolymp.community.DescribeMemberOutput\"H\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\x12\x14/members/{member_id}\x12\x94\x01\n\x0bListMembers\x12\".eolymp.community.ListMembersInput\x1a#.eolymp.community.ListMembersOutput\"<\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\x12\x08/members\x12\x9b\x01\n\x0c\x41\x64\x64\x41ttribute\x12#.eolymp.community.AddAttributeInput\x1a$.eolymp.community.AddAttributeOutput\"@\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\"\x0b/attributes\x12\xb4\x01\n\x0fUpdateAttribute\x12&.eolymp.community.UpdateAttributeInput\x1a\'.eolymp.community.UpdateAttributeOutput\"P\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\"\x1b/attributes/{attribute_key}\x12\xb4\x01\n\x0fRemoveAttribute\x12&.eolymp.community.RemoveAttributeInput\x1a\'.eolymp.community.RemoveAttributeOutput\"P\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d*\x1b/attributes/{attribute_key}\x12\xb9\x01\n\x11\x44\x65scribeAttribute\x12(.eolymp.community.DescribeAttributeInput\x1a).eolymp.community.DescribeAttributeOutput\"O\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\x12\x1b/attributes/{attribute_key}\x12\xa0\x01\n\x0eListAttributes\x12%.eolymp.community.ListAttributesInput\x1a&.eolymp.community.ListAttributesOutput\"?\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\x12\x0b/attributesB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/community/community.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a\x1a\x65olymp/community/idp.proto\x1a\x1d\x65olymp/community/member.proto\x1a!eolymp/wellknown/expression.proto\"N\n\x0eJoinSpaceInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x06values\x18\x14 \x03(\x0b\x32\x1e.eolymp.community.Member.Value\"2\n\x0fJoinSpaceOutput\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\x12\x11\n\tmember_id\x18\x01 \x01(\t\"E\n\x13RegisterMemberInput\x12.\n\x06values\x18\x01 \x03(\x0b\x32\x1e.eolymp.community.Member.Value\"\x16\n\x14RegisterMemberOutput\"\x11\n\x0fLeaveSpaceInput\"\x12\n\x10LeaveSpaceOutput\":\n\x0e\x41\x64\x64MemberInput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"2\n\x0f\x41\x64\x64MemberOutput\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\x12\x11\n\tmember_id\x18\x01 \x01(\t\"P\n\x11UpdateMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\x12(\n\x06member\x18\x02 \x01(\x0b\x32\x18.eolymp.community.Member\"\x14\n\x12UpdateMemberOutput\"&\n\x11RemoveMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"\x14\n\x12RemoveMemberOutput\"(\n\x13\x44\x65scribeMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"@\n\x14\x44\x65scribeMemberOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\x17\n\x15IntrospectMemberInput\"B\n\x16IntrospectMemberOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\xba\x02\n\x10ListMembersInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12:\n\x07\x66ilters\x18( \x01(\x0b\x32).eolymp.community.ListMembersInput.Filter\x1a\xcb\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12/\n\x07user_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x32\n\x08\x64isabled\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x30\n\x04name\x18\x04 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\"K\n\x11ListMembersOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\'\n\x05items\x18\x02 \x03(\x0b\x32\x18.eolymp.community.Member\"Z\n\x11\x41\x64\x64\x41ttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\"\n\x12\x41\x64\x64\x41ttributeOutput\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\"]\n\x14UpdateAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\x17\n\x15UpdateAttributeOutput\"-\n\x14RemoveAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"\x17\n\x15RemoveAttributeOutput\"/\n\x16\x44\x65scribeAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"I\n\x17\x44\x65scribeAttributeOutput\x12.\n\tattribute\x18\x01 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\xee\x02\n\x13ListAttributesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.community.ListAttributesInput.Filter\x1a\xf9\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12-\n\x03key\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x06hidden\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x32\n\x08required\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12.\n\x04type\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"Q\n\x14ListAttributesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.community.Attribute\"\x1f\n\x1d\x44\x65scribeIdentityProviderInput\"e\n\x1e\x44\x65scribeIdentityProviderOutput\x12\x37\n\x04oidc\x18\x03 \x01(\x0b\x32\'.eolymp.community.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"e\n\x1e\x43onfigureIdentityProviderInput\x12\x37\n\x04oidc\x18\x0c \x01(\x0b\x32\'.eolymp.community.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"!\n\x1f\x43onfigureIdentityProviderOutput2\xe6\x14\n\tCommunity\x12\x94\x01\n\tJoinSpace\x12 .eolymp.community.JoinSpaceInput\x1a!.eolymp.community.JoinSpaceOutput\"B\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:join\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x10\"\x0e/members/_self\x12\x97\x01\n\nLeaveSpace\x12!.eolymp.community.LeaveSpaceInput\x1a\".eolymp.community.LeaveSpaceOutput\"B\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:join\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x10*\x0e/members/_self\x12\xaf\x01\n\x0eRegisterMember\x12%.eolymp.community.RegisterMemberInput\x1a&.eolymp.community.RegisterMemberOutput\"N\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1b\"\x19/members/_self/attributes\x12\x8c\x01\n\x10IntrospectMember\x12\'.eolymp.community.IntrospectMemberInput\x1a(.eolymp.community.IntrospectMemberOutput\"%\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x10\x12\x0e/members/_self\x12\x8f\x01\n\tAddMember\x12 .eolymp.community.AddMemberInput\x1a!.eolymp.community.AddMemberOutput\"=\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\"\x08/members\x12\xa4\x01\n\x0cUpdateMember\x12#.eolymp.community.UpdateMemberInput\x1a$.eolymp.community.UpdateMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\"\x14/members/{member_id}\x12\xa4\x01\n\x0cRemoveMember\x12#.eolymp.community.RemoveMemberInput\x1a$.eolymp.community.RemoveMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16*\x14/members/{member_id}\x12\xa9\x01\n\x0e\x44\x65scribeMember\x12%.eolymp.community.DescribeMemberInput\x1a&.eolymp.community.DescribeMemberOutput\"H\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\x12\x14/members/{member_id}\x12\x94\x01\n\x0bListMembers\x12\".eolymp.community.ListMembersInput\x1a#.eolymp.community.ListMembersOutput\"<\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\x12\x08/members\x12\x9b\x01\n\x0c\x41\x64\x64\x41ttribute\x12#.eolymp.community.AddAttributeInput\x1a$.eolymp.community.AddAttributeOutput\"@\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\"\x0b/attributes\x12\xb4\x01\n\x0fUpdateAttribute\x12&.eolymp.community.UpdateAttributeInput\x1a\'.eolymp.community.UpdateAttributeOutput\"P\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\"\x1b/attributes/{attribute_key}\x12\xb4\x01\n\x0fRemoveAttribute\x12&.eolymp.community.RemoveAttributeInput\x1a\'.eolymp.community.RemoveAttributeOutput\"P\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d*\x1b/attributes/{attribute_key}\x12\xb9\x01\n\x11\x44\x65scribeAttribute\x12(.eolymp.community.DescribeAttributeInput\x1a).eolymp.community.DescribeAttributeOutput\"O\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\x12\x1b/attributes/{attribute_key}\x12\xa0\x01\n\x0eListAttributes\x12%.eolymp.community.ListAttributesInput\x1a&.eolymp.community.ListAttributesOutput\"?\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\x12\x0b/attributes\x12\x9a\x01\n\x18\x44\x65scribeIdentityProvider\x12/.eolymp.community.DescribeIdentityProviderInput\x1a\x30.eolymp.community.DescribeIdentityProviderOutput\"\x1b\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x06\x12\x04/idp\x12\xbb\x01\n\x19\x43onfigureIdentityProvider\x12\x30.eolymp.community.ConfigureIdentityProviderInput\x1a\x31.eolymp.community.ConfigureIdentityProviderOutput\"9\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x06\x1a\x04/idpB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.community_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
@@ -51,70 +52,82 @@
   _COMMUNITY.methods_by_name['UpdateAttribute']._serialized_options = b'\202\343\n\032\212\343\n\026community:member:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\035\"\033/attributes/{attribute_key}'
   _COMMUNITY.methods_by_name['RemoveAttribute']._options = None
   _COMMUNITY.methods_by_name['RemoveAttribute']._serialized_options = b'\202\343\n\032\212\343\n\026community:member:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\035*\033/attributes/{attribute_key}'
   _COMMUNITY.methods_by_name['DescribeAttribute']._options = None
   _COMMUNITY.methods_by_name['DescribeAttribute']._serialized_options = b'\202\343\n\031\212\343\n\025community:member:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\035\022\033/attributes/{attribute_key}'
   _COMMUNITY.methods_by_name['ListAttributes']._options = None
   _COMMUNITY.methods_by_name['ListAttributes']._serialized_options = b'\202\343\n\031\212\343\n\025community:member:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\r\022\013/attributes'
-  _JOINSPACEINPUT._serialized_start=253
-  _JOINSPACEINPUT._serialized_end=331
-  _JOINSPACEOUTPUT._serialized_start=333
-  _JOINSPACEOUTPUT._serialized_end=383
-  _REGISTERMEMBERINPUT._serialized_start=385
-  _REGISTERMEMBERINPUT._serialized_end=454
-  _REGISTERMEMBEROUTPUT._serialized_start=456
-  _REGISTERMEMBEROUTPUT._serialized_end=478
-  _LEAVESPACEINPUT._serialized_start=480
-  _LEAVESPACEINPUT._serialized_end=497
-  _LEAVESPACEOUTPUT._serialized_start=499
-  _LEAVESPACEOUTPUT._serialized_end=517
-  _ADDMEMBERINPUT._serialized_start=519
-  _ADDMEMBERINPUT._serialized_end=577
-  _ADDMEMBEROUTPUT._serialized_start=579
-  _ADDMEMBEROUTPUT._serialized_end=629
-  _UPDATEMEMBERINPUT._serialized_start=631
-  _UPDATEMEMBERINPUT._serialized_end=711
-  _UPDATEMEMBEROUTPUT._serialized_start=713
-  _UPDATEMEMBEROUTPUT._serialized_end=733
-  _REMOVEMEMBERINPUT._serialized_start=735
-  _REMOVEMEMBERINPUT._serialized_end=773
-  _REMOVEMEMBEROUTPUT._serialized_start=775
-  _REMOVEMEMBEROUTPUT._serialized_end=795
-  _DESCRIBEMEMBERINPUT._serialized_start=797
-  _DESCRIBEMEMBERINPUT._serialized_end=837
-  _DESCRIBEMEMBEROUTPUT._serialized_start=839
-  _DESCRIBEMEMBEROUTPUT._serialized_end=903
-  _INTROSPECTMEMBERINPUT._serialized_start=905
-  _INTROSPECTMEMBERINPUT._serialized_end=928
-  _INTROSPECTMEMBEROUTPUT._serialized_start=930
-  _INTROSPECTMEMBEROUTPUT._serialized_end=996
-  _LISTMEMBERSINPUT._serialized_start=999
-  _LISTMEMBERSINPUT._serialized_end=1313
-  _LISTMEMBERSINPUT_FILTER._serialized_start=1110
-  _LISTMEMBERSINPUT_FILTER._serialized_end=1313
-  _LISTMEMBERSOUTPUT._serialized_start=1315
-  _LISTMEMBERSOUTPUT._serialized_end=1390
-  _ADDATTRIBUTEINPUT._serialized_start=1392
-  _ADDATTRIBUTEINPUT._serialized_end=1482
-  _ADDATTRIBUTEOUTPUT._serialized_start=1484
-  _ADDATTRIBUTEOUTPUT._serialized_end=1518
-  _UPDATEATTRIBUTEINPUT._serialized_start=1520
-  _UPDATEATTRIBUTEINPUT._serialized_end=1613
-  _UPDATEATTRIBUTEOUTPUT._serialized_start=1615
-  _UPDATEATTRIBUTEOUTPUT._serialized_end=1638
-  _REMOVEATTRIBUTEINPUT._serialized_start=1640
-  _REMOVEATTRIBUTEINPUT._serialized_end=1685
-  _REMOVEATTRIBUTEOUTPUT._serialized_start=1687
-  _REMOVEATTRIBUTEOUTPUT._serialized_end=1710
-  _DESCRIBEATTRIBUTEINPUT._serialized_start=1712
-  _DESCRIBEATTRIBUTEINPUT._serialized_end=1759
-  _DESCRIBEATTRIBUTEOUTPUT._serialized_start=1761
-  _DESCRIBEATTRIBUTEOUTPUT._serialized_end=1834
-  _LISTATTRIBUTESINPUT._serialized_start=1837
-  _LISTATTRIBUTESINPUT._serialized_end=2203
-  _LISTATTRIBUTESINPUT_FILTER._serialized_start=1954
-  _LISTATTRIBUTESINPUT_FILTER._serialized_end=2203
-  _LISTATTRIBUTESOUTPUT._serialized_start=2205
-  _LISTATTRIBUTESOUTPUT._serialized_end=2286
-  _COMMUNITY._serialized_start=2289
-  _COMMUNITY._serialized_end=4604
+  _COMMUNITY.methods_by_name['DescribeIdentityProvider']._options = None
+  _COMMUNITY.methods_by_name['DescribeIdentityProvider']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\nd\202\323\344\223\002\006\022\004/idp'
+  _COMMUNITY.methods_by_name['ConfigureIdentityProvider']._options = None
+  _COMMUNITY.methods_by_name['ConfigureIdentityProvider']._serialized_options = b'\202\343\n\032\212\343\n\026community:member:write\352\342\n\013\365\342\n\000\000\200?\370\342\n\005\202\323\344\223\002\006\032\004/idp'
+  _JOINSPACEINPUT._serialized_start=281
+  _JOINSPACEINPUT._serialized_end=359
+  _JOINSPACEOUTPUT._serialized_start=361
+  _JOINSPACEOUTPUT._serialized_end=411
+  _REGISTERMEMBERINPUT._serialized_start=413
+  _REGISTERMEMBERINPUT._serialized_end=482
+  _REGISTERMEMBEROUTPUT._serialized_start=484
+  _REGISTERMEMBEROUTPUT._serialized_end=506
+  _LEAVESPACEINPUT._serialized_start=508
+  _LEAVESPACEINPUT._serialized_end=525
+  _LEAVESPACEOUTPUT._serialized_start=527
+  _LEAVESPACEOUTPUT._serialized_end=545
+  _ADDMEMBERINPUT._serialized_start=547
+  _ADDMEMBERINPUT._serialized_end=605
+  _ADDMEMBEROUTPUT._serialized_start=607
+  _ADDMEMBEROUTPUT._serialized_end=657
+  _UPDATEMEMBERINPUT._serialized_start=659
+  _UPDATEMEMBERINPUT._serialized_end=739
+  _UPDATEMEMBEROUTPUT._serialized_start=741
+  _UPDATEMEMBEROUTPUT._serialized_end=761
+  _REMOVEMEMBERINPUT._serialized_start=763
+  _REMOVEMEMBERINPUT._serialized_end=801
+  _REMOVEMEMBEROUTPUT._serialized_start=803
+  _REMOVEMEMBEROUTPUT._serialized_end=823
+  _DESCRIBEMEMBERINPUT._serialized_start=825
+  _DESCRIBEMEMBERINPUT._serialized_end=865
+  _DESCRIBEMEMBEROUTPUT._serialized_start=867
+  _DESCRIBEMEMBEROUTPUT._serialized_end=931
+  _INTROSPECTMEMBERINPUT._serialized_start=933
+  _INTROSPECTMEMBERINPUT._serialized_end=956
+  _INTROSPECTMEMBEROUTPUT._serialized_start=958
+  _INTROSPECTMEMBEROUTPUT._serialized_end=1024
+  _LISTMEMBERSINPUT._serialized_start=1027
+  _LISTMEMBERSINPUT._serialized_end=1341
+  _LISTMEMBERSINPUT_FILTER._serialized_start=1138
+  _LISTMEMBERSINPUT_FILTER._serialized_end=1341
+  _LISTMEMBERSOUTPUT._serialized_start=1343
+  _LISTMEMBERSOUTPUT._serialized_end=1418
+  _ADDATTRIBUTEINPUT._serialized_start=1420
+  _ADDATTRIBUTEINPUT._serialized_end=1510
+  _ADDATTRIBUTEOUTPUT._serialized_start=1512
+  _ADDATTRIBUTEOUTPUT._serialized_end=1546
+  _UPDATEATTRIBUTEINPUT._serialized_start=1548
+  _UPDATEATTRIBUTEINPUT._serialized_end=1641
+  _UPDATEATTRIBUTEOUTPUT._serialized_start=1643
+  _UPDATEATTRIBUTEOUTPUT._serialized_end=1666
+  _REMOVEATTRIBUTEINPUT._serialized_start=1668
+  _REMOVEATTRIBUTEINPUT._serialized_end=1713
+  _REMOVEATTRIBUTEOUTPUT._serialized_start=1715
+  _REMOVEATTRIBUTEOUTPUT._serialized_end=1738
+  _DESCRIBEATTRIBUTEINPUT._serialized_start=1740
+  _DESCRIBEATTRIBUTEINPUT._serialized_end=1787
+  _DESCRIBEATTRIBUTEOUTPUT._serialized_start=1789
+  _DESCRIBEATTRIBUTEOUTPUT._serialized_end=1862
+  _LISTATTRIBUTESINPUT._serialized_start=1865
+  _LISTATTRIBUTESINPUT._serialized_end=2231
+  _LISTATTRIBUTESINPUT_FILTER._serialized_start=1982
+  _LISTATTRIBUTESINPUT_FILTER._serialized_end=2231
+  _LISTATTRIBUTESOUTPUT._serialized_start=2233
+  _LISTATTRIBUTESOUTPUT._serialized_end=2314
+  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_start=2316
+  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_end=2347
+  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_start=2349
+  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_end=2450
+  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_start=2452
+  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_end=2553
+  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_start=2555
+  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_end=2588
+  _COMMUNITY._serialized_start=2591
+  _COMMUNITY._serialized_end=5253
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.7.8/eolymp/community/community_pb2.pyi` & `eolymp-0.7.9/eolymp/community/community_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
 from eolymp.community import attribute_pb2 as _attribute_pb2
+from eolymp.community import idp_pb2 as _idp_pb2
 from eolymp.community import member_pb2 as _member_pb2
 from eolymp.wellknown import expression_pb2 as _expression_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
@@ -35,26 +36,46 @@
     __slots__ = ["ern", "member_id"]
     ERN_FIELD_NUMBER: _ClassVar[int]
     MEMBER_ID_FIELD_NUMBER: _ClassVar[int]
     ern: str
     member_id: str
     def __init__(self, ern: _Optional[str] = ..., member_id: _Optional[str] = ...) -> None: ...
 
+class ConfigureIdentityProviderInput(_message.Message):
+    __slots__ = ["oidc"]
+    OIDC_FIELD_NUMBER: _ClassVar[int]
+    oidc: _idp_pb2.IdentityProvider.OIDC
+    def __init__(self, oidc: _Optional[_Union[_idp_pb2.IdentityProvider.OIDC, _Mapping]] = ...) -> None: ...
+
+class ConfigureIdentityProviderOutput(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
 class DescribeAttributeInput(_message.Message):
     __slots__ = ["attribute_key"]
     ATTRIBUTE_KEY_FIELD_NUMBER: _ClassVar[int]
     attribute_key: str
     def __init__(self, attribute_key: _Optional[str] = ...) -> None: ...
 
 class DescribeAttributeOutput(_message.Message):
     __slots__ = ["attribute"]
     ATTRIBUTE_FIELD_NUMBER: _ClassVar[int]
     attribute: _attribute_pb2.Attribute
     def __init__(self, attribute: _Optional[_Union[_attribute_pb2.Attribute, _Mapping]] = ...) -> None: ...
 
+class DescribeIdentityProviderInput(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class DescribeIdentityProviderOutput(_message.Message):
+    __slots__ = ["oidc"]
+    OIDC_FIELD_NUMBER: _ClassVar[int]
+    oidc: _idp_pb2.IdentityProvider.OIDC
+    def __init__(self, oidc: _Optional[_Union[_idp_pb2.IdentityProvider.OIDC, _Mapping]] = ...) -> None: ...
+
 class DescribeMemberInput(_message.Message):
     __slots__ = ["member_id"]
     MEMBER_ID_FIELD_NUMBER: _ClassVar[int]
     member_id: str
     def __init__(self, member_id: _Optional[str] = ...) -> None: ...
 
 class DescribeMemberOutput(_message.Message):
```

### Comparing `eolymp-0.7.8/eolymp/community/events_pb2.py` & `eolymp-0.7.9/eolymp/community/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/community/events_pb2.pyi` & `eolymp-0.7.9/eolymp/community/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/community/member_pb2.py` & `eolymp-0.7.9/eolymp/community/member_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/community/member_pb2.pyi` & `eolymp-0.7.9/eolymp/community/member_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/core/http_client.py` & `eolymp-0.7.9/eolymp/core/http_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/core/oauth_client.py` & `eolymp-0.7.9/eolymp/core/oauth_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/events_pb2.py` & `eolymp-0.7.9/eolymp/executor/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/events_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/executor_http.py` & `eolymp-0.7.9/eolymp/executor/executor_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/executor_pb2.py` & `eolymp-0.7.9/eolymp/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/executor_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/executor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/interactor_pb2.py` & `eolymp-0.7.9/eolymp/executor/interactor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/interactor_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/interactor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/job_pb2.py` & `eolymp-0.7.9/eolymp/executor/job_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/job_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/language_pb2.py` & `eolymp-0.7.9/eolymp/executor/language_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/language_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/language_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/report_pb2.py` & `eolymp-0.7.9/eolymp/executor/report_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/report_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/runtime_pb2.py` & `eolymp-0.7.9/eolymp/executor/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/runtime_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/runtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/status_pb2.py` & `eolymp-0.7.9/eolymp/executor/status_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/status_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/task_pb2.py` & `eolymp-0.7.9/eolymp/executor/task_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/task_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/usage_pb2.py` & `eolymp-0.7.9/eolymp/executor/usage_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/usage_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/verifier_pb2.py` & `eolymp-0.7.9/eolymp/executor/verifier_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/executor/verifier_pb2.pyi` & `eolymp-0.7.9/eolymp/executor/verifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/geography/country_pb2.py` & `eolymp-0.7.9/eolymp/geography/country_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/geography/country_pb2.pyi` & `eolymp-0.7.9/eolymp/geography/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/geography/geography_http.py` & `eolymp-0.7.9/eolymp/geography/geography_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/geography/geography_pb2.py` & `eolymp-0.7.9/eolymp/geography/geography_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/geography/geography_pb2.pyi` & `eolymp-0.7.9/eolymp/geography/geography_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/geography/region_pb2.py` & `eolymp-0.7.9/eolymp/geography/region_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/geography/region_pb2.pyi` & `eolymp-0.7.9/eolymp/geography/region_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/helpdesk/document_pb2.py` & `eolymp-0.7.9/eolymp/helpdesk/document_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/helpdesk/document_pb2.pyi` & `eolymp-0.7.9/eolymp/helpdesk/document_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/helpdesk/events_pb2.py` & `eolymp-0.7.9/eolymp/helpdesk/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/helpdesk/events_pb2.pyi` & `eolymp-0.7.9/eolymp/helpdesk/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/helpdesk/helpdesk_http.py` & `eolymp-0.7.9/eolymp/helpdesk/helpdesk_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/helpdesk/helpdesk_pb2.py` & `eolymp-0.7.9/eolymp/helpdesk/helpdesk_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/helpdesk/helpdesk_pb2.pyi` & `eolymp-0.7.9/eolymp/helpdesk/helpdesk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/activity_pb2.py` & `eolymp-0.7.9/eolymp/judge/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/activity_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/activity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/announcement_pb2.py` & `eolymp-0.7.9/eolymp/judge/announcement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/announcement_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/announcement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/contest_pb2.py` & `eolymp-0.7.9/eolymp/judge/contest_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/contest_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/contest_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/entitlement_pb2.py` & `eolymp-0.7.9/eolymp/judge/entitlement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/entitlement_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/entitlement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/events_pb2.py` & `eolymp-0.7.9/eolymp/judge/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/events_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/judge_http.py` & `eolymp-0.7.9/eolymp/judge/judge_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/judge_pb2.py` & `eolymp-0.7.9/eolymp/judge/judge_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/judge_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/judge_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/participant_pb2.py` & `eolymp-0.7.9/eolymp/judge/participant_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/participant_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/participant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/problem_pb2.py` & `eolymp-0.7.9/eolymp/judge/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/problem_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/problem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/reply_pb2.py` & `eolymp-0.7.9/eolymp/judge/reply_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/reply_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/reply_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/result_pb2.py` & `eolymp-0.7.9/eolymp/judge/result_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/result_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/score_pb2.py` & `eolymp-0.7.9/eolymp/judge/score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/score_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/submission_pb2.py` & `eolymp-0.7.9/eolymp/judge/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/submission_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/template_pb2.py` & `eolymp-0.7.9/eolymp/judge/template_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/template_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/ticket_pb2.py` & `eolymp-0.7.9/eolymp/judge/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/judge/ticket_pb2.pyi` & `eolymp-0.7.9/eolymp/judge/ticket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/keeper/blob_pb2.py` & `eolymp-0.7.9/eolymp/keeper/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/keeper/blob_pb2.pyi` & `eolymp-0.7.9/eolymp/keeper/blob_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/keeper/keeper_http.py` & `eolymp-0.7.9/eolymp/keeper/keeper_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/keeper/keeper_pb2.py` & `eolymp-0.7.9/eolymp/keeper/keeper_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/keeper/keeper_pb2.pyi` & `eolymp-0.7.9/eolymp/keeper/keeper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/oauth2/oauth2_http.py` & `eolymp-0.7.9/eolymp/oauth2/oauth2_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/oauth2/oauth2_pb2.py` & `eolymp-0.7.9/eolymp/oauth2/oauth2_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/oauth2/oauth2_pb2.pyi` & `eolymp-0.7.9/eolymp/oauth2/oauth2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/playground/playground_http.py` & `eolymp-0.7.9/eolymp/playground/playground_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/playground/playground_pb2.py` & `eolymp-0.7.9/eolymp/playground/playground_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/playground/playground_pb2.pyi` & `eolymp-0.7.9/eolymp/playground/playground_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/playground/run_pb2.py` & `eolymp-0.7.9/eolymp/playground/run_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/playground/run_pb2.pyi` & `eolymp-0.7.9/eolymp/playground/run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/activity_pb2.py` & `eolymp-0.7.9/eolymp/ranker/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/activity_pb2.pyi` & `eolymp-0.7.9/eolymp/ranker/activity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/events_pb2.py` & `eolymp-0.7.9/eolymp/ranker/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/events_pb2.pyi` & `eolymp-0.7.9/eolymp/ranker/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/format_pb2.py` & `eolymp-0.7.9/eolymp/ranker/format_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/ranker_http.py` & `eolymp-0.7.9/eolymp/ranker/ranker_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/ranker_pb2.py` & `eolymp-0.7.9/eolymp/ranker/ranker_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/ranker_pb2.pyi` & `eolymp-0.7.9/eolymp/ranker/ranker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/scoreboard_pb2.py` & `eolymp-0.7.9/eolymp/ranker/scoreboard_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/ranker/scoreboard_pb2.pyi` & `eolymp-0.7.9/eolymp/ranker/scoreboard_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/resolver/resolver_http.py` & `eolymp-0.7.9/eolymp/resolver/resolver_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/resolver/resolver_pb2.py` & `eolymp-0.7.9/eolymp/resolver/resolver_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/resolver/resolver_pb2.pyi` & `eolymp-0.7.9/eolymp/resolver/resolver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/typewriter/block_pb2.py` & `eolymp-0.7.9/eolymp/typewriter/block_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/typewriter/block_pb2.pyi` & `eolymp-0.7.9/eolymp/typewriter/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/typewriter/inline_pb2.py` & `eolymp-0.7.9/eolymp/typewriter/inline_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/typewriter/inline_pb2.pyi` & `eolymp-0.7.9/eolymp/typewriter/inline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/typewriter/typewriter_http.py` & `eolymp-0.7.9/eolymp/typewriter/typewriter_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/typewriter/typewriter_pb2.py` & `eolymp-0.7.9/eolymp/typewriter/typewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/typewriter/typewriter_pb2.pyi` & `eolymp-0.7.9/eolymp/typewriter/typewriter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/universe/idp_pb2.py` & `eolymp-0.7.9/eolymp/community/idp_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/universe/idp.proto
+# source: eolymp/community/idp.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x65olymp/universe/idp.proto\x12\x0f\x65olymp.universe\"\xab\x01\n\x10IdentityProvider\x1a\x96\x01\n\x04OIDC\x12\x11\n\tclient_id\x18\n \x01(\t\x12\x15\n\rclient_secret\x18\x0b \x01(\t\x12\x1a\n\x12\x61uthorize_endpoint\x18\x14 \x01(\t\x12\x16\n\x0etoken_endpoint\x18\x15 \x01(\t\x12\x15\n\rkeys_endpoint\x18\x16 \x01(\t\x12\x19\n\x11userinfo_endpoint\x18\x17 \x01(\tB3Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/community/idp.proto\x12\x10\x65olymp.community\"\xd1\x01\n\x10IdentityProvider\x1a\xbc\x01\n\x04OIDC\x12\x11\n\tclient_id\x18\n \x01(\t\x12\x15\n\rclient_secret\x18\x0b \x01(\t\x12\x0e\n\x06issuer\x18\x14 \x01(\t\x12\x1a\n\x12\x61uthorize_endpoint\x18\x15 \x01(\t\x12\x16\n\x0etoken_endpoint\x18\x16 \x01(\t\x12\x15\n\rkeys_endpoint\x18\x17 \x01(\t\x12\x19\n\x11userinfo_endpoint\x18\x18 \x01(\t\x12\x14\n\x0credirect_uri\x18\x19 \x01(\tB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.universe.idp_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.idp_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/universe;universe'
-  _IDENTITYPROVIDER._serialized_start=47
-  _IDENTITYPROVIDER._serialized_end=218
-  _IDENTITYPROVIDER_OIDC._serialized_start=68
-  _IDENTITYPROVIDER_OIDC._serialized_end=218
+  DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
+  _IDENTITYPROVIDER._serialized_start=49
+  _IDENTITYPROVIDER._serialized_end=258
+  _IDENTITYPROVIDER_OIDC._serialized_start=70
+  _IDENTITYPROVIDER_OIDC._serialized_end=258
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.7.8/eolymp/universe/idp_pb2.pyi` & `eolymp-0.7.9/eolymp/community/idp_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class IdentityProvider(_message.Message):
     __slots__ = []
     class OIDC(_message.Message):
-        __slots__ = ["authorize_endpoint", "client_id", "client_secret", "keys_endpoint", "token_endpoint", "userinfo_endpoint"]
+        __slots__ = ["authorize_endpoint", "client_id", "client_secret", "issuer", "keys_endpoint", "redirect_uri", "token_endpoint", "userinfo_endpoint"]
         AUTHORIZE_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
         CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
         CLIENT_SECRET_FIELD_NUMBER: _ClassVar[int]
+        ISSUER_FIELD_NUMBER: _ClassVar[int]
         KEYS_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
+        REDIRECT_URI_FIELD_NUMBER: _ClassVar[int]
         TOKEN_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
         USERINFO_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
         authorize_endpoint: str
         client_id: str
         client_secret: str
+        issuer: str
         keys_endpoint: str
+        redirect_uri: str
         token_endpoint: str
         userinfo_endpoint: str
-        def __init__(self, client_id: _Optional[str] = ..., client_secret: _Optional[str] = ..., authorize_endpoint: _Optional[str] = ..., token_endpoint: _Optional[str] = ..., keys_endpoint: _Optional[str] = ..., userinfo_endpoint: _Optional[str] = ...) -> None: ...
+        def __init__(self, client_id: _Optional[str] = ..., client_secret: _Optional[str] = ..., issuer: _Optional[str] = ..., authorize_endpoint: _Optional[str] = ..., token_endpoint: _Optional[str] = ..., keys_endpoint: _Optional[str] = ..., userinfo_endpoint: _Optional[str] = ..., redirect_uri: _Optional[str] = ...) -> None: ...
     def __init__(self) -> None: ...
```

### Comparing `eolymp-0.7.8/eolymp/universe/permission_pb2.py` & `eolymp-0.7.9/eolymp/universe/permission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/universe/permission_pb2.pyi` & `eolymp-0.7.9/eolymp/universe/permission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/universe/space_pb2.py` & `eolymp-0.7.9/eolymp/universe/space_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/universe/space_pb2.pyi` & `eolymp-0.7.9/eolymp/universe/space_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/universe/universe_http.py` & `eolymp-0.7.9/eolymp/universe/universe_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,46 +116,14 @@
             url=self.url+path,
             path=path,
             request_data=request,
             response_symbol=_sym_db.GetSymbol("eolymp.universe.ListSpacesOutput"),
             **kwargs,
         )
 
-    def DescribeIdentityProvider(self, request, **kwargs):
-        path = "/spaces/"+urllib.parse.quote(request.space_id)+"/idp"
-
-        # Cleanup URL parameters to avoid any ambiguity
-        request.space_id = ""
-
-        return self.transport.request(
-            name="eolymp.universe.Universe/DescribeIdentityProvider",
-            method="GET",
-            url=self.url+path,
-            path=path,
-            request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.universe.DescribeIdentityProviderOutput"),
-            **kwargs,
-        )
-
-    def ConfigureIdentityProvider(self, request, **kwargs):
-        path = "/spaces/"+urllib.parse.quote(request.space_id)+"/idp"
-
-        # Cleanup URL parameters to avoid any ambiguity
-        request.space_id = ""
-
-        return self.transport.request(
-            name="eolymp.universe.Universe/ConfigureIdentityProvider",
-            method="PUT",
-            url=self.url+path,
-            path=path,
-            request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.universe.ConfigureIdentityProviderOutput"),
-            **kwargs,
-        )
-
     def GrantPermission(self, request, **kwargs):
         path = "/spaces/"+urllib.parse.quote(request.space_id)+"/permissions/"+urllib.parse.quote(request.user_id)
 
         # Cleanup URL parameters to avoid any ambiguity
         request.space_id = ""
         request.user_id = ""
```

### Comparing `eolymp-0.7.8/eolymp/universe/universe_pb2.py` & `eolymp-0.7.9/eolymp/universe/universe_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
-from eolymp.universe import idp_pb2 as eolymp_dot_universe_dot_idp__pb2
 from eolymp.universe import permission_pb2 as eolymp_dot_universe_dot_permission__pb2
 from eolymp.universe import space_pb2 as eolymp_dot_universe_dot_space__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/universe/universe.proto\x12\x0f\x65olymp.universe\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x19\x65olymp/universe/idp.proto\x1a eolymp/universe/permission.proto\x1a\x1b\x65olymp/universe/space.proto\x1a!eolymp/wellknown/expression.proto\"9\n\x10\x43reateSpaceInput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"%\n\x11\x43reateSpaceOutput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"K\n\x10UpdateSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12%\n\x05space\x18\x02 \x01(\x0b\x32\x16.eolymp.universe.Space\"\x13\n\x11UpdateSpaceOutput\"$\n\x10\x44\x65leteSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"\x13\n\x11\x44\x65leteSpaceOutput\"\x1f\n\x10LookupSpaceInput\x12\x0b\n\x03key\x18\x01 \x01(\t\":\n\x11LookupSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"<\n\x13\x44\x65scribeSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeQuotaInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"B\n\x13\x44\x65scribeQuotaOutput\x12+\n\x05quota\x18\x01 \x01(\x0b\x32\x1c.eolymp.universe.Space.Quota\"\xef\x02\n\x0fListSpacesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x38\n\x07\x66ilters\x18( \x01(\x0b\x32\'.eolymp.universe.ListSpacesInput.Filter\x1a\x83\x02\n\x06\x46ilter\x12\r\n\x05query\x18\x64 \x01(\t\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12+\n\x03key\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x04name\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12-\n\x03own\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x30\n\x06member\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"H\n\x10ListSpacesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12%\n\x05items\x18\x02 \x03(\x0b\x32\x16.eolymp.universe.Space\"1\n\x1d\x44\x65scribeIdentityProviderInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"d\n\x1e\x44\x65scribeIdentityProviderOutput\x12\x36\n\x04oidc\x18\x01 \x01(\x0b\x32&.eolymp.universe.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"v\n\x1e\x43onfigureIdentityProviderInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x36\n\x04oidc\x18\n \x01(\x0b\x32&.eolymp.universe.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"!\n\x1f\x43onfigureIdentityProviderOutput\"i\n\x14GrantPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12.\n\x04role\x18\x02 \x01(\x0e\x32 .eolymp.universe.Permission.Role\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x17\n\x15GrantPermissionOutput\":\n\x15RevokePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x18\n\x16RevokePermissionOutput\"<\n\x17\x44\x65scribePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\"K\n\x18\x44\x65scribePermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"-\n\x19IntrospectPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"M\n\x1aIntrospectPermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"\x9d\x02\n\x14ListPermissionsInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.universe.ListPermissionsInput.Filter\x1a\x95\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12/\n\x07user_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12.\n\x04role\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"R\n\x15ListPermissionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.universe.Permission2\xb0\x12\n\x08Universe\x12\x83\x01\n\x0bLookupSpace\x12!.eolymp.universe.LookupSpaceInput\x1a\".eolymp.universe.LookupSpaceOutput\"-\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/spaces/__lookup/{key}\x12\x90\x01\n\x0b\x43reateSpace\x12!.eolymp.universe.CreateSpaceInput\x1a\".eolymp.universe.CreateSpaceOutput\":\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\t\"\x07/spaces\x12\x9b\x01\n\x0bUpdateSpace\x12!.eolymp.universe.UpdateSpaceInput\x1a\".eolymp.universe.UpdateSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x14\x1a\x12/spaces/{space_id}\x12\x9b\x01\n\x0b\x44\x65leteSpace\x12!.eolymp.universe.DeleteSpaceInput\x1a\".eolymp.universe.DeleteSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x14*\x12/spaces/{space_id}\x12\x85\x01\n\rDescribeSpace\x12#.eolymp.universe.DescribeSpaceInput\x1a$.eolymp.universe.DescribeSpaceOutput\")\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x14\x12\x12/spaces/{space_id}\x12\x8b\x01\n\rDescribeQuota\x12#.eolymp.universe.DescribeQuotaInput\x1a$.eolymp.universe.DescribeQuotaOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1a\x12\x18/spaces/{space_id}/quota\x12\x8c\x01\n\nListSpaces\x12 .eolymp.universe.ListSpacesInput\x1a!.eolymp.universe.ListSpacesOutput\"9\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\t\x12\x07/spaces\x12\xaa\x01\n\x18\x44\x65scribeIdentityProvider\x12..eolymp.universe.DescribeIdentityProviderInput\x1a/.eolymp.universe.DescribeIdentityProviderOutput\"-\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/spaces/{space_id}/idp\x12\xc9\x01\n\x19\x43onfigureIdentityProvider\x12/.eolymp.universe.ConfigureIdentityProviderInput\x1a\x30.eolymp.universe.ConfigureIdentityProviderOutput\"I\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18\x1a\x16/spaces/{space_id}/idp\x12\xbd\x01\n\x0fGrantPermission\x12%.eolymp.universe.GrantPermissionInput\x1a&.eolymp.universe.GrantPermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x1a(/spaces/{space_id}/permissions/{user_id}\x12\xc0\x01\n\x10RevokePermission\x12&.eolymp.universe.RevokePermissionInput\x1a\'.eolymp.universe.RevokePermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02**(/spaces/{space_id}/permissions/{user_id}\x12\xc5\x01\n\x12\x44\x65scribePermission\x12(.eolymp.universe.DescribePermissionInput\x1a).eolymp.universe.DescribePermissionOutput\"Z\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/permissions/{user_id}\x12\xb0\x01\n\x14IntrospectPermission\x12*.eolymp.universe.IntrospectPermissionInput\x1a+.eolymp.universe.IntrospectPermissionOutput\"?\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/introspect-permission\x12\xb2\x01\n\x0fListPermissions\x12%.eolymp.universe.ListPermissionsInput\x1a&.eolymp.universe.ListPermissionsOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02 \x12\x1e/spaces/{space_id}/permissionsB3Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/universe/universe.proto\x12\x0f\x65olymp.universe\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/universe/permission.proto\x1a\x1b\x65olymp/universe/space.proto\x1a!eolymp/wellknown/expression.proto\"9\n\x10\x43reateSpaceInput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"%\n\x11\x43reateSpaceOutput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"K\n\x10UpdateSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12%\n\x05space\x18\x02 \x01(\x0b\x32\x16.eolymp.universe.Space\"\x13\n\x11UpdateSpaceOutput\"$\n\x10\x44\x65leteSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"\x13\n\x11\x44\x65leteSpaceOutput\"\x1f\n\x10LookupSpaceInput\x12\x0b\n\x03key\x18\x01 \x01(\t\":\n\x11LookupSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"<\n\x13\x44\x65scribeSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeQuotaInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"B\n\x13\x44\x65scribeQuotaOutput\x12+\n\x05quota\x18\x01 \x01(\x0b\x32\x1c.eolymp.universe.Space.Quota\"\xef\x02\n\x0fListSpacesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x38\n\x07\x66ilters\x18( \x01(\x0b\x32\'.eolymp.universe.ListSpacesInput.Filter\x1a\x83\x02\n\x06\x46ilter\x12\r\n\x05query\x18\x64 \x01(\t\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12+\n\x03key\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x04name\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12-\n\x03own\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x30\n\x06member\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"H\n\x10ListSpacesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12%\n\x05items\x18\x02 \x03(\x0b\x32\x16.eolymp.universe.Space\"i\n\x14GrantPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12.\n\x04role\x18\x02 \x01(\x0e\x32 .eolymp.universe.Permission.Role\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x17\n\x15GrantPermissionOutput\":\n\x15RevokePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x18\n\x16RevokePermissionOutput\"<\n\x17\x44\x65scribePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\"K\n\x18\x44\x65scribePermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"-\n\x19IntrospectPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"M\n\x1aIntrospectPermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"\x9d\x02\n\x14ListPermissionsInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.universe.ListPermissionsInput.Filter\x1a\x95\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12/\n\x07user_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12.\n\x04role\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"R\n\x15ListPermissionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.universe.Permission2\xb7\x0f\n\x08Universe\x12\x83\x01\n\x0bLookupSpace\x12!.eolymp.universe.LookupSpaceInput\x1a\".eolymp.universe.LookupSpaceOutput\"-\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/spaces/__lookup/{key}\x12\x90\x01\n\x0b\x43reateSpace\x12!.eolymp.universe.CreateSpaceInput\x1a\".eolymp.universe.CreateSpaceOutput\":\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\t\"\x07/spaces\x12\x9b\x01\n\x0bUpdateSpace\x12!.eolymp.universe.UpdateSpaceInput\x1a\".eolymp.universe.UpdateSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x14\x1a\x12/spaces/{space_id}\x12\x9b\x01\n\x0b\x44\x65leteSpace\x12!.eolymp.universe.DeleteSpaceInput\x1a\".eolymp.universe.DeleteSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x14*\x12/spaces/{space_id}\x12\x85\x01\n\rDescribeSpace\x12#.eolymp.universe.DescribeSpaceInput\x1a$.eolymp.universe.DescribeSpaceOutput\")\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x14\x12\x12/spaces/{space_id}\x12\x8b\x01\n\rDescribeQuota\x12#.eolymp.universe.DescribeQuotaInput\x1a$.eolymp.universe.DescribeQuotaOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1a\x12\x18/spaces/{space_id}/quota\x12\x8c\x01\n\nListSpaces\x12 .eolymp.universe.ListSpacesInput\x1a!.eolymp.universe.ListSpacesOutput\"9\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\t\x12\x07/spaces\x12\xbd\x01\n\x0fGrantPermission\x12%.eolymp.universe.GrantPermissionInput\x1a&.eolymp.universe.GrantPermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x1a(/spaces/{space_id}/permissions/{user_id}\x12\xc0\x01\n\x10RevokePermission\x12&.eolymp.universe.RevokePermissionInput\x1a\'.eolymp.universe.RevokePermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02**(/spaces/{space_id}/permissions/{user_id}\x12\xc5\x01\n\x12\x44\x65scribePermission\x12(.eolymp.universe.DescribePermissionInput\x1a).eolymp.universe.DescribePermissionOutput\"Z\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/permissions/{user_id}\x12\xb0\x01\n\x14IntrospectPermission\x12*.eolymp.universe.IntrospectPermissionInput\x1a+.eolymp.universe.IntrospectPermissionOutput\"?\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/introspect-permission\x12\xb2\x01\n\x0fListPermissions\x12%.eolymp.universe.ListPermissionsInput\x1a&.eolymp.universe.ListPermissionsOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02 \x12\x1e/spaces/{space_id}/permissionsB3Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.universe.universe_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/universe;universe'
@@ -38,84 +37,72 @@
   _UNIVERSE.methods_by_name['DeleteSpace']._serialized_options = b'\202\343\n\030\212\343\n\024universe:space:write\352\342\n\013\365\342\n\000\000\000@\370\342\n\n\202\323\344\223\002\024*\022/spaces/{space_id}'
   _UNIVERSE.methods_by_name['DescribeSpace']._options = None
   _UNIVERSE.methods_by_name['DescribeSpace']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\nd\202\323\344\223\002\024\022\022/spaces/{space_id}'
   _UNIVERSE.methods_by_name['DescribeQuota']._options = None
   _UNIVERSE.methods_by_name['DescribeQuota']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\nd\202\323\344\223\002\032\022\030/spaces/{space_id}/quota'
   _UNIVERSE.methods_by_name['ListSpaces']._options = None
   _UNIVERSE.methods_by_name['ListSpaces']._serialized_options = b'\202\343\n\027\212\343\n\023universe:space:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\t\022\007/spaces'
-  _UNIVERSE.methods_by_name['DescribeIdentityProvider']._options = None
-  _UNIVERSE.methods_by_name['DescribeIdentityProvider']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\nd\202\323\344\223\002\030\022\026/spaces/{space_id}/idp'
-  _UNIVERSE.methods_by_name['ConfigureIdentityProvider']._options = None
-  _UNIVERSE.methods_by_name['ConfigureIdentityProvider']._serialized_options = b'\202\343\n\030\212\343\n\024universe:space:write\352\342\n\013\365\342\n\000\000\200?\370\342\n\005\202\323\344\223\002\030\032\026/spaces/{space_id}/idp'
   _UNIVERSE.methods_by_name['GrantPermission']._options = None
   _UNIVERSE.methods_by_name['GrantPermission']._serialized_options = b'\202\343\n\030\212\343\n\024universe:space:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002*\032(/spaces/{space_id}/permissions/{user_id}'
   _UNIVERSE.methods_by_name['RevokePermission']._options = None
   _UNIVERSE.methods_by_name['RevokePermission']._serialized_options = b'\202\343\n\030\212\343\n\024universe:space:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002**(/spaces/{space_id}/permissions/{user_id}'
   _UNIVERSE.methods_by_name['DescribePermission']._options = None
   _UNIVERSE.methods_by_name['DescribePermission']._serialized_options = b'\202\343\n\027\212\343\n\023universe:space:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002*\022(/spaces/{space_id}/permissions/{user_id}'
   _UNIVERSE.methods_by_name['IntrospectPermission']._options = None
   _UNIVERSE.methods_by_name['IntrospectPermission']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\n2\202\323\344\223\002*\022(/spaces/{space_id}/introspect-permission'
   _UNIVERSE.methods_by_name['ListPermissions']._options = None
   _UNIVERSE.methods_by_name['ListPermissions']._serialized_options = b'\202\343\n\027\212\343\n\023universe:space:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002 \022\036/spaces/{space_id}/permissions'
-  _CREATESPACEINPUT._serialized_start=275
-  _CREATESPACEINPUT._serialized_end=332
-  _CREATESPACEOUTPUT._serialized_start=334
-  _CREATESPACEOUTPUT._serialized_end=371
-  _UPDATESPACEINPUT._serialized_start=373
-  _UPDATESPACEINPUT._serialized_end=448
-  _UPDATESPACEOUTPUT._serialized_start=450
-  _UPDATESPACEOUTPUT._serialized_end=469
-  _DELETESPACEINPUT._serialized_start=471
-  _DELETESPACEINPUT._serialized_end=507
-  _DELETESPACEOUTPUT._serialized_start=509
-  _DELETESPACEOUTPUT._serialized_end=528
-  _LOOKUPSPACEINPUT._serialized_start=530
-  _LOOKUPSPACEINPUT._serialized_end=561
-  _LOOKUPSPACEOUTPUT._serialized_start=563
-  _LOOKUPSPACEOUTPUT._serialized_end=621
-  _DESCRIBESPACEINPUT._serialized_start=623
-  _DESCRIBESPACEINPUT._serialized_end=661
-  _DESCRIBESPACEOUTPUT._serialized_start=663
-  _DESCRIBESPACEOUTPUT._serialized_end=723
-  _DESCRIBEQUOTAINPUT._serialized_start=725
-  _DESCRIBEQUOTAINPUT._serialized_end=763
-  _DESCRIBEQUOTAOUTPUT._serialized_start=765
-  _DESCRIBEQUOTAOUTPUT._serialized_end=831
-  _LISTSPACESINPUT._serialized_start=834
-  _LISTSPACESINPUT._serialized_end=1201
-  _LISTSPACESINPUT_FILTER._serialized_start=942
-  _LISTSPACESINPUT_FILTER._serialized_end=1201
-  _LISTSPACESOUTPUT._serialized_start=1203
-  _LISTSPACESOUTPUT._serialized_end=1275
-  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_start=1277
-  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_end=1326
-  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_start=1328
-  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_end=1428
-  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_start=1430
-  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_end=1548
-  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_start=1550
-  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_end=1583
-  _GRANTPERMISSIONINPUT._serialized_start=1585
-  _GRANTPERMISSIONINPUT._serialized_end=1690
-  _GRANTPERMISSIONOUTPUT._serialized_start=1692
-  _GRANTPERMISSIONOUTPUT._serialized_end=1715
-  _REVOKEPERMISSIONINPUT._serialized_start=1717
-  _REVOKEPERMISSIONINPUT._serialized_end=1775
-  _REVOKEPERMISSIONOUTPUT._serialized_start=1777
-  _REVOKEPERMISSIONOUTPUT._serialized_end=1801
-  _DESCRIBEPERMISSIONINPUT._serialized_start=1803
-  _DESCRIBEPERMISSIONINPUT._serialized_end=1863
-  _DESCRIBEPERMISSIONOUTPUT._serialized_start=1865
-  _DESCRIBEPERMISSIONOUTPUT._serialized_end=1940
-  _INTROSPECTPERMISSIONINPUT._serialized_start=1942
-  _INTROSPECTPERMISSIONINPUT._serialized_end=1987
-  _INTROSPECTPERMISSIONOUTPUT._serialized_start=1989
-  _INTROSPECTPERMISSIONOUTPUT._serialized_end=2066
-  _LISTPERMISSIONSINPUT._serialized_start=2069
-  _LISTPERMISSIONSINPUT._serialized_end=2354
-  _LISTPERMISSIONSINPUT_FILTER._serialized_start=2205
-  _LISTPERMISSIONSINPUT_FILTER._serialized_end=2354
-  _LISTPERMISSIONSOUTPUT._serialized_start=2356
-  _LISTPERMISSIONSOUTPUT._serialized_end=2438
-  _UNIVERSE._serialized_start=2441
-  _UNIVERSE._serialized_end=4793
+  _CREATESPACEINPUT._serialized_start=248
+  _CREATESPACEINPUT._serialized_end=305
+  _CREATESPACEOUTPUT._serialized_start=307
+  _CREATESPACEOUTPUT._serialized_end=344
+  _UPDATESPACEINPUT._serialized_start=346
+  _UPDATESPACEINPUT._serialized_end=421
+  _UPDATESPACEOUTPUT._serialized_start=423
+  _UPDATESPACEOUTPUT._serialized_end=442
+  _DELETESPACEINPUT._serialized_start=444
+  _DELETESPACEINPUT._serialized_end=480
+  _DELETESPACEOUTPUT._serialized_start=482
+  _DELETESPACEOUTPUT._serialized_end=501
+  _LOOKUPSPACEINPUT._serialized_start=503
+  _LOOKUPSPACEINPUT._serialized_end=534
+  _LOOKUPSPACEOUTPUT._serialized_start=536
+  _LOOKUPSPACEOUTPUT._serialized_end=594
+  _DESCRIBESPACEINPUT._serialized_start=596
+  _DESCRIBESPACEINPUT._serialized_end=634
+  _DESCRIBESPACEOUTPUT._serialized_start=636
+  _DESCRIBESPACEOUTPUT._serialized_end=696
+  _DESCRIBEQUOTAINPUT._serialized_start=698
+  _DESCRIBEQUOTAINPUT._serialized_end=736
+  _DESCRIBEQUOTAOUTPUT._serialized_start=738
+  _DESCRIBEQUOTAOUTPUT._serialized_end=804
+  _LISTSPACESINPUT._serialized_start=807
+  _LISTSPACESINPUT._serialized_end=1174
+  _LISTSPACESINPUT_FILTER._serialized_start=915
+  _LISTSPACESINPUT_FILTER._serialized_end=1174
+  _LISTSPACESOUTPUT._serialized_start=1176
+  _LISTSPACESOUTPUT._serialized_end=1248
+  _GRANTPERMISSIONINPUT._serialized_start=1250
+  _GRANTPERMISSIONINPUT._serialized_end=1355
+  _GRANTPERMISSIONOUTPUT._serialized_start=1357
+  _GRANTPERMISSIONOUTPUT._serialized_end=1380
+  _REVOKEPERMISSIONINPUT._serialized_start=1382
+  _REVOKEPERMISSIONINPUT._serialized_end=1440
+  _REVOKEPERMISSIONOUTPUT._serialized_start=1442
+  _REVOKEPERMISSIONOUTPUT._serialized_end=1466
+  _DESCRIBEPERMISSIONINPUT._serialized_start=1468
+  _DESCRIBEPERMISSIONINPUT._serialized_end=1528
+  _DESCRIBEPERMISSIONOUTPUT._serialized_start=1530
+  _DESCRIBEPERMISSIONOUTPUT._serialized_end=1605
+  _INTROSPECTPERMISSIONINPUT._serialized_start=1607
+  _INTROSPECTPERMISSIONINPUT._serialized_end=1652
+  _INTROSPECTPERMISSIONOUTPUT._serialized_start=1654
+  _INTROSPECTPERMISSIONOUTPUT._serialized_end=1731
+  _LISTPERMISSIONSINPUT._serialized_start=1734
+  _LISTPERMISSIONSINPUT._serialized_end=2019
+  _LISTPERMISSIONSINPUT_FILTER._serialized_start=1870
+  _LISTPERMISSIONSINPUT_FILTER._serialized_end=2019
+  _LISTPERMISSIONSOUTPUT._serialized_start=2021
+  _LISTPERMISSIONSOUTPUT._serialized_end=2103
+  _UNIVERSE._serialized_start=2106
+  _UNIVERSE._serialized_end=4081
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.7.8/eolymp/universe/universe_pb2.pyi` & `eolymp-0.7.9/eolymp/universe/universe_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,20 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
-from eolymp.universe import idp_pb2 as _idp_pb2
 from eolymp.universe import permission_pb2 as _permission_pb2
 from eolymp.universe import space_pb2 as _space_pb2
 from eolymp.wellknown import expression_pb2 as _expression_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class ConfigureIdentityProviderInput(_message.Message):
-    __slots__ = ["oidc", "space_id"]
-    OIDC_FIELD_NUMBER: _ClassVar[int]
-    SPACE_ID_FIELD_NUMBER: _ClassVar[int]
-    oidc: _idp_pb2.IdentityProvider.OIDC
-    space_id: str
-    def __init__(self, space_id: _Optional[str] = ..., oidc: _Optional[_Union[_idp_pb2.IdentityProvider.OIDC, _Mapping]] = ...) -> None: ...
-
-class ConfigureIdentityProviderOutput(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
 class CreateSpaceInput(_message.Message):
     __slots__ = ["space"]
     SPACE_FIELD_NUMBER: _ClassVar[int]
     space: _space_pb2.Space
     def __init__(self, space: _Optional[_Union[_space_pb2.Space, _Mapping]] = ...) -> None: ...
 
 class CreateSpaceOutput(_message.Message):
@@ -42,26 +29,14 @@
     space_id: str
     def __init__(self, space_id: _Optional[str] = ...) -> None: ...
 
 class DeleteSpaceOutput(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class DescribeIdentityProviderInput(_message.Message):
-    __slots__ = ["space_id"]
-    SPACE_ID_FIELD_NUMBER: _ClassVar[int]
-    space_id: str
-    def __init__(self, space_id: _Optional[str] = ...) -> None: ...
-
-class DescribeIdentityProviderOutput(_message.Message):
-    __slots__ = ["oidc"]
-    OIDC_FIELD_NUMBER: _ClassVar[int]
-    oidc: _idp_pb2.IdentityProvider.OIDC
-    def __init__(self, oidc: _Optional[_Union[_idp_pb2.IdentityProvider.OIDC, _Mapping]] = ...) -> None: ...
-
 class DescribePermissionInput(_message.Message):
     __slots__ = ["space_id", "user_id"]
     SPACE_ID_FIELD_NUMBER: _ClassVar[int]
     USER_ID_FIELD_NUMBER: _ClassVar[int]
     space_id: str
     user_id: str
     def __init__(self, space_id: _Optional[str] = ..., user_id: _Optional[str] = ...) -> None: ...
```

### Comparing `eolymp-0.7.8/eolymp/wellknown/direction_pb2.py` & `eolymp-0.7.9/eolymp/wellknown/direction_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/wellknown/errors_pb2.py` & `eolymp-0.7.9/eolymp/wellknown/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/wellknown/errors_pb2.pyi` & `eolymp-0.7.9/eolymp/wellknown/errors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/wellknown/expression_pb2.py` & `eolymp-0.7.9/eolymp/wellknown/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/wellknown/expression_pb2.pyi` & `eolymp-0.7.9/eolymp/wellknown/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/events_pb2.py` & `eolymp-0.7.9/eolymp/workspace/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/events_pb2.pyi` & `eolymp-0.7.9/eolymp/workspace/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/file_pb2.py` & `eolymp-0.7.9/eolymp/workspace/file_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/file_pb2.pyi` & `eolymp-0.7.9/eolymp/workspace/file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/project_pb2.py` & `eolymp-0.7.9/eolymp/workspace/project_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/project_pb2.pyi` & `eolymp-0.7.9/eolymp/workspace/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/workspace_http.py` & `eolymp-0.7.9/eolymp/workspace/workspace_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/workspace_pb2.py` & `eolymp-0.7.9/eolymp/workspace/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp/workspace/workspace_pb2.pyi` & `eolymp-0.7.9/eolymp/workspace/workspace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.7.8/eolymp.egg-info/PKG-INFO` & `eolymp-0.7.9/eolymp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.7.8
+Version: 0.7.9
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.7.8/eolymp.egg-info/SOURCES.txt` & `eolymp-0.7.9/eolymp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 eolymp/community/attribute_pb2.py
 eolymp/community/attribute_pb2.pyi
 eolymp/community/community_http.py
 eolymp/community/community_pb2.py
 eolymp/community/community_pb2.pyi
 eolymp/community/events_pb2.py
 eolymp/community/events_pb2.pyi
+eolymp/community/idp_pb2.py
+eolymp/community/idp_pb2.pyi
 eolymp/community/member_pb2.py
 eolymp/community/member_pb2.pyi
 eolymp/core/__init__.py
 eolymp/core/http_client.py
 eolymp/core/oauth_client.py
 eolymp/executor/__init__.py
 eolymp/executor/events_pb2.py
@@ -187,16 +189,14 @@
 eolymp/typewriter/block_pb2.pyi
 eolymp/typewriter/inline_pb2.py
 eolymp/typewriter/inline_pb2.pyi
 eolymp/typewriter/typewriter_http.py
 eolymp/typewriter/typewriter_pb2.py
 eolymp/typewriter/typewriter_pb2.pyi
 eolymp/universe/__init__.py
-eolymp/universe/idp_pb2.py
-eolymp/universe/idp_pb2.pyi
 eolymp/universe/permission_pb2.py
 eolymp/universe/permission_pb2.pyi
 eolymp/universe/space_pb2.py
 eolymp/universe/space_pb2.pyi
 eolymp/universe/universe_http.py
 eolymp/universe/universe_pb2.py
 eolymp/universe/universe_pb2.pyi
```

### Comparing `eolymp-0.7.8/setup.py` & `eolymp-0.7.9/setup.py`

 * *Files identical despite different names*

