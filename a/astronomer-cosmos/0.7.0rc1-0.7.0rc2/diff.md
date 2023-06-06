# Comparing `tmp/astronomer_cosmos-0.7.0rc1.tar.gz` & `tmp/astronomer_cosmos-0.7.0rc2.tar.gz`

## Comparing `astronomer_cosmos-0.7.0rc1.tar` & `astronomer_cosmos-0.7.0rc2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/tests/test_airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/dataset.py
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0    13421 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_docker.py
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_local.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/base.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/token.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/thrift.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/tests/test_base.py
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/tests/test_profiles.py.tmp
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/base.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/warn_parsing.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/tests/test_project.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_dataset.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_export.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_render.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/tests/test_version.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/LICENSE
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/README.rst
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/core/tests/test_airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0    13421 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_docker.py
+-rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_local.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/base.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/token.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/thrift.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/tests/test_base.py
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/tests/test_profiles.py.tmp
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/base.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/warn_parsing.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/tests/test_project.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_dataset.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_export.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_render.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/cosmos/tests/test_version.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/README.rst
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc2/PKG-INFO
```

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/core/airflow.py` & `astronomer_cosmos-0.7.0rc2/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.7.0rc2/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/core/tests/test_airflow.py` & `astronomer_cosmos-0.7.0rc2/cosmos/core/tests/test_airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_docker.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_local.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/operators/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/base.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/token.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/thrift.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/tests/test_base.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/tests/test_profiles.py.tmp` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/tests/test_profiles.py.tmp`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/base.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/certificate.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/jwt.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/jwt.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,34 +11,35 @@
     Maps Airflow Trino connections to JWT Trino dbt profiles.
 
     https://docs.getdbt.com/reference/warehouse-setups/trino-setup#jwt
     https://airflow.apache.org/docs/apache-airflow-providers-trino/stable/connections.html
     """
 
     required_fields = TrinoBaseProfileMapping.required_fields + [
-        "jwt",
+        "jwt_token",
     ]
     secret_fields = [
-        "jwt",
+        "jwt_token",
     ]
     airflow_param_mapping = {
-        "jwt": "extra.jwt__token",
+        "jwt_token": "extra.jwt__token",
         **TrinoBaseProfileMapping.airflow_param_mapping,
     }
 
     def get_profile(self) -> dict[str, Any | None]:
         "Gets profile."
         common_profile_vars = super().get_profile()
 
         # need to remove jwt from profile_args because it will be set as an environment variable
         profile_args = self.profile_args.copy()
         profile_args.pop("jwt", None)
 
         profile_vars = {
             **common_profile_vars,
             "method": "jwt",
-            "jwt": self.get_env_var_format("jwt"),
             **profile_args,
+            # jwt_token should always get set as env var
+            "jwt_token": self.get_env_var_format("jwt_token"),
         }
 
         # remove any null values
         return self.filter_null(profile_vars)
```

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/ldap.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py`

 * *Files 11% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     assert profile_mapping.get_profile() == {
         "type": "trino",
         "method": "jwt",
         "host": "my_host",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
-        "jwt": "{{ env_var('COSMOS_CONN_TRINO_JWT') }}",
+        "jwt_token": "{{ env_var('COSMOS_CONN_TRINO_JWT_TOKEN') }}",
     }
 
 
 def test_profile_args_overrides(
     mock_trino_conn: Connection,
 ) -> None:
     """
@@ -152,32 +152,32 @@
     """
     profile_mapping = get_profile_mapping(
         mock_trino_conn.conn_id,
         profile_args={
             "database": "my_database",
             "schema": "my_schema",
             "host": "my_host_override",
-            "jwt": "my_jwt_token_override",
+            "jwt_token": "my_jwt_token_override",
         },
     )
     assert profile_mapping.profile_args == {
         "database": "my_database",
         "schema": "my_schema",
         "host": "my_host_override",
-        "jwt": "my_jwt_token_override",
+        "jwt_token": "my_jwt_token_override",
     }
 
     assert profile_mapping.get_profile() == {
         "type": "trino",
         "method": "jwt",
         "host": "my_host_override",
         "port": 8080,
         "database": "my_database",
         "schema": "my_schema",
-        "jwt": "{{ env_var('COSMOS_CONN_TRINO_JWT') }}",
+        "jwt_token": "{{ env_var('COSMOS_CONN_TRINO_JWT_TOKEN') }}",
     }
 
 
 def test_profile_env_vars(
     mock_trino_conn: Connection,
 ) -> None:
     """
@@ -187,9 +187,9 @@
         mock_trino_conn.conn_id,
         profile_args={
             "database": "my_database",
             "schema": "my_schema",
         },
     )
     assert profile_mapping.get_env_vars() == {
-        "COSMOS_CONN_TRINO_JWT": "my_jwt_token",
+        "COSMOS_CONN_TRINO_JWT_TOKEN": "my_jwt_token",
     }
```

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/warn_parsing.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/tests/test_project.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_dataset.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_export.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_render.py` & `astronomer_cosmos-0.7.0rc2/cosmos/providers/dbt/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/.gitignore` & `astronomer_cosmos-0.7.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/LICENSE` & `astronomer_cosmos-0.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/README.rst` & `astronomer_cosmos-0.7.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/pyproject.toml` & `astronomer_cosmos-0.7.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.0rc1/PKG-INFO` & `astronomer_cosmos-0.7.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.7.0rc1
+Version: 0.7.0rc2
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
```

