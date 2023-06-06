# Comparing `tmp/servicefoundry-0.9.3rc1.tar.gz` & `tmp/servicefoundry-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.9.3rc1.tar", max compression
+gzip compressed data, was "servicefoundry-0.9.4.tar", max compression
```

## Comparing `servicefoundry-0.9.3rc1.tar` & `servicefoundry-0.9.4.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0      672 2023-05-31 18:48:39.178525 servicefoundry-0.9.3rc1/README.md
--rw-r--r--   0        0        0     2119 2023-05-31 18:48:51.271391 servicefoundry-0.9.3rc1/pyproject.toml
--rw-r--r--   0        0        0     1315 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/__init__.py
--rw-r--r--   0        0        0    38045 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4294 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      632 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1317 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
--rw-r--r--   0        0        0     1369 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     1357 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6496 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6480 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     2795 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     3587 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     3863 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      242 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     2492 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-05-31 18:48:39.182525 servicefoundry-0.9.3rc1/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    23939 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     5624 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1123 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0    10072 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5318 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8890 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-05-31 18:48:39.186525 servicefoundry-0.9.3rc1/servicefoundry/version.py
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.9.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/README.md
+-rw-r--r--   0        0        0     2116 2023-06-06 13:14:50.381547 servicefoundry-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1365 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    39576 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4294 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1364 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1317 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
+-rw-r--r--   0        0        0     1369 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     1357 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6496 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6480 2023-06-06 13:14:37.765556 servicefoundry-0.9.4/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     3536 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     4462 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     4134 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2970 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    25229 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0    10866 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-06-06 13:14:37.769556 servicefoundry-0.9.4/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-06-06 13:14:37.773556 servicefoundry-0.9.4/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0    10072 2023-06-06 13:14:37.773556 servicefoundry-0.9.4/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-06-06 13:14:37.773556 servicefoundry-0.9.4/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-06-06 13:14:37.773556 servicefoundry-0.9.4/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5396 2023-06-06 13:14:37.773556 servicefoundry-0.9.4/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8890 2023-06-06 13:14:37.773556 servicefoundry-0.9.4/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-06-06 13:14:37.773556 servicefoundry-0.9.4/servicefoundry/version.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.9.4/PKG-INFO
```

### Comparing `servicefoundry-0.9.3rc1/README.md` & `servicefoundry-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/pyproject.toml` & `servicefoundry-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.9.3rc1"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.4"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/__init__.py` & `servicefoundry-0.9.4/servicefoundry/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     CapacityType,
     ParamType,
 )
 from servicefoundry.core import login, logout
 from servicefoundry.lib.dao.application import (
     delete_application,
     get_application,
+    get_job_run,
     list_applications,
+    list_job_runs,
     trigger_job,
 )
 from servicefoundry.lib.dao.version import (
     get_version as get_application_version,
     list_versions as list_application_versions,
 )
 from servicefoundry.lib.dao.workspace import (
@@ -55,9 +57,10 @@
     Schedule,
     SecretMount,
     StringDataMount,
     VolumeMount,
     TruefoundryModelRegistry,
     NodepoolSelector,
     NodeSelector,
+    Endpoint,
 )
 from servicefoundry.version import __version__
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/auto_gen/models.py` & `servicefoundry-0.9.4/servicefoundry/auto_gen/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  application.json
-#   timestamp: 2023-05-31T15:52:02+00:00
+#   timestamp: 2023-06-06T08:33:20+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, confloat, conint, constr
@@ -25,15 +25,15 @@
         ...,
         description="+label=Password for service auth\n+message=Password should not be more than 64 characters\n+sort=2",
     )
 
 
 class BlueGreen(BaseModel):
     """
-    +docs=This strategy brings up the new release completely before switching the complete load to the new release.
+        +docs=This strategy brings up the new release completely before switching the complete load to the new release.
     This minimizes the time that two versions are serving traffic at the same time.
     +label=Blue Green strategy
     """
 
     type: Literal["blue_green"] = Field(..., description="+value=blue_green")
     enable_auto_promotion: bool = Field(
         False,
@@ -62,15 +62,15 @@
         30,
         description="+docs=Duration for which to pause the release. The release process will wait for these seconds before proceeding to the next step.\nIf this is not set, the step will pause indefinitely on this step\n+label=Pause duration\n+unit=seconds\n+placeholder=Duration",
     )
 
 
 class DockerFileBuild(BaseModel):
     """
-    +docs=Describes that we are using a dockerfile to build our image
+        +docs=Describes that we are using a dockerfile to build our image
     +label=Docker File (I already have Docker File)
     +icon=fa-brands fa-docker:#0db7ed
     """
 
     type: constr(regex=r"^dockerfile$") = Field(..., description="+value=dockerfile")
     dockerfile_path: str = Field(
         "./Dockerfile",
@@ -82,17 +82,32 @@
     )
     command: Optional[Union[str, List[str]]] = Field(
         None,
         description="+label=Entrypoint Override\n+usage=Override the command to run when the container starts\nWhen deploying a Job, the command can be templatized by defining `params` and referencing them in command\nE.g. `python main.py --learning_rate {{learning_rate}}`",
     )
 
 
+class Endpoint(BaseModel):
+    host: constr(
+        regex=r"^(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\-]*[a-zA-Z0-9])\.)(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\-]*[a-zA-Z0-9])\.)*([A-Za-z0-9]|[A-Za-z0-9][A-Za-z0-9\-]*[A-Za-z0-9])$"
+    ) = Field(
+        ...,
+        description="+usage=Host e.g. ai.example.com, app.truefoundry.com\n+message=Upto 253 characters, each part of host should be at most 63 characters long, can contain alphabets, digits and hypen, must begin and end with an alphanumeric characters. Parts must be separated by periods (.)",
+    )
+    path: Optional[
+        constr(regex=r"^(/([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\-_\.]*[a-zA-Z0-9]))*/$")
+    ] = Field(
+        None,
+        description="+usage=Path e.g. /v1/api/ml/, /v2/docs/\n+message=Should begin and end with a forward slash (/). Each part can can contain alphabets, digits and hypen, must begin and end with an alphanumeric characters. Parts should be separated by forward slashes (/)",
+    )
+
+
 class GitSource(BaseModel):
     """
-    +docs=Describes that we are using code stored in a git repository to build our image
+        +docs=Describes that we are using code stored in a git repository to build our image
     +label=Git Source
     +icon=fa-solid fa-code-branch:black
     +sort=300
     """
 
     type: constr(regex=r"^git$") = Field(..., description="+value=git")
     repo_url: constr(
@@ -108,15 +123,15 @@
         None,
         description="+label=Branch Name\n+usage=Selecting branch will select latest commit SHA of the branch.\n+sort=3\n+ignore",
     )
 
 
 class HttpProbe(BaseModel):
     """
-    +docs=Describes the Instructions for assessing container health by executing an HTTP GET request.
+        +docs=Describes the Instructions for assessing container health by executing an HTTP GET request.
     To learn more you can go [here](https://docs.truefoundry.com/docs/add-health-checks-to-deployments)
     +label=Instructions for assessing container health by executing an HTTP GET request.
     """
 
     type: constr(regex=r"^http$") = Field(..., description="+sort=1\n+value=http")
     path: str = Field(
         ...,
@@ -133,15 +148,15 @@
     scheme: str = Field(
         "HTTP", description="+sort=5\n+usage=Scheme to use for connecting to the host"
     )
 
 
 class HuggingfaceModelHub(BaseModel):
     """
-    +docs=Huggingface model hub (deploy a model from HF model hub)
+        +docs=Huggingface model hub (deploy a model from HF model hub)
     +label=Huggingface model hub
     +usage=Deploy a model from HF model hub
     """
 
     type: constr(regex=r"^hf-model-hub$") = Field(
         ..., description="+value=hf-model-hub"
     )
@@ -153,15 +168,15 @@
         None,
         description="+label=Pipeline\n+usage=Pipeline to use for inference. If not set, we will try to infer the `task` name for the given model.\nExamples:- `summarization`, `text-generation`, `text-classification`, etc.\nYou can read more about HF pipelines here:- https://huggingface.co/docs/transformers/pipeline_tutorial\nYou can find a list of tasks here:- https://huggingface.co/docs/transformers/v4.24.0/en/main_classes/pipelines#transformers.pipeline.task\n+placeholder=summarization",
     )
 
 
 class Image(BaseModel):
     """
-    +docs=Describes that we are using a pre-built image stored in a Docker Image registry
+        +docs=Describes that we are using a pre-built image stored in a Docker Image registry
     +label=Docker Image (Deploy an existing image)
     +icon=fa-brands fa-docker:#0db7ed
     """
 
     type: constr(regex=r"^image$") = Field(..., description="+value=image")
     image_uri: constr(regex=r"^\S*$") = Field(
         ...,
@@ -186,38 +201,38 @@
         None,
         description="+label=Additional Manifests\n+usage=Additional kubernetes manifests to be included in the application",
     )
 
 
 class LocalSource(BaseModel):
     """
-    +docs=Describes that we are using code stored in a local developement environment to build our image
+        +docs=Describes that we are using code stored in a local developement environment to build our image
     +label=Local
     +icon=fa-folder:black
     +sort=100
     """
 
     type: constr(regex=r"^local$") = Field(..., description="+value=local")
     project_root_path: str = Field("./", description="+usage=Local project root path.")
     local_build: bool = Field(True, description="run docker build locally")
 
 
 class Manual(BaseModel):
     """
-    +docs=Describes that we are going to manually trigger our job.
+        +docs=Describes that we are going to manually trigger our job.
     +label=Manual
     +usage=Trigger the job manually. [Docs](https://docs.truefoundry.com/docs/more-configurations)
     """
 
     type: constr(regex=r"^manual$") = Field(..., description="+value=manual")
 
 
 class CapacityType(str, Enum):
     """
-    +label=Capacity Type
+        +label=Capacity Type
     +usage=Configure what type of nodes to run the app. By default no placement logic is applied.
     "spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.
     "spot" will strictly place the application on spot nodes.
     "on_demand" will strictly place the application on on-demand nodes.
     """
 
     spot_fallback_on_demand = "spot_fallback_on_demand"
@@ -287,15 +302,15 @@
 
     TCP = "TCP"
     UDP = "UDP"
 
 
 class AppProtocol(str, Enum):
     """
-    +label=Application Protocol
+        +label=Application Protocol
     +usage=Application Protocol for the port.
     Select the application protocol used by your service. For most use cases, this should be `http`(HTTP/1.1).
     If you are running a gRPC server, select the `grpc` option.
     This is only applicable if `expose=true`.
     """
 
     http = "http"
@@ -338,15 +353,15 @@
         description="+label=Application Protocol\n+usage=Application Protocol for the port.\nSelect the application protocol used by your service. For most use cases, this should be `http`(HTTP/1.1).\nIf you are running a gRPC server, select the `grpc` option.\nThis is only applicable if `expose=true`.",
     )
     auth: Optional[BasicAuthCreds] = None
 
 
 class PythonBuild(BaseModel):
     """
-    +docs=Describes that we are using python to build a container image with a specific python version and pip packages installed.
+        +docs=Describes that we are using python to build a container image with a specific python version and pip packages installed.
     +label=Python Code (I don't have Dockerfile)
     +icon=fa-brands fa-python:#306998
     """
 
     type: constr(regex=r"^tfy-python-buildpack$") = Field(
         ..., description="+value=tfy-python-buildpack"
     )
@@ -390,29 +405,29 @@
         ...,
         description="+label=Requests per second\n+usage=Average request per second averaged over all replicas that autoscaler should try to maintain",
     )
 
 
 class RemoteSource(BaseModel):
     """
-    +docs=Describes that we are using code stored in a remote respository to build our image
+        +docs=Describes that we are using code stored in a remote respository to build our image
     +label=S3
     +icon=fa-brands fa-aws:black
     +sort=200
     """
 
     type: constr(regex=r"^remote$") = Field(..., description="+value=remote")
     remote_uri: str = Field(
         ..., description="+docs=Remote repository URI\n+label=Remote URI"
     )
 
 
 class Resources(BaseModel):
     """
-    +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
+        +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
     To learn more you can go [here](https://docs.truefoundry.com/docs/resources)
     +icon=fa-microchip
     +label=Resources
     +usage=Set resource constraints for the application. [Docs](https://docs.truefoundry.com/docs/resources)
     """
 
     cpu_request: confloat(ge=0.001, le=128.0) = Field(
@@ -451,15 +466,15 @@
         None,
         description="+label=Node\n+usage=This field determines how the underlying node resource is to be utilized",
     )
 
 
 class Rolling(BaseModel):
     """
-    +docs=This strategy updates the pods in a rolling fashion such that a subset of the
+        +docs=This strategy updates the pods in a rolling fashion such that a subset of the
     total pods are replaced with new version at one time.
     A commonly used strategy can be to have maxUnavailablePercentage close to 0 so that there
     is no downtime and keep the maxSurgePercentage to around 25%. If you are anyways running
     a large number of pods, the service can often tolerate a few pods going down - so you
     max maxUnavailablePercentage = 10 and maxSurgePercentage=0. You can read about it more
     [here](https://spot.io/resources/kubernetes-autoscaling/5-kubernetes-deployment-strategies-roll-out-like-the-pros/)
     +label=Rolling update strategy
@@ -476,27 +491,27 @@
         0,
         description="+label=Max Surge(%)\n+usage=Percentage of total replicas of updated image that can be brought up over the total replicas count.\nFor a value of 25 when replicas are set to 12 this would mean (12+(25% of 12) = 15) pods might be running at one time.\nSetting this to a higher value can help in speeding up the deployment process.",
     )
 
 
 class ConcurrencyPolicy(str, Enum):
     """
-    +usage=Choose whether to allow this job to run while another instance of the job is running, or to replace the currently running instance. Allow
+        +usage=Choose whether to allow this job to run while another instance of the job is running, or to replace the currently running instance. Allow
     will enable multiple instances of this job to run. Forbid will keep the current instance of the job running and stop a new instance from being run.
     Replace will terminate any currently running instance of the job and start a new one.
     """
 
     Forbid = "Forbid"
     Allow = "Allow"
     Replace = "Replace"
 
 
 class Schedule(BaseModel):
     """
-    +docs=Describes that we are going to schedule our job to run at a schedule, making our job a cron job.
+        +docs=Describes that we are going to schedule our job to run at a schedule, making our job a cron job.
     +label=Schedule
     +usage=Run the job on a schedule. [Docs](https://docs.truefoundry.com/docs/deploy-a-cron-job)
     """
 
     type: constr(regex=r"^scheduled$") = Field(..., description="+value=scheduled")
     schedule: str = Field(
         ...,
@@ -531,15 +546,15 @@
         description="+label=File Path\n+usage=Absolute file path where the file will be created.\n+message=Please enter a valid file path",
     )
     data: str = Field(..., description="+label=Data\n+usage=The file content.")
 
 
 class TruefoundryModelRegistry(BaseModel):
     """
-    +docs=Truefoundry model registry (deploy a model from TFY model registry)
+        +docs=Truefoundry model registry (deploy a model from TFY model registry)
     +label=Truefoundry model registry
     +usage=Deploy a model from TFY model registry
     """
 
     type: constr(regex=r"^tfy-model-registry$") = Field(
         ..., description="+value=tfy-model-registry"
     )
@@ -574,15 +589,15 @@
         ...,
         description="+label=Autoscaling metrics\n+usage=Metrics to use for the autoscaler",
     )
 
 
 class Build(BaseModel):
     """
-    +docs=Describes how we build our code into a Docker image.
+        +docs=Describes how we build our code into a Docker image.
     +label=Source Code (Build and deploy source code)
     +icon=fa-code
     """
 
     type: constr(regex=r"^build$") = Field(..., description="+value=build")
     docker_registry: Optional[str] = Field(
         None,
@@ -596,29 +611,29 @@
         ...,
         description="+docs=Instructions to build a container image out of the build source\n+label=Build using DockerFile or using Buildpack\n+icon=fa-wrench\n+sort=2",
     )
 
 
 class Canary(BaseModel):
     """
-    +docs=This strategy brings up the new release without bringing the older release down. Traffic is shifted from the older release to the newer release in a staged manner.
+        +docs=This strategy brings up the new release without bringing the older release down. Traffic is shifted from the older release to the newer release in a staged manner.
     This can help with verifying the health of the new release without shifting complete traffic.
     +label=Canary strategy
     """
 
     type: Literal["canary"] = Field(..., description="+value=canary")
     steps: List[CanaryStep] = Field(
         ...,
         description="+docs=These steps would be executed in order to enable shifting of traffic slowly from stable to canary version\n+label=Steps",
     )
 
 
 class HealthProbe(BaseModel):
     """
-    +docs=Describes the configuration for the Health Probe's
+        +docs=Describes the configuration for the Health Probe's
     To learn more you can go [here](https://docs.truefoundry.com/docs/add-health-checks-to-deployments)
     +icon=fa-heart
     """
 
     config: HttpProbe
     initial_delay_seconds: conint(ge=0, le=36000) = Field(
         0,
@@ -684,31 +699,40 @@
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
 
 
 class ModelDeployment(BaseModel):
     """
-    +docs=Describes the configuration for the model deployment
+        +docs=Describes the configuration for the model deployment
     +usage=To learn more you can go [here](https://dash.readme.com/project/truefoundry/v0.1.1/docs/model-deployment-2)
     """
 
     type: constr(regex=r"^model-deployment$") = Field(
         ..., description="+value=model-deployment"
     )
     name: constr(regex=r"^[a-z][a-z0-9\-]{1,17}[a-z0-9]$") = Field(
         ...,
         description="+usage=Name of the model deployment. This uniquely identifies this deployment in the workspace.\n> Name can only contain alphanumeric characters and '-' and can be atmost 20 characters long\n+sort=1\n+label=Model deployment name\n+message=3 to 19 lower case characters long alphanumeric word, may contain - in between, cannot start with a number",
     )
     model_source: Union[TruefoundryModelRegistry, HuggingfaceModelHub] = Field(
         ...,
         description="+docs=Specify the model to be deployed\n+sort=2\n+label=Model to deploy",
     )
+    env: Optional[Dict[str, str]] = Field(
+        None,
+        description="+label=Environment Variables\n+usage=Configure environment variables to be injected in the service. [Docs](https://docs.truefoundry.com/docs/env-variables)\n+icon=fa-globe\n+sort=3",
+    )
+    endpoint: Optional[Endpoint] = None
+    grpc: bool = Field(False, description="+docs=Use grpc\n+sort=5\n+label=Use gRPC")
     resources: Optional[Resources] = None
-    grpc: bool = Field(False, description="+docs=Use grpc\n+sort=4\n+label=Use gRPC")
+    replicas: conint(ge=0, le=20) = Field(
+        1,
+        description="+label=Replicas\n+usage=Replicas of service you want to run\n+icon=fa-clone\n+sort=7",
+    )
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
 
 
 class Service(BaseModel):
     """
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/__init__.py` & `servicefoundry-0.9.4/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.9.4/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.9.4/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py` & `servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py` & `servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.9.4/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/builder/docker_service.py` & `servicefoundry-0.9.4/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/cli_main.py` & `servicefoundry-0.9.4/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/get_command.py`

 * *Files 17% similar despite different names*

```diff
@@ -89,12 +89,41 @@
     version = version_lib.get_version(application_fqn=application_fqn, version=version)
     if CliConfig.get("json"):
         print_json(data=version.dict())
     else:
         print_entity_obj("Version", version)
 
 
+@click.command(name="job-run", cls=COMMAND_CLS, help="Get Job Run")
+@click.option(
+    "--application-fqn",
+    "--application_fqn",
+    type=click.STRING,
+    default=None,
+    help="FQN of the application",
+    required=True,
+)
+@click.option(
+    "--job-run-name",
+    "--job_run_name",
+    type=click.STRING,
+    default=None,
+    help="Run name of the job",
+    required=True,
+)
+@handle_exception_wrapper
+def get_job_run(application_fqn, job_run_name):
+    job_run = application_lib.get_job_run(
+        application_fqn=application_fqn, job_run_name=job_run_name
+    )
+    if CliConfig.get("json"):
+        print_json(data=job_run.dict())
+    else:
+        print_entity_obj("Job Run", job_run)
+
+
 def get_get_command():
     get_command.add_command(get_workspace)
     get_command.add_command(get_application)
     get_command.add_command(get_version)
+    get_command.add_command(get_job_run)
     return get_command
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/list_command.py`

 * *Files 13% similar despite different names*

```diff
@@ -125,13 +125,47 @@
 
     print_entity_list(
         "Application Versions",
         versions,
     )
 
 
+@click.command(name="job-run", cls=COMMAND_CLS, help="List Job Runs")
+@click.option(
+    "--application-fqn",
+    "--application_fqn",
+    type=click.STRING,
+    default=None,
+    help="FQN of the application",
+    required=True,
+)
+@click.option(
+    "--max-results",
+    "--max_results",
+    type=click.STRING,
+    default=None,
+    help="Maximum number of Runs to fetch",
+)
+@click.option(
+    "--offset",
+    type=click.STRING,
+    default=None,
+    help="Number of Runs to skip",
+)
+@handle_exception_wrapper
+def list_job_runs(application_fqn, max_results, offset):
+    job_runs = application_lib.list_job_runs(
+        application_fqn=application_fqn, max_results=max_results, offset=offset
+    )
+    if CliConfig.get("json"):
+        print_json(data=job_runs.dict())
+    else:
+        print_entity_list("Job Runs", job_runs)
+
+
 def get_list_command():
     list_command.add_command(list_workspaces)
     list_command.add_command(list_applications)
     list_command.add_command(list_versions)
+    list_command.add_command(list_job_runs)
 
     return list_command
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/logs_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 @click.option(
     "--application-fqn",
     type=click.STRING,
     help="FQN of the application",
     required=True,
 )
 @click.option(
+    "--job-run-name",
+    "--job_run_name",
+    type=click.STRING,
+    default=None,
+    help="Run name of the job (if application is a job)",
+)
+@click.option(
     "--version",
     type=click.INT,
     help="Version number of the application deployment",
     default=None,
 )
 @click.option(
     "--since",
@@ -43,14 +50,15 @@
 @click.option(
     "-n", "--tail", type=click.INT, help="Number of logs to tail", default=None
 )
 @click.option("-f", "--follow", help="Follow log output", is_flag=True, default=False)
 @handle_exception_wrapper
 def logs_command(
     application_fqn: str,
+    job_run_name: Optional[str],
     version: Optional[int],
     since: str,
     until: Optional[str],
     tail: Optional[int],
     follow: bool,
 ) -> None:
     """
@@ -99,24 +107,26 @@
         )
 
     if until or not follow:
         tfs_client.fetch_deployment_logs(
             workspace_id=workspace_id,
             application_id=application_id,
             deployment_id=deployment_id,
+            job_run_name=job_run_name,
             start_ts=start_ts,
             end_ts=end_ts,
             limit=tail,
             callback=output_hook,
         )
     else:
         tfs_client.poll_logs_for_deployment(
             workspace_id=workspace_id,
             application_id=application_id,
             deployment_id=deployment_id,
+            job_run_name=job_run_name,
             start_ts=start_ts,
             limit=tail,
             poll_interval_seconds=5,
             callback=output_hook,
         )
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.9.4/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/cli/util.py` & `servicefoundry-0.9.4/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/__main__.py` & `servicefoundry-0.9.4/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/app.py` & `servicefoundry-0.9.4/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/build.py` & `servicefoundry-0.9.4/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.9.4/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.9.4/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.9.4/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/route.py` & `servicefoundry-0.9.4/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/service.py` & `servicefoundry-0.9.4/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/function_service/utils.py` & `servicefoundry-0.9.4/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/internal/experimental.py` & `servicefoundry-0.9.4/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/io/output_callback.py` & `servicefoundry-0.9.4/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.9.4/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.9.4/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.9.4/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.9.4/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.9.4/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.9.4/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.9.4/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.9.4/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.9.4/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from servicefoundry.lib.clients.utils import request_handling
 from servicefoundry.lib.const import API_SERVER_RELATIVE_PATH, VERSION_PREFIX
 from servicefoundry.lib.model.entity import (
     Application,
     CreateDockerRepositoryResponse,
     Deployment,
     DockerRegistryCredentials,
+    JobRun,
     TenantInfo,
     Token,
     TriggerJobResult,
     Workspace,
     WorkspaceResources,
 )
 from servicefoundry.lib.win32 import allow_interrupt
@@ -360,14 +361,15 @@
         return parse_obj_as(List[BuildResponse], res)
 
     def _get_deployment_logs(
         self,
         workspace_id: str,
         application_id: str,
         deployment_id: str,
+        job_run_name: Optional[str] = None,
         start_ts_nano: Optional[int] = None,
         end_ts_nano: Optional[int] = None,
         limit: Optional[int] = None,
         num_logs_to_ignore: Optional[int] = None,
     ) -> List:
         get_logs_query = {"applicationId": application_id}
         if deployment_id:
@@ -377,14 +379,16 @@
             data["startTs"] = str(start_ts_nano)
         if end_ts_nano:
             data["endTs"] = str(end_ts_nano)
         if limit:
             data["limit"] = str(limit)
         if num_logs_to_ignore:
             data["numLogsToIgnore"] = int(num_logs_to_ignore)
+        if job_run_name:
+            data["jobRunName"] = job_run_name
 
         url = f"{self._api_server_url}/{VERSION_PREFIX}/logs/{workspace_id}"
         res = requests.get(url=url, params=data, headers=self._get_header())
         res = request_handling(res)
         return list(res["logs"])
 
     @check_min_cli_version
@@ -438,14 +442,15 @@
 
     @check_min_cli_version
     def poll_logs_for_deployment(
         self,
         workspace_id: str,
         application_id: str,
         deployment_id: str,
+        job_run_name: Optional[str],
         start_ts: int,
         limit: int,
         poll_interval_seconds: int,
         callback=OutputCallBack(),
     ):
         start_ts_nano = int(start_ts * 1e6)
 
@@ -453,14 +458,15 @@
             num_logs_to_ignore = 0
 
             while True:
                 logs_list = self._get_deployment_logs(
                     workspace_id=workspace_id,
                     application_id=application_id,
                     deployment_id=deployment_id,
+                    job_run_name=job_run_name,
                     start_ts_nano=start_ts_nano,
                     limit=limit,
                     num_logs_to_ignore=num_logs_to_ignore,
                 )
 
                 if len(logs_list) == 0:
                     logger.warning("Did not receive any logs")
@@ -483,23 +489,25 @@
 
     @check_min_cli_version
     def fetch_deployment_logs(
         self,
         workspace_id: str,
         application_id: str,
         deployment_id: str,
+        job_run_name: Optional[str],
         start_ts: Optional[int],
         end_ts: Optional[int],
         limit: Optional[int],
         callback=OutputCallBack(),
     ):
         logs_list = self._get_deployment_logs(
             workspace_id=workspace_id,
             application_id=application_id,
             deployment_id=deployment_id,
+            job_run_name=job_run_name,
             start_ts_nano=int(start_ts * 1e6),
             end_ts_nano=int(end_ts * 1e6),
             limit=limit,
         )
         for log in logs_list:
             callback.print_line(self._get_log_print_line(log))
 
@@ -559,14 +567,43 @@
             url,
             headers=self._get_header(),
             json={"manifest": infra_manifest},
         )
         response = request_handling(res)
         return response
 
+    def list_job_runs(
+        self,
+        application_id: str,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        search_prefix: Optional[str] = None,
+    ) -> List[JobRun]:
+        url = f"{self._api_server_url}/{VERSION_PREFIX}/jobs/{application_id}/runs"
+        params = {}
+        if limit:
+            params["limit"] = limit
+        if offset:
+            params["offset"] = offset
+        if search_prefix:
+            params["searchPrefix"] = search_prefix
+        res = requests.get(url, headers=self._get_header(), params=params)
+        res = request_handling(res)
+        return parse_obj_as(List[JobRun], res["data"])
+
+    def get_job_run(
+        self,
+        application_id: str,
+        job_run_name: str,
+    ):
+        url = f"{self._api_server_url}/{VERSION_PREFIX}/jobs/{application_id}/runs/{job_run_name}"
+        res = requests.get(url, headers=self._get_header())
+        res = request_handling(res)
+        return parse_obj_as(JobRun, res)
+
     def trigger_job(
         self,
         deployment_id: str,
         component_name: str,
         command: Optional[str] = None,
         params: Optional[Dict[str, str]] = None,
     ) -> TriggerJobResult:
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.9.4/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.9.4/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.9.4/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.9.4/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.9.4/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.9.4/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/const.py` & `servicefoundry-0.9.4/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/dao/application.py` & `servicefoundry-0.9.4/servicefoundry/lib/dao/application.py`

 * *Files 17% similar despite different names*

```diff
@@ -74,14 +74,41 @@
     workspace_fqn = application_info.workspace.fqn
 
     application = Application.parse_obj(manifest)
     deployment = application.deploy(workspace_fqn=workspace_fqn, wait=wait)
     return deployment
 
 
+def list_job_runs(
+    application_fqn: str,
+    max_results: Optional[int] = None,
+    offset: Optional[int] = None,
+    client: Optional[ServiceFoundryServiceClient] = None,
+):
+    client = client or ServiceFoundryServiceClient()
+    application = client.get_id_from_fqn(fqn=application_fqn, fqn_type="app")
+    response = client.list_job_runs(
+        application_id=application["applicationId"], limit=max_results, offset=offset
+    )
+    return response
+
+
+def get_job_run(
+    application_fqn: str,
+    job_run_name: str,
+    client: Optional[ServiceFoundryServiceClient] = None,
+):
+    client = client or ServiceFoundryServiceClient()
+    application = client.get_id_from_fqn(fqn=application_fqn, fqn_type="app")
+    response = client.get_job_run(
+        application_id=application["applicationId"], job_run_name=job_run_name
+    )
+    return response
+
+
 def trigger_job(
     application_fqn: str,
     command: Optional[Union[str, Sequence[str]]] = None,
     params: Optional[Dict[str, str]] = None,
 ) -> TriggerJobResult:
     """
     Trigger a Job on Truefoundry platform
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/dao/version.py` & `servicefoundry-0.9.4/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.9.4/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/exceptions.py` & `servicefoundry-0.9.4/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.9.4/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.9.4/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.9.4/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.9.4/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.9.4/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.9.4/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/messages.py` & `servicefoundry-0.9.4/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/model/entity.py` & `servicefoundry-0.9.4/servicefoundry/lib/model/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -294,14 +294,65 @@
         allow_population_by_field_name = True
         allow_mutation = False
 
     def get_user_clickable_url(self, auth_host: str) -> str:
         return f"{auth_host}/authorize/device?userCode={self.user_code}"
 
 
+class JobRun(Base):
+    name: str
+    applicationName: str
+    deploymentVersion: int
+    createdAt: int
+    endTime: Optional[int] = None
+    duration: Optional[str] = None
+    command: str
+    totalRetries: Optional[int] = 0
+    status: str
+
+    def list_row_data(self) -> Dict[str, Any]:
+        from servicefoundry.cli.display_util import display_time_passed
+
+        triggered_at = (
+            (datetime.datetime.now().timestamp() * 1000) - self.createdAt
+        ) // 1000
+        triggered_at = f"{display_time_passed(triggered_at)} ago"
+        duration = ""
+        if self.duration:
+            duration = display_time_passed(int(float(self.duration)))
+        return {
+            "name": self.name,
+            "deployment_version": self.deploymentVersion,
+            "status": self.status,
+            "triggered_at": triggered_at,
+            "duration": duration,
+        }
+
+    def get_data(self) -> Dict[str, Any]:
+        from servicefoundry.cli.display_util import display_time_passed
+
+        created_at = datetime.datetime.fromtimestamp(self.createdAt // 1000)
+        end_time = ""
+        if self.endTime:
+            end_time = datetime.datetime.fromtimestamp(self.endTime // 1000)
+        duration = ""
+        if self.duration:
+            duration = display_time_passed(int(float(self.duration)))
+        return {
+            "name": self.name,
+            "application_name": self.applicationName,
+            "deployment_version": self.deploymentVersion,
+            "created_at": created_at,
+            "end_time": end_time,
+            "duration": duration,
+            "command": self.command,
+            "status": self.status,
+        }
+
+
 class TriggerJobResult(Base):
     message: str = Field(default="Unknown")
     jobRunName: str = Field(default=None)
 
 
 class DockerRegistryCredentials(Base):
     fqn: str
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/session.py` & `servicefoundry-0.9.4/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/util.py` & `servicefoundry-0.9.4/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/lib/win32.py` & `servicefoundry-0.9.4/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/logger.py` & `servicefoundry-0.9.4/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.9.4/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.9.4/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.9.4/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.9.4/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.9.4/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.9.4/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.9.4/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/lib/models.py` & `servicefoundry-0.9.4/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.9.4/servicefoundry/v2/lib/patched_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,7 +233,12 @@
 
 
 class NodepoolSelector(models.NodepoolSelector):
     class Config:
         extra = "forbid"
 
     type: Literal["nodepool_selector"] = "nodepool_selector"
+
+
+class Endpoint(models.Endpoint):
+    class Config:
+        extra = "forbid"
```

### Comparing `servicefoundry-0.9.3rc1/servicefoundry/v2/lib/source.py` & `servicefoundry-0.9.4/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.3rc1/PKG-INFO` & `servicefoundry-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.9.3rc1
+Version: 0.9.4
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

