# Comparing `tmp/matcha_ml-0.2.4.tar.gz` & `tmp/matcha_ml-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matcha_ml-0.2.4.tar", max compression
+gzip compressed data, was "matcha_ml-0.2.5.tar", max compression
```

## Comparing `matcha_ml-0.2.4.tar` & `matcha_ml-0.2.5.tar`

### file list

```diff
@@ -1,98 +1,117 @@
--rw-r--r--   0        0        0    11357 2023-03-17 08:00:09.565529 matcha_ml-0.2.4/LICENSE
--rw-r--r--   0        0        0     4177 2023-05-23 16:25:08.463286 matcha_ml-0.2.4/README.md
--rw-r--r--   0        0        0     3484 2023-05-23 16:25:08.463286 matcha_ml-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        6 2023-05-23 14:07:24.530758 matcha_ml-0.2.4/src/matcha_ml/VERSION
--rw-r--r--   0        0        0      220 2023-03-22 07:07:40.360053 matcha_ml-0.2.4/src/matcha_ml/__init__.py
--rw-r--r--   0        0        0       70 2023-03-22 07:07:40.360053 matcha_ml-0.2.4/src/matcha_ml/cli/__init__.py
--rw-r--r--   0        0        0     7710 2023-05-23 16:25:08.463286 matcha_ml-0.2.4/src/matcha_ml/cli/_validation.py
--rw-r--r--   0        0        0     3928 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/cli/cli.py
--rw-r--r--   0        0        0     1298 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/cli/destroy.py
--rw-r--r--   0        0        0      152 2023-05-22 13:24:54.226769 matcha_ml-0.2.4/src/matcha_ml/cli/matcha.config.json
--rw-r--r--   0        0        0     3571 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/cli/provision.py
--rw-r--r--   0        0        0      278 2023-04-03 13:03:18.850286 matcha_ml-0.2.4/src/matcha_ml/cli/ui/emojis.py
--rw-r--r--   0        0        0     1173 2023-05-09 09:06:21.320096 matcha_ml-0.2.4/src/matcha_ml/cli/ui/print_messages.py
--rw-r--r--   0        0        0      472 2023-05-09 14:46:05.874041 matcha_ml-0.2.4/src/matcha_ml/cli/ui/prompt.py
--rw-r--r--   0        0        0     2549 2023-05-09 09:06:21.320096 matcha_ml-0.2.4/src/matcha_ml/cli/ui/resource_message_builders.py
--rw-r--r--   0        0        0     1249 2023-04-03 13:03:18.850286 matcha_ml-0.2.4/src/matcha_ml/cli/ui/spinner.py
--rw-r--r--   0        0        0     1703 2023-04-03 13:03:18.850286 matcha_ml-0.2.4/src/matcha_ml/cli/ui/status_message_builders.py
--rw-r--r--   0        0        0     1780 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/core/core.py
--rw-r--r--   0        0        0     2535 2023-05-09 09:06:21.320096 matcha_ml-0.2.4/src/matcha_ml/errors.py
--rw-r--r--   0        0        0      882 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/.gitignore
--rw-r--r--   0        0        0     9245 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/.terraform.lock.hcl
--rw-r--r--   0        0        0     4696 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/README.md
--rw-r--r--   0        0        0        0 2023-05-16 12:17:59.941060 matcha_ml-0.2.4/src/matcha_ml/infrastructure/__init__.py
--rw-r--r--   0        0        0     2213 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/aks/README.md
--rw-r--r--   0        0        0      439 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/aks/main.tf
--rw-r--r--   0        0        0     1437 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/aks/output.tf
--rw-r--r--   0        0        0      386 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/aks/variables.tf
--rw-r--r--   0        0        0     1605 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/azure_container_registry/README.md
--rw-r--r--   0        0        0      484 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/azure_container_registry/main.tf
--rw-r--r--   0        0        0      327 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/azure_container_registry/output.tf
--rw-r--r--   0        0        0      462 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/azure_container_registry/variables.tf
--rw-r--r--   0        0        0      625 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/configure_kubectl.tf
--rw-r--r--   0        0        0      337 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/helm.tf
--rw-r--r--   0        0        0     1107 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/kubernetes.tf
--rw-r--r--   0        0        0     1912 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/main.tf
--rw-r--r--   0        0        0     2208 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/README.md
--rw-r--r--   0        0        0      308 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/getURI.tf
--rw-r--r--   0        0        0     1314 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/main.tf
--rw-r--r--   0        0        0      251 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/output.tf
--rw-r--r--   0        0        0      383 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/providers.tf
--rw-r--r--   0        0        0      803 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/variables.tf
--rw-r--r--   0        0        0       81 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/zenml_namespace.tf
--rw-r--r--   0        0        0     1945 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/output.tf
--rw-r--r--   0        0        0       33 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/printf.cmd
--rw-r--r--   0        0        0      782 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/providers.tf
--rw-r--r--   0        0        0      892 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/resource_group/README.md
--rw-r--r--   0        0        0      110 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/resource_group/main.tf
--rw-r--r--   0        0        0      106 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/resource_group/output.tf
--rw-r--r--   0        0        0      224 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/resource_group/variables.tf
--rw-r--r--   0        0        0     3010 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/README.md
--rw-r--r--   0        0        0     1894 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/istio.tf
--rw-r--r--   0        0        0     1158 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/main.tf
--rw-r--r--   0        0        0      663 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/outputs.tf
--rw-r--r--   0        0        0      925 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/permissions.tf
--rw-r--r--   0        0        0      380 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/providers.tf
--rw-r--r--   0        0        0      453 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/variables.tf
--rw-r--r--   0        0        0     2914 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/README.md
--rw-r--r--   0        0        0      866 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/main.tf
--rw-r--r--   0        0        0     1779 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/output.tf
--rw-r--r--   0        0        0      124 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/providers.tf
--rw-r--r--   0        0        0      454 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/variables.tf
--rw-r--r--   0        0        0      754 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/variables.tf
--rw-r--r--   0        0        0     6080 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/README.md
--rw-r--r--   0        0        0        0 2023-05-16 12:17:59.944393 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/__init__.py
--rw-r--r--   0        0        0      216 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/getURL.tf
--rw-r--r--   0        0        0      979 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/ingress.tf
--rw-r--r--   0        0        0     3026 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/main.tf
--rw-r--r--   0        0        0      704 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/outputs.tf
--rw-r--r--   0        0        0      292 2023-05-23 16:25:08.466620 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/providers.tf
--rw-r--r--   0        0        0     1943 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/sql.tf
--rw-r--r--   0        0        0     4701 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/variables.tf
--rw-r--r--   0        0        0      342 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/Chart.yaml
--rw-r--r--   0        0        0        0 2023-05-16 12:17:59.944393 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/__init__.py
--rw-r--r--   0        0        0     1987 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt
--rw-r--r--   0        0        0        0 2023-05-16 12:17:59.947726 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/__init__.py
--rw-r--r--   0        0        0     2054 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl
--rw-r--r--   0        0        0     1565 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml
--rw-r--r--   0        0        0      910 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml
--rw-r--r--   0        0        0    10774 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml
--rw-r--r--   0        0        0     2225 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml
--rw-r--r--   0        0        0     3584 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml
--rw-r--r--   0        0        0      367 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-service.yaml
--rw-r--r--   0        0        0      316 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/serviceaccount.yaml
--rw-r--r--   0        0        0        0 2023-05-16 12:17:59.947726 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/tests/__init__.py
--rw-r--r--   0        0        0      379 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0    11587 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml
--rw-r--r--   0        0        0     3453 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zenml_storage/README.md
--rw-r--r--   0        0        0     1102 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zenml_storage/main.tf
--rw-r--r--   0        0        0     1926 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zenml_storage/output.tf
--rw-r--r--   0        0        0      468 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/infrastructure/zenml_storage/variables.tf
--rw-r--r--   0        0        0      103 2023-04-04 14:27:13.046719 matcha_ml-0.2.4/src/matcha_ml/services/__init__.py
--rw-r--r--   0        0        0     7929 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/services/azure_service.py
--rw-r--r--   0        0        0     2652 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/services/matcha_state.py
--rw-r--r--   0        0        0     5503 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/services/terraform_service.py
--rw-r--r--   0        0        0       41 2023-04-26 10:37:10.407733 matcha_ml-0.2.4/src/matcha_ml/templates/__init__.py
--rw-r--r--   0        0        0     7439 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/templates/build_templates/azure_template.py
--rw-r--r--   0        0        0    10536 2023-05-23 16:25:08.469953 matcha_ml-0.2.4/src/matcha_ml/templates/run_template.py
--rw-r--r--   0        0        0     6012 1970-01-01 00:00:00.000000 matcha_ml-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 07:24:38.008574 matcha_ml-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4289 2023-05-19 10:23:10.003833 matcha_ml-0.2.5/README.md
+-rw-r--r--   0        0        0     3706 2023-06-06 14:47:51.925733 matcha_ml-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-06-06 14:47:51.925990 matcha_ml-0.2.5/src/matcha_ml/VERSION
+-rw-r--r--   0        0        0      220 2023-05-16 13:30:52.737917 matcha_ml-0.2.5/src/matcha_ml/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-16 13:30:52.738233 matcha_ml-0.2.5/src/matcha_ml/cli/__init__.py
+-rw-r--r--   0        0        0     7712 2023-06-06 14:40:41.482127 matcha_ml-0.2.5/src/matcha_ml/cli/_validation.py
+-rw-r--r--   0        0        0     5473 2023-06-06 14:40:41.482478 matcha_ml-0.2.5/src/matcha_ml/cli/cli.py
+-rw-r--r--   0        0        0      769 2023-06-06 14:40:41.483120 matcha_ml-0.2.5/src/matcha_ml/cli/constants.py
+-rw-r--r--   0        0        0     2038 2023-06-06 14:40:41.483427 matcha_ml-0.2.5/src/matcha_ml/cli/destroy.py
+-rw-r--r--   0        0        0     4668 2023-06-06 14:40:41.483729 matcha_ml-0.2.5/src/matcha_ml/cli/provision.py
+-rw-r--r--   0        0        0      278 2023-05-16 13:30:52.739662 matcha_ml-0.2.5/src/matcha_ml/cli/ui/emojis.py
+-rw-r--r--   0        0        0     1173 2023-05-16 13:30:52.739975 matcha_ml-0.2.5/src/matcha_ml/cli/ui/print_messages.py
+-rw-r--r--   0        0        0     2549 2023-05-16 13:30:52.740225 matcha_ml-0.2.5/src/matcha_ml/cli/ui/resource_message_builders.py
+-rw-r--r--   0        0        0     1249 2023-05-16 13:30:52.740423 matcha_ml-0.2.5/src/matcha_ml/cli/ui/spinner.py
+-rw-r--r--   0        0        0     1961 2023-06-06 14:40:41.484003 matcha_ml-0.2.5/src/matcha_ml/cli/ui/status_message_builders.py
+-rw-r--r--   0        0        0       61 2023-06-06 14:40:41.484582 matcha_ml-0.2.5/src/matcha_ml/constants.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:40:41.484744 matcha_ml-0.2.5/src/matcha_ml/core/__init__.py
+-rw-r--r--   0        0        0     3027 2023-06-06 14:40:41.485190 matcha_ml-0.2.5/src/matcha_ml/core/core.py
+-rw-r--r--   0        0        0     2535 2023-05-16 13:30:52.741158 matcha_ml-0.2.5/src/matcha_ml/errors.py
+-rw-r--r--   0        0        0      882 2023-06-06 14:40:41.485449 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/.gitignore
+-rw-r--r--   0        0        0     1156 2023-06-06 14:40:41.485898 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/.terraform.lock.hcl
+-rw-r--r--   0        0        0      440 2023-06-06 14:40:41.486078 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/main.tf
+-rw-r--r--   0        0        0      762 2023-06-06 14:40:41.486477 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/output.tf
+-rw-r--r--   0        0        0      110 2023-06-06 14:40:41.486807 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/resource_group/main.tf
+-rw-r--r--   0        0        0      106 2023-06-06 14:40:41.486990 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/resource_group/output.tf
+-rw-r--r--   0        0        0      235 2023-06-06 14:40:41.487228 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/resource_group/variables.tf
+-rw-r--r--   0        0        0      776 2023-06-06 14:40:41.487495 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/main.tf
+-rw-r--r--   0        0        0     1819 2023-06-06 14:40:41.487697 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/output.tf
+-rw-r--r--   0        0        0      457 2023-06-06 14:40:41.487864 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/state_storage/variables.tf
+-rw-r--r--   0        0        0      256 2023-06-06 14:40:41.488045 matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/variables.tf
+-rw-r--r--   0        0        0      882 2023-06-06 14:40:41.488497 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/.gitignore
+-rw-r--r--   0        0        0     9245 2023-06-06 14:40:41.488748 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl
+-rw-r--r--   0        0        0     4696 2023-06-06 14:40:41.488954 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/README.md
+-rw-r--r--   0        0        0     2213 2023-06-06 14:40:41.489267 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/README.md
+-rw-r--r--   0        0        0      439 2023-06-06 14:40:41.489453 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/main.tf
+-rw-r--r--   0        0        0     1437 2023-06-06 14:40:41.489761 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/output.tf
+-rw-r--r--   0        0        0      386 2023-06-06 14:40:41.489995 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/variables.tf
+-rw-r--r--   0        0        0     1605 2023-06-06 14:40:41.490242 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md
+-rw-r--r--   0        0        0      484 2023-06-06 14:40:41.490406 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/main.tf
+-rw-r--r--   0        0        0      327 2023-06-06 14:40:41.490543 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/output.tf
+-rw-r--r--   0        0        0      462 2023-06-06 14:40:41.490689 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/variables.tf
+-rw-r--r--   0        0        0      625 2023-06-06 14:40:41.490863 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/configure_kubectl.tf
+-rw-r--r--   0        0        0      337 2023-06-06 14:40:41.491218 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/helm.tf
+-rw-r--r--   0        0        0     1107 2023-06-06 14:40:41.491487 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/kubernetes.tf
+-rw-r--r--   0        0        0     1886 2023-06-06 14:40:41.491920 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/main.tf
+-rw-r--r--   0        0        0     2208 2023-06-06 14:40:41.492315 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/README.md
+-rw-r--r--   0        0        0      308 2023-06-06 14:40:41.492557 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/getURI.tf
+-rw-r--r--   0        0        0     1314 2023-06-06 14:40:41.492749 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf
+-rw-r--r--   0        0        0      251 2023-06-06 14:40:41.493013 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/output.tf
+-rw-r--r--   0        0        0      383 2023-06-06 14:40:41.493196 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/providers.tf
+-rw-r--r--   0        0        0      803 2023-06-06 14:40:41.493371 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf
+-rw-r--r--   0        0        0       81 2023-06-06 14:40:41.493536 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/zenml_namespace.tf
+-rw-r--r--   0        0        0     2238 2023-06-06 14:40:41.493726 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/output.tf
+-rw-r--r--   0        0        0       33 2023-06-06 14:40:41.493980 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/printf.cmd
+-rw-r--r--   0        0        0      782 2023-06-06 14:40:41.494229 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/providers.tf
+-rw-r--r--   0        0        0      892 2023-06-06 14:40:41.494515 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/README.md
+-rw-r--r--   0        0        0       80 2023-06-06 14:40:41.494699 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/main.tf
+-rw-r--r--   0        0        0      111 2023-06-06 14:40:41.494857 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/output.tf
+-rw-r--r--   0        0        0       95 2023-06-06 14:40:41.494999 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/variables.tf
+-rw-r--r--   0        0        0     3010 2023-06-06 14:40:41.495268 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/README.md
+-rw-r--r--   0        0        0     1894 2023-06-06 14:40:41.495454 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/istio.tf
+-rw-r--r--   0        0        0     1158 2023-06-06 14:40:41.495616 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/main.tf
+-rw-r--r--   0        0        0      663 2023-06-06 14:40:41.495788 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/outputs.tf
+-rw-r--r--   0        0        0      925 2023-06-06 14:40:41.495982 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/permissions.tf
+-rw-r--r--   0        0        0      380 2023-06-06 14:40:41.496142 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/providers.tf
+-rw-r--r--   0        0        0      453 2023-06-06 14:40:41.496307 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/variables.tf
+-rw-r--r--   0        0        0     2914 2023-06-06 14:40:41.496622 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/README.md
+-rw-r--r--   0        0        0      866 2023-06-06 14:40:41.496785 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/main.tf
+-rw-r--r--   0        0        0     1779 2023-06-06 14:40:41.497058 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/output.tf
+-rw-r--r--   0        0        0      124 2023-06-06 14:40:41.497317 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/providers.tf
+-rw-r--r--   0        0        0      454 2023-06-06 14:40:41.497501 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/variables.tf
+-rw-r--r--   0        0        0      754 2023-06-06 14:40:41.497715 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/variables.tf
+-rw-r--r--   0        0        0     6080 2023-06-06 14:40:41.497973 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/README.md
+-rw-r--r--   0        0        0      216 2023-06-06 14:40:41.498149 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/getURL.tf
+-rw-r--r--   0        0        0      979 2023-06-06 14:40:41.498297 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf
+-rw-r--r--   0        0        0     3026 2023-06-06 14:40:41.498465 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/main.tf
+-rw-r--r--   0        0        0      704 2023-06-06 14:40:41.498642 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf
+-rw-r--r--   0        0        0      292 2023-06-06 14:40:41.498805 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/providers.tf
+-rw-r--r--   0        0        0     1943 2023-06-06 14:40:41.498971 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/sql.tf
+-rw-r--r--   0        0        0     4701 2023-06-06 14:40:41.499130 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/variables.tf
+-rw-r--r--   0        0        0      342 2023-06-06 14:40:41.499392 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/Chart.yaml
+-rw-r--r--   0        0        0     1987 2023-06-06 14:40:41.499652 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt
+-rw-r--r--   0        0        0     2054 2023-06-06 14:40:41.499882 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1565 2023-06-06 14:40:41.500086 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml
+-rw-r--r--   0        0        0      910 2023-06-06 14:40:41.500241 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml
+-rw-r--r--   0        0        0    10774 2023-06-06 14:40:41.500516 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml
+-rw-r--r--   0        0        0     2225 2023-06-06 14:40:41.500698 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml
+-rw-r--r--   0        0        0     3584 2023-06-06 14:40:41.500854 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml
+-rw-r--r--   0        0        0      367 2023-06-06 14:40:41.500996 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-service.yaml
+-rw-r--r--   0        0        0      316 2023-06-06 14:40:41.501165 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      379 2023-06-06 14:40:41.501430 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0    11587 2023-06-06 14:40:41.501640 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml
+-rw-r--r--   0        0        0     3453 2023-06-06 14:40:41.501870 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/README.md
+-rw-r--r--   0        0        0     1102 2023-06-06 14:40:41.502010 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf
+-rw-r--r--   0        0        0     1926 2023-06-06 14:40:41.502178 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf
+-rw-r--r--   0        0        0      468 2023-06-06 14:40:41.502319 matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/variables.tf
+-rw-r--r--   0        0        0      170 2023-06-06 14:40:41.502514 matcha_ml-0.2.5/src/matcha_ml/runners/__init__.py
+-rw-r--r--   0        0        0     5732 2023-06-06 14:40:41.502828 matcha_ml-0.2.5/src/matcha_ml/runners/azure_runner.py
+-rw-r--r--   0        0        0     6611 2023-06-06 14:40:41.503191 matcha_ml-0.2.5/src/matcha_ml/runners/base_runner.py
+-rw-r--r--   0        0        0     2825 2023-06-06 14:40:41.503498 matcha_ml-0.2.5/src/matcha_ml/runners/remote_state_runner.py
+-rw-r--r--   0        0        0      103 2023-05-16 13:30:52.757540 matcha_ml-0.2.5/src/matcha_ml/services/__init__.py
+-rw-r--r--   0        0        0      646 2023-06-06 14:40:41.504545 matcha_ml-0.2.5/src/matcha_ml/services/_validation.py
+-rw-r--r--   0        0        0     3409 2023-06-06 14:40:41.505438 matcha_ml-0.2.5/src/matcha_ml/services/analytics_service.py
+-rw-r--r--   0        0        0    10848 2023-06-06 14:40:41.505839 matcha_ml-0.2.5/src/matcha_ml/services/azure_service.py
+-rw-r--r--   0        0        0     4542 2023-06-06 14:40:41.506364 matcha_ml-0.2.5/src/matcha_ml/services/global_parameters_service.py
+-rw-r--r--   0        0        0     5796 2023-06-06 14:40:41.507481 matcha_ml-0.2.5/src/matcha_ml/services/terraform_service.py
+-rw-r--r--   0        0        0      185 2023-05-19 10:43:53.173299 matcha_ml-0.2.5/src/matcha_ml/state/__init__.py
+-rw-r--r--   0        0        0     3028 2023-06-06 14:40:41.507988 matcha_ml-0.2.5/src/matcha_ml/state/matcha_state.py
+-rw-r--r--   0        0        0    11303 2023-06-06 14:40:41.508573 matcha_ml-0.2.5/src/matcha_ml/state/remote_state_manager.py
+-rw-r--r--   0        0        0       94 2023-05-19 10:43:53.174430 matcha_ml-0.2.5/src/matcha_ml/storage/__init__.py
+-rw-r--r--   0        0        0     9692 2023-06-06 14:40:41.508964 matcha_ml-0.2.5/src/matcha_ml/storage/azure_storage.py
+-rw-r--r--   0        0        0      184 2023-06-06 14:40:41.509200 matcha_ml-0.2.5/src/matcha_ml/templates/__init__.py
+-rw-r--r--   0        0        0     1952 2023-06-06 14:40:41.509416 matcha_ml-0.2.5/src/matcha_ml/templates/azure_template.py
+-rw-r--r--   0        0        0     7255 2023-06-06 14:40:41.509594 matcha_ml-0.2.5/src/matcha_ml/templates/base_template.py
+-rw-r--r--   0        0        0      635 2023-06-06 14:40:41.509704 matcha_ml-0.2.5/src/matcha_ml/templates/remote_state_template.py
+-rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 matcha_ml-0.2.5/PKG-INFO
```

### Comparing `matcha_ml-0.2.4/LICENSE` & `matcha_ml-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/README.md` & `matcha_ml-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-    <img src="docs/img/logo.png" width="200" style="max-width: 200px"></img>
+    <img src="https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/logo.png" width="200" style="max-width: 200px"></img>
 </h1>
 
 <p align="center">
     <a href="https://github.com/fuzzylabs/matcha/actions/workflows/ci.yml">
         <img alt="Build" src="https://img.shields.io/github/actions/workflow/status/fuzzylabs/matcha/ci.yml">
     </a>
     <a href="https://github.com/fuzzylabs/matcha/blob/main/LICENSE">
@@ -22,15 +22,15 @@
 </h3>
 
 If you train machine learning models, then you know the challenge of going from _experiment_ to _production_. There's a vast range of tools that promise to help, from experiment tracking through to model deployment, but setting these up requires a lot of time and cloud engineering knowledge.
 
 **Matcha removes the complexity of provisioning your machine learning infrastructure**. With one step, you'll have a complete _machine learning operations (MLOps)_ stack up and running in your Microsoft® Azure cloud environment. This means you'll be able to track your experiments, train your models, as well as deploy and serve those models.
 
 <div align="center">
-    <img src="docs/img/matcha-provision.gif"></img>
+    <img src="https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/matcha-provision.gif"></img>
 </div>
 
 # &#127861; Who is Matcha for?
 
 Matcha is for data scientists, machine learning engineers, and anybody who trains machine learning models. If you're using Azure, and want an intuitive way to deploy machine learning infrastructure, Matcha is for you.
 
 # &#127939; How do I get started?
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
-                       ****** [docs/img/logo.png] ******
+   ****** [https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/
+                               logo.png] ******
                     [Build] [License] [Release] [Downloads]
                **** Open source MLOps on Azure in one step ****
 If you train machine learning models, then you know the challenge of going from
 _experiment_ to _production_. There's a vast range of tools that promise to
 help, from experiment tracking through to model deployment, but setting these
 up requires a lot of time and cloud engineering knowledge. **Matcha removes the
 complexity of provisioning your machine learning infrastructure**. With one
 step, you'll have a complete _machine learning operations (MLOps)_ stack up and
 running in your MicrosoftÂ® Azure cloud environment. This means you'll be able
 to track your experiments, train your models, as well as deploy and serve those
 models.
-                        [docs/img/matcha-provision.gif]
+   [https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/matcha-
+                                provision.gif]
 #  Who is Matcha for? Matcha is for data scientists, machine learning
 engineers, and anybody who trains machine learning models. If you're using
 Azure, and want an intuitive way to deploy machine learning infrastructure,
 Matcha is for you. #  How do I get started? If you're new to Matcha, the best
 place to start is [our guide to deploying your first model](http://
 www.mymatcha.ai/getting-started). If you're happy with the basics, then you
 might want to dive into our [Matcha examples](https://github.com/fuzzylabs/
```

### Comparing `matcha_ml-0.2.4/pyproject.toml` & `matcha_ml-0.2.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "matcha-ml"
-version = "0.2.4"
-description = "Matcha: A open source tool for provisioning MLOps environments to the cloud."
+version = "0.2.5"
+description = "Matcha: An open source tool for provisioning MLOps environments to the cloud."
 authors = ["FuzzyLabs <info@fuzzylabs.ai>"]
 license = "Apache-2.0"
 homepage = "http://fuzzylabs.github.io/matcha"
 documentation = "http://fuzzylabs.github.io/matcha"
 repository = "https://github.com/fuzzylabs/matcha"
 readme = "README.md"
 keywords = ["production", "mlops", "devops", "machine learning"]
@@ -41,22 +41,28 @@
 [tool.poetry.scripts]
 matcha = "matcha_ml.cli.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = {extras = ["all"], version = "^0.7.0"}
 python-terraform = "^0.10.1"
-
 azure-identity = "^1.12.0"
 azure-mgmt-resource = "^23.0.0"
 azure-mgmt-subscription = "^3.1.1"
 azure-mgmt-authorization = "^3.0.0"
 azure-mgmt-confluent = "^1.0.0"
 pyyaml = "^5.4.1"
+types-pyyaml = "^6.0.12.9"
+segment-analytics-python = "^2.2.2"
+azure-mgmt-storage = "^21.0.0"
+dataclasses-json = "^0.5.7"
+azure-storage-blob = "^12.16.0"
 urllib3 = "1.26.6"
+types-urllib3 = "^1.26.25.13"
+requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 mypy = "^1.1.1"
@@ -137,10 +143,11 @@
 | buck-out
 | build
 )/
 '''
 
 [[tool.mypy.overrides]]
 module = [
-    "python_terraform.*"
+    "python_terraform.*",
+    "segment.*"
 ]
 ignore_missing_imports = true
```

### Comparing `matcha_ml-0.2.4/src/matcha_ml/cli/_validation.py` & `matcha_ml-0.2.5/src/matcha_ml/cli/_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from matcha_ml.cli.ui.print_messages import print_error
 from matcha_ml.errors import MatchaInputError
 from matcha_ml.services import AzureClient
 
 # TODO: dynamically set both of these variables
 LONGEST_RESOURCE_NAME = "artifactstore"
 MAXIMUM_RESOURCE_NAME_LEN = 24
-
-MATCHA_STATE_DIR = os.path.join(".matcha", "infrastructure", "matcha.state")
+MATCHA_STATE_PATH = os.path.join(".matcha", "infrastructure", "matcha.state")
 
 
 def _is_alphanumeric(prefix: str) -> bool:
     """Check whether the prefix is an alphanumeric string.
 
     Args:
         prefix (str): the prefix to be checked.
@@ -217,18 +216,18 @@
     """Checks the current deployment using the .matcha directory current contents if it exists.
 
     Specifically, it checks whether the resource group exists on Azure.
 
     Returns:
         bool: True if a deployment currently exists, else False.
     """
-    if not os.path.isfile(MATCHA_STATE_DIR):
+    if not os.path.isfile(MATCHA_STATE_PATH):
         return False
 
-    with open(MATCHA_STATE_DIR) as f:
+    with open(MATCHA_STATE_PATH) as f:
         data = json.load(f)
 
     # Check if a resource group name prefix is present in matcha.state file
     if data.get("cloud") is not None and "prefix" in data.get("cloud"):
         resource_group_name = data["cloud"]["prefix"] + "-resources"
 
         client = get_azure_client()
```

### Comparing `matcha_ml-0.2.4/src/matcha_ml/cli/ui/print_messages.py` & `matcha_ml-0.2.5/src/matcha_ml/cli/ui/print_messages.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/cli/ui/resource_message_builders.py` & `matcha_ml-0.2.5/src/matcha_ml/cli/ui/resource_message_builders.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/cli/ui/spinner.py` & `matcha_ml-0.2.5/src/matcha_ml/cli/ui/spinner.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/cli/ui/status_message_builders.py` & `matcha_ml-0.2.5/src/matcha_ml/cli/ui/status_message_builders.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,7 +65,21 @@
     Args:
         status: status message
 
     Returns:
         str: formatted message
     """
     return f"[green]{status}[/green]"
+
+
+def build_warning_status(status: str) -> str:
+    """Build warning status message.
+
+    Use yellow colour for formatting
+
+    Args:
+        status: status message
+
+    Returns:
+        str: formatted message
+    """
+    return f"[yellow]{status}[/yellow]"
```

### Comparing `matcha_ml-0.2.4/src/matcha_ml/errors.py` & `matcha_ml-0.2.5/src/matcha_ml/errors.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/.gitignore` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/remote_state_storage/.gitignore`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/.terraform.lock.hcl` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/aks/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/aks/output.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/aks/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/azure_container_registry/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/azure_container_registry/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/configure_kubectl.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/configure_kubectl.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/kubernetes.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/kubernetes.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/main.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/main.tf`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
   }
 }
 
 module "resource_group" {
   source = "./resource_group"
 
   prefix   = var.prefix
-  location = var.location
 }
 
 module "storage" {
   source = "./storage"
 
   resource_group_name = module.resource_group.name
   prefix              = var.prefix
```

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/main.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/mlflow_module/variables.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/mlflow_module/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/output.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/output.tf`

 * *Files 6% similar despite different names*

```diff
@@ -52,9 +52,20 @@
 
 output "model_deployer_seldon_base_url" {
   description = "The base URL for the Seldon API server"
   value       = module.seldon.base_url
 }
 
 output "cloud_azure_resource_group_name" {
+  description = "Name of the Azure resource group"
   value = module.resource_group.name
 }
+
+output "cloud_azure_prefix"{
+  description = "The Azure resource group name prefix"
+  value = var.prefix
+}
+
+output "cloud_azure_location"{
+  description = "The Azure location in which the resources are provisioned" 
+  value = var.location
+}
```

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/providers.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/providers.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/resource_group/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/resource_group/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/istio.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/istio.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/main.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/outputs.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/seldon/permissions.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/seldon/permissions.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/main.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/storage/output.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/variables.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/ingress.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/ingress.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/main.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/outputs.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/sql.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/sql.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/variables.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/cert-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-ingress.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/templates/server-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zen_server/zenml_helm/values.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zenml_storage/README.md` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zenml_storage/main.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/infrastructure/zenml_storage/output.tf` & `matcha_ml-0.2.5/src/matcha_ml/infrastructure/resources/zenml_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.4/src/matcha_ml/services/matcha_state.py` & `matcha_ml-0.2.5/src/matcha_ml/state/matcha_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """The matcha state interface."""
+import hashlib
 import json
 import os
 from typing import Dict, List, Optional
 
 
 class MatchaStateService:
     """A matcha state service for handling to matcha.state file."""
 
-    matcha_state_dir = os.path.join(".matcha", "infrastructure", "matcha.state")
+    matcha_state_path = os.path.join(".matcha", "infrastructure", "matcha.state")
 
     def __init__(self) -> None:
         """MatchaStateService constructor."""
         self.state_file_exists = self.check_state_file_exists()
         if self.state_file_exists:
             self._state = self.state_file
 
     @classmethod
     def check_state_file_exists(cls) -> bool:
         """Check if state file exists.
 
         Returns:
             bool: returns True if exists, otherwise False.
         """
-        return bool(os.path.isfile(cls.matcha_state_dir))
+        return bool(os.path.isfile(cls.matcha_state_path))
 
     @property
     def state_file(self) -> Dict[str, Dict[str, str]]:
         """Getter of the state file.
 
         Returns:
             Dict[str, Dict[str, str]]: the state file in the format of a dictionary.
         """
-        with open(self.matcha_state_dir) as f:
+        with open(self.matcha_state_path) as f:
             self._state = dict(json.load(f))
             return dict(self._state)
 
     def fetch_resources_from_state_file(
         self,
         resource_name: Optional[str] = None,
         property_name: Optional[str] = None,
@@ -73,7 +74,18 @@
         Args:
             resource_name (str): the resource name to get properties from.
 
         Returns:
             List[str]: a list of existing properties for a given resource.
         """
         return list(self._state.get(resource_name, {}).keys())
+
+    def get_hash_local_state(self) -> str:
+        """Get hash of the local matcha state file.
+
+        Returns:
+            str: Hash contents of the blob in hexadecimal string
+        """
+        local_hash = None
+        with open(self.matcha_state_path, "rb") as fp:
+            local_hash = hashlib.md5(fp.read()).hexdigest()
+        return local_hash
```

### Comparing `matcha_ml-0.2.4/src/matcha_ml/services/terraform_service.py` & `matcha_ml-0.2.5/src/matcha_ml/services/terraform_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,42 @@
 
 
 @dataclasses.dataclass
 class TerraformConfig:
     """Configuration required for terraform."""
 
     # Path to terraform template are stored
-    working_dir: str = os.path.join(os.getcwd(), ".matcha", "infrastructure")
+    working_dir: str = os.path.join(
+        os.getcwd(), ".matcha", "infrastructure", "resources"
+    )
 
     # state file to store output after terraform apply
-    state_file: str = os.path.join(working_dir, "matcha.state")
+    @property
+    def state_file(self) -> str:
+        """The path to the state file."""
+        return os.path.join(self.working_dir, os.pardir, "matcha.state")
 
     # variables file
-    var_file: str = os.path.join(working_dir, "terraform.tfvars.json")
+    @property
+    def var_file(self) -> str:
+        """The path to the variables file."""
+        return os.path.join(self.working_dir, "terraform.tfvars.json")
 
     # if set to False terraform output will be printed to stdout/stderr
     # else no output will be printed and (ret_code, out, err) tuple will be returned
     capture_output: bool = True
 
 
 class TerraformService:
     """TerraformService class to provision and deprovision resources."""
 
     # configuration required for terraform
-    config: TerraformConfig = TerraformConfig()
+    def __init__(self, terraform_config: TerraformConfig):
+        """Constructor for the TerraformService class."""
+        self.config = terraform_config
 
     # terraform client
     _terraform_client: Optional[python_terraform.Terraform] = None
 
     @property
     def terraform_client(self) -> python_terraform.Terraform:
         """Initialize and/or return the terraform client.
@@ -104,21 +114,20 @@
 
         Returns:
             bool: True when the config file exists.
         """
         return Path(self.config.var_file).exists()
 
     def get_tf_state_dir(self) -> Path:
-        """Get the path of the terraform.tfstate file generated on completion of `terraform init`.
+        """Get the path to the `.terraform` folder generated on completion of `terraform init`.
 
         Returns:
-            Path: a Path object that represents the path to the terraform.tfstate file
-        directory.
+            Path: a Path object that represents the path to the `.terraform` folder.
         """
-        return Path(os.path.join(self.config.working_dir, "terraform.tfstate"))
+        return Path(os.path.join(self.config.working_dir, ".terraform"))
 
     def init(self) -> Tuple[int, str, str]:
         """Run `terraform init` with the initialised Terraform client from the python_terraform module.
 
         Returns:
             Tuple[int, str, str]: return code of Terraform, standard output and standard error.
         """
```

### Comparing `matcha_ml-0.2.4/PKG-INFO` & `matcha_ml-0.2.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: matcha-ml
-Version: 0.2.4
-Summary: Matcha: A open source tool for provisioning MLOps environments to the cloud.
+Version: 0.2.5
+Summary: Matcha: An open source tool for provisioning MLOps environments to the cloud.
 Home-page: http://fuzzylabs.github.io/matcha
 License: Apache-2.0
 Keywords: production,mlops,devops,machine learning
 Author: FuzzyLabs
 Author-email: info@fuzzylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -24,26 +24,33 @@
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-mgmt-authorization (>=3.0.0,<4.0.0)
 Requires-Dist: azure-mgmt-confluent (>=1.0.0,<2.0.0)
 Requires-Dist: azure-mgmt-resource (>=23.0.0,<24.0.0)
+Requires-Dist: azure-mgmt-storage (>=21.0.0,<22.0.0)
 Requires-Dist: azure-mgmt-subscription (>=3.1.1,<4.0.0)
+Requires-Dist: azure-storage-blob (>=12.16.0,<13.0.0)
+Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: python-terraform (>=0.10.1,<0.11.0)
 Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: segment-analytics-python (>=2.2.2,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: types-pyyaml (>=6.0.12.9,<7.0.0.0)
+Requires-Dist: types-urllib3 (>=1.26.25.13,<2.0.0.0)
 Requires-Dist: urllib3 (==1.26.6)
 Project-URL: Bug Tracker, https://github.com/fuzzylabs/matcha/issues
 Project-URL: Documentation, http://fuzzylabs.github.io/matcha
 Project-URL: Repository, https://github.com/fuzzylabs/matcha
 Description-Content-Type: text/markdown
 
 <h1 align="center">
-    <img src="docs/img/logo.png" width="200" style="max-width: 200px"></img>
+    <img src="https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/logo.png" width="200" style="max-width: 200px"></img>
 </h1>
 
 <p align="center">
     <a href="https://github.com/fuzzylabs/matcha/actions/workflows/ci.yml">
         <img alt="Build" src="https://img.shields.io/github/actions/workflow/status/fuzzylabs/matcha/ci.yml">
     </a>
     <a href="https://github.com/fuzzylabs/matcha/blob/main/LICENSE">
@@ -62,15 +69,15 @@
 </h3>
 
 If you train machine learning models, then you know the challenge of going from _experiment_ to _production_. There's a vast range of tools that promise to help, from experiment tracking through to model deployment, but setting these up requires a lot of time and cloud engineering knowledge.
 
 **Matcha removes the complexity of provisioning your machine learning infrastructure**. With one step, you'll have a complete _machine learning operations (MLOps)_ stack up and running in your Microsoft® Azure cloud environment. This means you'll be able to track your experiments, train your models, as well as deploy and serve those models.
 
 <div align="center">
-    <img src="docs/img/matcha-provision.gif"></img>
+    <img src="https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/matcha-provision.gif"></img>
 </div>
 
 # &#127861; Who is Matcha for?
 
 Matcha is for data scientists, machine learning engineers, and anybody who trains machine learning models. If you're using Azure, and want an intuitive way to deploy machine learning infrastructure, Matcha is for you.
 
 # &#127939; How do I get started?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.4 Summary: Matcha: A open
+Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.5 Summary: Matcha: An open
 source tool for provisioning MLOps environments to the cloud. Home-page: http:/
 /fuzzylabs.github.io/matcha License: Apache-2.0 Keywords:
 production,mlops,devops,machine learning Author: FuzzyLabs Author-email:
 info@fuzzylabs.ai Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -12,34 +12,41 @@
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Dist: azure-identity
 (>=1.12.0,<2.0.0) Requires-Dist: azure-mgmt-authorization (>=3.0.0,<4.0.0)
 Requires-Dist: azure-mgmt-confluent (>=1.0.0,<2.0.0) Requires-Dist: azure-mgmt-
-resource (>=23.0.0,<24.0.0) Requires-Dist: azure-mgmt-subscription
-(>=3.1.1,<4.0.0) Requires-Dist: python-terraform (>=0.10.1,<0.11.0) Requires-
-Dist: pyyaml (>=5.4.1,<6.0.0) Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Requires-Dist: urllib3 (==1.26.6) Project-URL: Bug Tracker, https://github.com/
-fuzzylabs/matcha/issues Project-URL: Documentation, http://fuzzylabs.github.io/
-matcha Project-URL: Repository, https://github.com/fuzzylabs/matcha
-Description-Content-Type: text/markdown
-                       ****** [docs/img/logo.png] ******
+resource (>=23.0.0,<24.0.0) Requires-Dist: azure-mgmt-storage
+(>=21.0.0,<22.0.0) Requires-Dist: azure-mgmt-subscription (>=3.1.1,<4.0.0)
+Requires-Dist: azure-storage-blob (>=12.16.0,<13.0.0) Requires-Dist:
+dataclasses-json (>=0.5.7,<0.6.0) Requires-Dist: python-terraform
+(>=0.10.1,<0.11.0) Requires-Dist: pyyaml (>=5.4.1,<6.0.0) Requires-Dist:
+requests (>=2.31.0,<3.0.0) Requires-Dist: segment-analytics-python
+(>=2.2.2,<3.0.0) Requires-Dist: typer[all] (>=0.7.0,<0.8.0) Requires-Dist:
+types-pyyaml (>=6.0.12.9,<7.0.0.0) Requires-Dist: types-urllib3
+(>=1.26.25.13,<2.0.0.0) Requires-Dist: urllib3 (==1.26.6) Project-URL: Bug
+Tracker, https://github.com/fuzzylabs/matcha/issues Project-URL: Documentation,
+http://fuzzylabs.github.io/matcha Project-URL: Repository, https://github.com/
+fuzzylabs/matcha Description-Content-Type: text/markdown
+   ****** [https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/
+                               logo.png] ******
                     [Build] [License] [Release] [Downloads]
                **** Open source MLOps on Azure in one step ****
 If you train machine learning models, then you know the challenge of going from
 _experiment_ to _production_. There's a vast range of tools that promise to
 help, from experiment tracking through to model deployment, but setting these
 up requires a lot of time and cloud engineering knowledge. **Matcha removes the
 complexity of provisioning your machine learning infrastructure**. With one
 step, you'll have a complete _machine learning operations (MLOps)_ stack up and
 running in your MicrosoftÂ® Azure cloud environment. This means you'll be able
 to track your experiments, train your models, as well as deploy and serve those
 models.
-                        [docs/img/matcha-provision.gif]
+   [https://raw.githubusercontent.com/fuzzylabs/matcha/main/docs/img/matcha-
+                                provision.gif]
 #  Who is Matcha for? Matcha is for data scientists, machine learning
 engineers, and anybody who trains machine learning models. If you're using
 Azure, and want an intuitive way to deploy machine learning infrastructure,
 Matcha is for you. #  How do I get started? If you're new to Matcha, the best
 place to start is [our guide to deploying your first model](http://
 www.mymatcha.ai/getting-started). If you're happy with the basics, then you
 might want to dive into our [Matcha examples](https://github.com/fuzzylabs/
```

