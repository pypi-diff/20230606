# Comparing `tmp/open-autonomy-0.9.0.tar.gz` & `tmp/open-autonomy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-autonomy-0.9.0.tar", last modified: Fri Feb 17 11:45:28 2023, max compression
+gzip compressed data, was "open-autonomy-0.9.1.tar", last modified: Thu Feb 23 16:08:23 2023, max compression
```

## Comparing `open-autonomy-0.9.0.tar` & `open-autonomy-0.9.1.tar`

### file list

```diff
@@ -1,1271 +1,1271 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.034167 open-autonomy-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    28535 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-02-17 11:45:28.034167 open-autonomy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.630160 open-autonomy-0.9.0/autonomy/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.634160 open-autonomy-0.9.0/autonomy/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.634160 open-autonomy-0.9.0/autonomy/analyse/abci/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/abci/app_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/abci/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/abci/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.638160 open-autonomy-0.9.0/autonomy/analyse/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/benchmark/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/benchmark/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.638160 open-autonomy-0.9.0/autonomy/analyse/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/logs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/logs/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/logs/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    17209 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/analyse/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.642160 open-autonomy-0.9.0/autonomy/chain/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/mint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/chain/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.646160 open-autonomy-0.9.0/autonomy/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12891 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/build_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.658161 open-autonomy-0.9.0/autonomy/cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/fsm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/ipfs_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/helpers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/mint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/push_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/scaffold_fsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.658161 open-autonomy-0.9.0/autonomy/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/cli/utils/click_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.662161 open-autonomy-0.9.0/autonomy/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/configurations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/configurations/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/configurations/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.662161 open-autonomy-0.9.0/autonomy/configurations/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/configurations/schemas/fsm_specification_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/configurations/schemas/service_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/configurations/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.662161 open-autonomy-0.9.0/autonomy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.518158 open-autonomy-0.9.0/autonomy/data/Dockerfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.662161 open-autonomy-0.9.0/autonomy/data/Dockerfiles/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/agent/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/agent/install.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/agent/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.666161 open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/openssl.cnf
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/start.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1123 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/start_dev.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.666161 open-autonomy-0.9.0/autonomy/data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/data/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.666161 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.666161 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/build/
--rw-r--r--   0 runner    (1001) docker     (123)    84073 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/build/AgentRegistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.666161 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.670161 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.670161 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/build/
--rw-r--r--   0 runner    (1001) docker     (123)    79782 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/build/ComponentRegistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.670161 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/component_registry/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.670161 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.670161 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/build/
--rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/build/RegistriesManager.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.674161 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.674161 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.674161 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/build/
--rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/build/ServiceManager.json
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.678161 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_manager/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.686161 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.686161 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/build/
--rw-r--r--   0 runner    (1001) docker     (123)   141766 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/build/ServiceRegistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.686161 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-02-17 11:45:26.000000 open-autonomy-0.9.0/autonomy/data/contracts/service_registry/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.686161 open-autonomy-0.9.0/autonomy/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.690161 open-autonomy-0.9.0/autonomy/deploy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.690161 open-autonomy-0.9.0/autonomy/deploy/generators/docker_compose/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/generators/docker_compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/generators/docker_compose/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/generators/docker_compose/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.690161 open-autonomy-0.9.0/autonomy/deploy/generators/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/generators/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/generators/kubernetes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/generators/kubernetes/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/deploy/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.690161 open-autonomy-0.9.0/autonomy/fsm/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.694161 open-autonomy-0.9.0/autonomy/fsm/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.694161 open-autonomy-0.9.0/autonomy/fsm/scaffold/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/generators/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/generators/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/scaffold_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.694161 open-autonomy-0.9.0/autonomy/fsm/scaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/templates/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/fsm/scaffold/templates/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.706161 open-autonomy-0.9.0/autonomy/replay/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/replay/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/replay/tendermint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/replay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.706161 open-autonomy-0.9.0/autonomy/services/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.706161 open-autonomy-0.9.0/autonomy/services/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/services/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/autonomy/services/scaffold/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.538159 open-autonomy-0.9.0/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.538159 open-autonomy-0.9.0/deployments/Dockerfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.706161 open-autonomy-0.9.0/deployments/Dockerfiles/autonomy/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/autonomy/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/autonomy/openssl.cnf
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/autonomy/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.706161 open-autonomy-0.9.0/deployments/Dockerfiles/autonomy-user/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/autonomy-user/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/autonomy-user/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.706161 open-autonomy-0.9.0/deployments/Dockerfiles/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/documentation/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.710162 open-autonomy-0.9.0/deployments/Dockerfiles/hardhat/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/hardhat/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.714161 open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/config-template.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/tendermint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/wait-for-it.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/wrapper.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.714161 open-autonomy-0.9.0/deployments/keys/
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/deployments/keys/hardhat_keys.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.730162 open-autonomy-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.730162 open-autonomy-0.9.0/docs/advanced_reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.734162 open-autonomy-0.9.0/docs/advanced_reference/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_analyse.md
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_build-image.md
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_deploy.md
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_fetch.md
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_mint.md
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_replay.md
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_scaffold.md
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_service.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.734162 open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/benchmarking.md
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/debugging_in_the_cluster.md
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/dev_mode.md
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/execution_replay.md
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/log_analysis.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/advanced_reference/use_custom_images.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.734162 open-autonomy-0.9.0/docs/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.734162 open-autonomy-0.9.0/docs/api/analyse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.738162 open-autonomy-0.9.0/docs/api/analyse/abci/
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/abci/app_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/abci/docstrings.md
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/abci/logs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.738162 open-autonomy-0.9.0/docs/api/analyse/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/benchmark/aggregate.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/benchmark/html.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/constants.md
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/dialogues.md
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/handlers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.738162 open-autonomy-0.9.0/docs/api/analyse/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/logs/base.md
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/logs/collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/logs/db.md
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/analyse/service.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.742162 open-autonomy-0.9.0/docs/api/chain/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/base.md
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/config.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/constants.md
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/metadata.md
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/mint.md
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/service.md
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/chain/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.746162 open-autonomy-0.9.0/docs/api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/analyse.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/build_images.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/core.md
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/deploy.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/fetch.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/hash.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.758162 open-autonomy-0.9.0/docs/api/cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/helpers/analyse.md
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/helpers/chain.md
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/helpers/deployment.md
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/helpers/docstring.md
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/helpers/fsm_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/helpers/ipfs_hash.md
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/helpers/registry.md
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/mint.md
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/packages.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/publish.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/push_all.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/replay.md
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/scaffold_fsm.md
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/service.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.758162 open-autonomy-0.9.0/docs/api/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/cli/utils/click_utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.758162 open-autonomy-0.9.0/docs/api/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/configurations/base.md
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/configurations/constants.md
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/configurations/loader.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/configurations/validation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.542159 open-autonomy-0.9.0/docs/api/connections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.762162 open-autonomy-0.9.0/docs/api/connections/abci/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/check_dependencies.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/connection.md
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/dialogues.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.762162 open-autonomy-0.9.0/docs/api/connections/abci/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/scripts/genproto.md
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tendermint_decoder.md
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tendermint_encoder.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.762162 open-autonomy-0.9.0/docs/api/connections/abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tests/helper.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/base.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/mock_node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/base.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/grpc_channel.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/tcp_channel.md
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/mock_node/node.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/constants.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.546159 open-autonomy-0.9.0/docs/api/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/contracts/gnosis_safe/
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/contracts/gnosis_safe/contract.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/contracts/gnosis_safe_proxy_factory/
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/contracts/gnosis_safe_proxy_factory/contract.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.546159 open-autonomy-0.9.0/docs/api/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.550159 open-autonomy-0.9.0/docs/api/data/Dockerfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/data/Dockerfiles/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/data/Dockerfiles/dev/watcher.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/base.md
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/build.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/constants.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.550159 open-autonomy-0.9.0/docs/api/deploy/generators/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/deploy/generators/docker_compose/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/generators/docker_compose/base.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/generators/docker_compose/templates.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/deploy/generators/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/generators/kubernetes/base.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/generators/kubernetes/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/deploy/image.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.550159 open-autonomy-0.9.0/docs/api/fsm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/fsm/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/fsm/scaffold/base.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/fsm/scaffold/constants.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/fsm/scaffold/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/fsm/scaffold/generators/components.md
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/fsm/scaffold/generators/tests.md
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/fsm/scaffold/scaffold_skill.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/fsm/scaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/fsm/scaffold/templates/components.md
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/fsm/scaffold/templates/tests.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.550159 open-autonomy-0.9.0/docs/api/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/base_test_classes/
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/base_test_classes/agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/base_test_classes/contracts.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/configurations.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.766162 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/acn_node.md
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/amm_net.md
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/base.md
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/ganache.md
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/gnosis_safe_net.md
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/registries.md
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/tendermint.md
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/fixture_helpers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.778163 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/async_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/base.md
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/contracts.md
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/tendermint_utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.554159 open-autonomy-0.9.0/docs/api/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.778163 open-autonomy-0.9.0/docs/api/protocols/abci/
--rw-r--r--   0 runner    (1001) docker     (123)    54108 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/protocols/abci/custom_types.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/protocols/abci/dialogues.md
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/protocols/abci/message.md
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/protocols/abci/serialization.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.782163 open-autonomy-0.9.0/docs/api/replay/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/replay/agent.md
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/replay/tendermint.md
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/replay/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.562159 open-autonomy-0.9.0/docs/api/skills/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.782163 open-autonomy-0.9.0/docs/api/skills/abstract_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_abci/dialogues.md
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_abci/handlers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.786163 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/abci_app_chain.md
--rw-r--r--   0 runner    (1001) docker     (123)    64335 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/base.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/behaviour_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/behaviours.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/common.md
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/dialogues.md
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/handlers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.786163 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/ipfs.md
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/load.md
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/paths.md
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/store.md
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/models.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.786163 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/abci_app.md
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/base.md
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/common.md
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/integration.md
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/rounds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.562159 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.562159 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.790163 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/dialogues.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/handlers.md
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/models.md
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/payloads.md
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/rounds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.790163 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/test_tools/base.md
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.802163 open-autonomy-0.9.0/docs/api/skills/registration_abci/
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/registration_abci/behaviours.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/registration_abci/dialogues.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/registration_abci/handlers.md
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/registration_abci/models.md
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/registration_abci/payloads.md
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/registration_abci/rounds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.802163 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/behaviours.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/dialogues.md
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/handlers.md
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/models.md
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/payload_tools.md
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/payloads.md
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/rounds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.806163 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/test_tools/integration.md
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/application_deployment.md
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/control_flow.md
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/counter_example.md
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/debugging.md
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/delegate_call.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.806163 open-autonomy-0.9.0/docs/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/demos/hello_world_demo.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/demos/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    33346 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/demos/price_oracle_fsms.md
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/demos/price_oracle_intro.md
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/demos/price_oracle_technical_details.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.806163 open-autonomy-0.9.0/docs/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/deployment/on-chain_deployment_checklist.md
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/ethereum_specifics.md
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/exceptions.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.566159 open-autonomy-0.9.0/docs/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.810163 open-autonomy-0.9.0/docs/fonts/Manrope/
--rw-r--r--   0 runner    (1001) docker     (123)    96364 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    97116 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96304 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96312 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96492 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96412 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96528 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/fonts/Manrope/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.810163 open-autonomy-0.9.0/docs/get_started/
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/get_started/agent_services_compared_to.md
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/get_started/use_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/get_started/what_is_an_agent_service.md
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/get_started/why_do_we_need_agent_services.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.818163 open-autonomy-0.9.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/configure_access_external_chains.md
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/create_fsm_app.md
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/create_service_existing_agent.md
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/create_service_from_scratch.md
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/deploy_service.md
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/overview_of_the_development_process.md
--rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/publish_fetch_packages.md
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/register_packages_on_chain.md
--rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/service_configuration_file.md
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/guides/set_up.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.846164 open-autonomy-0.9.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/abci_requests.svg
--rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/agent_service_architecture.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/agent_service_index_page.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22210 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/centralized_decentralized_world.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/counter_diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/development-process-simplified.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46903 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/development_process.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46831 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/development_process_create_fsm_app.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46776 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/development_process_create_service_existing_agent.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45719 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/development_process_define_service.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/development_process_publish_fetch_packages.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45825 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/development_process_register_packages_on_chain.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/do_name_servers.png
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/fsm.svg
--rw-r--r--   0 runner    (1001) docker     (123)    50819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/fsm_composition.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/fsm_composition_2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29965 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_action.svg
--rw-r--r--   0 runner    (1001) docker     (123)    40598 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_agent_internal.svg
--rw-r--r--   0 runner    (1001) docker     (123)    54165 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_demo_architecture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_demo_architecture_simplified.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_fsm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_result.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_sequence_1.svg
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_sequence_2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_sequence_3.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_sequence_4.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_sequence_5.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15072 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/hello_world_zoom_agent.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113949 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/name_server_setup.png
--rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/networking_page.png
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/open-autonomy-framework-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/oracle_composition.svg
--rw-r--r--   0 runner    (1001) docker     (123)    42238 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/oracle_diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/package_management.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/register_package.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/service-level_overrides.svg
--rw-r--r--   0 runner    (1001) docker     (123)    54123 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/simple_demo_architecture.svg
--rw-r--r--   0 runner    (1001) docker     (123)    55927 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/simplified-aea.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/skill-components.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/tendermint.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25496 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/images/tendermint_transaction.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.850164 open-autonomy-0.9.0/docs/key_concepts/
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/abci.md
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/abci_app_abstract_round.md
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/abci_app_abstract_round_behaviour.md
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/abci_app_async_behaviour.md
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/abci_app_class.md
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/abci_app_interactions.md
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/aea.md
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/fsm.md
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/fsm_app_components.md
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/fsm_app_introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/poc-diagram.md
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/key_concepts/threat_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/package_list.md
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/questions-and-answers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.850164 open-autonomy-0.9.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/upgrading.md
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/using_stack_deployment.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/docs/version.md
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.854164 open-autonomy-0.9.0/open_autonomy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-02-17 11:45:27.000000 open-autonomy-0.9.0/open_autonomy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49373 2023-02-17 11:45:27.000000 open-autonomy-0.9.0/open_autonomy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:45:27.000000 open-autonomy-0.9.0/open_autonomy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-17 11:45:27.000000 open-autonomy-0.9.0/open_autonomy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:45:27.000000 open-autonomy-0.9.0/open_autonomy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-17 11:45:27.000000 open-autonomy-0.9.0/open_autonomy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-17 11:45:27.000000 open-autonomy-0.9.0/open_autonomy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.854164 open-autonomy-0.9.0/packages/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/packages.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.854164 open-autonomy-0.9.0/packages/valory/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.854164 open-autonomy-0.9.0/packages/valory/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.858164 open-autonomy-0.9.0/packages/valory/agents/abstract_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/abstract_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/abstract_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/abstract_abci/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.858164 open-autonomy-0.9.0/packages/valory/agents/abstract_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/abstract_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/abstract_abci/tests/test_abstract_abci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.858164 open-autonomy-0.9.0/packages/valory/agents/counter/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/counter/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/counter/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.858164 open-autonomy-0.9.0/packages/valory/agents/counter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/counter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/counter/tests/test_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.862164 open-autonomy-0.9.0/packages/valory/agents/counter_client/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/counter_client/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/counter_client/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.862164 open-autonomy-0.9.0/packages/valory/agents/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/hello_world/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/hello_world/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.862164 open-autonomy-0.9.0/packages/valory/agents/hello_world/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/hello_world/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/hello_world/tests/test_hello_world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.862164 open-autonomy-0.9.0/packages/valory/agents/register_reset/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.866164 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.866164 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.866164 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/docker/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.870164 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/config-template.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/tendermint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/wrapper.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/test_hard_reset_race_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/test_register_reset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.870164 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.870164 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/tests/test_register_reset_recovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.874164 open-autonomy-0.9.0/packages/valory/agents/register_termination/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_termination/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_termination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_termination/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.874164 open-autonomy-0.9.0/packages/valory/agents/register_termination/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_termination/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_termination/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/register_termination/tests/test_register_reset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.874164 open-autonomy-0.9.0/packages/valory/agents/registration_start_up/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/registration_start_up/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/registration_start_up/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/registration_start_up/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.874164 open-autonomy-0.9.0/packages/valory/agents/registration_start_up/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/registration_start_up/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/registration_start_up/tests/test_registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.878164 open-autonomy-0.9.0/packages/valory/agents/test_abci/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/test_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/test_abci/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.878164 open-autonomy-0.9.0/packages/valory/agents/test_ipfs/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/test_ipfs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/test_ipfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/test_ipfs/aea-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.878164 open-autonomy-0.9.0/packages/valory/agents/test_ipfs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/test_ipfs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/agents/test_ipfs/tests/test_ipfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.878164 open-autonomy-0.9.0/packages/valory/connections/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.882164 open-autonomy-0.9.0/packages/valory/connections/abci/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    53091 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/connection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/dialogues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.882164 open-autonomy-0.9.0/packages/valory/connections/abci/gogoproto/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/gogoproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56837 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/gogoproto/gogo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.570159 open-autonomy-0.9.0/packages/valory/connections/abci/protos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.886164 open-autonomy-0.9.0/packages/valory/connections/abci/protos/gogoproto/
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/gogoproto/gogo.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.570159 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.886164 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/abci/
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/abci/types.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.886164 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/crypto/keys.proto
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/crypto/proof.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.886164 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/types/params.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/types/types.proto
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/types/validator.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.886164 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/version/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/version/types.proto
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.886164 open-autonomy-0.9.0/packages/valory/connections/abci/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/scripts/genproto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.886164 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.890164 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/abci/
--rw-r--r--   0 runner    (1001) docker     (123)   167050 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/abci/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26712 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/abci/types_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.890164 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/crypto/keys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/crypto/proof_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.890164 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/types/
--rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/types/params_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57736 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/types/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/types/validator_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.890164 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/version/
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/version/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tendermint_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.894164 open-autonomy-0.9.0/packages/valory/connections/abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_abci.py
--rw-r--r--   0 runner    (1001) docker     (123)    11835 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_abci_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_abci_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.894164 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.894164 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/grpc_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/tcp_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17798 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_tendermint_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_tendermint_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/abci/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/connections/ipfs/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/ipfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/ipfs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/ipfs/connection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/ipfs/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/connections/ipfs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/ipfs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/connections/ipfs/tests/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/build/
--rw-r--r--   0 runner    (1001) docker     (123)    84073 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/build/AgentRegistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/agent_registry/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/component_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/component_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/component_registry/build/
--rw-r--r--   0 runner    (1001) docker     (123)    79782 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/component_registry/build/ComponentRegistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/component_registry/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/component_registry/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/component_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/component_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/component_registry/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.898165 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/build/
--rw-r--r--   0 runner    (1001) docker     (123)   122983 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/build/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    38396 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.902165 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32033 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.906165 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.906165 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/build/
--rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/build/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.906165 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.906165 open-autonomy-0.9.0/packages/valory/contracts/multicall2/
--rwxr-xr-x   0 runner    (1001) docker     (123)      925 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multicall2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.906165 open-autonomy-0.9.0/packages/valory/contracts/multicall2/build/
--rwxr-xr-x   0 runner    (1001) docker     (123)    17861 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multicall2/build/multicall2.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5408 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multicall2/contract.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multicall2/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.910165 open-autonomy-0.9.0/packages/valory/contracts/multicall2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multicall2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multicall2/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.910165 open-autonomy-0.9.0/packages/valory/contracts/multisend/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multisend/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multisend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.910165 open-autonomy-0.9.0/packages/valory/contracts/multisend/build/
--rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multisend/build/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multisend/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multisend/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.910165 open-autonomy-0.9.0/packages/valory/contracts/multisend/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multisend/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/multisend/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.914165 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.914165 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/build/
--rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/build/RegistriesManager.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.914165 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/registries_manager/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.914165 open-autonomy-0.9.0/packages/valory/contracts/service_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.914165 open-autonomy-0.9.0/packages/valory/contracts/service_manager/build/
--rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_manager/build/ServiceManager.json
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_manager/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_manager/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.914165 open-autonomy-0.9.0/packages/valory/contracts/service_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_manager/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.918165 open-autonomy-0.9.0/packages/valory/contracts/service_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.918165 open-autonomy-0.9.0/packages/valory/contracts/service_registry/build/
--rw-r--r--   0 runner    (1001) docker     (123)   141766 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_registry/build/ServiceRegistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_registry/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_registry/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.918165 open-autonomy-0.9.0/packages/valory/contracts/service_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/contracts/service_registry/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.918165 open-autonomy-0.9.0/packages/valory/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.926165 open-autonomy-0.9.0/packages/valory/protocols/abci/
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/abci.proto
--rw-r--r--   0 runner    (1001) docker     (123)    61490 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/abci_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    70004 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)    52109 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33035 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.926165 open-autonomy-0.9.0/packages/valory/protocols/abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    30458 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/tests/test_abci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/tests/test_abci_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/abci/tests/test_abci_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.930165 open-autonomy-0.9.0/packages/valory/protocols/ipfs/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/ipfs.proto
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/ipfs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.930165 open-autonomy-0.9.0/packages/valory/protocols/ipfs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/tests/test_ipfs_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/ipfs/tests/test_ipfs_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.934165 open-autonomy-0.9.0/packages/valory/protocols/tendermint/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/tendermint.proto
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/tendermint_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.938165 open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/test_tendermint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/test_tendermint_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/test_tendermint_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.594159 open-autonomy-0.9.0/packages/valory/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.938165 open-autonomy-0.9.0/packages/valory/services/counter/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/services/counter/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/services/counter/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.938165 open-autonomy-0.9.0/packages/valory/services/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/services/hello_world/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/services/hello_world/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.938165 open-autonomy-0.9.0/packages/valory/services/register_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/services/register_reset/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/services/register_reset/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.942165 open-autonomy-0.9.0/packages/valory/skills/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.942165 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.942165 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_abci/tests/test_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.962166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/abci_app_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)   110959 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    91028 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/behaviour_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)    30368 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.962166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.966166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/abci_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.978166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.978166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.982166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/skill.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_abci_app_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    89395 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_base_rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)    92972 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_behaviours_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)    23074 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.982166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/test_ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/test_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    26092 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.982166 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.986166 open-autonomy-0.9.0/packages/valory/skills/counter/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.986166 open-autonomy-0.9.0/packages/valory/skills/counter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter/tests/test_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.990166 open-autonomy-0.9.0/packages/valory/skills/counter_client/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.990166 open-autonomy-0.9.0/packages/valory/skills/counter_client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/counter_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.994166 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/fsm_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.994166 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.998166 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/fsm_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.998166 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.002166 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.002166 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.006166 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.006166 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.006166 open-autonomy-0.9.0/packages/valory/skills/registration_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/fsm_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.010167 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24376 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.010167 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/fsm_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.010167 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.010167 open-autonomy-0.9.0/packages/valory/skills/termination_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.014166 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25882 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.014166 open-autonomy-0.9.0/packages/valory/skills/test_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.014166 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.014166 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/fsm_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.018167 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.018167 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35977 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/fsm_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/payload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    31996 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/rounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/skill.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.018167 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/test_tools/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.018167 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_payload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    36035 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.018167 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_tools/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/RELEASE_PROCESS.md
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12076 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/check_copyright.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14693 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/check_doc_ipfs_hashes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6805 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/check_doc_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3825 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/check_ipfs_hashes_pushed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1911 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/check_pipfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8212 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/generate_api_documentation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1963 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/generate_package_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/pre-add
--rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/pre-push
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/spell-check.sh
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/scripts/whitelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-02-17 11:45:28.034167 open-autonomy-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.610160 open-autonomy-0.9.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/data/dummy_packages/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.606160 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.606160 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/agents/dummy_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/agents/dummy_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/agents/dummy_agent/aea-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/agents/dummy_agent/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.606160 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.606160 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/contract.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.606160 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.606160 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/services/dummy_service/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/services/dummy_service/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/services/dummy_service/service.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:27.606160 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.022167 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/my_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/skill.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_packages/packages.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/data/dummy_service_config_files/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/data/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/specs/fsm_specification.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/specs/fsm_specification_empty.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/data/specs/fsm_specification_extra.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/test_autonomy/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/test_autonomy/test_chain/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_chain/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_chain/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_chain/test_mint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_chain/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstring_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/test_log_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_check_dialogues.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_check_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_verify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_build_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.026167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_build/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21389 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_build/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_from_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_run_deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_develop/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_develop/test_local_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/test_chain_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/test_fsm_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_mint/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_mint/test_mint_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_push_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_replay/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_replay/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_replay/test_tendermint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_scaffold_fsm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_service/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_service/test_service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_utils/test_click_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_deploy/test_deployment_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_deploy/test_service_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_autonomy/test_images/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_images/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_images/test_autonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_images/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_images/test_tendermint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_package_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_autonomy/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.030167 open-autonomy-0.9.0/tests/test_deployments/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_deployments/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_deployments/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_deployments/test_deployment_code_identical.py
--rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_deployments/test_deployments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.034167 open-autonomy-0.9.0/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_docs/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_docs/test_code_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_docs/test_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:45:28.034167 open-autonomy-0.9.0/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tests/test_scripts/test_check_doc_ipfs_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-02-17 11:45:01.000000 open-autonomy-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.868810 open-autonomy-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28907 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-02-23 16:08:23.868810 open-autonomy-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.296805 open-autonomy-0.9.1/autonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.296805 open-autonomy-0.9.1/autonomy/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.296805 open-autonomy-0.9.1/autonomy/analyse/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/abci/app_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/abci/docstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.296805 open-autonomy-0.9.1/autonomy/analyse/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/benchmark/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/benchmark/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.296805 open-autonomy-0.9.1/autonomy/analyse/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/logs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/logs/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/logs/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17209 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/analyse/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.304805 open-autonomy-0.9.1/autonomy/chain/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/chain/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.304805 open-autonomy-0.9.1/autonomy/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13247 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/build_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/fsm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/ipfs_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/helpers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/push_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/scaffold_fsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/cli/utils/click_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/configurations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/configurations/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/configurations/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/configurations/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/configurations/schemas/fsm_specification_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/configurations/schemas/service_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/configurations/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.216804 open-autonomy-0.9.1/autonomy/data/Dockerfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/data/Dockerfiles/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/agent/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/agent/install.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/agent/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/openssl.cnf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/start.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1123 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/start_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.324805 open-autonomy-0.9.1/autonomy/data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/data/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    84073 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/build/AgentRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    79782 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/build/ComponentRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/component_registry/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/build/RegistriesManager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/build/ServiceManager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.328805 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_manager/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/build/
+-rw-r--r--   0 runner    (1001) docker     (123)   141766 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/build/ServiceRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-02-23 16:08:22.000000 open-autonomy-0.9.1/autonomy/data/contracts/service_registry/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/deploy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/deploy/generators/docker_compose/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/generators/docker_compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/generators/docker_compose/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/generators/docker_compose/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/deploy/generators/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/generators/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/generators/kubernetes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/generators/kubernetes/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/deploy/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/fsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.356805 open-autonomy-0.9.1/autonomy/fsm/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/autonomy/fsm/scaffold/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/generators/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/generators/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/scaffold_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/autonomy/fsm/scaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/templates/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/fsm/scaffold/templates/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/autonomy/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/replay/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/replay/tendermint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/replay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/autonomy/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/autonomy/services/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/services/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/autonomy/services/scaffold/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.232804 open-autonomy-0.9.1/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.232804 open-autonomy-0.9.1/deployments/Dockerfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/deployments/Dockerfiles/autonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/autonomy/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/autonomy/openssl.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/autonomy/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/deployments/Dockerfiles/autonomy-user/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/autonomy-user/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/autonomy-user/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/deployments/Dockerfiles/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/documentation/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/deployments/Dockerfiles/hardhat/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/hardhat/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.360805 open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/config-template.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/tendermint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/wait-for-it.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/wrapper.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.380805 open-autonomy-0.9.1/deployments/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/deployments/keys/hardhat_keys.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.380805 open-autonomy-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.380805 open-autonomy-0.9.1/docs/advanced_reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.384805 open-autonomy-0.9.1/docs/advanced_reference/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_analyse.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_build-image.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_deploy.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_fetch.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_mint.md
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_replay.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_scaffold.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_service.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.384805 open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/benchmarking.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/debugging_in_the_cluster.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/dev_mode.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/execution_replay.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/log_analysis.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/advanced_reference/use_custom_images.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.384805 open-autonomy-0.9.1/docs/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.392805 open-autonomy-0.9.1/docs/api/analyse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.392805 open-autonomy-0.9.1/docs/api/analyse/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/abci/app_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/abci/docstrings.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.392805 open-autonomy-0.9.1/docs/api/analyse/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/benchmark/aggregate.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/benchmark/html.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/constants.md
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/dialogues.md
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/handlers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.392805 open-autonomy-0.9.1/docs/api/analyse/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/logs/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/logs/collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/logs/db.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/analyse/service.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.400806 open-autonomy-0.9.1/docs/api/chain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/constants.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/metadata.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/mint.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/service.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/chain/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.400806 open-autonomy-0.9.1/docs/api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/analyse.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/build_images.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/core.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/deploy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/fetch.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/hash.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.412806 open-autonomy-0.9.1/docs/api/cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/helpers/analyse.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/helpers/chain.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/helpers/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/helpers/docstring.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/helpers/fsm_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/helpers/ipfs_hash.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/helpers/registry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/mint.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/packages.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/publish.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/push_all.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/replay.md
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/scaffold_fsm.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/service.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.412806 open-autonomy-0.9.1/docs/api/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/cli/utils/click_utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.412806 open-autonomy-0.9.1/docs/api/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/configurations/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/configurations/constants.md
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/configurations/loader.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/configurations/validation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.236804 open-autonomy-0.9.1/docs/api/connections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/connections/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/check_dependencies.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/connection.md
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/dialogues.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/connections/abci/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/scripts/genproto.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tendermint_decoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tendermint_encoder.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/connections/abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tests/helper.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/base.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/mock_node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/grpc_channel.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/mock_node/channels/tcp_channel.md
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/mock_node/node.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/constants.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.240804 open-autonomy-0.9.1/docs/api/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/contracts/gnosis_safe/
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/contracts/gnosis_safe/contract.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/contracts/gnosis_safe_proxy_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/contracts/gnosis_safe_proxy_factory/contract.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.240804 open-autonomy-0.9.1/docs/api/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.240804 open-autonomy-0.9.1/docs/api/data/Dockerfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.416806 open-autonomy-0.9.1/docs/api/data/Dockerfiles/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/data/Dockerfiles/dev/watcher.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.424806 open-autonomy-0.9.1/docs/api/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/build.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/constants.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.240804 open-autonomy-0.9.1/docs/api/deploy/generators/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.424806 open-autonomy-0.9.1/docs/api/deploy/generators/docker_compose/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/generators/docker_compose/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/generators/docker_compose/templates.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.424806 open-autonomy-0.9.1/docs/api/deploy/generators/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/generators/kubernetes/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/generators/kubernetes/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/deploy/image.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.244804 open-autonomy-0.9.1/docs/api/fsm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.424806 open-autonomy-0.9.1/docs/api/fsm/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/fsm/scaffold/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/fsm/scaffold/constants.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.428806 open-autonomy-0.9.1/docs/api/fsm/scaffold/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/fsm/scaffold/generators/components.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/fsm/scaffold/generators/tests.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/fsm/scaffold/scaffold_skill.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.428806 open-autonomy-0.9.1/docs/api/fsm/scaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/fsm/scaffold/templates/components.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/fsm/scaffold/templates/tests.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.244804 open-autonomy-0.9.1/docs/api/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.428806 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.428806 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/base_test_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/base_test_classes/agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/base_test_classes/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/configurations.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.440806 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/acn_node.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/amm_net.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/ganache.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/gnosis_safe_net.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/registries.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/tendermint.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/fixture_helpers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.440806 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/async_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/tendermint_utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.244804 open-autonomy-0.9.1/docs/api/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.440806 open-autonomy-0.9.1/docs/api/protocols/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)    54108 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/protocols/abci/custom_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/protocols/abci/dialogues.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/protocols/abci/message.md
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/protocols/abci/serialization.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.444806 open-autonomy-0.9.1/docs/api/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/replay/agent.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/replay/tendermint.md
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/replay/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.248804 open-autonomy-0.9.1/docs/api/skills/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.444806 open-autonomy-0.9.1/docs/api/skills/abstract_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_abci/dialogues.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_abci/handlers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.448806 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/abci_app_chain.md
+-rw-r--r--   0 runner    (1001) docker     (123)    64335 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/behaviour_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/behaviours.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/common.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/dialogues.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/handlers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.448806 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/ipfs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/load.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/paths.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/store.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/models.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.456806 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/abci_app.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/common.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/integration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/rounds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.248804 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.248804 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.456806 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/dialogues.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/handlers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/payloads.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/rounds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.456806 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/test_tools/base.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.456806 open-autonomy-0.9.1/docs/api/skills/registration_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/registration_abci/behaviours.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/registration_abci/dialogues.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/registration_abci/handlers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/registration_abci/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/registration_abci/payloads.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/registration_abci/rounds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.460806 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/behaviours.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/dialogues.md
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/handlers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/payload_tools.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/payloads.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/rounds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.460806 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/test_tools/integration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/application_deployment.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/control_flow.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/counter_example.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/debugging.md
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/delegate_call.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.460806 open-autonomy-0.9.1/docs/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/demos/hello_world_demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/demos/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33346 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/demos/price_oracle_fsms.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/demos/price_oracle_intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/demos/price_oracle_technical_details.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.460806 open-autonomy-0.9.1/docs/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/deployment/on-chain_deployment_checklist.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/ethereum_specifics.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/exceptions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.248804 open-autonomy-0.9.1/docs/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.460806 open-autonomy-0.9.1/docs/fonts/Manrope/
+-rw-r--r--   0 runner    (1001) docker     (123)    96364 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    97116 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96304 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96312 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96492 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96412 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96528 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/fonts/Manrope/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.468806 open-autonomy-0.9.1/docs/get_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/get_started/agent_services_compared_to.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/get_started/use_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/get_started/what_is_an_agent_service.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/get_started/why_do_we_need_agent_services.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.476806 open-autonomy-0.9.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/configure_access_external_chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/create_fsm_app.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/create_service_existing_agent.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/create_service_from_scratch.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/deploy_service.md
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/overview_of_the_development_process.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/publish_fetch_packages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/register_packages_on_chain.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/service_configuration_file.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/guides/set_up.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.496806 open-autonomy-0.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/abci_requests.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/agent_service_architecture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/agent_service_index_page.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22210 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/centralized_decentralized_world.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/counter_diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/development-process-simplified.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46903 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/development_process.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46831 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/development_process_create_fsm_app.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46776 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/development_process_create_service_existing_agent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45719 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/development_process_define_service.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/development_process_publish_fetch_packages.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45825 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/development_process_register_packages_on_chain.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/do_name_servers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/fsm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    50819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/fsm_composition.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/fsm_composition_2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29965 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_action.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    40598 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_agent_internal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    54165 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_demo_architecture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_demo_architecture_simplified.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_fsm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_result.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_sequence_1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_sequence_2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_sequence_3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_sequence_4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_sequence_5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15072 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/hello_world_zoom_agent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113949 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/name_server_setup.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/networking_page.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/open-autonomy-framework-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/oracle_composition.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    42238 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/oracle_diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/package_management.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/register_package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/service-level_overrides.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    54123 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/simple_demo_architecture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    55927 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/simplified-aea.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/skill-components.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/tendermint.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25496 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/images/tendermint_transaction.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.500806 open-autonomy-0.9.1/docs/key_concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/abci.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/abci_app_abstract_round.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/abci_app_abstract_round_behaviour.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/abci_app_async_behaviour.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/abci_app_class.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/abci_app_interactions.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/aea.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/fsm.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/fsm_app_components.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/fsm_app_introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/poc-diagram.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/key_concepts/threat_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/package_list.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/questions-and-answers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.500806 open-autonomy-0.9.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/upgrading.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/using_stack_deployment.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/docs/version.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.508807 open-autonomy-0.9.1/open_autonomy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-02-23 16:08:23.000000 open-autonomy-0.9.1/open_autonomy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49323 2023-02-23 16:08:23.000000 open-autonomy-0.9.1/open_autonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:08:23.000000 open-autonomy-0.9.1/open_autonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-23 16:08:23.000000 open-autonomy-0.9.1/open_autonomy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:08:23.000000 open-autonomy-0.9.1/open_autonomy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-23 16:08:23.000000 open-autonomy-0.9.1/open_autonomy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-23 16:08:23.000000 open-autonomy-0.9.1/open_autonomy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.508807 open-autonomy-0.9.1/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/packages.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.508807 open-autonomy-0.9.1/packages/valory/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.508807 open-autonomy-0.9.1/packages/valory/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.508807 open-autonomy-0.9.1/packages/valory/agents/abstract_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/abstract_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/abstract_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/abstract_abci/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.508807 open-autonomy-0.9.1/packages/valory/agents/abstract_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/abstract_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/abstract_abci/tests/test_abstract_abci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.512807 open-autonomy-0.9.1/packages/valory/agents/counter/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/counter/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/counter/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.512807 open-autonomy-0.9.1/packages/valory/agents/counter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/counter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/counter/tests/test_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.520807 open-autonomy-0.9.1/packages/valory/agents/counter_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/counter_client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/counter_client/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.520807 open-autonomy-0.9.1/packages/valory/agents/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/hello_world/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/hello_world/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.520807 open-autonomy-0.9.1/packages/valory/agents/hello_world/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/hello_world/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/hello_world/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.520807 open-autonomy-0.9.1/packages/valory/agents/register_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.520807 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.520807 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.524807 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/docker/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.524807 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/config-template.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/tendermint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/wrapper.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/test_hard_reset_race_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/test_register_reset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.536807 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.536807 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/tests/test_register_reset_recovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.536807 open-autonomy-0.9.1/packages/valory/agents/register_termination/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_termination/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_termination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_termination/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.536807 open-autonomy-0.9.1/packages/valory/agents/register_termination/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_termination/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_termination/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/register_termination/tests/test_register_reset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.536807 open-autonomy-0.9.1/packages/valory/agents/registration_start_up/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/registration_start_up/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/registration_start_up/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/registration_start_up/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.540807 open-autonomy-0.9.1/packages/valory/agents/registration_start_up/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/registration_start_up/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/registration_start_up/tests/test_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.540807 open-autonomy-0.9.1/packages/valory/agents/test_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/test_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/test_abci/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.540807 open-autonomy-0.9.1/packages/valory/agents/test_ipfs/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/test_ipfs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/test_ipfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/test_ipfs/aea-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.540807 open-autonomy-0.9.1/packages/valory/agents/test_ipfs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/test_ipfs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/agents/test_ipfs/tests/test_ipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.540807 open-autonomy-0.9.1/packages/valory/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.544807 open-autonomy-0.9.1/packages/valory/connections/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53091 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/connection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/dialogues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/gogoproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/gogoproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56837 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/gogoproto/gogo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.268804 open-autonomy-0.9.1/packages/valory/connections/abci/protos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/protos/gogoproto/
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/gogoproto/gogo.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.268804 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/abci/types.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/crypto/keys.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/crypto/proof.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/types/params.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/types/types.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/types/validator.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/version/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/version/types.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/scripts/genproto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.552807 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)   167050 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/abci/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26712 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/abci/types_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.556807 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/crypto/keys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/crypto/proof_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.556807 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/types/
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/types/params_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57736 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/types/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/types/validator_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.556807 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/version/
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/version/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tendermint_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.556807 open-autonomy-0.9.1/packages/valory/connections/abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_abci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11835 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_abci_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_abci_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.560807 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.560807 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.568807 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/grpc_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/tcp_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17798 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_tendermint_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_tendermint_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/abci/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.568807 open-autonomy-0.9.1/packages/valory/connections/ipfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/ipfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/ipfs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/ipfs/connection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/ipfs/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.568807 open-autonomy-0.9.1/packages/valory/connections/ipfs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/ipfs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/connections/ipfs/tests/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.568807 open-autonomy-0.9.1/packages/valory/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.568807 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.568807 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    84073 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/build/AgentRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.572807 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/agent_registry/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.572807 open-autonomy-0.9.1/packages/valory/contracts/component_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/component_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.572807 open-autonomy-0.9.1/packages/valory/contracts/component_registry/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    79782 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/component_registry/build/ComponentRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/component_registry/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/component_registry/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.572807 open-autonomy-0.9.1/packages/valory/contracts/component_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/component_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/component_registry/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.572807 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.572807 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/build/
+-rw-r--r--   0 runner    (1001) docker     (123)   122983 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/build/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38396 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.576807 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32033 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.576807 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.576807 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/build/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.584807 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.584807 open-autonomy-0.9.1/packages/valory/contracts/multicall2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      925 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multicall2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.584807 open-autonomy-0.9.1/packages/valory/contracts/multicall2/build/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17861 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multicall2/build/multicall2.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5408 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multicall2/contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multicall2/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.584807 open-autonomy-0.9.1/packages/valory/contracts/multicall2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multicall2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multicall2/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.584807 open-autonomy-0.9.1/packages/valory/contracts/multisend/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multisend/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multisend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.584807 open-autonomy-0.9.1/packages/valory/contracts/multisend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multisend/build/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multisend/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multisend/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.588807 open-autonomy-0.9.1/packages/valory/contracts/multisend/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multisend/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/multisend/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.588807 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.588807 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/build/RegistriesManager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.588807 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/registries_manager/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.588807 open-autonomy-0.9.1/packages/valory/contracts/service_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.588807 open-autonomy-0.9.1/packages/valory/contracts/service_manager/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_manager/build/ServiceManager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_manager/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_manager/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.588807 open-autonomy-0.9.1/packages/valory/contracts/service_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_manager/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.592807 open-autonomy-0.9.1/packages/valory/contracts/service_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.592807 open-autonomy-0.9.1/packages/valory/contracts/service_registry/build/
+-rw-r--r--   0 runner    (1001) docker     (123)   141766 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_registry/build/ServiceRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_registry/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_registry/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.596807 open-autonomy-0.9.1/packages/valory/contracts/service_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/contracts/service_registry/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.596807 open-autonomy-0.9.1/packages/valory/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.600807 open-autonomy-0.9.1/packages/valory/protocols/abci/
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/abci.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    61490 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/abci_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70004 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52109 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    33035 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.600807 open-autonomy-0.9.1/packages/valory/protocols/abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30458 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/tests/test_abci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/tests/test_abci_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/abci/tests/test_abci_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.608807 open-autonomy-0.9.1/packages/valory/protocols/ipfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/ipfs.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/ipfs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.608807 open-autonomy-0.9.1/packages/valory/protocols/ipfs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/tests/test_ipfs_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/ipfs/tests/test_ipfs_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.612807 open-autonomy-0.9.1/packages/valory/protocols/tendermint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/tendermint.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/tendermint_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.616808 open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/test_tendermint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/test_tendermint_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/test_tendermint_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.272804 open-autonomy-0.9.1/packages/valory/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.620808 open-autonomy-0.9.1/packages/valory/services/counter/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/services/counter/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/services/counter/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.620808 open-autonomy-0.9.1/packages/valory/services/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/services/hello_world/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/services/hello_world/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.620808 open-autonomy-0.9.1/packages/valory/services/register_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/services/register_reset/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/services/register_reset/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.624808 open-autonomy-0.9.1/packages/valory/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.636808 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.636808 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_abci/tests/test_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.640808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/abci_app_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110959 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91028 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/behaviour_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30368 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.644808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.648808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/abci_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.652808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.652808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.660808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/skill.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_abci_app_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89395 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_base_rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92972 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_behaviours_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23074 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.664808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/test_ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26092 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.664808 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.668808 open-autonomy-0.9.1/packages/valory/skills/counter/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.668808 open-autonomy-0.9.1/packages/valory/skills/counter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter/tests/test_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.672808 open-autonomy-0.9.1/packages/valory/skills/counter_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.680808 open-autonomy-0.9.1/packages/valory/skills/counter_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/counter_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.684808 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/fsm_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.684808 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.692808 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/fsm_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.696808 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.700808 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.704808 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.720808 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.724809 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.728808 open-autonomy-0.9.1/packages/valory/skills/registration_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/fsm_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.732809 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24376 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.740809 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/fsm_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.740809 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.752809 open-autonomy-0.9.1/packages/valory/skills/termination_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.756809 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25882 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.760809 open-autonomy-0.9.1/packages/valory/skills/test_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.764809 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.776809 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/fsm_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.780809 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.788809 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35977 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/fsm_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/payload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31996 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/rounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/skill.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.788809 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/test_tools/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.792809 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_payload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36035 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.792809 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_tools/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.800809 open-autonomy-0.9.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/RELEASE_PROCESS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12076 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/check_copyright.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14693 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/check_doc_ipfs_hashes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6867 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/check_doc_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3825 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/check_ipfs_hashes_pushed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1911 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/check_pipfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8212 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/generate_api_documentation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1963 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/generate_package_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/pre-add
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/pre-push
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/spell-check.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/scripts/whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-02-23 16:08:23.872810 open-autonomy-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.800809 open-autonomy-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.288805 open-autonomy-0.9.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.804809 open-autonomy-0.9.1/tests/data/dummy_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.288805 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.284804 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.804809 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/agents/dummy_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/agents/dummy_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/agents/dummy_agent/aea-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/agents/dummy_agent/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.284804 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.808809 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.284804 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.808809 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/contract.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.288805 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.808809 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.288805 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.812809 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/services/dummy_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/services/dummy_service/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/services/dummy_service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.288805 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.812809 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/my_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/skill.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_packages/packages.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.816809 open-autonomy-0.9.1/tests/data/dummy_service_config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.816809 open-autonomy-0.9.1/tests/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)   143205 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/logs/aea_0.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.816809 open-autonomy-0.9.1/tests/data/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/specs/fsm_specification.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/specs/fsm_specification_empty.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/data/specs/fsm_specification_extra.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.828809 open-autonomy-0.9.1/tests/test_autonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.832810 open-autonomy-0.9.1/tests/test_autonomy/test_chain/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_chain/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_chain/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_chain/test_mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_chain/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.836809 open-autonomy-0.9.1/tests/test_autonomy/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.840810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.840810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_abci/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_abci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstring_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_check_dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_check_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_verify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_build_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.844810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.844810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_build/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21146 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_build/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_from_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_run_deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.844810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_develop/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_develop/test_local_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.856810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/test_chain_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/test_fsm_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.856810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_mint/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_mint/test_mint_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_push_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.856810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_replay/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_replay/test_tendermint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_scaffold_fsm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.860810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_service/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_service/test_service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.860810 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_utils/test_click_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.860810 open-autonomy-0.9.1/tests/test_autonomy/test_deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_deploy/test_deployment_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_deploy/test_service_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.864810 open-autonomy-0.9.1/tests/test_autonomy/test_images/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_images/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_images/test_autonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_images/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_images/test_tendermint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_autonomy/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.864810 open-autonomy-0.9.1/tests/test_deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_deployments/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_deployments/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_deployments/test_deployment_code_identical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_deployments/test_deployments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.868810 open-autonomy-0.9.1/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_docs/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_docs/test_code_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_docs/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:08:23.868810 open-autonomy-0.9.1/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tests/test_scripts/test_check_doc_ipfs_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-02-23 16:08:00.000000 open-autonomy-0.9.1/tox.ini
```

### Comparing `open-autonomy-0.9.0/AUTHORS.md` & `open-autonomy-0.9.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/HISTORY.md` & `open-autonomy-0.9.1/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # Release History - `open-autonomy`
 
+# 0.9.1 (2023-02-22)
+
+Autonomy:
+- Updates the `docker-compose` template to enable the usage of `host.docker.internal` as host machine gateway
+
+Tests:
+- Adds test coverage for newly introduced commands on `autonomy analyse` group
+
+Docs:
+- Updates the documentation on the usage of custom images in agent deployments.
+
+Chore:
+- Updates the `tomte` version in the `Pipfile`
+
 # 0.9.0 (2023-02-16)
 
 Autonomy:
 - Updates the on-chain interaction functionalities to wait for the relevant event to make sure the interaction was successful
 - Makes the usage of local tendermint chain optional in the deployment setup
 - Introduces `autonomy analyse dialogues` command for analysing the dialogue definitions in a skill package
 - Introduces `autonomy analyse service` command for checking the deployment readiness of a service
```

### Comparing `open-autonomy-0.9.0/LICENSE` & `open-autonomy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/PKG-INFO` & `open-autonomy-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-autonomy
-Version: 0.9.0
+Version: 0.9.1
 Summary: A framework for the creation of autonomous agent services.
 Home-page: https://github.com/valory-xyz/open-autonomy.git
 Author: Valory AG
 License: Apache-2.0
 Project-URL: Bug Reports, https://github.com/valory-xyz/open-autonomy/issues
 Project-URL: Source, https://github.com/valory/open-autonomy
 Keywords: autonomy open-autonomy aea open-aea autonomous-economic-agents agent-framework multi-agent-systems multi-agent cryptocurrency cryptocurrencies dezentralized dezentralized-network
@@ -81,23 +81,23 @@
 smart contracts provide, making it possible to execute **arbitrarily complex operations**
 (such as machine-learning algorithms). Most importantly, agent services are
 **decentralized**, **trust-minimized**, **transparent**, and **robust**.
 
 
 ## Get started developing agent services
 
-Read the [Open Autonomy documentation](https://docs.autonolas.network/) to learn more about agent services. Follow the [set up](https://docs.autonolas.network/guides/set_up/) and [quick start](https://docs.autonolas.network/guides/quick_start/) guides to start building your own services.
+Read the [Open Autonomy documentation](https://docs.autonolas.network/open-autonomy/) to learn more about agent services. Follow the [set up](https://docs.autonolas.network/open-autonomy/guides/set_up/) and [quick start](https://docs.autonolas.network/open-autonomy/guides/quick_start/) guides to start building your own services.
 
 
 ## For developers contributing to the framework: install from source
 
 - Ensure your machine satisfies the following requirements:
 
     - Python `>= 3.7`
-    - [Tendermint](https://docs.tendermint.com/master/introduction/install.html) `==0.34.19`
+    - [Tendermint](https://docs.tendermint.com/v0.34/introduction/install.html) `==0.34.19`
     - [IPFS node](https://docs.ipfs.io/install/command-line/#official-distributions) `==v0.6.0`
     - [Pip](https://pip.pypa.io/en/stable/installation/)
     - [Pipenv](https://pipenv.pypa.io/en/latest/install/) `>=2021.x.xx`
     - [Go](https://go.dev/doc/install) `==1.17.7`
     - [Kubectl](https://kubernetes.io/docs/tasks/tools/)
     - [Docker Engine](https://docs.docker.com/engine/install/)
     - [Docker Compose](https://docs.docker.com/compose/install/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-autonomy Version: 0.9.0 Summary: A framework
+Metadata-Version: 2.1 Name: open-autonomy Version: 0.9.1 Summary: A framework
 for the creation of autonomous agent services. Home-page: https://github.com/
 valory-xyz/open-autonomy.git Author: Valory AG License: Apache-2.0 Project-URL:
 Bug Reports, https://github.com/valory-xyz/open-autonomy/issues Project-URL:
 Source, https://github.com/valory/open-autonomy Keywords: autonomy open-
 autonomy aea open-aea autonomous-economic-agents agent-framework multi-agent-
 systems multi-agent cryptocurrency cryptocurrencies dezentralized
 dezentralized-network Classifier: Environment :: Console Classifier:
@@ -25,39 +25,40 @@
 chain autonomous services which run as a multi-agent-system (MAS) and offer
 enhanced functionalities on-chain. Agent services expand the range of
 operations that traditional smart contracts provide, making it possible to
 execute **arbitrarily complex operations** (such as machine-learning
 algorithms). Most importantly, agent services are **decentralized**, **trust-
 minimized**, **transparent**, and **robust**. ## Get started developing agent
 services Read the [Open Autonomy documentation](https://docs.autonolas.network/
-) to learn more about agent services. Follow the [set up](https://
-docs.autonolas.network/guides/set_up/) and [quick start](https://
-docs.autonolas.network/guides/quick_start/) guides to start building your own
-services. ## For developers contributing to the framework: install from source
-- Ensure your machine satisfies the following requirements: - Python `>= 3.7` -
-[Tendermint](https://docs.tendermint.com/master/introduction/install.html)
-`==0.34.19` - [IPFS node](https://docs.ipfs.io/install/command-line/#official-
-distributions) `==v0.6.0` - [Pip](https://pip.pypa.io/en/stable/installation/
-) - [Pipenv](https://pipenv.pypa.io/en/latest/install/) `>=2021.x.xx` - [Go]
-(https://go.dev/doc/install) `==1.17.7` - [Kubectl](https://kubernetes.io/docs/
-tasks/tools/) - [Docker Engine](https://docs.docker.com/engine/install/) -
-[Docker Compose](https://docs.docker.com/compose/install/) - [Skaffold](https:/
-/skaffold.dev/docs/install/#standalone-binary) `>= 1.39.1` - [Gitleaks](https:/
-/github.com/zricethezav/gitleaks/releases/latest) - Clone the repository: git
-clone git@github.com:valory-xyz/open-autonomy.git - Pull pre-built images:
-docker pull valory/autonolas-registries:latest docker pull valory/acn-node:
-latest docker pull valory/contracts-amm:latest docker pull valory/safe-
-contract-net:latest docker pull valory/slow-tendermint-server:0.1.0 - Create
-and launch a virtual environment. Also, run this during development, every time
-you need to re-create and launch the virtual environment and update the
-dependencies: make new_env && pipenv shell > :information_source: Note: we are
-using [atheris](https://github.com/google/atheris) in order to perform fuzzy
-testing. > The dependency is not listed in the `Pipfile` because it is not
-supported on Windows. > If you need to run or implement a fuzzy test, please
-manually install the dependency. > If you are developing on Mac, please follow
-the extra steps described [here](https://github.com/google/atheris#mac). -
-Fetch packages: autonomy packages sync --update-packages ## Cite If you are
-using our software in a publication, please consider to cite it with the
-following BibTex entry: ``` @misc{open-autonomy, Author = {David Minarsch and
-Marco Favorito and Viraj Patel and Adamantios Zaras and David Vilela Freire and
-Michiel Karrenbelt and 8baller and Ardian Abazi and Yuri Turchenkov and JosÃ©
-Moreira SÃ¡nchez}, Title = {Open Autonomy Framework}, Year = {2021}, } ```
+open-autonomy/) to learn more about agent services. Follow the [set up](https:/
+/docs.autonolas.network/open-autonomy/guides/set_up/) and [quick start](https:/
+/docs.autonolas.network/open-autonomy/guides/quick_start/) guides to start
+building your own services. ## For developers contributing to the framework:
+install from source - Ensure your machine satisfies the following requirements:
+- Python `>= 3.7` - [Tendermint](https://docs.tendermint.com/v0.34/
+introduction/install.html) `==0.34.19` - [IPFS node](https://docs.ipfs.io/
+install/command-line/#official-distributions) `==v0.6.0` - [Pip](https://
+pip.pypa.io/en/stable/installation/) - [Pipenv](https://pipenv.pypa.io/en/
+latest/install/) `>=2021.x.xx` - [Go](https://go.dev/doc/install) `==1.17.7` -
+[Kubectl](https://kubernetes.io/docs/tasks/tools/) - [Docker Engine](https://
+docs.docker.com/engine/install/) - [Docker Compose](https://docs.docker.com/
+compose/install/) - [Skaffold](https://skaffold.dev/docs/install/#standalone-
+binary) `>= 1.39.1` - [Gitleaks](https://github.com/zricethezav/gitleaks/
+releases/latest) - Clone the repository: git clone git@github.com:valory-xyz/
+open-autonomy.git - Pull pre-built images: docker pull valory/autonolas-
+registries:latest docker pull valory/acn-node:latest docker pull valory/
+contracts-amm:latest docker pull valory/safe-contract-net:latest docker pull
+valory/slow-tendermint-server:0.1.0 - Create and launch a virtual environment.
+Also, run this during development, every time you need to re-create and launch
+the virtual environment and update the dependencies: make new_env && pipenv
+shell > :information_source: Note: we are using [atheris](https://github.com/
+google/atheris) in order to perform fuzzy testing. > The dependency is not
+listed in the `Pipfile` because it is not supported on Windows. > If you need
+to run or implement a fuzzy test, please manually install the dependency. > If
+you are developing on Mac, please follow the extra steps described [here]
+(https://github.com/google/atheris#mac). - Fetch packages: autonomy packages
+sync --update-packages ## Cite If you are using our software in a publication,
+please consider to cite it with the following BibTex entry: ``` @misc{open-
+autonomy, Author = {David Minarsch and Marco Favorito and Viraj Patel and
+Adamantios Zaras and David Vilela Freire and Michiel Karrenbelt and 8baller and
+Ardian Abazi and Yuri Turchenkov and JosÃ© Moreira SÃ¡nchez}, Title = {Open
+Autonomy Framework}, Year = {2021}, } ```
```

### Comparing `open-autonomy-0.9.0/Pipfile` & `open-autonomy-0.9.1/Pipfile`

 * *Files 12% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 pandas-stubs = "==1.2.0.62"
 protobuf = "==3.19.4"
 pytz = "==2022.2.1"
 py-ecc = "==5.2.0"
 py-eth-sig-utils = "==0.4.0"
 ### tests deps
 mistune = "==2.0.3"
-tomte = {version = "==0.1.5", extras = ["tox", "tests"]}
+tomte = {version = "==0.2.2", extras = ["tox", "tests"]}
 
 [requires]
 python_version = "3.10"
```

### Comparing `open-autonomy-0.9.0/README.md` & `open-autonomy-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,23 +46,23 @@
 smart contracts provide, making it possible to execute **arbitrarily complex operations**
 (such as machine-learning algorithms). Most importantly, agent services are
 **decentralized**, **trust-minimized**, **transparent**, and **robust**.
 
 
 ## Get started developing agent services
 
-Read the [Open Autonomy documentation](https://docs.autonolas.network/) to learn more about agent services. Follow the [set up](https://docs.autonolas.network/guides/set_up/) and [quick start](https://docs.autonolas.network/guides/quick_start/) guides to start building your own services.
+Read the [Open Autonomy documentation](https://docs.autonolas.network/open-autonomy/) to learn more about agent services. Follow the [set up](https://docs.autonolas.network/open-autonomy/guides/set_up/) and [quick start](https://docs.autonolas.network/open-autonomy/guides/quick_start/) guides to start building your own services.
 
 
 ## For developers contributing to the framework: install from source
 
 - Ensure your machine satisfies the following requirements:
 
     - Python `>= 3.7`
-    - [Tendermint](https://docs.tendermint.com/master/introduction/install.html) `==0.34.19`
+    - [Tendermint](https://docs.tendermint.com/v0.34/introduction/install.html) `==0.34.19`
     - [IPFS node](https://docs.ipfs.io/install/command-line/#official-distributions) `==v0.6.0`
     - [Pip](https://pip.pypa.io/en/stable/installation/)
     - [Pipenv](https://pipenv.pypa.io/en/latest/install/) `>=2021.x.xx`
     - [Go](https://go.dev/doc/install) `==1.17.7`
     - [Kubectl](https://kubernetes.io/docs/tasks/tools/)
     - [Docker Engine](https://docs.docker.com/engine/install/)
     - [Docker Compose](https://docs.docker.com/compose/install/)
```

#### html2text {}

```diff
@@ -5,39 +5,40 @@
 chain autonomous services which run as a multi-agent-system (MAS) and offer
 enhanced functionalities on-chain. Agent services expand the range of
 operations that traditional smart contracts provide, making it possible to
 execute **arbitrarily complex operations** (such as machine-learning
 algorithms). Most importantly, agent services are **decentralized**, **trust-
 minimized**, **transparent**, and **robust**. ## Get started developing agent
 services Read the [Open Autonomy documentation](https://docs.autonolas.network/
-) to learn more about agent services. Follow the [set up](https://
-docs.autonolas.network/guides/set_up/) and [quick start](https://
-docs.autonolas.network/guides/quick_start/) guides to start building your own
-services. ## For developers contributing to the framework: install from source
-- Ensure your machine satisfies the following requirements: - Python `>= 3.7` -
-[Tendermint](https://docs.tendermint.com/master/introduction/install.html)
-`==0.34.19` - [IPFS node](https://docs.ipfs.io/install/command-line/#official-
-distributions) `==v0.6.0` - [Pip](https://pip.pypa.io/en/stable/installation/
-) - [Pipenv](https://pipenv.pypa.io/en/latest/install/) `>=2021.x.xx` - [Go]
-(https://go.dev/doc/install) `==1.17.7` - [Kubectl](https://kubernetes.io/docs/
-tasks/tools/) - [Docker Engine](https://docs.docker.com/engine/install/) -
-[Docker Compose](https://docs.docker.com/compose/install/) - [Skaffold](https:/
-/skaffold.dev/docs/install/#standalone-binary) `>= 1.39.1` - [Gitleaks](https:/
-/github.com/zricethezav/gitleaks/releases/latest) - Clone the repository: git
-clone git@github.com:valory-xyz/open-autonomy.git - Pull pre-built images:
-docker pull valory/autonolas-registries:latest docker pull valory/acn-node:
-latest docker pull valory/contracts-amm:latest docker pull valory/safe-
-contract-net:latest docker pull valory/slow-tendermint-server:0.1.0 - Create
-and launch a virtual environment. Also, run this during development, every time
-you need to re-create and launch the virtual environment and update the
-dependencies: make new_env && pipenv shell > :information_source: Note: we are
-using [atheris](https://github.com/google/atheris) in order to perform fuzzy
-testing. > The dependency is not listed in the `Pipfile` because it is not
-supported on Windows. > If you need to run or implement a fuzzy test, please
-manually install the dependency. > If you are developing on Mac, please follow
-the extra steps described [here](https://github.com/google/atheris#mac). -
-Fetch packages: autonomy packages sync --update-packages ## Cite If you are
-using our software in a publication, please consider to cite it with the
-following BibTex entry: ``` @misc{open-autonomy, Author = {David Minarsch and
-Marco Favorito and Viraj Patel and Adamantios Zaras and David Vilela Freire and
-Michiel Karrenbelt and 8baller and Ardian Abazi and Yuri Turchenkov and JosÃ©
-Moreira SÃ¡nchez}, Title = {Open Autonomy Framework}, Year = {2021}, } ```
+open-autonomy/) to learn more about agent services. Follow the [set up](https:/
+/docs.autonolas.network/open-autonomy/guides/set_up/) and [quick start](https:/
+/docs.autonolas.network/open-autonomy/guides/quick_start/) guides to start
+building your own services. ## For developers contributing to the framework:
+install from source - Ensure your machine satisfies the following requirements:
+- Python `>= 3.7` - [Tendermint](https://docs.tendermint.com/v0.34/
+introduction/install.html) `==0.34.19` - [IPFS node](https://docs.ipfs.io/
+install/command-line/#official-distributions) `==v0.6.0` - [Pip](https://
+pip.pypa.io/en/stable/installation/) - [Pipenv](https://pipenv.pypa.io/en/
+latest/install/) `>=2021.x.xx` - [Go](https://go.dev/doc/install) `==1.17.7` -
+[Kubectl](https://kubernetes.io/docs/tasks/tools/) - [Docker Engine](https://
+docs.docker.com/engine/install/) - [Docker Compose](https://docs.docker.com/
+compose/install/) - [Skaffold](https://skaffold.dev/docs/install/#standalone-
+binary) `>= 1.39.1` - [Gitleaks](https://github.com/zricethezav/gitleaks/
+releases/latest) - Clone the repository: git clone git@github.com:valory-xyz/
+open-autonomy.git - Pull pre-built images: docker pull valory/autonolas-
+registries:latest docker pull valory/acn-node:latest docker pull valory/
+contracts-amm:latest docker pull valory/safe-contract-net:latest docker pull
+valory/slow-tendermint-server:0.1.0 - Create and launch a virtual environment.
+Also, run this during development, every time you need to re-create and launch
+the virtual environment and update the dependencies: make new_env && pipenv
+shell > :information_source: Note: we are using [atheris](https://github.com/
+google/atheris) in order to perform fuzzy testing. > The dependency is not
+listed in the `Pipfile` because it is not supported on Windows. > If you need
+to run or implement a fuzzy test, please manually install the dependency. > If
+you are developing on Mac, please follow the extra steps described [here]
+(https://github.com/google/atheris#mac). - Fetch packages: autonomy packages
+sync --update-packages ## Cite If you are using our software in a publication,
+please consider to cite it with the following BibTex entry: ``` @misc{open-
+autonomy, Author = {David Minarsch and Marco Favorito and Viraj Patel and
+Adamantios Zaras and David Vilela Freire and Michiel Karrenbelt and 8baller and
+Ardian Abazi and Yuri Turchenkov and JosÃ© Moreira SÃ¡nchez}, Title = {Open
+Autonomy Framework}, Year = {2021}, } ```
```

### Comparing `open-autonomy-0.9.0/SECURITY.md` & `open-autonomy-0.9.1/SECURITY.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 ## Supported Versions
 
 The following table shows which versions of `open-autonomy` are currently being supported with security updates.
 
 | Version   | Supported          |
 | --------- | ------------------ |
-| `0.9.0`   | :white_check_mark: |
-| `< 0.9.0` | :x:                |
+| `0.9.1`   | :white_check_mark: |
+| `< 0.9.1` | :x:                |
 
 ## Reporting a Vulnerability
 
 The `open-autonomy` team and community take all security bugs in `open-autonomy` seriously. Thank you for improving the security of `open-autonomy`. We appreciate your efforts and responsible disclosure and will make every effort to acknowledge your contributions.
 
 Report security bugs by emailing `info@valory.xyz`.
```

### Comparing `open-autonomy-0.9.0/autonomy/__init__.py` & `open-autonomy-0.9.1/autonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/__version__.py` & `open-autonomy-0.9.1/autonomy/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 # ------------------------------------------------------------------------------
 
 """Specifies the version of the AEA package."""
 
 __title__ = "open-autonomy"
 __description__ = "A framework for the creation of autonomous agent services."
 __url__ = "https://github.com/valory-xyz/open-autonomy.git"
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 __author__ = "Valory AG"
 __license__ = "Apache-2.0"
 __copyright__ = "2021-2022 Valory AG"
```

### Comparing `open-autonomy-0.9.0/autonomy/analyse/__init__.py` & `open-autonomy-0.9.1/autonomy/analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/abci/__init__.py` & `open-autonomy-0.9.1/autonomy/analyse/abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/abci/app_spec.py` & `open-autonomy-0.9.1/autonomy/analyse/abci/app_spec.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/abci/docstrings.py` & `open-autonomy-0.9.1/autonomy/analyse/abci/docstrings.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/benchmark/__init__.py` & `open-autonomy-0.9.1/autonomy/analyse/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/benchmark/aggregate.py` & `open-autonomy-0.9.1/autonomy/analyse/benchmark/aggregate.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/benchmark/html.py` & `open-autonomy-0.9.1/autonomy/analyse/benchmark/html.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/constants.py` & `open-autonomy-0.9.1/autonomy/analyse/constants.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/dialogues.py` & `open-autonomy-0.9.1/autonomy/analyse/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/handlers.py` & `open-autonomy-0.9.1/autonomy/analyse/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/logs/__init__.py` & `open-autonomy-0.9.1/autonomy/analyse/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/logs/base.py` & `open-autonomy-0.9.1/autonomy/analyse/logs/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/logs/collection.py` & `open-autonomy-0.9.1/autonomy/analyse/logs/collection.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/analyse/logs/db.py` & `open-autonomy-0.9.1/autonomy/analyse/logs/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,32 +143,14 @@
             self.delete()
 
         self.cursor.execute(QUERY_CREATE_LOG_TABLE.format(agent=self.agent))
         self._db.commit()
 
         return self
 
-    def insert_one(  # pylint: disable=too-many-arguments
-        self,
-        timestamp: datetime,
-        log_level: str,
-        message: str,
-        period: int,
-        round_name: str,
-        behaviour_name: str,
-    ) -> "AgentLogsDB":
-        """Insert a record"""
-        self.cursor.execute(
-            QUERY_INSERT_LOG,
-            (timestamp, log_level, message, period, round_name, behaviour_name),
-        )
-        self._db.commit()
-
-        return self
-
     def insert_many(
         self,
         logs: Iterator[LogRow],
     ) -> "AgentLogsDB":
         """Insert a record"""
         for timestamp, log_level, message, period, round_name, behaviour_name in logs:
             self.cursor.execute(
```

### Comparing `open-autonomy-0.9.0/autonomy/analyse/service.py` & `open-autonomy-0.9.1/autonomy/analyse/service.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/__init__.py` & `open-autonomy-0.9.1/autonomy/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/base.py` & `open-autonomy-0.9.1/autonomy/chain/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/config.py` & `open-autonomy-0.9.1/autonomy/chain/config.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/constants.py` & `open-autonomy-0.9.1/autonomy/chain/constants.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/exceptions.py` & `open-autonomy-0.9.1/autonomy/chain/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/metadata.py` & `open-autonomy-0.9.1/autonomy/chain/metadata.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/mint.py` & `open-autonomy-0.9.1/autonomy/chain/mint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/service.py` & `open-autonomy-0.9.1/autonomy/chain/service.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/chain/utils.py` & `open-autonomy-0.9.1/autonomy/chain/utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/__init__.py` & `open-autonomy-0.9.1/autonomy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/__main__.py` & `open-autonomy-0.9.1/autonomy/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/analyse.py` & `open-autonomy-0.9.1/autonomy/cli/analyse.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 
 """Analyse CLI module."""
+from datetime import datetime
 from pathlib import Path
 from typing import List, Optional, cast
 from warnings import filterwarnings
 
 import click
 from aea.cli.utils.click_utils import PublicIdParameter, reraise_as_click_exception
 from aea.cli.utils.context import Context
 from aea.cli.utils.decorators import pass_ctx
 from aea.configurations.constants import PACKAGES
 from aea.configurations.data_types import PublicId
 
 from autonomy.analyse.benchmark.aggregate import BlockTypes, aggregate
 from autonomy.analyse.handlers import check_handlers
+from autonomy.analyse.logs.base import TIME_FORMAT
 from autonomy.chain.config import ChainType
 from autonomy.cli.helpers.analyse import (
     ParseLogs,
     check_service_readiness,
     list_all_skill_yaml_files,
     load_package_tree,
     run_dialogues_check,
@@ -168,14 +170,16 @@
 
 @analyse_group.command("logs")
 @click.option(
     "--from-dir",
     "logs_dir",
     type=click.Path(
         exists=True,
+        file_okay=False,
+        dir_okay=True,
     ),
     required=True,
     help="Path to logs directory",
 )
 @click.option(
     "--reset-db",
     is_flag=True,
@@ -187,20 +191,24 @@
     "agents",
     type=str,
     multiple=True,
     help="Agent IDs to include in analysis",
 )
 @click.option(
     "--start-time",
-    type=str,
+    type=click.DateTime(
+        formats=(TIME_FORMAT,),
+    ),
     help=f"Start time in `{TIME_FORMAT_TEMPLATE}` format",
 )
 @click.option(
     "--end-time",
-    type=str,
+    type=click.DateTime(
+        formats=(TIME_FORMAT,),
+    ),
     help=f"End time in `{TIME_FORMAT_TEMPLATE}` format",
 )
 @click.option(
     "--log-level",
     type=click.Choice(choices=LOGGING_LEVELS, case_sensitive=True),
     help="Logging level.",
 )
@@ -243,30 +251,32 @@
     multiple=True,
     type=str,
     help="Regex pattern to exclude from the result.",
 )
 def _parse_logs(  # pylint: disable=too-many-arguments
     logs_dir: Optional[Path],
     agents: List[str],
-    start_time: Optional[str],
-    end_time: Optional[str],
+    start_time: Optional[datetime],
+    end_time: Optional[datetime],
     log_level: Optional[str],
     period: Optional[int],
     round_name: Optional[str],
     behaviour_name: Optional[str],
     include_regexes: List[str],
     exclude_regexes: List[str],
     reset_db: bool = False,
     fsm_path: bool = False,
 ) -> None:
     """A tool for analysing autonomous agent runtime logs"""
 
     parser = ParseLogs()
     if logs_dir is not None:
         parser.from_dir(logs_dir=Path(logs_dir))
+        if parser.n_agents == 0:
+            raise click.ClickException(f"Cannot find agent log data in {logs_dir}")
 
     if len(agents) == 0:
         raise click.ClickException(
             f"Please provide agent IDs to select logs; Available agents: {parser.agents}"
         )
 
     parser.create_tables(reset=reset_db)
```

### Comparing `open-autonomy-0.9.0/autonomy/cli/build_images.py` & `open-autonomy-0.9.1/autonomy/cli/build_images.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/core.py` & `open-autonomy-0.9.1/autonomy/cli/core.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/deploy.py` & `open-autonomy-0.9.1/autonomy/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/develop.py` & `open-autonomy-0.9.1/autonomy/cli/develop.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/fetch.py` & `open-autonomy-0.9.1/autonomy/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/hash.py` & `open-autonomy-0.9.1/autonomy/cli/hash.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/__init__.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/analyse.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/analyse.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 """Helpers for analyse command"""
 
 import re
 import tempfile
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Optional, Set, Tuple, Union, cast
+from typing import Dict, List, Optional, Set, Tuple, cast
 
 import click
 from aea.components.base import load_aea_package
 from aea.configurations.base import AgentConfig, PackageConfiguration, SkillConfig
 from aea.configurations.constants import (
     DEFAULT_SKILL_CONFIG_FILE,
     PACKAGE_TYPE_TO_CONFIG_FILE,
@@ -36,24 +36,24 @@
     ComponentId,
     ComponentType,
     PackageId,
     PackageType,
     PublicId,
 )
 from aea.configurations.loader import load_configuration_object
+from aea.crypto.base import LedgerApi
 from aea.package_manager.v1 import PackageManagerV1
 from aea_cli_ipfs.ipfs_utils import IPFSTool
 
 from autonomy.analyse.dialogues import check_dialogues_in_a_skill_package
 from autonomy.analyse.logs.base import (
     ENTER_ROUND_REGEX,
     EXIT_ROUND_REGEX,
     LOGS_DB,
     LogRow,
-    TIME_FORMAT,
 )
 from autonomy.analyse.logs.collection import FromDirectory, LogCollection
 from autonomy.analyse.logs.db import AgentLogsDB
 from autonomy.analyse.service import ServiceAnalyser, ServiceValidationFailed
 from autonomy.chain.config import ChainType, ContractConfigs
 from autonomy.chain.exceptions import FailedToRetrieveComponentMetadata
 from autonomy.chain.utils import resolve_component_id
@@ -122,14 +122,20 @@
 
     @property
     def agents(self) -> List[str]:
         """Available agents."""
 
         return self._collection.agents
 
+    @property
+    def n_agents(self) -> int:
+        """Available agents."""
+
+        return self._collection.n_agents
+
     def from_dir(self, logs_dir: Path) -> "ParseLogs":
         """From directory"""
 
         self._db_path = logs_dir / LOGS_DB
         self._collection = FromDirectory(directory=logs_dir)
         self._dbs = {
             agent: AgentLogsDB(agent=agent, file=self._db_path)
@@ -153,29 +159,23 @@
             )
 
         return self
 
     def select(  # pylint: disable=too-many-arguments
         self,
         agents: List[str],
-        start_time: Optional[Union[str, datetime]],
-        end_time: Optional[Union[str, datetime]],
+        start_time: Optional[datetime],
+        end_time: Optional[datetime],
         log_level: Optional[str],
         period: Optional[int],
         round_name: Optional[str],
         behaviour_name: Optional[str],
     ) -> "ParseLogs":
         """Query and return results."""
 
-        if start_time is not None:
-            start_time = datetime.strptime(cast(str, start_time), TIME_FORMAT)
-
-        if end_time is not None:
-            end_time = datetime.strptime(cast(str, end_time), TIME_FORMAT)
-
         results = {}
         for agent in agents:
             results[agent] = self._dbs[agent].select(
                 start_time=start_time,
                 end_time=end_time,
                 log_level=log_level,
                 period=period,
@@ -343,23 +343,42 @@
         return skill_config
 
     return None
 
 
 def _get_ipfs_pins(is_on_chain_check: bool = False) -> Set[str]:
     """Get IPFS pins."""
-    ipfs_tool = IPFSTool()
     if is_on_chain_check:
+        ipfs_tool = IPFSTool()
         if not ipfs_tool.daemon.is_started():
             raise click.ClickException("Cannot connect to the IPFS daemon.")
         return ipfs_tool.all_pins()
 
     return set()
 
 
+def _get_on_chain_service_id(
+    ledger_api: LedgerApi,
+    chain_type: ChainType,
+    token_id: int,
+) -> PackageId:
+    """Get on chain service ID with package hash"""
+    service_info = resolve_component_id(
+        ledger_api=ledger_api,
+        contract_address=ContractConfigs.service_registry.contracts[chain_type],
+        token_id=cast(int, token_id),
+        is_service=True,
+    )
+    package_hash = cast(str, service_info["code_uri"]).replace("ipfs://", "")
+    public_id = PublicId.from_str(service_info["name"]).with_hash(
+        package_hash=package_hash
+    )
+    return PackageId(package_type=PackageType.SERVICE, public_id=public_id)
+
+
 def check_service_readiness(  # pylint: disable=too-many-locals
     token_id: Optional[int],
     public_id: Optional[PublicId],
     chain_type: ChainType,
     packages_dir: Path,
 ) -> None:
     """Check deployment readiness of a service."""
@@ -367,26 +386,18 @@
     is_on_chain_check = token_id is not None
     ledger_api, _ = get_ledger_and_crypto_objects(chain_type=chain_type)
     package_manager = PackageManagerV1.from_dir(packages_dir=packages_dir)
     ipfs_pins = _get_ipfs_pins(is_on_chain_check=is_on_chain_check)
 
     if is_on_chain_check:
         try:
-            service_info = resolve_component_id(
+            service_id = _get_on_chain_service_id(
                 ledger_api=ledger_api,
-                contract_address=ContractConfigs.service_registry.contracts[chain_type],
+                chain_type=chain_type,
                 token_id=cast(int, token_id),
-                is_service=True,
-            )
-            package_hash = cast(str, service_info["code_uri"]).replace("ipfs://", "")
-            public_id = PublicId.from_str(service_info["name"]).with_hash(
-                package_hash=package_hash
-            )
-            service_id = PackageId(
-                package_type=PackageType.SERVICE, public_id=public_id
             )
         except FailedToRetrieveComponentMetadata as e:
             raise click.ClickException(
                 f"On chain service verification failed; {e}"
             ) from e
     else:
         service_id = PackageId(package_type=PackageType.SERVICE, public_id=public_id)
@@ -427,14 +438,15 @@
         )
 
     try:
         service_analyser = ServiceAnalyser(
             service_config=service_config,
             is_on_chain_check=is_on_chain_check,
         )
+
         service_analyser.check_on_chain_state(
             ledger_api=ledger_api,
             chain_type=chain_type,
             token_id=cast(int, token_id),
         )
         service_analyser.validate_service_overrides()
         service_analyser.validate_agent_overrides(agent_config=agent_config)
```

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/chain.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/chain.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/deployment.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/deployment.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/docstring.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/docstring.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/fsm_spec.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/fsm_spec.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/ipfs_hash.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/ipfs_hash.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/helpers/registry.py` & `open-autonomy-0.9.1/autonomy/cli/helpers/registry.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/mint.py` & `open-autonomy-0.9.1/autonomy/cli/mint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/packages.py` & `open-autonomy-0.9.1/autonomy/cli/packages.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/publish.py` & `open-autonomy-0.9.1/autonomy/cli/publish.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/push_all.py` & `open-autonomy-0.9.1/autonomy/cli/push_all.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/replay.py` & `open-autonomy-0.9.1/autonomy/cli/replay.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/scaffold_fsm.py` & `open-autonomy-0.9.1/autonomy/cli/scaffold_fsm.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/service.py` & `open-autonomy-0.9.1/autonomy/cli/service.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/utils/__init__.py` & `open-autonomy-0.9.1/autonomy/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/cli/utils/click_utils.py` & `open-autonomy-0.9.1/autonomy/cli/utils/click_utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/configurations/__init__.py` & `open-autonomy-0.9.1/autonomy/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/configurations/base.py` & `open-autonomy-0.9.1/autonomy/configurations/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/configurations/constants.py` & `open-autonomy-0.9.1/autonomy/configurations/constants.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/configurations/loader.py` & `open-autonomy-0.9.1/autonomy/configurations/loader.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/configurations/schemas/fsm_specification_schema.json` & `open-autonomy-0.9.1/autonomy/configurations/schemas/fsm_specification_schema.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/configurations/schemas/service_schema.json` & `open-autonomy-0.9.1/autonomy/configurations/schemas/service_schema.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/configurations/validation.py` & `open-autonomy-0.9.1/autonomy/configurations/validation.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/constants.py` & `open-autonomy-0.9.1/autonomy/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 
 DEFAULT_SERVICE_REGISTRY_CONTRACTS_IMAGE = (
     f"{SERVICE_REGISTRY_IMAGE_NAME}:{SERVICE_REGISTRY_IMAGE_VERSION}"
 )
 ACN_IMAGE_NAME = os.environ.get("ACN_IMAGE_NAME", "valory/open-acn-node")
 DEFAULT_DOCKER_IMAGE_AUTHOR = "valory"
 OAR_IMAGE = "{image_author}/oar-{agent}:{version}"
-ABSTRACT_ROUND_ABCI_SKILL_WITH_HASH = "valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi"
+ABSTRACT_ROUND_ABCI_SKILL_WITH_HASH = "valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4"
```

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/agent/Dockerfile` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/agent/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/agent/start.sh` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/agent/start.sh`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/Dockerfile` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/Pipfile` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/Pipfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/openssl.cnf` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/openssl.cnf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/start.sh` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/start.sh`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/start_dev.sh` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/start_dev.sh`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/Dockerfiles/dev/watcher.py` & `open-autonomy-0.9.1/autonomy/data/Dockerfiles/dev/watcher.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/__init__.py` & `open-autonomy-0.9.1/autonomy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/build/AgentRegistry.json` & `open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/build/AgentRegistry.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/contract.yaml` & `open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/tests/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/agent_registry/tests/test_contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/agent_registry/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/component_registry/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/component_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/component_registry/build/ComponentRegistry.json` & `open-autonomy-0.9.1/autonomy/data/contracts/component_registry/build/ComponentRegistry.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/component_registry/contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/component_registry/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/component_registry/contract.yaml` & `open-autonomy-0.9.1/autonomy/data/contracts/component_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/component_registry/tests/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/component_registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/component_registry/tests/test_contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/component_registry/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/build/RegistriesManager.json` & `open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/build/RegistriesManager.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/contract.yaml` & `open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/tests/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/registries_manager/tests/test_contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/registries_manager/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_manager/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_manager/build/ServiceManager.json` & `open-autonomy-0.9.1/autonomy/data/contracts/service_manager/build/ServiceManager.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_manager/contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_manager/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_manager/contract.yaml` & `open-autonomy-0.9.1/autonomy/data/contracts/service_manager/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_manager/tests/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_manager/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_manager/tests/test_contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_manager/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_registry/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_registry/build/ServiceRegistry.json` & `open-autonomy-0.9.1/autonomy/data/contracts/service_registry/build/ServiceRegistry.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_registry/contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_registry/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_registry/contract.yaml` & `open-autonomy-0.9.1/autonomy/data/contracts/service_registry/contract.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 class_name: ServiceRegistryContract
 contract_interface_paths:
   ethereum: build/ServiceRegistry.json
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
```

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_registry/tests/__init__.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/data/contracts/service_registry/tests/test_contract.py` & `open-autonomy-0.9.1/autonomy/data/contracts/service_registry/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/__init__.py` & `open-autonomy-0.9.1/autonomy/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/base.py` & `open-autonomy-0.9.1/autonomy/deploy/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/build.py` & `open-autonomy-0.9.1/autonomy/deploy/build.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/constants.py` & `open-autonomy-0.9.1/autonomy/deploy/constants.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/generators/__init__.py` & `open-autonomy-0.9.1/autonomy/deploy/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/generators/docker_compose/__init__.py` & `open-autonomy-0.9.1/autonomy/deploy/generators/docker_compose/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/generators/docker_compose/base.py` & `open-autonomy-0.9.1/autonomy/deploy/generators/docker_compose/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/generators/docker_compose/templates.py` & `open-autonomy-0.9.1/autonomy/deploy/generators/docker_compose/templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # ------------------------------------------------------------------------------
 #
-#   Copyright 2021-2022 Valory AG
+#   Copyright 2021-2023 Valory AG
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -108,11 +108,13 @@
     environment:
       - PYTHONHASHSEED=0
       - LOG_FILE=/logs/aea_{node_id}.txt
 {agent_vars}
     networks:
       localnet:
         ipv4_address: 192.167.11.{localnet_address_postfix}
+    extra_hosts:
+      - "host.docker.internal:host-gateway"
     volumes:
       - ./persistent_data/logs:/logs:Z
       - ./agent_keys/agent_{node_id}:/agent_key:Z
 """
```

### Comparing `open-autonomy-0.9.0/autonomy/deploy/generators/kubernetes/__init__.py` & `open-autonomy-0.9.1/autonomy/deploy/generators/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/generators/kubernetes/base.py` & `open-autonomy-0.9.1/autonomy/deploy/generators/kubernetes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,19 +190,15 @@
         return self
 
     def write_config(
         self,
     ) -> "KubernetesGenerator":
         """Write output to build dir"""
 
-        if self.use_tm_testnet_setup:
-            output = "---\n".join([self.output, cast(str, self.tendermint_job_config)])
-        else:
-            output = self.output
-
+        output = "---\n".join([self.output, cast(str, self.tendermint_job_config)])
         if not self.build_dir.is_dir():  # pragma: no cover
             self.build_dir.mkdir()
         with open(
             self.build_dir / self.output_name, "w", encoding=DEFAULT_ENCODING
         ) as f:
             f.write(output)
```

### Comparing `open-autonomy-0.9.0/autonomy/deploy/generators/kubernetes/templates.py` & `open-autonomy-0.9.1/autonomy/deploy/generators/kubernetes/templates.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/deploy/image.py` & `open-autonomy-0.9.1/autonomy/deploy/image.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/__init__.py` & `open-autonomy-0.9.1/autonomy/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/__init__.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/base.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/constants.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/constants.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/generators/__init__.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/generators/components.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/generators/components.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/generators/tests.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/generators/tests.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/scaffold_skill.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/scaffold_skill.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/templates/__init__.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/templates/components.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/templates/components.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/fsm/scaffold/templates/tests.py` & `open-autonomy-0.9.1/autonomy/fsm/scaffold/templates/tests.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/replay/__init__.py` & `open-autonomy-0.9.1/autonomy/replay/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/replay/agent.py` & `open-autonomy-0.9.1/autonomy/replay/agent.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/replay/tendermint.py` & `open-autonomy-0.9.1/autonomy/replay/tendermint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/replay/utils.py` & `open-autonomy-0.9.1/autonomy/replay/utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/services/__init__.py` & `open-autonomy-0.9.1/autonomy/services/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/autonomy/services/scaffold/__init__.py` & `open-autonomy-0.9.1/autonomy/services/scaffold/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/autonomy/Dockerfile` & `open-autonomy-0.9.1/deployments/Dockerfiles/autonomy/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/autonomy/openssl.cnf` & `open-autonomy-0.9.1/deployments/Dockerfiles/autonomy/openssl.cnf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/autonomy-user/Dockerfile` & `open-autonomy-0.9.1/deployments/Dockerfiles/autonomy-user/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/documentation/Dockerfile` & `open-autonomy-0.9.1/deployments/Dockerfiles/documentation/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/Dockerfile` & `open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/app.py` & `open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/app.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/tendermint.py` & `open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/tendermint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/wait-for-it.sh` & `open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/Dockerfiles/tendermint/wrapper.sh` & `open-autonomy-0.9.1/deployments/Dockerfiles/tendermint/wrapper.sh`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/deployments/keys/hardhat_keys.json` & `open-autonomy-0.9.1/deployments/keys/hardhat_keys.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_analyse.md` & `open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_analyse.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_deploy.md` & `open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_deploy.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
 `--use-hardhat`
 :   Include a hardhat node in the deployment setup.
 
 `--use-acn`
 :   Include an ACN node in the deployment setup.
 
+`-ltm, --local-tm-setup`
+:   Use local tendermint chain setup.
+
 `--image-version TEXT`
 :   Define runtime image version.
 
 `--remote`
 :   To use a remote registry.
 
 `--local`
@@ -73,22 +76,20 @@
 
 `--help`
 :   Show the help message and exit.
 
 
 ### Examples
 ```bash
-autonomy deploy build keys.json
+autonomy deploy build keys.json -ltm
 ```
 
 Builds a service deployment using the keys stored in the file `keys.json` and applying environment variables to the service configuration file. The deployment will be generated by default for as many agents as keys are stored in `keys.json`. By default, the command searches for the file `keys.json`, if no file name is provided.
 
 
-
-
 ## `autonomy deploy run`
 
 Run a service deployment locally stored.
 
 This command is a wrapper around `docker-compose up` to run the service deployment. To execute this command you need to be located within the deployment environment subfolder (`./abci_build`), or specify it with the option `--build-dir`.
 
 ### Usage
```

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_fetch.md` & `open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_fetch.md`

 * *Files 7% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 Fetch the agent service `hello_world` from a local registry with an explicit path:
 ```bash
 autonomy --registry-path=./packages fetch valory/hello_world:0.1.0 --service --local
 ```
 
 Fetch the agent service `hello_world` from a remote registry ([IPFS](https://ipfs.io)):
 ```bash
-autonomy fetch valory/hello_world:0.1.0:bafybeidzmbyyyitioj4mz6xwlnqlvnmjwb5pzfw7qcpgtrv3ytozgbhnri --service --remote
+autonomy fetch valory/hello_world:0.1.0:bafybeiangkjd6y5jjpubeog25lggrmq3y64b2cqurhmxs26i4tddksbhiq --service --remote
 ```
```

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_mint.md` & `open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_mint.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_replay.md` & `open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_replay.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_scaffold.md` & `open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_scaffold.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/commands/autonomy_service.md` & `open-autonomy-0.9.1/docs/advanced_reference/commands/autonomy_service.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/benchmarking.md` & `open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/benchmarking.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/debugging_in_the_cluster.md` & `open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/debugging_in_the_cluster.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 Now, push the image  to make it accessible for the cluster to pull it. You can get the tag from the previous command:
 ```bash
 docker image push <tag>
 ```
 
 Finally, build the deployment and run it:
 ```bash
-autonomy deploy build  ../generated_keys.json --force --password ${PASSWORD} --kubernetes --dev
+autonomy deploy build  ../generated_keys.json --force --password ${PASSWORD} --kubernetes --dev -ltm
 kubectl apply -f abci_build/
 kubectl apply -f abci_build/agent_keys
 ```
 
 This will deploy a private hardhat container to the cluster, along with the associated agent service, configured to use the hardhat container.
```

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/dev_mode.md` & `open-autonomy-0.9.1/docs/guides/deploy_service.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,38 @@
-The {{open_autonomy}} framework comes with *dev mode* tooling to enable faster service developing and debugging. The dev mode supports running agent services with a number of functionalities enabled:
+Deploying a service with the {{open_autonomy}} framework requires that you have an already available service configuration, which you could be a service created from scratch, fetched from the [IPFS](https://ipfs.io/), or already registered in the on-chain protocol.
 
-* **Hot reload,** which enables hot code swapping and reflects changes on the agent code as well as on the local `open-aea` repository without rebuilding or restarting the containers manually.
-* **Execution replay** of a previous agent in the service.
-* **Benchmark** the performance of an agent service.
+## What you will learn
 
+In this guide, you will learn how to:
 
-Before starting this guide, ensure that your machine satisfies the framework requirements and that you have followed the [set up guide](../../guides/set_up.md). As a result you should have a Pipenv workspace folder.
+* Create a local deployment for testing purposes of
+  * a service stored in your machine.
+  * a service available in the on-chain registry.
+* Create a cloud deployment of a service.
 
-## Build and run an agent service in dev mode
+Before starting this guide, ensure that your machine satisfies the framework requirements and that you have followed the [set up guide](./set_up.md). As a result you should have a Pipenv workspace folder.
 
-This example is based on the Price Oracle service. The service requires a local Hardhat node. Open a dedicated terminal and run:
+## Local deployment
 
-```bash
-docker run -p 8545:8545 -it valory/open-autonomy-hardhat:0.1.0
-```
+Local deployments of a service are recommended to test your service before you publish it to a remote registry. Open a terminal and follow the steps below.
 
-Execute the next steps in a separate terminal.
-
-1. **Fetch the service.** Fetch the Price Oracle service from the remote registry.
-
-    ```bash
-    autonomy fetch valory/oracle_hardhat:0.1.0:<hash> --service
-    ```
-
-2. **Build the agents' image.** Navigate to the local folder of the service, and build the Docker image of the service agents in dev mode.
+1. **Build the agents' image.** Navigate to the local folder of the service that you want to deploy, that is, the folder containing the `service.yaml` file, and build the Docker image of the service agents:
 
     ```bash
-    cd oracle_hardhat
-    autonomy build-image --dev
+    cd <service_folder>
+    autonomy build-image
     ```
 
     After the command finishes building the image, you can see that it has been created by executing:
 
     ```bash
-    docker image ls | grep oracle_hardhat
+    docker image ls | grep <service_agent_name>
     ```
 
-3. **Prepare the keys file.** Within the service folder, prepare a JSON file `keys.json` containing the wallet address and the private key for each of the agents that make up the service.
+2. **Prepare the keys file.** Prepare a JSON file `keys.json` containing the wallet address and the private key for each of the agents that make up the service.
 
     ??? example "Example of a `keys.json` file"
 
         Find below an example of the structure of a `keys.json` file.
 
         <span style="color:red">**WARNING: Use this file for testing purposes only. Never use the keys or addresses provided in this example in a production environment or for personal use.**</span>
 
@@ -61,35 +53,77 @@
           {
               "address": "0x14dC79964da2C08b23698B3D3cc7Ca32193d9955",
               "private_key": "0x4bbbf85ce3377467afe5d46f804f221813b2bb87f24d81f60f1fcdbf7cbf4356"
           }
         ]
         ```
 
-4. **Build the deployment.** Within the service folder, execute the command below to build the service deployment in dev mode.
+3. **Build the deployment.** Within the service folder, execute the command below to build the service deployment.
 
     ```bash
-    autonomy deploy build keys.json --dev --packages-dir ~/git/open-autonomy/packages --open-autonomy-dir ~/git/open-aea/ --open-aea-dir ~/git/open-autonomy/
+    autonomy deploy build keys.json --aev -ltm
     ```
 
-    You must modify the paths in the command above aproppriately, pointing to:
+    This will create a deployment environment within the `./abci_build` folder with the following structure:
 
-    * the path to the local registry (/packages directory),
-    * the path to the local {{open_autonomy_repository}},
-    * the path to the local {{open_aea_repository}}.
-
-    This will create a deployment environment in dev mode within the `./abci_build` folder.
+    ```bash
+    abci_build/
+    ├── agent_keys
+    │   ├── agent_0
+    │   ├── agent_1
+    │   ├── agent_2
+    │   └── agent_3
+    ├── nodes
+    │   ├── node0
+    │   ├── node1
+    │   ├── node2
+    │   └── node3
+    ├── persistent_data
+    │   ├── benchmarks
+    │   ├── logs
+    │   ├── tm_state
+    │   └── venvs
+    └── docker-compose.yaml
+    ```
 
-5. **Run the service.** Navigate to the deployment environment folder (`./abci_build`) and run the deployment locally.
+4. **Run the service.** Navigate to the deployment environment folder (`./abci_build`) and run the deployment locally.
 
     ```bash
     cd abci_build
     autonomy deploy run
     ```
 
     You can cancel the local execution by pressing `Ctrl-C`.
 
-## Hot reload
+## On-chain deployment
+
+The {{open_autonomy}} framework provides a convenient interface for services that are [registered in the on-chain protocol](./register_packages_on_chain.md##register-a-service).
+
+  1. **Find the service ID.** Explore the [services section](https://protocol.autonolas.network/agents) of the protocol frontend, and note the ID of the service that you want to deploy. The service must be in [Deployed state](https://docs.autonolas.network/protocol/life_cycle_of_a_service/#deployed).
+
+  2. **Execute the service deployment.** Execute the following command
+
+    ```bash
+    autonomy deploy from-token <ID> keys.json --use-goerli
+    ```
+    where `keys.json` contains the addresses and keys of (some of) the registered agents in the service.
+
+!!! warning "Important"
+    When deploying a service registered on-chain, the framework automatically overrides a number of configuration arguments (under `setup`) in the agent containers with the values registered in the on-chain protocol:
+
+    === "skill.yaml"
+
+    ```yaml
+    (...)
+    models:
+      params:
+        args:
+          setup:
+            all_participants: # Overridden with the registered values
+            safe_contract_address: # Overridden with the registered values
+            consensus_threshold: # Overridden with the registered values
+    ```
 
-Once the agents are running, you can make changes to the agent's code as well as the local {{open_aea_repository}}, and it will trigger the service restart.
+## Cloud deployment
 
-The trigger is caused by any Python file closing in either the `open-autonomy/packages` or the `open-aea/` directory. So even if you haven't made any change and still want to restart the service, just open any Python file press `Ctrl+S` or save it from the file menu and it will trigger the restart.
+!!! info
+    This section will be added soon.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/execution_replay.md` & `open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/execution_replay.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/advanced_reference/developer_tooling/log_analysis.md` & `open-autonomy-0.9.1/docs/advanced_reference/developer_tooling/log_analysis.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/analyse/abci/app_spec.md` & `open-autonomy-0.9.1/docs/api/analyse/abci/app_spec.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/analyse/abci/docstrings.md` & `open-autonomy-0.9.1/docs/api/analyse/abci/docstrings.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/analyse/benchmark/aggregate.md` & `open-autonomy-0.9.1/docs/api/analyse/benchmark/aggregate.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/analyse/dialogues.md` & `open-autonomy-0.9.1/docs/api/analyse/dialogues.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/analyse/handlers.md` & `open-autonomy-0.9.1/docs/api/analyse/handlers.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/analyse/logs/collection.md` & `open-autonomy-0.9.1/docs/api/analyse/logs/collection.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/analyse/logs/db.md` & `open-autonomy-0.9.1/docs/api/analyse/logs/db.md`

 * *Files 17% similar despite different names*

```diff
@@ -86,25 +86,14 @@
 
 ```python
 def create(reset: bool = False) -> "AgentLogsDB"
 ```
 
 Create agent table
 
-<a id="autonomy.analyse.logs.db.AgentLogsDB.insert_one"></a>
-
-#### insert`_`one
-
-```python
-def insert_one(timestamp: datetime, log_level: str, message: str, period: int,
-               round_name: str, behaviour_name: str) -> "AgentLogsDB"
-```
-
-Insert a record
-
 <a id="autonomy.analyse.logs.db.AgentLogsDB.insert_many"></a>
 
 #### insert`_`many
 
 ```python
 def insert_many(logs: Iterator[LogRow]) -> "AgentLogsDB"
 ```
```

### Comparing `open-autonomy-0.9.0/docs/api/analyse/service.md` & `open-autonomy-0.9.1/docs/api/analyse/service.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/chain/base.md` & `open-autonomy-0.9.1/docs/api/chain/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/chain/config.md` & `open-autonomy-0.9.1/docs/api/chain/config.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/chain/exceptions.md` & `open-autonomy-0.9.1/docs/api/chain/exceptions.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/chain/metadata.md` & `open-autonomy-0.9.1/docs/api/chain/metadata.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/chain/mint.md` & `open-autonomy-0.9.1/docs/api/chain/mint.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/chain/service.md` & `open-autonomy-0.9.1/docs/api/chain/service.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/chain/utils.md` & `open-autonomy-0.9.1/docs/api/chain/utils.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/analyse.md` & `open-autonomy-0.9.1/docs/api/cli/analyse.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/build_images.md` & `open-autonomy-0.9.1/docs/api/cli/build_images.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/deploy.md` & `open-autonomy-0.9.1/docs/api/cli/deploy.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/develop.md` & `open-autonomy-0.9.1/docs/api/cli/develop.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/fetch.md` & `open-autonomy-0.9.1/docs/api/cli/fetch.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/hash.md` & `open-autonomy-0.9.1/docs/api/cli/hash.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/helpers/analyse.md` & `open-autonomy-0.9.1/docs/api/cli/helpers/analyse.md`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,25 @@
 ```python
 @property
 def agents() -> List[str]
 ```
 
 Available agents.
 
+<a id="autonomy.cli.helpers.analyse.ParseLogs.n_agents"></a>
+
+#### n`_`agents
+
+```python
+@property
+def n_agents() -> int
+```
+
+Available agents.
+
 <a id="autonomy.cli.helpers.analyse.ParseLogs.from_dir"></a>
 
 #### from`_`dir
 
 ```python
 def from_dir(logs_dir: Path) -> "ParseLogs"
 ```
@@ -87,16 +98,16 @@
 Create required tables.
 
 <a id="autonomy.cli.helpers.analyse.ParseLogs.select"></a>
 
 #### select
 
 ```python
-def select(agents: List[str], start_time: Optional[Union[str, datetime]],
-           end_time: Optional[Union[str, datetime]], log_level: Optional[str],
+def select(agents: List[str], start_time: Optional[datetime],
+           end_time: Optional[datetime], log_level: Optional[str],
            period: Optional[int], round_name: Optional[str],
            behaviour_name: Optional[str]) -> "ParseLogs"
 ```
 
 Query and return results.
 
 <a id="autonomy.cli.helpers.analyse.ParseLogs.re_include"></a>
```

### Comparing `open-autonomy-0.9.0/docs/api/cli/helpers/chain.md` & `open-autonomy-0.9.1/docs/api/cli/helpers/chain.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/helpers/deployment.md` & `open-autonomy-0.9.1/docs/api/cli/helpers/deployment.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/helpers/docstring.md` & `open-autonomy-0.9.1/docs/api/cli/helpers/docstring.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/helpers/fsm_spec.md` & `open-autonomy-0.9.1/docs/api/cli/helpers/fsm_spec.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/helpers/ipfs_hash.md` & `open-autonomy-0.9.1/docs/api/cli/helpers/ipfs_hash.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/helpers/registry.md` & `open-autonomy-0.9.1/docs/api/cli/helpers/registry.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/mint.md` & `open-autonomy-0.9.1/docs/api/cli/mint.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/packages.md` & `open-autonomy-0.9.1/docs/api/cli/packages.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/publish.md` & `open-autonomy-0.9.1/docs/api/cli/publish.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/push_all.md` & `open-autonomy-0.9.1/docs/api/cli/push_all.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/replay.md` & `open-autonomy-0.9.1/docs/api/cli/replay.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/scaffold_fsm.md` & `open-autonomy-0.9.1/docs/api/cli/scaffold_fsm.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/service.md` & `open-autonomy-0.9.1/docs/api/cli/service.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/cli/utils/click_utils.md` & `open-autonomy-0.9.1/docs/api/cli/utils/click_utils.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/configurations/base.md` & `open-autonomy-0.9.1/docs/api/configurations/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/configurations/validation.md` & `open-autonomy-0.9.1/docs/api/configurations/validation.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/check_dependencies.md` & `open-autonomy-0.9.1/docs/api/connections/abci/check_dependencies.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/dialogues.md` & `open-autonomy-0.9.1/docs/api/connections/abci/dialogues.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/scripts/genproto.md` & `open-autonomy-0.9.1/docs/api/connections/abci/scripts/genproto.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/tendermint_decoder.md` & `open-autonomy-0.9.1/docs/api/connections/abci/tendermint_decoder.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/tendermint_encoder.md` & `open-autonomy-0.9.1/docs/api/connections/abci/tendermint_encoder.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/tests/helper.md` & `open-autonomy-0.9.1/docs/api/connections/abci/tests/helper.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/base.md` & `open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/connections/abci/tests/test_fuzz/mock_node/node.md` & `open-autonomy-0.9.1/docs/api/connections/abci/tests/test_fuzz/mock_node/node.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/contracts/gnosis_safe/contract.md` & `open-autonomy-0.9.1/docs/api/contracts/gnosis_safe/contract.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/contracts/gnosis_safe_proxy_factory/contract.md` & `open-autonomy-0.9.1/docs/api/contracts/gnosis_safe_proxy_factory/contract.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/data/Dockerfiles/dev/watcher.md` & `open-autonomy-0.9.1/docs/api/data/Dockerfiles/dev/watcher.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/deploy/base.md` & `open-autonomy-0.9.1/docs/api/deploy/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/deploy/build.md` & `open-autonomy-0.9.1/docs/api/deploy/build.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/deploy/generators/docker_compose/base.md` & `open-autonomy-0.9.1/docs/api/deploy/generators/docker_compose/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/deploy/generators/kubernetes/base.md` & `open-autonomy-0.9.1/docs/api/deploy/generators/kubernetes/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/deploy/image.md` & `open-autonomy-0.9.1/docs/api/deploy/image.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/fsm/scaffold/base.md` & `open-autonomy-0.9.1/docs/api/fsm/scaffold/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/fsm/scaffold/generators/components.md` & `open-autonomy-0.9.1/docs/api/fsm/scaffold/generators/components.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/fsm/scaffold/generators/tests.md` & `open-autonomy-0.9.1/docs/api/fsm/scaffold/generators/tests.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/fsm/scaffold/scaffold_skill.md` & `open-autonomy-0.9.1/docs/api/fsm/scaffold/scaffold_skill.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/fsm/scaffold/templates/components.md` & `open-autonomy-0.9.1/docs/api/fsm/scaffold/templates/components.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/fsm/scaffold/templates/tests.md` & `open-autonomy-0.9.1/docs/api/fsm/scaffold/templates/tests.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/base_test_classes/agents.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/base_test_classes/agents.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/base_test_classes/contracts.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/base_test_classes/contracts.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/acn_node.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/acn_node.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/amm_net.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/amm_net.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/base.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/ganache.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/ganache.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/gnosis_safe_net.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/gnosis_safe_net.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/registries.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/registries.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/docker/tendermint.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/docker/tendermint.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/fixture_helpers.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/fixture_helpers.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/async_utils.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/async_utils.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/base.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/plugins/aea_test_autonomy/helpers/tendermint_utils.md` & `open-autonomy-0.9.1/docs/api/plugins/aea_test_autonomy/helpers/tendermint_utils.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/protocols/abci/custom_types.md` & `open-autonomy-0.9.1/docs/api/protocols/abci/custom_types.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/protocols/abci/dialogues.md` & `open-autonomy-0.9.1/docs/api/protocols/abci/dialogues.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/protocols/abci/message.md` & `open-autonomy-0.9.1/docs/api/protocols/abci/message.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/protocols/abci/serialization.md` & `open-autonomy-0.9.1/docs/api/protocols/abci/serialization.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/replay/agent.md` & `open-autonomy-0.9.1/docs/api/replay/agent.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/replay/tendermint.md` & `open-autonomy-0.9.1/docs/api/replay/tendermint.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/replay/utils.md` & `open-autonomy-0.9.1/docs/api/replay/utils.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_abci/dialogues.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_abci/dialogues.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_abci/handlers.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_abci/handlers.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/abci_app_chain.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/abci_app_chain.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/base.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/behaviours.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/behaviours.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/dialogues.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/dialogues.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/handlers.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/handlers.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/ipfs.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/ipfs.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/load.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/load.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/io_/store.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/io_/store.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/models.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/models.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/abci_app.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/abci_app.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/base.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/common.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/common.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/integration.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/integration.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/test_tools/rounds.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/test_tools/rounds.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/payloads.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/payloads.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/rounds.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/data/dummy_abci/rounds.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/tests/test_tools/base.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/tests/test_tools/base.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/abstract_round_abci/utils.md` & `open-autonomy-0.9.1/docs/api/skills/abstract_round_abci/utils.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/registration_abci/behaviours.md` & `open-autonomy-0.9.1/docs/api/skills/registration_abci/behaviours.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/registration_abci/rounds.md` & `open-autonomy-0.9.1/docs/api/skills/registration_abci/rounds.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/behaviours.md` & `open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/behaviours.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/models.md` & `open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/models.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/payload_tools.md` & `open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/payload_tools.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/payloads.md` & `open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/payloads.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/rounds.md` & `open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/rounds.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/api/skills/transaction_settlement_abci/test_tools/integration.md` & `open-autonomy-0.9.1/docs/api/skills/transaction_settlement_abci/test_tools/integration.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/application_deployment.md` & `open-autonomy-0.9.1/docs/application_deployment.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                                   Logging level for runtime.
   --packages-dir PATH             Path to packages dir (Use with dev mode)
   --open-aea-dir PATH             Path to open-aea repo (Use with dev mode)
   --open-autonomy-dir PATH        Path to open-autonomy repo (Use with dev
                                   mode)
   --aev                           Apply environment variable when loading
                                   service config.
+  -ltm, --local-tm-setup          Use local tendermint chain setup.
   --image-version TEXT            Define runtime image version.
   --remote                        To use a remote registry.
   --local                         To use a local registry.
   -p                              Ask for password interactively
   --password PASSWORD             Set password for key encryption/decryption
   --help                          Show this message and exit.
```

### Comparing `open-autonomy-0.9.0/docs/control_flow.md` & `open-autonomy-0.9.1/docs/control_flow.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/counter_example.md` & `open-autonomy-0.9.1/docs/counter_example.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 The steps below will guide you to download the counter agent service configuration from the Service Registry, build and run a deployment that will run locally.
 
 1. Ensure that your machine satisfies the [framework requirements](guides/quick_start.md#requirements) and that
 you have followed the [setup instructions](guides/quick_start.md#setup). As a result you should have a Pipenv workspace folder.
 
 2. Use the CLI to download the `valory/counter` service.
     ```bash
-    autonomy fetch valory/counter:0.1.0:bafybeiedev5vi5bxkx53fsbqy54onrdtdjq64hkz7b2pzoqw64y2qmzefe --remote --service
+    autonomy fetch valory/counter:0.1.0:bafybeihnd72avnqtn5ig6ikuxge2kgcoo2clt5bxqo3ar4mesdg7s7744q --remote --service
     cd counter
     ```
 
 3. Inside the workspace folder, create a JSON file `keys.json` containing the addresses and keys of the four agents that are
    part of this demo. Below you have a sample `keys.json` file that you can use for testing.
 
     !!! warning "Important"
@@ -60,15 +60,15 @@
     ```bash
     autonomy build-image
     ```
     The command above generates the required images to run the agent service.
 
 5. Build a deployment setup for the demo service:
     ```bash
-    autonomy deploy build keys.json
+    autonomy deploy build keys.json -ltm
     ```
 
     This will build the deployment setup required to run the service locally.
     !!!note
         It is also possible to generate a deployment using a local service configuration. See the Commands section for the complete details.
 
 6. The build configuration will be located in `./abci_build`. Run the deployment using
```

### Comparing `open-autonomy-0.9.0/docs/debugging.md` & `open-autonomy-0.9.1/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/demos/hello_world_demo.md` & `open-autonomy-0.9.1/docs/demos/hello_world_demo.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/demos/index.md` & `open-autonomy-0.9.1/docs/demos/index.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/demos/price_oracle_fsms.md` & `open-autonomy-0.9.1/docs/demos/price_oracle_fsms.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/demos/price_oracle_intro.md` & `open-autonomy-0.9.1/docs/demos/price_oracle_intro.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/demos/price_oracle_technical_details.md` & `open-autonomy-0.9.1/docs/demos/price_oracle_technical_details.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/deployment/on-chain_deployment_checklist.md` & `open-autonomy-0.9.1/docs/deployment/on-chain_deployment_checklist.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/ethereum_specifics.md` & `open-autonomy-0.9.1/docs/ethereum_specifics.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/exceptions.md` & `open-autonomy-0.9.1/docs/exceptions.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Bold.ttf` & `open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Bold.ttf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-ExtraBold.ttf` & `open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-ExtraLight.ttf` & `open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Light.ttf` & `open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Light.ttf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Medium.ttf` & `open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Medium.ttf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-Regular.ttf` & `open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/Manrope-SemiBold.ttf` & `open-autonomy-0.9.1/docs/fonts/Manrope/Manrope-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/fonts/Manrope/stylesheet.css` & `open-autonomy-0.9.1/docs/fonts/Manrope/stylesheet.css`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/get_started/agent_services_compared_to.md` & `open-autonomy-0.9.1/docs/get_started/agent_services_compared_to.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/get_started/use_cases.md` & `open-autonomy-0.9.1/docs/get_started/use_cases.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/get_started/what_is_an_agent_service.md` & `open-autonomy-0.9.1/docs/get_started/what_is_an_agent_service.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/get_started/why_do_we_need_agent_services.md` & `open-autonomy-0.9.1/docs/get_started/why_do_we_need_agent_services.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/configure_access_external_chains.md` & `open-autonomy-0.9.1/docs/guides/configure_access_external_chains.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/create_fsm_app.md` & `open-autonomy-0.9.1/docs/guides/create_fsm_app.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/create_service_existing_agent.md` & `open-autonomy-0.9.1/docs/guides/create_service_existing_agent.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/create_service_from_scratch.md` & `open-autonomy-0.9.1/docs/guides/create_service_from_scratch.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/index.md` & `open-autonomy-0.9.1/docs/guides/index.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/overview_of_the_development_process.md` & `open-autonomy-0.9.1/docs/guides/overview_of_the_development_process.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/publish_fetch_packages.md` & `open-autonomy-0.9.1/docs/guides/publish_fetch_packages.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/quick_start.md` & `open-autonomy-0.9.1/docs/guides/quick_start.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     On **MacOS** and **Windows**, running Docker containers requires having Docker Desktop running as well. If you're using one of those operating systems, remember to start Docker Desktop
     before you run agent services.
 
 Now that you have set up your machine to work with {{open_autonomy}}, we are in position to use the CLI to fetch the agent service from the remote registry and deploy it locally.
 
 1. Use the CLI to fetch the [Hello World agent service](../demos/hello_world_demo.md). This will connect to the remote registry and download the files that make up the service to the `hello_world` folder:
     ```bash
-    autonomy fetch valory/hello_world:0.1.0:bafybeidzmbyyyitioj4mz6xwlnqlvnmjwb5pzfw7qcpgtrv3ytozgbhnri --service
+    autonomy fetch valory/hello_world:0.1.0:bafybeiangkjd6y5jjpubeog25lggrmq3y64b2cqurhmxs26i4tddksbhiq --service
     cd hello_world
     ```
 
 2. Build the Docker image of the service agents:
     ```bash
     autonomy build-image
     ```
@@ -54,15 +54,15 @@
               "private_key": "0x4bbbf85ce3377467afe5d46f804f221813b2bb87f24d81f60f1fcdbf7cbf4356"
           }
         ]
         ```
 
 4. Build the deployment setup for the service:
     ```bash
-    autonomy deploy build keys.json --aev
+    autonomy deploy build keys.json --aev -ltm
     ```
 
 5. Navigate to the deployment environment folder (`./abci_build`) and run the deployment locally using
     ```bash
     cd abci_build
     autonomy deploy run
     ```
```

### Comparing `open-autonomy-0.9.0/docs/guides/register_packages_on_chain.md` & `open-autonomy-0.9.1/docs/guides/register_packages_on_chain.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/service_configuration_file.md` & `open-autonomy-0.9.1/docs/guides/service_configuration_file.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/guides/set_up.md` & `open-autonomy-0.9.1/docs/guides/set_up.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/abci_requests.svg` & `open-autonomy-0.9.1/docs/images/abci_requests.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/agent_service_architecture.svg` & `open-autonomy-0.9.1/docs/images/agent_service_architecture.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/agent_service_index_page.svg` & `open-autonomy-0.9.1/docs/images/agent_service_index_page.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/centralized_decentralized_world.svg` & `open-autonomy-0.9.1/docs/images/centralized_decentralized_world.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/counter_diagram.svg` & `open-autonomy-0.9.1/docs/images/counter_diagram.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/development-process-simplified.svg` & `open-autonomy-0.9.1/docs/images/development-process-simplified.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/development_process.svg` & `open-autonomy-0.9.1/docs/images/development_process.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/development_process_create_fsm_app.svg` & `open-autonomy-0.9.1/docs/images/development_process_create_fsm_app.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/development_process_create_service_existing_agent.svg` & `open-autonomy-0.9.1/docs/images/development_process_create_service_existing_agent.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/development_process_define_service.svg` & `open-autonomy-0.9.1/docs/images/development_process_define_service.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/development_process_publish_fetch_packages.svg` & `open-autonomy-0.9.1/docs/images/development_process_publish_fetch_packages.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/development_process_register_packages_on_chain.svg` & `open-autonomy-0.9.1/docs/images/development_process_register_packages_on_chain.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/do_name_servers.png` & `open-autonomy-0.9.1/docs/images/do_name_servers.png`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/fsm.svg` & `open-autonomy-0.9.1/docs/images/fsm.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/fsm_composition.svg` & `open-autonomy-0.9.1/docs/images/fsm_composition.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/fsm_composition_2.svg` & `open-autonomy-0.9.1/docs/images/fsm_composition_2.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_action.svg` & `open-autonomy-0.9.1/docs/images/hello_world_action.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_agent_internal.svg` & `open-autonomy-0.9.1/docs/images/hello_world_agent_internal.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_demo_architecture.svg` & `open-autonomy-0.9.1/docs/images/hello_world_demo_architecture.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_demo_architecture_simplified.svg` & `open-autonomy-0.9.1/docs/images/hello_world_demo_architecture_simplified.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_fsm.svg` & `open-autonomy-0.9.1/docs/images/hello_world_fsm.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_result.svg` & `open-autonomy-0.9.1/docs/images/hello_world_result.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_sequence_1.svg` & `open-autonomy-0.9.1/docs/images/hello_world_sequence_1.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_sequence_2.svg` & `open-autonomy-0.9.1/docs/images/hello_world_sequence_2.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_sequence_3.svg` & `open-autonomy-0.9.1/docs/images/hello_world_sequence_3.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_sequence_4.svg` & `open-autonomy-0.9.1/docs/images/hello_world_sequence_4.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_sequence_5.svg` & `open-autonomy-0.9.1/docs/images/hello_world_sequence_5.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/hello_world_zoom_agent.svg` & `open-autonomy-0.9.1/docs/images/hello_world_zoom_agent.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/name_server_setup.png` & `open-autonomy-0.9.1/docs/images/name_server_setup.png`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/networking_page.png` & `open-autonomy-0.9.1/docs/images/networking_page.png`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/open-autonomy-framework-logo.png` & `open-autonomy-0.9.1/docs/images/open-autonomy-framework-logo.png`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/oracle_composition.svg` & `open-autonomy-0.9.1/docs/images/oracle_composition.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/oracle_diagram.svg` & `open-autonomy-0.9.1/docs/images/oracle_diagram.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/package_management.svg` & `open-autonomy-0.9.1/docs/images/package_management.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/register_package.svg` & `open-autonomy-0.9.1/docs/images/register_package.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/service-level_overrides.svg` & `open-autonomy-0.9.1/docs/images/service-level_overrides.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/simple_demo_architecture.svg` & `open-autonomy-0.9.1/docs/images/simple_demo_architecture.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/simplified-aea.svg` & `open-autonomy-0.9.1/docs/images/simplified-aea.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/skill-components.svg` & `open-autonomy-0.9.1/docs/images/skill-components.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/tendermint.svg` & `open-autonomy-0.9.1/docs/images/tendermint.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/images/tendermint_transaction.svg` & `open-autonomy-0.9.1/docs/images/tendermint_transaction.svg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/index.md` & `open-autonomy-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/abci.md` & `open-autonomy-0.9.1/docs/key_concepts/abci.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/abci_app_abstract_round.md` & `open-autonomy-0.9.1/docs/key_concepts/abci_app_abstract_round.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/abci_app_abstract_round_behaviour.md` & `open-autonomy-0.9.1/docs/key_concepts/abci_app_abstract_round_behaviour.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/abci_app_async_behaviour.md` & `open-autonomy-0.9.1/docs/key_concepts/abci_app_async_behaviour.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/abci_app_class.md` & `open-autonomy-0.9.1/docs/key_concepts/abci_app_class.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/abci_app_interactions.md` & `open-autonomy-0.9.1/docs/key_concepts/abci_app_interactions.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/aea.md` & `open-autonomy-0.9.1/docs/key_concepts/aea.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/fsm.md` & `open-autonomy-0.9.1/docs/key_concepts/fsm.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/fsm_app_components.md` & `open-autonomy-0.9.1/docs/key_concepts/fsm_app_components.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/fsm_app_introduction.md` & `open-autonomy-0.9.1/docs/key_concepts/fsm_app_introduction.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/index.md` & `open-autonomy-0.9.1/docs/key_concepts/index.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/poc-diagram.md` & `open-autonomy-0.9.1/docs/key_concepts/poc-diagram.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/key_concepts/threat_model.md` & `open-autonomy-0.9.1/docs/key_concepts/threat_model.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/package_list.md` & `open-autonomy-0.9.1/docs/package_list.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 | Package name                                                  | Package hash                                                  |
 | ------------------------------------------------------------- | ------------------------------------------------------------- |
 | protocol/valory/abci/0.1.0                                    | `bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4` |
-| connection/valory/abci/0.1.0                                  | `bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a` |
+| connection/valory/abci/0.1.0                                  | `bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey` |
 | connection/valory/ipfs/0.1.0                                  | `bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu` |
-| contract/valory/gnosis_safe_proxy_factory/0.1.0               | `bafybeieuivicfjkow3asmrj57mygrqbvjnecxqaybyxf6egktdty7qxac4` |
+| contract/valory/gnosis_safe_proxy_factory/0.1.0               | `bafybeidzdv6zjst5likperhuqdzsb4yix6ey5ir45nwdcquw3asuqmqdlu` |
 | contract/valory/component_registry/0.1.0                      | `bafybeialw5eaa4v54s7i3sjsuy6d5k624quhxhziqntwq5hnz4g646sb7m` |
 | contract/valory/agent_registry/0.1.0                          | `bafybeibkj4pm6ziqh2fl3xfsjiou4ibnxlipmvmqhgvc7xwpnaddbtxzli` |
 | contract/valory/registries_manager/0.1.0                      | `bafybeighjuqdj2oq6tqckf7j3mqtighe7lpaahh7qt3sqxtbtjlur4tmj4` |
 | contract/valory/service_manager/0.1.0                         | `bafybeiea3bophgb6ikqvpd7lzyluthlhoazbbrknvfncu4j7wbubfsrjeu` |
-| skill/valory/test_ipfs_abci/0.1.0                             | `bafybeiasijop7eizwyxbwxnkh4iiitk6banuxz5u3bn7ijdvkzm77xtgju` |
-| agent/valory/test_ipfs/0.1.0                                  | `bafybeidtrr73c72kbrkpn6tjsichjy6ge4qg36arelw4ufonseqyhcmwau` |
-| contract/valory/service_registry/0.1.0                        | `bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi` |
+| skill/valory/test_ipfs_abci/0.1.0                             | `bafybeicxpeo5ypjvu367pksuufsrza4cngxl4nncdido53r3ryovwmvxfy` |
+| agent/valory/test_ipfs/0.1.0                                  | `bafybeibixyacbe3hr7nhv4lnumvhhljy7p6ys7itfkqhhtiyjkvavjj5ou` |
+| contract/valory/service_registry/0.1.0                        | `bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi` |
 | protocol/valory/tendermint/0.1.0                              | `bafybeicusvezoqlmyt6iqomcbwaz3xkhk2qf3d56q5zprmj3xdxfy64k54` |
 | protocol/valory/ipfs/0.1.0                                    | `bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4` |
-| skill/valory/abstract_abci/0.1.0                              | `bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti` |
-| contract/valory/gnosis_safe/0.1.0                             | `bafybeihwwv5aodluykglsbuhhrwusvjof6vvnr37rznwvlutmfwtvoju34` |
-| skill/valory/abstract_round_abci/0.1.0                        | `bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi` |
+| skill/valory/abstract_abci/0.1.0                              | `bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou` |
+| contract/valory/gnosis_safe/0.1.0                             | `bafybeibzfhpib5fw3wady6dhq5bfgo37o437bi4s3hthbvvit7byvbalg4` |
+| skill/valory/abstract_round_abci/0.1.0                        | `bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4` |
 | contract/valory/multisend/0.1.0                               | `bafybeigjywkl7hydjsrkogob3xebj2ifhqwmfhhxoeyrndzhhxi5u6amey` |
-| skill/valory/transaction_settlement_abci/0.1.0                | `bafybeiajvxzaeeeamvb3guxtihlrj7xoyrmfeuo5chp4f3pdd2sgiecayq` |
-| skill/valory/registration_abci/0.1.0                          | `bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq` |
-| skill/valory/reset_pause_abci/0.1.0                           | `bafybeic6ayed23np6ngkawsf2you6nnfuvbq4smcepdvvcrw5wxn5jaevy` |
-| skill/valory/termination_abci/0.1.0                           | `bafybeigg4eyjaeidojnvxdenztaywb7ijtjdtjirpc6pvhglscfqdhfupe` |
-| skill/valory/counter/0.1.0                                    | `bafybeied3rhikmiulc2qdwl3lfyw3kgvsrpz674epoaulrn2zrbfdu23ra` |
+| skill/valory/transaction_settlement_abci/0.1.0                | `bafybeiftbgfzp36bknbwus3fx2equmhgmboy4qd5myex76xfc4ze6o7b54` |
+| skill/valory/registration_abci/0.1.0                          | `bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya` |
+| skill/valory/reset_pause_abci/0.1.0                           | `bafybeievxhu6u5r5wlpjfzcwuowlbanhfbi25saf25qit53jauv4kq6gne` |
+| skill/valory/termination_abci/0.1.0                           | `bafybeihpp4li6jw3co4c4jferrtzobq2ydoc3dcn67esqrg5ebvyoac66e` |
+| skill/valory/counter/0.1.0                                    | `bafybeibzjqpzumbj2ts6lh6mgfj2t2mabgq25qrdhubbwjonnxwnhcj3cu` |
 | skill/valory/counter_client/0.1.0                             | `bafybeiaqdfulxamdshw7fykfkqvkpvjb5bnmhv7ffrjiwdi4ktiulklx6q` |
-| skill/valory/hello_world_abci/0.1.0                           | `bafybeiagih5lel6ccikc6d36r5mntzj374x6brxt4a62bqa23w7khorcte` |
-| skill/valory/register_reset_abci/0.1.0                        | `bafybeifezziaezqhqmbyvee26sw5wkrwsc3wlmas7c2vvghe7xwyxycpey` |
-| skill/valory/register_termination_abci/0.1.0                  | `bafybeigkwb3rp7rwv2jjcep6z5zma5muu2ulm65oxo6yhispponchcvor4` |
-| skill/valory/test_abci/0.1.0                                  | `bafybeickt7snjkd2365nyr7r2xjozxwaiy2swcy6xh6hstleam6ouujctu` |
-| agent/valory/abstract_abci/0.1.0                              | `bafybeig5qj4huxbj2g2vf27vliyrnu6kmr3cpxfmqaslzakb43xd7l3jzq` |
-| agent/valory/counter/0.1.0                                    | `bafybeiaabwbh5oerjritw6ucqseh2sqirfhxnlnm6vlst2jh2qhgrucmxa` |
+| skill/valory/hello_world_abci/0.1.0                           | `bafybeidhftdlf24itdpzs456btixret4deeis35jdqesh3xo54ukxegdrq` |
+| skill/valory/register_reset_abci/0.1.0                        | `bafybeigda2s3nouoehbttbcyewhdolngq4m5ibnwr2driell2ufustgxga` |
+| skill/valory/register_termination_abci/0.1.0                  | `bafybeih67ylxwvmc7wamw2sjkfd77zglovqn2gziwewlgeo6pndhonbkyu` |
+| skill/valory/test_abci/0.1.0                                  | `bafybeibsosoucoq6oiohxrpzllen63r6ul5q7ne2kwfvnp44sw43cpeady` |
+| agent/valory/abstract_abci/0.1.0                              | `bafybeib4o2zojkbk4kympvyahbhezzbmcottzk7cmnr6yosoiruwr4ze5i` |
+| agent/valory/counter/0.1.0                                    | `bafybeidkwjanxwjnx74gpmm4x4nvevif5bhofyunyhsi6r2qtzxsqnsafq` |
 | agent/valory/counter_client/0.1.0                             | `bafybeicv6jsvvhvtzizko7eewukcfkg3is5dzn47l5ylgvdo4dzjof5inu` |
-| agent/valory/hello_world/0.1.0                                | `bafybeifcl3izwfurgxdbhf4n4mu2jv5vlj5vygw6bgjlcjj66wsxefc7ry` |
-| agent/valory/register_reset/0.1.0                             | `bafybeid6i5jpihanjzfaykdgbwb5kg3y6fwdps62ivhpzd5mbldmzxgxai` |
-| agent/valory/register_termination/0.1.0                       | `bafybeifynadq24eche7jkfcbiybxr2kvkjgtj5oeueurlejswxcepy5gvq` |
-| agent/valory/registration_start_up/0.1.0                      | `bafybeidvebjdpignfsgv7sp6ux6bl444afvpmiiblzb7kr5qx6v3uioiwi` |
-| agent/valory/test_abci/0.1.0                                  | `bafybeia5f4zmb6judsbicwkzvf7udqj5o4t7epegywir3ivmybicztr434` |
-| service/valory/counter/0.1.0                                  | `bafybeiedev5vi5bxkx53fsbqy54onrdtdjq64hkz7b2pzoqw64y2qmzefe` |
-| service/valory/hello_world/0.1.0                              | `bafybeidzmbyyyitioj4mz6xwlnqlvnmjwb5pzfw7qcpgtrv3ytozgbhnri` |
-| service/valory/register_reset/0.1.0                           | `bafybeidd7jjkgptascvegeelkvympjam5gvmsogvphlh5d7jalvznv7tr4` |
-| skill/valory/register_reset_recovery_abci/0.1.0               | `bafybeicmyjgiogc3dmc6iwryxbhwzs4pxnymgoqihpp7ibvs6xmkvzdzwm` |
-| agent/valory/register_reset_recovery/0.1.0                    | `bafybeiannsxcsd5b3nwwxifyj5ihio4pkaexdzfgfdnwnkflksmgdwc42i` |
+| agent/valory/hello_world/0.1.0                                | `bafybeic3czcb7fpzru3fl4noxdwgwyzirqk6cqh763h6aio7ugl6qm5gha` |
+| agent/valory/register_reset/0.1.0                             | `bafybeibjuczg4bpkpt5m26mdeolg5ooh6wfsfhm3e5xsmmw3th6nsawsne` |
+| agent/valory/register_termination/0.1.0                       | `bafybeig4yehd4oseko3pbp6x23h7qmmcvckro66uw5hpecezcslygtjtym` |
+| agent/valory/registration_start_up/0.1.0                      | `bafybeied4jwpijvcudlvu3h63gwvkdr4cnazcjk3b335ibgdjpkq4llrn4` |
+| agent/valory/test_abci/0.1.0                                  | `bafybeid2daa6abk4z42so7bbpbgy6mgfrxwa5upjmayf5jw3ej2du2ozqa` |
+| service/valory/counter/0.1.0                                  | `bafybeihnd72avnqtn5ig6ikuxge2kgcoo2clt5bxqo3ar4mesdg7s7744q` |
+| service/valory/hello_world/0.1.0                              | `bafybeiangkjd6y5jjpubeog25lggrmq3y64b2cqurhmxs26i4tddksbhiq` |
+| service/valory/register_reset/0.1.0                           | `bafybeig2hgffe3nijhr6wlia2sluzt4p2al63faqxrriwpss4y5gutqbj4` |
+| skill/valory/register_reset_recovery_abci/0.1.0               | `bafybeienpr3zxuddgfwuqpgdc32qez6tdldluka6t4dwyltyx2twy6toze` |
+| agent/valory/register_reset_recovery/0.1.0                    | `bafybeicyxwchnbuqmbr3tvbesd7me4xpeuesgj7oo4wjwppkpcq6qgc7fq` |
 | contract/valory/multicall2/0.1.0                              | `bafybeiaegx2j5w6le2fhvzmx7stzujuezqfvicvnyqebtipivkek2cgh7m` |
 | protocol/open_aea/signing/1.0.0                               | `bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4` |
 | protocol/valory/acn/1.1.0                                     | `bafybeignmc5uh3vgpuckljcj2tgg7hdqyytkm6m5b6v6mxtazdcvubibva` |
 | protocol/valory/http/1.0.0                                    | `bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty` |
 | protocol/valory/ledger_api/1.0.0                              | `bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom` |
 | protocol/valory/contract_api/1.0.0                            | `bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy` |
 | connection/valory/http_client/0.23.0                          | `bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi` |
-| connection/valory/ledger/0.19.0                               | `bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi` |
+| connection/valory/ledger/0.19.0                               | `bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui` |
 | connection/valory/p2p_libp2p_client/0.1.0                     | `bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva` |
```

### Comparing `open-autonomy-0.9.0/docs/questions-and-answers.md` & `open-autonomy-0.9.1/docs/questions-and-answers.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/stylesheets/extra.css` & `open-autonomy-0.9.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/docs/upgrading.md` & `open-autonomy-0.9.1/docs/upgrading.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 This page provides some tips on how to upgrade agent services between different versions of the {{open_autonomy}} framework. For full release notes check the <a href="https://github.com/valory-xyz/open-autonomy/tags" target="_blank">Open-Autonomy repo</a>.
 
 Below we describe the additional manual steps required to upgrade between different versions:
 
 
 # Open Autonomy
 
+## `v0.9.0` to `v0.9.1`
+
+No backwards incompatible changes
+
 ## `v0.8.0` to `v0.9.0`
 
 Breaking changes
 
 - On the skill configuration
-  - The `max_participants` parameter has been removed
+  - The `max_participants` parameter has been removed. If the `consensus` configuration is empty after removing `max_participants`, it should be removed as well.
   - The `consensus_threshold` should now be specified in the `setup` parameters. If `null`, the recommended setting, then it is calculated automatically from the participants provided.
 - The synchronized database is now `serializable` and `hashable`. This means that the data inserted into the database are now enforced to be primitive or non-primitive built-in types only, except for `sets` and `frozensets` since an error is raised as they cannot be `serialized`/`hashed` and therefore cannot be inserted into the database. In essence, the data should be `json serializable`.
 - The usage of local Tendermint Consensus Gadget is optional in the deployment setup, use `-ltm, --local-tm-setup` when building a deployment using `autonomy deploy build` command to include a Tendermint Consensus Gadget setup.
 - The `cross_period_persisted_keys` and database conditions needs to be defined as sets as part of the `AbciApp` class, before this they were defined using a list
 - On the round class implementation
   - `payload_attribute` attribute has been removed
   - Usage of payloads with multiple attributes has been simplified since the user can now specify a tuple of keys in order to store all the data of a payload to the database.
+- Round `selection_key` is now a tuple for multiple-attribute payloads.
 
 ## `v0.7.0` to `v0.8.0`
 
 - Support for `--rpc` and `--sca` flags has been deprecated on `autonomy deploy from-token` command. Refer to the CLI documentation to understand how to use custom `RPC`.
 - The transaction payload classes needs to be defined using the data classes and needs to be immutable
 - `Transaction` is a data class
 - IPFS connection and protocol need to be added to your `aea-config.yaml`, if they utilize `valory/abstract_round_abci` skill.
@@ -58,15 +63,15 @@
 
 ## `v0.4.0` to `v0.5.0`
 
 
 One backwards incompatible change
 ## Service component
 
-- This release introduces a new format for defining multiple overrides for an agent on a service configuration. Please follow this [guide](https://github.com/valory-xyz/open-autonomy/blob/main/docs/guides/service_configuration_file.md) to update your service configurations accordingly. 
+- This release introduces a new format for defining multiple overrides for an agent on a service configuration. Please follow this [guide](https://github.com/valory-xyz/open-autonomy/blob/main/docs/guides/service_configuration_file.md) to update your service configurations accordingly.
 
 ## `v0.3.5` to `v0.4.0`
 
 Multiple backwards incompatible changes
 
 ### Autonomy CLI module
 
@@ -78,15 +83,15 @@
   - Users will have to manually switch to the newer version, i.e., remove the path prefix in all their FSM specifications. For example an FSM specification with a `label: packages.author.skills.my_abci.rounds.MyAbciApp` now becomes `label: MyAbciApp`
 
 - `autonomy analyse abci check-handlers` has been moved to `autonomy analyse handlers`
   - `--packages-dr` flag has been deprecated, use `--registry-path` at top level instead
   - Input format for common handlers and skip skills options has been updated
     - Old format - `--common abci,http,contract_api,ledger_api,signing --skip abstract_abci,counter,counter_client,hello_world_abci`
     - New format `-h abci -h http -h contract_api -h ledger_api -h signing -i abstract_abci -i counter -i counter_client -i hello_world_abci`
-  
+
 - `autonomy analyse abci docstrings` has been moved to `autonomy analyse docstrings`
   - `--check` flag has been deprecated and the command will perform the check by default
   - `--update` flag has been introduced to update the docstring if necessary
 
 - `autonomy analyse abci logs` has been moved to `autonomy analyse logs`
 
 ### Autonomy test plugin
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 This page provides some tips on how to upgrade agent services between different
 versions of the {{open_autonomy}} framework. For full release notes check the
 Open-Autonomy_repo. Below we describe the additional manual steps required to
-upgrade between different versions: # Open Autonomy ## `v0.8.0` to `v0.9.0`
-Breaking changes - On the skill configuration - The `max_participants`
-parameter has been removed - The `consensus_threshold` should now be specified
+upgrade between different versions: # Open Autonomy ## `v0.9.0` to `v0.9.1` No
+backwards incompatible changes ## `v0.8.0` to `v0.9.0` Breaking changes - On
+the skill configuration - The `max_participants` parameter has been removed. If
+the `consensus` configuration is empty after removing `max_participants`, it
+should be removed as well. - The `consensus_threshold` should now be specified
 in the `setup` parameters. If `null`, the recommended setting, then it is
 calculated automatically from the participants provided. - The synchronized
 database is now `serializable` and `hashable`. This means that the data
 inserted into the database are now enforced to be primitive or non-primitive
 built-in types only, except for `sets` and `frozensets` since an error is
 raised as they cannot be `serialized`/`hashed` and therefore cannot be inserted
 into the database. In essence, the data should be `json serializable`. - The
@@ -15,20 +17,21 @@
 use `-ltm, --local-tm-setup` when building a deployment using `autonomy deploy
 build` command to include a Tendermint Consensus Gadget setup. - The
 `cross_period_persisted_keys` and database conditions needs to be defined as
 sets as part of the `AbciApp` class, before this they were defined using a list
 - On the round class implementation - `payload_attribute` attribute has been
 removed - Usage of payloads with multiple attributes has been simplified since
 the user can now specify a tuple of keys in order to store all the data of a
-payload to the database. ## `v0.7.0` to `v0.8.0` - Support for `--rpc` and `--
-sca` flags has been deprecated on `autonomy deploy from-token` command. Refer
-to the CLI documentation to understand how to use custom `RPC`. - The
-transaction payload classes needs to be defined using the data classes and
-needs to be immutable - `Transaction` is a data class - IPFS connection and
-protocol need to be added to your `aea-config.yaml`, if they utilize `valory/
+payload to the database. - Round `selection_key` is now a tuple for multiple-
+attribute payloads. ## `v0.7.0` to `v0.8.0` - Support for `--rpc` and `--sca`
+flags has been deprecated on `autonomy deploy from-token` command. Refer to the
+CLI documentation to understand how to use custom `RPC`. - The transaction
+payload classes needs to be defined using the data classes and needs to be
+immutable - `Transaction` is a data class - IPFS connection and protocol need
+to be added to your `aea-config.yaml`, if they utilize `valory/
 abstract_round_abci` skill. - IPFS dialogues and handler need to be specified.
 - `send_to_ipfs` and `get_from_ipfs` are now moved to `BaseBehaviour` and are
 generators. - E2E tests now utilize a local deployment of the IPFS, as such you
 will need to import the `ipfs_daemon` and `ipfs_domain` fixtures from
 `aea_test_autonomy.fixture_helpers`. ## `v0.6.0` to `v0.7.0` Breaking changes -
 The new `AbstractRound` and `BaseBehaviour` meta classes enforce checks on the
 class attributes. For concrete classes inheriting from `AbstractRound` the
```

### Comparing `open-autonomy-0.9.0/docs/using_stack_deployment.md` & `open-autonomy-0.9.1/docs/using_stack_deployment.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/mkdocs.yml` & `open-autonomy-0.9.1/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,18 @@
       - Library:
         - Constants: 'api/constants.md'
         - Analyse:
           - ABCI:
             - App Spec: 'api/analyse/abci/app_spec.md'
             - Docstrings: 'api/analyse/abci/docstrings.md'
             - Handlers: 'api/analyse/handlers.md'
-            - Logs: 'api/analyse/abci/logs.md'
+            - Logs:
+              - Base: 'api/analyse/logs/base.md'
+              - Collection: 'api/analyse/logs/collection.md'
+              - Db: 'api/analyse/logs/db.md'
           - Benchmark:
             - Aggregate: 'api/analyse/benchmark/aggregate.md'
             - HTML: 'api/analyse/benchmark/html.md'
         - CLI:
           - Analyse: 'api/cli/analyse.md'
           - Core: 'api/cli/core.md'
           - Deploy: 'api/cli/deploy.md'
```

### Comparing `open-autonomy-0.9.0/open_autonomy.egg-info/PKG-INFO` & `open-autonomy-0.9.1/open_autonomy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-autonomy
-Version: 0.9.0
+Version: 0.9.1
 Summary: A framework for the creation of autonomous agent services.
 Home-page: https://github.com/valory-xyz/open-autonomy.git
 Author: Valory AG
 License: Apache-2.0
 Project-URL: Bug Reports, https://github.com/valory-xyz/open-autonomy/issues
 Project-URL: Source, https://github.com/valory/open-autonomy
 Keywords: autonomy open-autonomy aea open-aea autonomous-economic-agents agent-framework multi-agent-systems multi-agent cryptocurrency cryptocurrencies dezentralized dezentralized-network
@@ -81,23 +81,23 @@
 smart contracts provide, making it possible to execute **arbitrarily complex operations**
 (such as machine-learning algorithms). Most importantly, agent services are
 **decentralized**, **trust-minimized**, **transparent**, and **robust**.
 
 
 ## Get started developing agent services
 
-Read the [Open Autonomy documentation](https://docs.autonolas.network/) to learn more about agent services. Follow the [set up](https://docs.autonolas.network/guides/set_up/) and [quick start](https://docs.autonolas.network/guides/quick_start/) guides to start building your own services.
+Read the [Open Autonomy documentation](https://docs.autonolas.network/open-autonomy/) to learn more about agent services. Follow the [set up](https://docs.autonolas.network/open-autonomy/guides/set_up/) and [quick start](https://docs.autonolas.network/open-autonomy/guides/quick_start/) guides to start building your own services.
 
 
 ## For developers contributing to the framework: install from source
 
 - Ensure your machine satisfies the following requirements:
 
     - Python `>= 3.7`
-    - [Tendermint](https://docs.tendermint.com/master/introduction/install.html) `==0.34.19`
+    - [Tendermint](https://docs.tendermint.com/v0.34/introduction/install.html) `==0.34.19`
     - [IPFS node](https://docs.ipfs.io/install/command-line/#official-distributions) `==v0.6.0`
     - [Pip](https://pip.pypa.io/en/stable/installation/)
     - [Pipenv](https://pipenv.pypa.io/en/latest/install/) `>=2021.x.xx`
     - [Go](https://go.dev/doc/install) `==1.17.7`
     - [Kubectl](https://kubernetes.io/docs/tasks/tools/)
     - [Docker Engine](https://docs.docker.com/engine/install/)
     - [Docker Compose](https://docs.docker.com/compose/install/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-autonomy Version: 0.9.0 Summary: A framework
+Metadata-Version: 2.1 Name: open-autonomy Version: 0.9.1 Summary: A framework
 for the creation of autonomous agent services. Home-page: https://github.com/
 valory-xyz/open-autonomy.git Author: Valory AG License: Apache-2.0 Project-URL:
 Bug Reports, https://github.com/valory-xyz/open-autonomy/issues Project-URL:
 Source, https://github.com/valory/open-autonomy Keywords: autonomy open-
 autonomy aea open-aea autonomous-economic-agents agent-framework multi-agent-
 systems multi-agent cryptocurrency cryptocurrencies dezentralized
 dezentralized-network Classifier: Environment :: Console Classifier:
@@ -25,39 +25,40 @@
 chain autonomous services which run as a multi-agent-system (MAS) and offer
 enhanced functionalities on-chain. Agent services expand the range of
 operations that traditional smart contracts provide, making it possible to
 execute **arbitrarily complex operations** (such as machine-learning
 algorithms). Most importantly, agent services are **decentralized**, **trust-
 minimized**, **transparent**, and **robust**. ## Get started developing agent
 services Read the [Open Autonomy documentation](https://docs.autonolas.network/
-) to learn more about agent services. Follow the [set up](https://
-docs.autonolas.network/guides/set_up/) and [quick start](https://
-docs.autonolas.network/guides/quick_start/) guides to start building your own
-services. ## For developers contributing to the framework: install from source
-- Ensure your machine satisfies the following requirements: - Python `>= 3.7` -
-[Tendermint](https://docs.tendermint.com/master/introduction/install.html)
-`==0.34.19` - [IPFS node](https://docs.ipfs.io/install/command-line/#official-
-distributions) `==v0.6.0` - [Pip](https://pip.pypa.io/en/stable/installation/
-) - [Pipenv](https://pipenv.pypa.io/en/latest/install/) `>=2021.x.xx` - [Go]
-(https://go.dev/doc/install) `==1.17.7` - [Kubectl](https://kubernetes.io/docs/
-tasks/tools/) - [Docker Engine](https://docs.docker.com/engine/install/) -
-[Docker Compose](https://docs.docker.com/compose/install/) - [Skaffold](https:/
-/skaffold.dev/docs/install/#standalone-binary) `>= 1.39.1` - [Gitleaks](https:/
-/github.com/zricethezav/gitleaks/releases/latest) - Clone the repository: git
-clone git@github.com:valory-xyz/open-autonomy.git - Pull pre-built images:
-docker pull valory/autonolas-registries:latest docker pull valory/acn-node:
-latest docker pull valory/contracts-amm:latest docker pull valory/safe-
-contract-net:latest docker pull valory/slow-tendermint-server:0.1.0 - Create
-and launch a virtual environment. Also, run this during development, every time
-you need to re-create and launch the virtual environment and update the
-dependencies: make new_env && pipenv shell > :information_source: Note: we are
-using [atheris](https://github.com/google/atheris) in order to perform fuzzy
-testing. > The dependency is not listed in the `Pipfile` because it is not
-supported on Windows. > If you need to run or implement a fuzzy test, please
-manually install the dependency. > If you are developing on Mac, please follow
-the extra steps described [here](https://github.com/google/atheris#mac). -
-Fetch packages: autonomy packages sync --update-packages ## Cite If you are
-using our software in a publication, please consider to cite it with the
-following BibTex entry: ``` @misc{open-autonomy, Author = {David Minarsch and
-Marco Favorito and Viraj Patel and Adamantios Zaras and David Vilela Freire and
-Michiel Karrenbelt and 8baller and Ardian Abazi and Yuri Turchenkov and JosÃ©
-Moreira SÃ¡nchez}, Title = {Open Autonomy Framework}, Year = {2021}, } ```
+open-autonomy/) to learn more about agent services. Follow the [set up](https:/
+/docs.autonolas.network/open-autonomy/guides/set_up/) and [quick start](https:/
+/docs.autonolas.network/open-autonomy/guides/quick_start/) guides to start
+building your own services. ## For developers contributing to the framework:
+install from source - Ensure your machine satisfies the following requirements:
+- Python `>= 3.7` - [Tendermint](https://docs.tendermint.com/v0.34/
+introduction/install.html) `==0.34.19` - [IPFS node](https://docs.ipfs.io/
+install/command-line/#official-distributions) `==v0.6.0` - [Pip](https://
+pip.pypa.io/en/stable/installation/) - [Pipenv](https://pipenv.pypa.io/en/
+latest/install/) `>=2021.x.xx` - [Go](https://go.dev/doc/install) `==1.17.7` -
+[Kubectl](https://kubernetes.io/docs/tasks/tools/) - [Docker Engine](https://
+docs.docker.com/engine/install/) - [Docker Compose](https://docs.docker.com/
+compose/install/) - [Skaffold](https://skaffold.dev/docs/install/#standalone-
+binary) `>= 1.39.1` - [Gitleaks](https://github.com/zricethezav/gitleaks/
+releases/latest) - Clone the repository: git clone git@github.com:valory-xyz/
+open-autonomy.git - Pull pre-built images: docker pull valory/autonolas-
+registries:latest docker pull valory/acn-node:latest docker pull valory/
+contracts-amm:latest docker pull valory/safe-contract-net:latest docker pull
+valory/slow-tendermint-server:0.1.0 - Create and launch a virtual environment.
+Also, run this during development, every time you need to re-create and launch
+the virtual environment and update the dependencies: make new_env && pipenv
+shell > :information_source: Note: we are using [atheris](https://github.com/
+google/atheris) in order to perform fuzzy testing. > The dependency is not
+listed in the `Pipfile` because it is not supported on Windows. > If you need
+to run or implement a fuzzy test, please manually install the dependency. > If
+you are developing on Mac, please follow the extra steps described [here]
+(https://github.com/google/atheris#mac). - Fetch packages: autonomy packages
+sync --update-packages ## Cite If you are using our software in a publication,
+please consider to cite it with the following BibTex entry: ``` @misc{open-
+autonomy, Author = {David Minarsch and Marco Favorito and Viraj Patel and
+Adamantios Zaras and David Vilela Freire and Michiel Karrenbelt and 8baller and
+Ardian Abazi and Yuri Turchenkov and JosÃ© Moreira SÃ¡nchez}, Title = {Open
+Autonomy Framework}, Year = {2021}, } ```
```

### Comparing `open-autonomy-0.9.0/open_autonomy.egg-info/SOURCES.txt` & `open-autonomy-0.9.1/open_autonomy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 autonomy/analyse/constants.py
 autonomy/analyse/dialogues.py
 autonomy/analyse/handlers.py
 autonomy/analyse/service.py
 autonomy/analyse/abci/__init__.py
 autonomy/analyse/abci/app_spec.py
 autonomy/analyse/abci/docstrings.py
-autonomy/analyse/abci/logs.py
 autonomy/analyse/benchmark/__init__.py
 autonomy/analyse/benchmark/aggregate.py
 autonomy/analyse/benchmark/html.py
 autonomy/analyse/logs/__init__.py
 autonomy/analyse/logs/base.py
 autonomy/analyse/logs/collection.py
 autonomy/analyse/logs/db.py
@@ -189,15 +188,14 @@
 docs/api/constants.md
 docs/api/analyse/constants.md
 docs/api/analyse/dialogues.md
 docs/api/analyse/handlers.md
 docs/api/analyse/service.md
 docs/api/analyse/abci/app_spec.md
 docs/api/analyse/abci/docstrings.md
-docs/api/analyse/abci/logs.md
 docs/api/analyse/benchmark/aggregate.md
 docs/api/analyse/benchmark/html.md
 docs/api/analyse/logs/base.md
 docs/api/analyse/logs/collection.md
 docs/api/analyse/logs/db.md
 docs/api/chain/base.md
 docs/api/chain/config.md
@@ -919,14 +917,15 @@
 tests/data/dummy_packages/dummy_author/skills/dummy_skill/my_model.py
 tests/data/dummy_packages/dummy_author/skills/dummy_skill/skill.yaml
 tests/data/dummy_service_config_files/service_0.yaml
 tests/data/dummy_service_config_files/service_1.yaml
 tests/data/dummy_service_config_files/service_2.yaml
 tests/data/dummy_service_config_files/service_3.yaml
 tests/data/dummy_service_config_files/service_4.yaml
+tests/data/logs/aea_0.txt
 tests/data/specs/fsm_specification.json
 tests/data/specs/fsm_specification_empty.json
 tests/data/specs/fsm_specification_extra.json
 tests/test_autonomy/__init__.py
 tests/test_autonomy/base.py
 tests/test_autonomy/test_configurations.py
 tests/test_autonomy/test_constants.py
@@ -946,20 +945,20 @@
 tests/test_autonomy/test_cli/test_publish.py
 tests/test_autonomy/test_cli/test_push_all.py
 tests/test_autonomy/test_cli/test_scaffold_fsm.py
 tests/test_autonomy/test_cli/test_analyse/__init__.py
 tests/test_autonomy/test_cli/test_analyse/test_benchmarks.py
 tests/test_autonomy/test_cli/test_analyse/test_check_dialogues.py
 tests/test_autonomy/test_cli/test_analyse/test_check_handlers.py
+tests/test_autonomy/test_cli/test_analyse/test_logs.py
 tests/test_autonomy/test_cli/test_analyse/test_specs.py
 tests/test_autonomy/test_cli/test_analyse/test_verify_service.py
 tests/test_autonomy/test_cli/test_analyse/test_abci/__init__.py
 tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstring_generator.py
 tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstrings.py
-tests/test_autonomy/test_cli/test_analyse/test_abci/test_log_parser.py
 tests/test_autonomy/test_cli/test_deploy/__init__.py
 tests/test_autonomy/test_cli/test_deploy/test_from_token.py
 tests/test_autonomy/test_cli/test_deploy/test_run_deployment.py
 tests/test_autonomy/test_cli/test_deploy/test_build/__init__.py
 tests/test_autonomy/test_cli/test_deploy/test_build/test_deployment.py
 tests/test_autonomy/test_cli/test_develop/__init__.py
 tests/test_autonomy/test_cli/test_develop/test_local_service_registry.py
```

### Comparing `open-autonomy-0.9.0/packages/__init__.py` & `open-autonomy-0.9.1/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/packages.json` & `open-autonomy-0.9.1/packages/packages.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8959603658536586%*

 * *Differences: {"'dev'": "{'connection/valory/abci/0.1.0': "*

 * *          "'bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey', "*

 * *          "'contract/valory/gnosis_safe_proxy_factory/0.1.0': "*

 * *          "'bafybeidzdv6zjst5likperhuqdzsb4yix6ey5ir45nwdcquw3asuqmqdlu', "*

 * *          "'skill/valory/test_ipfs_abci/0.1.0': "*

 * *          "'bafybeicxpeo5ypjvu367pksuufsrza4cngxl4nncdido53r3ryovwmvxfy', "*

 * *          "'agent/valory/test_ipfs/0.1.0': "*

 * *          "'bafybeibixyacbe3hr7nhv4lnumvhhljy7p6ys7itfkqhhtiyjkvavjj5ou', "*

 * *    […]*

```diff
@@ -1,54 +1,54 @@
 {
     "dev": {
-        "agent/valory/abstract_abci/0.1.0": "bafybeig5qj4huxbj2g2vf27vliyrnu6kmr3cpxfmqaslzakb43xd7l3jzq",
-        "agent/valory/counter/0.1.0": "bafybeiaabwbh5oerjritw6ucqseh2sqirfhxnlnm6vlst2jh2qhgrucmxa",
+        "agent/valory/abstract_abci/0.1.0": "bafybeib4o2zojkbk4kympvyahbhezzbmcottzk7cmnr6yosoiruwr4ze5i",
+        "agent/valory/counter/0.1.0": "bafybeidkwjanxwjnx74gpmm4x4nvevif5bhofyunyhsi6r2qtzxsqnsafq",
         "agent/valory/counter_client/0.1.0": "bafybeicv6jsvvhvtzizko7eewukcfkg3is5dzn47l5ylgvdo4dzjof5inu",
-        "agent/valory/hello_world/0.1.0": "bafybeifcl3izwfurgxdbhf4n4mu2jv5vlj5vygw6bgjlcjj66wsxefc7ry",
-        "agent/valory/register_reset/0.1.0": "bafybeid6i5jpihanjzfaykdgbwb5kg3y6fwdps62ivhpzd5mbldmzxgxai",
-        "agent/valory/register_reset_recovery/0.1.0": "bafybeiannsxcsd5b3nwwxifyj5ihio4pkaexdzfgfdnwnkflksmgdwc42i",
-        "agent/valory/register_termination/0.1.0": "bafybeifynadq24eche7jkfcbiybxr2kvkjgtj5oeueurlejswxcepy5gvq",
-        "agent/valory/registration_start_up/0.1.0": "bafybeidvebjdpignfsgv7sp6ux6bl444afvpmiiblzb7kr5qx6v3uioiwi",
-        "agent/valory/test_abci/0.1.0": "bafybeia5f4zmb6judsbicwkzvf7udqj5o4t7epegywir3ivmybicztr434",
-        "agent/valory/test_ipfs/0.1.0": "bafybeidtrr73c72kbrkpn6tjsichjy6ge4qg36arelw4ufonseqyhcmwau",
-        "connection/valory/abci/0.1.0": "bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a",
+        "agent/valory/hello_world/0.1.0": "bafybeic3czcb7fpzru3fl4noxdwgwyzirqk6cqh763h6aio7ugl6qm5gha",
+        "agent/valory/register_reset/0.1.0": "bafybeibjuczg4bpkpt5m26mdeolg5ooh6wfsfhm3e5xsmmw3th6nsawsne",
+        "agent/valory/register_reset_recovery/0.1.0": "bafybeicyxwchnbuqmbr3tvbesd7me4xpeuesgj7oo4wjwppkpcq6qgc7fq",
+        "agent/valory/register_termination/0.1.0": "bafybeig4yehd4oseko3pbp6x23h7qmmcvckro66uw5hpecezcslygtjtym",
+        "agent/valory/registration_start_up/0.1.0": "bafybeied4jwpijvcudlvu3h63gwvkdr4cnazcjk3b335ibgdjpkq4llrn4",
+        "agent/valory/test_abci/0.1.0": "bafybeid2daa6abk4z42so7bbpbgy6mgfrxwa5upjmayf5jw3ej2du2ozqa",
+        "agent/valory/test_ipfs/0.1.0": "bafybeibixyacbe3hr7nhv4lnumvhhljy7p6ys7itfkqhhtiyjkvavjj5ou",
+        "connection/valory/abci/0.1.0": "bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey",
         "connection/valory/ipfs/0.1.0": "bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu",
         "contract/valory/agent_registry/0.1.0": "bafybeibkj4pm6ziqh2fl3xfsjiou4ibnxlipmvmqhgvc7xwpnaddbtxzli",
         "contract/valory/component_registry/0.1.0": "bafybeialw5eaa4v54s7i3sjsuy6d5k624quhxhziqntwq5hnz4g646sb7m",
-        "contract/valory/gnosis_safe/0.1.0": "bafybeihwwv5aodluykglsbuhhrwusvjof6vvnr37rznwvlutmfwtvoju34",
-        "contract/valory/gnosis_safe_proxy_factory/0.1.0": "bafybeieuivicfjkow3asmrj57mygrqbvjnecxqaybyxf6egktdty7qxac4",
+        "contract/valory/gnosis_safe/0.1.0": "bafybeibzfhpib5fw3wady6dhq5bfgo37o437bi4s3hthbvvit7byvbalg4",
+        "contract/valory/gnosis_safe_proxy_factory/0.1.0": "bafybeidzdv6zjst5likperhuqdzsb4yix6ey5ir45nwdcquw3asuqmqdlu",
         "contract/valory/multicall2/0.1.0": "bafybeiaegx2j5w6le2fhvzmx7stzujuezqfvicvnyqebtipivkek2cgh7m",
         "contract/valory/multisend/0.1.0": "bafybeigjywkl7hydjsrkogob3xebj2ifhqwmfhhxoeyrndzhhxi5u6amey",
         "contract/valory/registries_manager/0.1.0": "bafybeighjuqdj2oq6tqckf7j3mqtighe7lpaahh7qt3sqxtbtjlur4tmj4",
         "contract/valory/service_manager/0.1.0": "bafybeiea3bophgb6ikqvpd7lzyluthlhoazbbrknvfncu4j7wbubfsrjeu",
-        "contract/valory/service_registry/0.1.0": "bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi",
+        "contract/valory/service_registry/0.1.0": "bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi",
         "protocol/valory/abci/0.1.0": "bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4",
         "protocol/valory/ipfs/0.1.0": "bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4",
         "protocol/valory/tendermint/0.1.0": "bafybeicusvezoqlmyt6iqomcbwaz3xkhk2qf3d56q5zprmj3xdxfy64k54",
-        "service/valory/counter/0.1.0": "bafybeiedev5vi5bxkx53fsbqy54onrdtdjq64hkz7b2pzoqw64y2qmzefe",
-        "service/valory/hello_world/0.1.0": "bafybeidzmbyyyitioj4mz6xwlnqlvnmjwb5pzfw7qcpgtrv3ytozgbhnri",
-        "service/valory/register_reset/0.1.0": "bafybeidd7jjkgptascvegeelkvympjam5gvmsogvphlh5d7jalvznv7tr4",
-        "skill/valory/abstract_abci/0.1.0": "bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti",
-        "skill/valory/abstract_round_abci/0.1.0": "bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi",
-        "skill/valory/counter/0.1.0": "bafybeied3rhikmiulc2qdwl3lfyw3kgvsrpz674epoaulrn2zrbfdu23ra",
+        "service/valory/counter/0.1.0": "bafybeihnd72avnqtn5ig6ikuxge2kgcoo2clt5bxqo3ar4mesdg7s7744q",
+        "service/valory/hello_world/0.1.0": "bafybeiangkjd6y5jjpubeog25lggrmq3y64b2cqurhmxs26i4tddksbhiq",
+        "service/valory/register_reset/0.1.0": "bafybeig2hgffe3nijhr6wlia2sluzt4p2al63faqxrriwpss4y5gutqbj4",
+        "skill/valory/abstract_abci/0.1.0": "bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou",
+        "skill/valory/abstract_round_abci/0.1.0": "bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4",
+        "skill/valory/counter/0.1.0": "bafybeibzjqpzumbj2ts6lh6mgfj2t2mabgq25qrdhubbwjonnxwnhcj3cu",
         "skill/valory/counter_client/0.1.0": "bafybeiaqdfulxamdshw7fykfkqvkpvjb5bnmhv7ffrjiwdi4ktiulklx6q",
-        "skill/valory/hello_world_abci/0.1.0": "bafybeiagih5lel6ccikc6d36r5mntzj374x6brxt4a62bqa23w7khorcte",
-        "skill/valory/register_reset_abci/0.1.0": "bafybeifezziaezqhqmbyvee26sw5wkrwsc3wlmas7c2vvghe7xwyxycpey",
-        "skill/valory/register_reset_recovery_abci/0.1.0": "bafybeicmyjgiogc3dmc6iwryxbhwzs4pxnymgoqihpp7ibvs6xmkvzdzwm",
-        "skill/valory/register_termination_abci/0.1.0": "bafybeigkwb3rp7rwv2jjcep6z5zma5muu2ulm65oxo6yhispponchcvor4",
-        "skill/valory/registration_abci/0.1.0": "bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq",
-        "skill/valory/reset_pause_abci/0.1.0": "bafybeic6ayed23np6ngkawsf2you6nnfuvbq4smcepdvvcrw5wxn5jaevy",
-        "skill/valory/termination_abci/0.1.0": "bafybeigg4eyjaeidojnvxdenztaywb7ijtjdtjirpc6pvhglscfqdhfupe",
-        "skill/valory/test_abci/0.1.0": "bafybeickt7snjkd2365nyr7r2xjozxwaiy2swcy6xh6hstleam6ouujctu",
-        "skill/valory/test_ipfs_abci/0.1.0": "bafybeiasijop7eizwyxbwxnkh4iiitk6banuxz5u3bn7ijdvkzm77xtgju",
-        "skill/valory/transaction_settlement_abci/0.1.0": "bafybeiajvxzaeeeamvb3guxtihlrj7xoyrmfeuo5chp4f3pdd2sgiecayq"
+        "skill/valory/hello_world_abci/0.1.0": "bafybeidhftdlf24itdpzs456btixret4deeis35jdqesh3xo54ukxegdrq",
+        "skill/valory/register_reset_abci/0.1.0": "bafybeigda2s3nouoehbttbcyewhdolngq4m5ibnwr2driell2ufustgxga",
+        "skill/valory/register_reset_recovery_abci/0.1.0": "bafybeienpr3zxuddgfwuqpgdc32qez6tdldluka6t4dwyltyx2twy6toze",
+        "skill/valory/register_termination_abci/0.1.0": "bafybeih67ylxwvmc7wamw2sjkfd77zglovqn2gziwewlgeo6pndhonbkyu",
+        "skill/valory/registration_abci/0.1.0": "bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya",
+        "skill/valory/reset_pause_abci/0.1.0": "bafybeievxhu6u5r5wlpjfzcwuowlbanhfbi25saf25qit53jauv4kq6gne",
+        "skill/valory/termination_abci/0.1.0": "bafybeihpp4li6jw3co4c4jferrtzobq2ydoc3dcn67esqrg5ebvyoac66e",
+        "skill/valory/test_abci/0.1.0": "bafybeibsosoucoq6oiohxrpzllen63r6ul5q7ne2kwfvnp44sw43cpeady",
+        "skill/valory/test_ipfs_abci/0.1.0": "bafybeicxpeo5ypjvu367pksuufsrza4cngxl4nncdido53r3ryovwmvxfy",
+        "skill/valory/transaction_settlement_abci/0.1.0": "bafybeiftbgfzp36bknbwus3fx2equmhgmboy4qd5myex76xfc4ze6o7b54"
     },
     "third_party": {
         "connection/valory/http_client/0.23.0": "bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi",
-        "connection/valory/ledger/0.19.0": "bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi",
+        "connection/valory/ledger/0.19.0": "bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui",
         "connection/valory/p2p_libp2p_client/0.1.0": "bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva",
         "protocol/open_aea/signing/1.0.0": "bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4",
         "protocol/valory/acn/1.1.0": "bafybeignmc5uh3vgpuckljcj2tgg7hdqyytkm6m5b6v6mxtazdcvubibva",
         "protocol/valory/contract_api/1.0.0": "bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy",
         "protocol/valory/http/1.0.0": "bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty",
         "protocol/valory/ledger_api/1.0.0": "bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom"
     }
```

### Comparing `open-autonomy-0.9.0/packages/valory/__init__.py` & `open-autonomy-0.9.1/packages/valory/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/abstract_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/abstract_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/abstract_abci/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/abstract_abci/aea-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 fingerprint:
   README.md: bafybeialqqea4ivqoc22bdfjgt6qnungfz26457q4cumujbuwinrg3ogky
   __init__.py: bafybeif3jvuzkmlibl6ufntm7b7pzy7dlw4fop5bqymmpcgcbwfna7ca44
   tests/__init__.py: bafybeiacoxpgjdkxogh4wbglh4n66jigwbuh2vnuzdfqjwlmvtj2eghf3m
   tests/test_abstract_abci.py: bafybeic4hileugdjd6bwy4n5beqrjo5auwalz5twt3lyx6m62kb65nc6ca
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts: []
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
 logging_config:
@@ -47,15 +47,15 @@
       - logfile
       - console
       propagate: true
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
 default_connection: valory/abci:0.1.0
 ---
 public_id: valory/abci:0.1.0
 type: connection
 config:
   target_skill_id: valory/abstract_abci:0.1.0
   use_tendermint: false
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/abstract_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/abstract_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/abstract_abci/tests/test_abstract_abci.py` & `open-autonomy-0.9.1/packages/valory/agents/abstract_abci/tests/test_abstract_abci.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/counter/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/counter/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/counter/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/counter/aea-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 fingerprint:
   README.md: bafybeib7it5qaocb3ixf64gb576dmvovd4ehsvbdd5tiilrb75do6q3hre
   __init__.py: bafybeifhegkalvgxfovnld7ni72nzyfeys6p27bgvt6hr2rzcn4zfise4i
   tests/__init__.py: bafybeie2owisfwjo4bkoz2dur64wzfzodyybjoe75acehwuiswu4jqtopy
   tests/test_counter.py: bafybeiafaruvutgm65f6wnc4u5z37cyiizuttbpelgs4bpmimnjyp5tnj4
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts: []
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/counter:0.1.0:bafybeied3rhikmiulc2qdwl3lfyw3kgvsrpz674epoaulrn2zrbfdu23ra
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/counter:0.1.0:bafybeibzjqpzumbj2ts6lh6mgfj2t2mabgq25qrdhubbwjonnxwnhcj3cu
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
 logging_config:
@@ -48,15 +48,15 @@
       - logfile
       - console
       propagate: true
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
 default_connection: null
 ---
 public_id: valory/abci:0.1.0
 type: connection
 config:
   target_skill_id: valory/counter:0.1.0
   host: ${ABCI_HOST:str:localhost}
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/counter/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/counter/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/counter/tests/test_counter.py` & `open-autonomy-0.9.1/packages/valory/agents/counter/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/counter_client/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/counter_client/aea-config.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/hello_world/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/hello_world/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/hello_world/aea-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 fingerprint:
   README.md: bafybeifzdekpjcas6egpwxj24tir5ozzffmkq5ecyi6rw3i6fqfd763etu
   __init__.py: bafybeiehvk4wlv2bcbplwc66owg4qdnisiihijq7iegcmjjxtz3dulnrgm
   tests/__init__.py: bafybeiasj5kqyvalbnedototb6ooxfnro3vjmgscja2iccccotfjnd6cha
   tests/test_hello_world.py: bafybeifd3wiuxd6bwixejgxig5omvutf3vfntidm7asqiwv2kbrtjidxbu
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts: []
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/hello_world_abci:0.1.0:bafybeiagih5lel6ccikc6d36r5mntzj374x6brxt4a62bqa23w7khorcte
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/hello_world_abci:0.1.0:bafybeidhftdlf24itdpzs456btixret4deeis35jdqesh3xo54ukxegdrq
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
 logging_config:
@@ -54,15 +54,15 @@
       - logfile
       - console
       propagate: true
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
 default_connection: null
 ---
 public_id: valory/hello_world_abci:0.1.0
 type: skill
 models:
   benchmark_tool:
     args:
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/hello_world/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/hello_world/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/hello_world/tests/test_hello_world.py` & `open-autonomy-0.9.1/packages/valory/agents/hello_world/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/aea-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -18,31 +18,31 @@
   tests/helpers/slow_tendermint_server/config-template.toml: bafybeibzoxwjjn5cacrtx4p2gov75ktg467xoyglistwjn5xt5l6d6tpea
   tests/helpers/slow_tendermint_server/tendermint.py: bafybeibdtbgu3yb7cczxnuui5ewp2npdxmpunjzoeqoqfv5itq567qw2em
   tests/helpers/slow_tendermint_server/wrapper.sh: bafybeif2wssashoaw7ifz6q3ocmejkuz32ycwta4w5dcjunns4g2awkv2y
   tests/test_hard_reset_race_condition.py: bafybeia75m3sxf76hutic7442jwhixltetlih7iev3z2lzlvxzasqqyjye
   tests/test_register_reset.py: bafybeiaprr5wemt57xr2rr2uqnojy2ax4mris5oxadrah2yosx5ecrajfy
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts: []
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/register_reset_abci:0.1.0:bafybeifezziaezqhqmbyvee26sw5wkrwsc3wlmas7c2vvghe7xwyxycpey
-- valory/registration_abci:0.1.0:bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq
-- valory/reset_pause_abci:0.1.0:bafybeic6ayed23np6ngkawsf2you6nnfuvbq4smcepdvvcrw5wxn5jaevy
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/register_reset_abci:0.1.0:bafybeigda2s3nouoehbttbcyewhdolngq4m5ibnwr2driell2ufustgxga
+- valory/registration_abci:0.1.0:bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya
+- valory/reset_pause_abci:0.1.0:bafybeievxhu6u5r5wlpjfzcwuowlbanhfbi25saf25qit53jauv4kq6gne
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
 logging_config:
@@ -67,15 +67,15 @@
       - logfile
       - console
       propagate: true
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
 default_connection: null
 ---
 public_id: valory/abci:0.1.0
 type: connection
 config:
   target_skill_id: valory/register_reset_abci:0.1.0
   host: ${ABCI_HOST:str:localhost}
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/conftest.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/conftest.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/docker/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/docker/docker.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/docker/docker.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/Dockerfile` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/Dockerfile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/app.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/app.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/tendermint.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/tendermint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/wrapper.sh` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/helpers/slow_tendermint_server/wrapper.sh`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/test_hard_reset_race_condition.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/test_hard_reset_race_condition.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset/tests/test_register_reset.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset/tests/test_register_reset.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/aea-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -8,30 +8,30 @@
   README.md: bafybeicocdojplie5z4kbs7cn7apunfydbxui2nigp6ci2osuvv3mybzfm
   __init__.py: bafybeihgxrmmp63exxkdmvlu565kehvuucg4iivnejwutaehb2p7xzxu4q
   tests/__init__.py: bafybeigkkq3hon4wuyrazwnt5tiu23idpelf6a7kzbmawty7zfrpqnmnhi
   tests/base.py: bafybeideqzbfh6sykp5j4asojcn26qg5hro3ot4xa4cl7uhtwrdgwbrxk4
   tests/test_register_reset_recovery.py: bafybeifn7hfnqyzxgdgcemflhbxmzqiq4g7qky477a7epku3d3zqiqoxiy
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts: []
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/register_reset_recovery_abci:0.1.0:bafybeicmyjgiogc3dmc6iwryxbhwzs4pxnymgoqihpp7ibvs6xmkvzdzwm
-- valory/registration_abci:0.1.0:bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/register_reset_recovery_abci:0.1.0:bafybeienpr3zxuddgfwuqpgdc32qez6tdldluka6t4dwyltyx2twy6toze
+- valory/registration_abci:0.1.0:bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 - cosmos
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/tests/base.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/tests/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_reset_recovery/tests/test_register_reset_recovery.py` & `open-autonomy-0.9.1/packages/valory/agents/register_reset_recovery/tests/test_register_reset_recovery.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_termination/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_termination/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_termination/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/register_termination/aea-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -8,41 +8,41 @@
   README.md: bafybeiamp5k2dtww2rxaxu4kqsi3yon6mhofezlgcyzrialt2rnigkk43y
   __init__.py: bafybeihgxrmmp63exxkdmvlu565kehvuucg4iivnejwutaehb2p7xzxu4q
   tests/__init__.py: bafybeiftvheymtbp6iilmx7dceh46hplfxa3lss4xghz623gdon7jhpidi
   tests/base.py: bafybeicly6lcxa32zjgfnvscfcgnzgiq5bfpvwfhrwx2dl2d4fhzxublle
   tests/test_register_reset.py: bafybeieaeelbyrorts3akgsu7xp27jdsv5u7r4psatdxph2agvpym7em6m
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts:
-- valory/gnosis_safe:0.1.0:bafybeihwwv5aodluykglsbuhhrwusvjof6vvnr37rznwvlutmfwtvoju34
-- valory/gnosis_safe_proxy_factory:0.1.0:bafybeieuivicfjkow3asmrj57mygrqbvjnecxqaybyxf6egktdty7qxac4
+- valory/gnosis_safe:0.1.0:bafybeibzfhpib5fw3wady6dhq5bfgo37o437bi4s3hthbvvit7byvbalg4
+- valory/gnosis_safe_proxy_factory:0.1.0:bafybeidzdv6zjst5likperhuqdzsb4yix6ey5ir45nwdcquw3asuqmqdlu
 - valory/multisend:0.1.0:bafybeigjywkl7hydjsrkogob3xebj2ifhqwmfhhxoeyrndzhhxi5u6amey
-- valory/service_registry:0.1.0:bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi
+- valory/service_registry:0.1.0:bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/acn:1.1.0:bafybeignmc5uh3vgpuckljcj2tgg7hdqyytkm6m5b6v6mxtazdcvubibva
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 - valory/ledger_api:1.0.0:bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom
 - valory/tendermint:0.1.0:bafybeicusvezoqlmyt6iqomcbwaz3xkhk2qf3d56q5zprmj3xdxfy64k54
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/register_termination_abci:0.1.0:bafybeigkwb3rp7rwv2jjcep6z5zma5muu2ulm65oxo6yhispponchcvor4
-- valory/registration_abci:0.1.0:bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq
-- valory/reset_pause_abci:0.1.0:bafybeic6ayed23np6ngkawsf2you6nnfuvbq4smcepdvvcrw5wxn5jaevy
-- valory/termination_abci:0.1.0:bafybeigg4eyjaeidojnvxdenztaywb7ijtjdtjirpc6pvhglscfqdhfupe
-- valory/transaction_settlement_abci:0.1.0:bafybeiajvxzaeeeamvb3guxtihlrj7xoyrmfeuo5chp4f3pdd2sgiecayq
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/register_termination_abci:0.1.0:bafybeih67ylxwvmc7wamw2sjkfd77zglovqn2gziwewlgeo6pndhonbkyu
+- valory/registration_abci:0.1.0:bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya
+- valory/reset_pause_abci:0.1.0:bafybeievxhu6u5r5wlpjfzcwuowlbanhfbi25saf25qit53jauv4kq6gne
+- valory/termination_abci:0.1.0:bafybeihpp4li6jw3co4c4jferrtzobq2ydoc3dcn67esqrg5ebvyoac66e
+- valory/transaction_settlement_abci:0.1.0:bafybeiftbgfzp36bknbwus3fx2equmhgmboy4qd5myex76xfc4ze6o7b54
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
 logging_config:
@@ -67,15 +67,15 @@
       - logfile
       - console
       propagate: false
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
 default_connection: null
 ---
 public_id: valory/abci:0.1.0
 type: connection
 config:
   target_skill_id: valory/register_termination_abci:0.1.0
   host: ${ABCI_HOST:str:localhost}
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_termination/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/register_termination/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_termination/tests/base.py` & `open-autonomy-0.9.1/packages/valory/agents/register_termination/tests/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/register_termination/tests/test_register_reset.py` & `open-autonomy-0.9.1/packages/valory/agents/register_termination/tests/test_register_reset.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/registration_start_up/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/registration_start_up/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/registration_start_up/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/registration_start_up/aea-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 fingerprint:
   README.md: bafybeicqrks6wbtytebsnuvkojqy4e7x7puttrgseebbdwazjazrik4rzq
   __init__.py: bafybeiafjxnpd5dldlw2nu2xxdzvry2mlixrlooath5kbkideuvvfyei4u
   tests/__init__.py: bafybeifmfadp3anskpzai4l6dg6ikxvqauzhp2iuizpxvu7q4vvnnpijoi
   tests/test_registration.py: bafybeiczxp4sjdxijrgem3wynpadxilzugiq7xmr4lvnnovrxqn2mv3si4
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts:
-- valory/service_registry:0.1.0:bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi
+- valory/service_registry:0.1.0:bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/acn:1.1.0:bafybeignmc5uh3vgpuckljcj2tgg7hdqyytkm6m5b6v6mxtazdcvubibva
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 - valory/ledger_api:1.0.0:bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom
 - valory/tendermint:0.1.0:bafybeicusvezoqlmyt6iqomcbwaz3xkhk2qf3d56q5zprmj3xdxfy64k54
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/registration_abci:0.1.0:bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/registration_abci:0.1.0:bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 - cosmos
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
@@ -62,15 +62,15 @@
       propagate: true
 dependencies:
   open-aea-ledger-cosmos:
     version: ==1.29.0
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
 skill_exception_policy: just_log
 connection_exception_policy: just_log
 default_connection: null
 ---
 public_id: valory/abci:0.1.0
 type: connection
 config:
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/registration_start_up/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/registration_start_up/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/registration_start_up/tests/test_registration.py` & `open-autonomy-0.9.1/packages/valory/agents/registration_start_up/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/test_abci/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/test_abci/aea-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 license: Apache-2.0
 description: Agent for testing the ABCI connection.
 aea_version: '>=1.0.0, <2.0.0'
 fingerprint:
   README.md: bafybeib2s5p42rb4mbn7ag4jmjwutcm2mhvhb7q7vekxevr565crxkk6zy
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts: []
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 - valory/ledger_api:1.0.0:bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/test_abci:0.1.0:bafybeickt7snjkd2365nyr7r2xjozxwaiy2swcy6xh6hstleam6ouujctu
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/test_abci:0.1.0:bafybeibsosoucoq6oiohxrpzllen63r6ul5q7ne2kwfvnp44sw43cpeady
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
 logging_config:
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/test_ipfs/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/test_ipfs/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/test_ipfs/aea-config.yaml` & `open-autonomy-0.9.1/packages/valory/agents/test_ipfs/aea-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 fingerprint:
   README.md: bafybeigvcqzjhlgvyhd6h6boxnil6clg4cfkfoke5fsnao73balsf3vv3y
   __init__.py: bafybeif4a7hw42rhaivspwz3pnq2hvioxoxhobicgrcjibxjntmw23kmmm
   tests/__init__.py: bafybeifiwgoilbwdy4ipme6gtzrds3qm33cbbpsl62lueltng7m6ltm44i
   tests/test_ipfs.py: bafybeib5fxk5gjuqyevp2rvzcjnyjfuwhfapappohc32xn7rnuu6lpwws4
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts:
-- valory/service_registry:0.1.0:bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi
+- valory/service_registry:0.1.0:bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/acn:1.1.0:bafybeignmc5uh3vgpuckljcj2tgg7hdqyytkm6m5b6v6mxtazdcvubibva
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 - valory/ledger_api:1.0.0:bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom
 - valory/tendermint:0.1.0:bafybeicusvezoqlmyt6iqomcbwaz3xkhk2qf3d56q5zprmj3xdxfy64k54
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/test_ipfs_abci:0.1.0:bafybeiasijop7eizwyxbwxnkh4iiitk6banuxz5u3bn7ijdvkzm77xtgju
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/test_ipfs_abci:0.1.0:bafybeicxpeo5ypjvu367pksuufsrza4cngxl4nncdido53r3ryovwmvxfy
 default_ledger: ethereum
 required_ledgers:
 - ethereum
 default_routing: {}
 connection_private_key_paths: {}
 private_key_paths: {}
 logging_config:
```

### Comparing `open-autonomy-0.9.0/packages/valory/agents/test_ipfs/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/agents/test_ipfs/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/agents/test_ipfs/tests/test_ipfs.py` & `open-autonomy-0.9.1/packages/valory/agents/test_ipfs/tests/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/Makefile` & `open-autonomy-0.9.1/packages/valory/connections/abci/Makefile`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/check_dependencies.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/connection.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/connection.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/connection.yaml` & `open-autonomy-0.9.1/packages/valory/connections/abci/connection.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -73,12 +73,12 @@
 restricted_to_protocols: []
 dependencies:
   grpcio:
     version: ==1.43.0
   hypothesis:
     version: ==6.21.6
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
   protobuf:
     version: ==3.19.4
 is_abstract: false
 cert_requests: []
```

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/gogoproto/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/gogoproto/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/gogoproto/gogo_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/protos/gogoproto/gogo.proto` & `open-autonomy-0.9.1/packages/valory/connections/abci/protos/gogoproto/gogo.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/abci/types.proto` & `open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/abci/types.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/crypto/proof.proto` & `open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/crypto/proof.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/types/params.proto` & `open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/types/params.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/types/types.proto` & `open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/types/types.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/types/validator.proto` & `open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/types/validator.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/protos/tendermint/version/types.proto` & `open-autonomy-0.9.1/packages/valory/connections/abci/protos/tendermint/version/types.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/scripts/genproto.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/scripts/genproto.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/abci/types_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/abci/types_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/abci/types_pb2_grpc.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/abci/types_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/crypto/keys_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/crypto/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/crypto/proof_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/crypto/proof_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/types/params_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/types/params_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/types/types_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/types/validator_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/types/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint/version/types_pb2.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint/version/types_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint_decoder.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint_decoder.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tendermint_encoder.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tendermint_encoder.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/helper.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/helper.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_abci.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_abci.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_abci_fuzz.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_abci_fuzz.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_abci_spec.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_abci_spec.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/base.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/base.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/grpc_channel.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/grpc_channel.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/tcp_channel.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/channels/tcp_channel.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/mock_node/node.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/mock_node/node.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_fuzz/test_fuzz.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_fuzz/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_tendermint_decoder.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_tendermint_decoder.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/abci/tests/test_tendermint_encoder.py` & `open-autonomy-0.9.1/packages/valory/connections/abci/tests/test_tendermint_encoder.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/ipfs/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/ipfs/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/ipfs/connection.py` & `open-autonomy-0.9.1/packages/valory/connections/ipfs/connection.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/ipfs/connection.yaml` & `open-autonomy-0.9.1/packages/valory/connections/ipfs/connection.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/ipfs/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/connections/ipfs/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/connections/ipfs/tests/test_connection.py` & `open-autonomy-0.9.1/packages/valory/connections/ipfs/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/agent_registry/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/agent_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/agent_registry/build/AgentRegistry.json` & `open-autonomy-0.9.1/packages/valory/contracts/agent_registry/build/AgentRegistry.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/agent_registry/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/agent_registry/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/agent_registry/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/agent_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/agent_registry/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/agent_registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/agent_registry/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/agent_registry/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/component_registry/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/component_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/component_registry/build/ComponentRegistry.json` & `open-autonomy-0.9.1/packages/valory/contracts/component_registry/build/ComponentRegistry.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/component_registry/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/component_registry/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/component_registry/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/component_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/component_registry/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/component_registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/component_registry/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/component_registry/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/build/GnosisSafe_V1_3_0.json` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/build/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/contract.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -10,25 +10,25 @@
   __init__.py: bafybeib4nfvueif2tkc7migc73qopyjvrbzedyehrexjx4y5vav3clmf34
   build/GnosisSafe_V1_3_0.json: bafybeifxc4pnyus43qfrvxrqunlmkzvwfr5chyjesyobbk5m4smb2hkd4y
   contract.py: bafybeihdb5oeg4xtnapwml5qz5rkckfetam4wnc2n3gdws23mstpq33ue4
   tests/__init__.py: bafybeihbclcqwfoxoljzwnbg3nf22srsyx5dgdbcyj27irwizktg4ygujy
   tests/test_contract.py: bafybeidnlxmcedoean6xfhjwvj5yvgbaxevjgtlu6wnu2w6y5a37hiniri
 fingerprint_ignore_patterns: []
 contracts:
-- valory/gnosis_safe_proxy_factory:0.1.0:bafybeieuivicfjkow3asmrj57mygrqbvjnecxqaybyxf6egktdty7qxac4
+- valory/gnosis_safe_proxy_factory:0.1.0:bafybeidzdv6zjst5likperhuqdzsb4yix6ey5ir45nwdcquw3asuqmqdlu
 class_name: GnosisSafeContract
 contract_interface_paths:
   ethereum: build/GnosisSafe_V1_3_0.json
 dependencies:
   ecdsa:
     version: '>=0.15'
   eth_typing: {}
   hexbytes: {}
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
   packaging: {}
   py-eth-sig-utils: {}
   requests: {}
   web3:
     version: ==5.25.0
```

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/build/ProxyFactory_V1_3_0.json` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/build/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/contract.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 class_name: GnosisSafeProxyFactoryContract
 contract_interface_paths:
   ethereum: build/ProxyFactory_V1_3_0.json
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
   py-eth-sig-utils: {}
   web3:
     version: ==5.25.0
```

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/gnosis_safe_proxy_factory/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/gnosis_safe_proxy_factory/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multicall2/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/multicall2/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multicall2/build/multicall2.json` & `open-autonomy-0.9.1/packages/valory/contracts/multicall2/build/multicall2.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multicall2/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/multicall2/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multicall2/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/multicall2/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multicall2/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/multicall2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multicall2/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/multicall2/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multisend/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/multisend/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multisend/build/MultiSend.json` & `open-autonomy-0.9.1/packages/valory/contracts/multisend/build/MultiSend.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multisend/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/multisend/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multisend/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/multisend/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multisend/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/multisend/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/multisend/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/multisend/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/registries_manager/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/registries_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/registries_manager/build/RegistriesManager.json` & `open-autonomy-0.9.1/packages/valory/contracts/registries_manager/build/RegistriesManager.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/registries_manager/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/registries_manager/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/registries_manager/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/registries_manager/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/registries_manager/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/registries_manager/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/registries_manager/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/registries_manager/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_manager/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_manager/build/ServiceManager.json` & `open-autonomy-0.9.1/packages/valory/contracts/service_manager/build/ServiceManager.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_manager/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_manager/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_manager/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/service_manager/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_manager/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_manager/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_manager/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_manager/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_registry/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_registry/build/ServiceRegistry.json` & `open-autonomy-0.9.1/packages/valory/contracts/service_registry/build/ServiceRegistry.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_registry/contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_registry/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_registry/contract.yaml` & `open-autonomy-0.9.1/packages/valory/contracts/service_registry/contract.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 class_name: ServiceRegistryContract
 contract_interface_paths:
   ethereum: build/ServiceRegistry.json
 dependencies:
   open-aea-ledger-ethereum:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
```

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_registry/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/contracts/service_registry/tests/test_contract.py` & `open-autonomy-0.9.1/packages/valory/contracts/service_registry/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/__init__.py` & `open-autonomy-0.9.1/packages/valory/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/README.md` & `open-autonomy-0.9.1/packages/valory/protocols/abci/README.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/abci.proto` & `open-autonomy-0.9.1/packages/valory/protocols/abci/abci.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/abci_pb2.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/abci_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/custom_types.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/custom_types.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/message.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/message.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/protocol.yaml` & `open-autonomy-0.9.1/packages/valory/protocols/abci/protocol.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/serialization.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/serialization.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/tests/conftest.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/tests/test_abci.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/tests/test_abci.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/tests/test_abci_dialogues.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/tests/test_abci_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/abci/tests/test_abci_messages.py` & `open-autonomy-0.9.1/packages/valory/protocols/abci/tests/test_abci_messages.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/README.md` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/README.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/__init__.py` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/dialogues.py` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/ipfs.proto` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/ipfs.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/ipfs_pb2.py` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/ipfs_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/message.py` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/message.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/protocol.yaml` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/protocol.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/serialization.py` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/serialization.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/tests/test_ipfs_dialogues.py` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/tests/test_ipfs_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/ipfs/tests/test_ipfs_messages.py` & `open-autonomy-0.9.1/packages/valory/protocols/ipfs/tests/test_ipfs_messages.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/README.md` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/README.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/__init__.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/custom_types.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/custom_types.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/dialogues.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/message.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/message.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/protocol.yaml` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/protocol.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/serialization.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/serialization.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/tendermint.proto` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/tendermint.proto`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/tendermint_pb2.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/tendermint_pb2.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/test_tendermint.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/test_tendermint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/test_tendermint_dialogues.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/test_tendermint_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/protocols/tendermint/tests/test_tendermint_messages.py` & `open-autonomy-0.9.1/packages/valory/protocols/tendermint/tests/test_tendermint_messages.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/services/counter/service.yaml` & `open-autonomy-0.9.1/packages/valory/services/register_reset/service.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-name: counter
+name: register_reset
 author: valory
 version: 0.1.0
-description: A set of agents incrementing a counter
+agent: valory/register_reset:0.1.0:bafybeibjuczg4bpkpt5m26mdeolg5ooh6wfsfhm3e5xsmmw3th6nsawsne
+number_of_agents: 4
+description: Test and debug tendermint reset mechanism.
 aea_version: '>=1.0.0, <2.0.0'
 license: Apache-2.0
 fingerprint:
-  README.md: bafybeidoybzzjch4djhhafqm4e4jcrpaqmlthntcnonlsjtowwpykbc5xi
+  README.md: bafybeiae4sog7e3hyjdujzp5qr2g3auobmqswqnaczh2zhlphuojnd2g6u
 fingerprint_ignore_patterns: []
-number_of_agents: 1
-agent: valory/counter:0.1.0:bafybeiaabwbh5oerjritw6ucqseh2sqirfhxnlnm6vlst2jh2qhgrucmxa
 ---
 public_id: valory/ledger:0.19.0
 type: connection
 config:
   ledger_apis:
     ethereum:
-      address: ${SERVICE_COUNTER_RPC:str:http://host.docker.internal:8545}
+      address: ${SERVICE_REGISTER_RESET_RPC:str:http://host.docker.internal:8545}
       chain_id: 31337
       poa_chain: false
       default_gas_price_strategy: eip1559
```

### Comparing `open-autonomy-0.9.0/packages/valory/services/hello_world/service.yaml` & `open-autonomy-0.9.1/packages/valory/services/hello_world/service.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version: 0.1.0
 description: A simple demonstration of a simple ABCI application
 aea_version: '>=1.0.0, <2.0.0'
 license: Apache-2.0
 fingerprint:
   README.md: bafybeiapubcoersqnsnh3acia5hd7otzt7kjxekr6gkbrlumv6tkajl6jm
 fingerprint_ignore_patterns: []
-agent: valory/hello_world:0.1.0:bafybeifcl3izwfurgxdbhf4n4mu2jv5vlj5vygw6bgjlcjj66wsxefc7ry
+agent: valory/hello_world:0.1.0:bafybeic3czcb7fpzru3fl4noxdwgwyzirqk6cqh763h6aio7ugl6qm5gha
 number_of_agents: 4
 ---
 extra:
   benchmark_persistence_params:
     args: &id002
       log_dir: /benchmarks
   params_args:
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/abstract_abci/skill.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   dialogues.py: bafybeib6cex55nl57xe6boa4c3z4ynlxstnospqjehdb5owpgtvzsu5ucm
   handlers.py: bafybeigcvm43vuj4tpjonlrpcgy7w7h5tylvyvjcdhshcpwomhsbio4ewy
   tests/__init__.py: bafybeicnx4gezk2zrgz23mco2kv7ws3yd5yspku5e3ng4cb5tw7s2zexsu
   tests/test_dialogues.py: bafybeig3kubiyq7bqmetrka67fjk7vymgtjwguyui3yubbvgtzzhfizsdu
   tests/test_handlers.py: bafybeieeuwtu35ddaevr2wgnk33l7kdhrx7ruoeb5jiltiyn65ufdcnopu
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 contracts: []
 protocols:
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 skills: []
 behaviours: {}
 handlers:
   abci:
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/README.md` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/README.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/abci_app_chain.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/abci_app_chain.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/base.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/behaviour_utils.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/behaviour_utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/common.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/common.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/ipfs.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/ipfs.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/load.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/load.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/paths.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/paths.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/io_/store.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/io_/store.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/skill.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -56,31 +56,31 @@
   tests/test_tools/test_common.py: bafybeieauphpcqm5on7d2u2lc5lrf3esbhojp6sxlf7phrlmpqy5cfoitq
   tests/test_tools/test_integration.py: bafybeidxkvb2kizi7djrpuw446dqxo2v5s7j2dbdrdpfmnd2ggezaxbnkm
   tests/test_tools/test_rounds.py: bafybeiccirhrajrvlhkwz4nmj4syw2jgxcrits5v4hfdxegepfd4idh6va
   tests/test_utils.py: bafybeibs7zjpepzdetcy4ybksqxoul45hw372z4evkop3avx6qhrss3bba
   utils.py: bafybeicckjeq5ubm25squfzevdwlwnios7enstmelc7tw4qpzcv2h7ysmq
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 - valory/http_client:0.23.0:bafybeidykl4elwbcjkqn32wt5h4h7tlpeqovrcq3c5bcplt6nhpznhgczi
 - valory/ipfs:0.1.0:bafybeia7kzgw4tmkl6k2vjbnss4egvhcf4fmt7cnmpjjjbjogz2bu2j3fu
-- valory/ledger:0.19.0:bafybeiavzloea5rtoxfdqjuexkqzpgbq73n4sl6af2vwa4bv2wd22qigyi
+- valory/ledger:0.19.0:bafybeicxcypcg2lxmtktbmuhqcyluzmasfsdeljyk2pvaabzc3h2jmcsui
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts:
-- valory/service_registry:0.1.0:bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi
+- valory/service_registry:0.1.0:bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/ipfs:0.1.0:bafybeihlgai5pbmkb6mjhvgy4gkql5uvpwvxbpdowczgz4ovxat6vajrq4
 - valory/ledger_api:1.0.0:bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom
 - valory/tendermint:0.1.0:bafybeicusvezoqlmyt6iqomcbwaz3xkhk2qf3d56q5zprmj3xdxfy64k54
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
 behaviours:
   main:
     args: {}
     class_name: AbstractRoundBehaviour
 handlers:
   abci:
     args: {}
@@ -143,15 +143,15 @@
   hypothesis:
     version: ==6.21.6
   ipfshttpclient:
     version: ==0.8.0a2
   open-aea-cli-ipfs:
     version: ==1.29.0
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
   protobuf:
     version: ==3.19.4
   py-ecc:
     version: ==5.2.0
   pytz:
     version: ==2022.2.1
   requests:
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/abci_app.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/abci_app.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/base.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/common.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/common.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/integration.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/integration.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/test_tools/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/test_tools/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/conftest.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/data/dummy_abci/skill.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_abci_app_chain.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_abci_app_chain.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_base.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_base_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_base_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_behaviours_utils.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_behaviours_utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_common.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/test_ipfs.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/test_ipfs.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/test_load.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/test_load.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_io/test_store.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_io/test_store.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/base.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_base.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_common.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_common.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_integration.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_integration.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_tools/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_tools/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/tests/test_utils.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/abstract_round_abci/utils.py` & `open-autonomy-0.9.1/packages/valory/skills/abstract_round_abci/utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/counter/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/counter/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/counter/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/counter/skill.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 author: valory
 version: 0.1.0
 type: skill
 description: The ABCI Counter application example.
 license: Apache-2.0
 aea_version: '>=1.0.0, <2.0.0'
 fingerprint:
-  README.md: bafybeiahjzi3gvwyorse6bxacvv7thc5nynwvimdqt2xzhpd5y5vxdwwwu
+  README.md: bafybeibmfgmw57jtco75kgk4wkhevwig377bmedbhpqb4nuwdkbphh6bbi
   __init__.py: bafybeic6edzuxlzxfechexteae6qyednm2feuvwmgyxzs7fopd6v5wqjgq
   dialogues.py: bafybeigocfxocz4ektda3iloefedpjru3hobmxop7czi6ekq7ifumvdtwa
   handlers.py: bafybeiazszy3rxyvitfseyey43wrfmhlcztku55jaxk3lg7hzmuxy4t4zm
   tests/__init__.py: bafybeico62tplfccctl7o2ixzpzpysjk5klj36nlk4uqqwzqxc5xrx2ldu
   tests/test_counter.py: bafybeiazi36djqnjzu5t6rn72mngsmntoqz7z7wqa53z3lccgblgsycnbi
 fingerprint_ignore_patterns: []
 connections:
-- valory/abci:0.1.0:bafybeihhidrulgjlrlvmk2c2ax7qmb47ywzjnjqv5gwp7fzzbcgplgaz5a
+- valory/abci:0.1.0:bafybeiedhipcrpx7sg7qwitwox6iqrbbb4vfnvqqyok2vc6wq6inrcszey
 contracts: []
 protocols:
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
 behaviours: {}
 handlers:
   abci:
     args: {}
     class_name: ABCICounterHandler
 models:
   abci_dialogues:
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/counter/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter/tests/test_counter.py` & `open-autonomy-0.9.1/packages/valory/skills/counter/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/models.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/skill.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/counter_client/utils.py` & `open-autonomy-0.9.1/packages/valory/skills/counter_client/utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/README.md` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/README.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/fsm_specification.yaml` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/fsm_specification.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/skill.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   tests/test_payloads.py: bafybeihgz46xtsaenago3bew5gxusyvbo4oivwqmv3r4oqwjgrnqoorcoe
   tests/test_rounds.py: bafybeihdxy7gdpacxnm3yjctdtd2ycdltdcx7thmo5ci4t3xxbtijvlyxq
 fingerprint_ignore_patterns: []
 connections: []
 contracts: []
 protocols: []
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
 behaviours:
   main:
     args: {}
     class_name: HelloWorldRoundBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/hello_world_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/hello_world_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/composition.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/composition.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/fsm_specification.yaml` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/fsm_specification.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/skill.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
   tests/test_handlers.py: bafybeiel2f6pom3bmn3bfpozysspfivvsgphozkhedrwtob2hszp6yqtt4
   tests/test_models.py: bafybeiei5hu6bqgmpjzq4ifrq2vg23pluxq7v72unoo3e4jlrnc3oaqsce
 fingerprint_ignore_patterns: []
 connections: []
 contracts: []
 protocols: []
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/registration_abci:0.1.0:bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq
-- valory/reset_pause_abci:0.1.0:bafybeic6ayed23np6ngkawsf2you6nnfuvbq4smcepdvvcrw5wxn5jaevy
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/registration_abci:0.1.0:bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya
+- valory/reset_pause_abci:0.1.0:bafybeievxhu6u5r5wlpjfzcwuowlbanhfbi25saf25qit53jauv4kq6gne
 behaviours:
   main:
     args: {}
     class_name: RegisterResetAbciAppConsensusBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/composition.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/composition.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/skill.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
   tests/test_models.py: bafybeiepyi7jgllfbnpfu6zoy3noha3usukpxiiavcdi272q6z2acqjphq
   tests/test_rounds.py: bafybeibhpcmhor6nuqrgrwkr3s6zz3ks42nxdbabwkmbvu7xq3i4uswvbu
 fingerprint_ignore_patterns: []
 connections: []
 contracts: []
 protocols: []
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/registration_abci:0.1.0:bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/registration_abci:0.1.0:bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya
 behaviours:
   main:
     args: {}
     class_name: RegisterResetRecoveryAbciAppConsensusBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_reset_recovery_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/register_reset_recovery_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/composition.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/composition.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/skill.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
   tests/test_handlers.py: bafybeidxd375se3fx5gpakpauglsmqom3bbizflpw3k265knyy6fxtckra
   tests/test_models.py: bafybeif2d4kqt7ettspc6fgbeb5y5cm5632rp7dnjcyzy7zfof2m7z6mzq
 fingerprint_ignore_patterns: []
 connections: []
 contracts: []
 protocols: []
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/registration_abci:0.1.0:bafybeieaggf6mc43tses5k7fg3pyxca43wsmfvnnzszzucohp5ebg3umwq
-- valory/reset_pause_abci:0.1.0:bafybeic6ayed23np6ngkawsf2you6nnfuvbq4smcepdvvcrw5wxn5jaevy
-- valory/termination_abci:0.1.0:bafybeigg4eyjaeidojnvxdenztaywb7ijtjdtjirpc6pvhglscfqdhfupe
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/registration_abci:0.1.0:bafybeidgoqi7fa2gb56hdfsf74bbunfii63zgeo4qhggb66ofver2n2gya
+- valory/reset_pause_abci:0.1.0:bafybeievxhu6u5r5wlpjfzcwuowlbanhfbi25saf25qit53jauv4kq6gne
+- valory/termination_abci:0.1.0:bafybeihpp4li6jw3co4c4jferrtzobq2ydoc3dcn67esqrg5ebvyoac66e
 behaviours:
   main:
     args: {}
     class_name: RegisterTerminationAbciAppConsensusBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/register_termination_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/register_termination_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/skill.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
   tests/test_models.py: bafybeiewxl7nio5av2aukql2u7hlhodzdvjjneleba32abr42xeirrycb4
   tests/test_payloads.py: bafybeifik6ek75ughyd4y6t2lchlmjadkzbrz4hsb332k6ul4pwhlo2oga
   tests/test_rounds.py: bafybeiefwk4quzkdn7m43rlahdhoe53xtzm4itlznjh26vdt5567oblgdm
 fingerprint_ignore_patterns: []
 connections:
 - valory/p2p_libp2p_client:0.1.0:bafybeidwcobzb7ut3efegoedad7jfckvt2n6prcmd4g7xnkm6hp6aafrva
 contracts:
-- valory/service_registry:0.1.0:bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi
+- valory/service_registry:0.1.0:bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi
 protocols:
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 - valory/http:1.0.0:bafybeifyoio7nlh5zzyn5yz7krkou56l22to3cwg7gw5v5o3vxwklibhty
 - valory/tendermint:0.1.0:bafybeicusvezoqlmyt6iqomcbwaz3xkhk2qf3d56q5zprmj3xdxfy64k54
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
 behaviours:
   main:
     args: {}
     class_name: AgentRegistrationRoundBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/registration_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/registration_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/fsm_specification.yaml` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/fsm_specification.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/skill.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   tests/test_payloads.py: bafybeifj343tlaiasebfgahfxehn4oi74omgah3ju2pze2fefoouid2zdq
   tests/test_rounds.py: bafybeierruld3cmsscthzcey3hvzzeaqnp5r6tuqfoetzzdbed33hx72pq
 fingerprint_ignore_patterns: []
 connections: []
 contracts: []
 protocols: []
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
 behaviours:
   main:
     args: {}
     class_name: ResetPauseABCIConsensusBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/reset_pause_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/reset_pause_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/skill.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,22 @@
   tests/test_handlers.py: bafybeiefz2ebr5rlyxziwr4bts2r75abpqgji3k47a6hnrj7e7t2yvgmpu
   tests/test_models.py: bafybeih5wtdjuv4hc25fxneeg7mgjiks55xj353zxfamvtrthkw2ydmbbe
   tests/test_payloads.py: bafybeibai4dzjjdeyeinyirjndcfzbj2qst6roj6prjvcqwut5m3won3fa
   tests/test_rounds.py: bafybeid57gov7piwazxot7qfpjtptkgw24xv67nbdpasqr7pdcwoa7eiea
 fingerprint_ignore_patterns: []
 connections: []
 contracts:
-- valory/gnosis_safe:0.1.0:bafybeihwwv5aodluykglsbuhhrwusvjof6vvnr37rznwvlutmfwtvoju34
+- valory/gnosis_safe:0.1.0:bafybeibzfhpib5fw3wady6dhq5bfgo37o437bi4s3hthbvvit7byvbalg4
 - valory/multisend:0.1.0:bafybeigjywkl7hydjsrkogob3xebj2ifhqwmfhhxoeyrndzhhxi5u6amey
-- valory/service_registry:0.1.0:bafybeickj26svokwax7pf3ytp4lpod646lx3yb5z2bh643xovkoy64ggwi
+- valory/service_registry:0.1.0:bafybeid4wyte27tanmeiyzkjfvtvf5yyjngdsvsqvve5bzxwtzjoioubgi
 protocols:
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
-- valory/transaction_settlement_abci:0.1.0:bafybeiajvxzaeeeamvb3guxtihlrj7xoyrmfeuo5chp4f3pdd2sgiecayq
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
+- valory/transaction_settlement_abci:0.1.0:bafybeiftbgfzp36bknbwus3fx2equmhgmboy4qd5myex76xfc4ze6o7b54
 behaviours:
   main:
     args: {}
     class_name: TerminationAbciBehaviours
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/termination_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/termination_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/skill.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
   tests/test_payloads.py: bafybeig54fcpcrxnakyyna6bkxb4dmd7arazsnpvve7tol6rdgkoybluve
   tests/test_rounds.py: bafybeifkxbhfcintdvmsgxilnxpfw7kjgst24caznp2moqgfzaah3bztvu
 fingerprint_ignore_patterns: []
 connections: []
 contracts: []
 protocols: []
 skills:
-- valory/abstract_abci:0.1.0:bafybeiheudaobfaj5lcrqvgwmdysq3za5yjrjtpdiuwhmw5c7lmbgglxti
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
+- valory/abstract_abci:0.1.0:bafybeihkrunmigvlcze7uxhafj2h3kvpf2kifggq7zqj42n2we4mcwuvou
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
 behaviours:
   main:
     args: {}
     class_name: TestAbciConsensusBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/test_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/skill.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   tests/test_payloads.py: bafybeihdizr6r5xnd5hudj7ho7ye3dkcppjt753ulaofyazqpokxnf6cga
   tests/test_rounds.py: bafybeidmmr4vevplodp6zz55cqarlyv5gufqnofmqpepwwhvpeitexhvl4
 fingerprint_ignore_patterns: []
 connections: []
 contracts: []
 protocols: []
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
 behaviours:
   main:
     args: {}
     class_name: TestAbciConsensusBehaviour
 handlers:
   abci:
     args: {}
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/test_ipfs_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/test_ipfs_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/README.md` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/README.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/fsm_specification.yaml` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/fsm_specification.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/models.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/payload_tools.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/payload_tools.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/skill.yaml` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/skill.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,22 @@
   tests/test_payloads.py: bafybeidvjqvjvnuw5vt4zgnqwzopvprznmefosqy3wcxukvobaiishygze
   tests/test_rounds.py: bafybeia6ftd7hfgb7wqnlua37u2bwre54nlh4jcbue2fgkmx3sxy2lijna
   tests/test_tools/__init__.py: bafybeiaq2ftmklvu5vqq6vdfa7mrlmrnusluki35jm5n2yzf57ox5dif74
   tests/test_tools/test_integration.py: bafybeigv6fxogm3aq3extahr75owdqnzepouv3rtxl3m4gai2urtz6u4ea
 fingerprint_ignore_patterns: []
 connections: []
 contracts:
-- valory/gnosis_safe:0.1.0:bafybeihwwv5aodluykglsbuhhrwusvjof6vvnr37rznwvlutmfwtvoju34
+- valory/gnosis_safe:0.1.0:bafybeibzfhpib5fw3wady6dhq5bfgo37o437bi4s3hthbvvit7byvbalg4
 protocols:
 - open_aea/signing:1.0.0:bafybeibqlfmikg5hk4phzak6gqzhpkt6akckx7xppbp53mvwt6r73h7tk4
 - valory/abci:0.1.0:bafybeig3dj5jhsowlvg3t73kgobf6xn4nka7rkttakdb2gwsg5bp7rt7q4
 - valory/contract_api:1.0.0:bafybeidv6wxpjyb2sdyibnmmum45et4zcla6tl63bnol6ztyoqvpl4spmy
 - valory/ledger_api:1.0.0:bafybeih6hfzj2obw5oajnt6ng6355edgvi5ngoaub44vpuszqoplfvyaom
 skills:
-- valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi
+- valory/abstract_round_abci:0.1.0:bafybeib2jw7hjccou42wis35orckwycb2dgjk7yw46anuqysf2h7su3fi4
 behaviours:
   main:
     args: {}
     class_name: TransactionSettlementRoundBehaviour
 handlers:
   abci:
     args: {}
@@ -156,11 +156,11 @@
     args: {}
     class_name: SharedState
   tendermint_dialogues:
     args: {}
     class_name: TendermintDialogues
 dependencies:
   open-aea-test-autonomy:
-    version: ==0.9.0
+    version: ==0.9.1
   web3:
     version: ==5.25.0
 is_abstract: true
```

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/test_tools/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/test_tools/integration.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/test_tools/integration.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_behaviours.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_dialogues.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_handlers.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_models.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_payload_tools.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_payload_tools.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_payloads.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_rounds.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_rounds.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_tools/__init__.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/packages/valory/skills/transaction_settlement_abci/tests/test_tools/test_integration.py` & `open-autonomy-0.9.1/packages/valory/skills/transaction_settlement_abci/tests/test_tools/test_integration.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/pytest.ini` & `open-autonomy-0.9.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/RELEASE_PROCESS.md` & `open-autonomy-0.9.1/scripts/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/__init__.py` & `open-autonomy-0.9.1/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/check_copyright.py` & `open-autonomy-0.9.1/scripts/check_copyright.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/check_doc_ipfs_hashes.py` & `open-autonomy-0.9.1/scripts/check_doc_ipfs_hashes.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/check_doc_links.py` & `open-autonomy-0.9.1/scripts/check_doc_links.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 """This module contains the tests for the links in the documentation."""
 
 
 import re
 import sys
 from concurrent.futures import ThreadPoolExecutor
+from itertools import chain
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import requests
 import urllib3  # type: ignore
 from requests.adapters import HTTPAdapter  # type: ignore
 from requests.packages.urllib3.util.retry import (  # type: ignore # pylint: disable=import-error
@@ -52,15 +53,14 @@
 
 # Special links that are allowed to respond with an error status
 # Remove non-url-allowed characters like ` before adding them here
 URL_SKIPS = [
     "https://gateway.autonolas.tech/ipfs/<hash>,",  # non link (400)
     "https://github.com/valory-xyz/open-autonomy/trunk/infrastructure",  # svn link (404)
     "http://host.docker.internal:8545",  # internal (ERR_NAME_NOT_RESOLVED)
-    "https://autonolas.network/whitepaper/autonolas-whitepaper.pdf",  # temporarily not available
 ]
 
 # Define here custom timeouts for some edge cases
 CUSTOM_TIMEOUTS = {
     "http://www.fipa.org/repository/ips.php3": 30,
 }
 
@@ -126,15 +126,22 @@
         "http_links": http_links,
         "broken_links": broken_links,
     }
 
 
 def main() -> None:  # pylint: disable=too-many-locals
     """Check for broken or HTTP links"""
-    all_md_files = [str(p.relative_to(".")) for p in Path("docs").rglob("*.md")]
+    all_md_files = [
+        str(p.relative_to("."))
+        for p in chain(
+            Path("docs").rglob("*.md"),
+            Path("packages").rglob("*.md"),
+            Path(".").glob("*.md"),
+        )
+    ]
 
     broken_links: Dict[str, Dict] = {}
     http_links: Dict[str, List[str]] = {}
 
     # Configure request retries
     retry_strategy = Retry(
         total=3,  # number of retries
```

### Comparing `open-autonomy-0.9.0/scripts/check_ipfs_hashes_pushed.py` & `open-autonomy-0.9.1/scripts/check_ipfs_hashes_pushed.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/check_pipfiles.py` & `open-autonomy-0.9.1/scripts/check_pipfiles.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/generate_api_documentation.py` & `open-autonomy-0.9.1/scripts/generate_api_documentation.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/generate_package_list.py` & `open-autonomy-0.9.1/scripts/generate_package_list.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/spell-check.sh` & `open-autonomy-0.9.1/scripts/spell-check.sh`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/scripts/whitelist.py` & `open-autonomy-0.9.1/scripts/whitelist.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/setup.cfg` & `open-autonomy-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/setup.py` & `open-autonomy-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/__init__.py` & `open-autonomy-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/conftest.py` & `open-autonomy-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/__init__.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/agents/dummy_agent/__init__.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/agents/dummy_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/agents/dummy_agent/aea-config.yaml` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/agents/dummy_agent/aea-config.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/__init__.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.yaml` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/connections/dummy_connection/connection.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/__init__.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/contract.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/contracts/dummy_contract/contract.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/__init__.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/message.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/message.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/protocol.yaml` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/protocol.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/serialization.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/protocols/dummy_protocol/serialization.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/__init__.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/behaviours.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/behaviours.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/handlers.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/my_model.py` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/my_model.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/dummy_author/skills/dummy_skill/skill.yaml` & `open-autonomy-0.9.1/tests/data/dummy_packages/dummy_author/skills/dummy_skill/skill.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_packages/packages.json` & `open-autonomy-0.9.1/tests/data/dummy_packages/packages.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_1.yaml` & `open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_1.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_2.yaml` & `open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_2.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_3.yaml` & `open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_3.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/dummy_service_config_files/service_4.yaml` & `open-autonomy-0.9.1/tests/data/dummy_service_config_files/service_4.yaml`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/specs/fsm_specification.json` & `open-autonomy-0.9.1/tests/data/specs/fsm_specification.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/data/specs/fsm_specification_extra.json` & `open-autonomy-0.9.1/tests/data/specs/fsm_specification_extra.json`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/base.py` & `open-autonomy-0.9.1/tests/test_autonomy/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_chain/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_chain/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_chain/base.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_chain/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_chain/test_metadata.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_chain/test_metadata.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_chain/test_mint.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_chain/test_mint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_chain/test_utils.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_chain/test_utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/base.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/base.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_abci/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstring_generator.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstring_generator.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstrings.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_abci/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_benchmarks.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_check_dialogues.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_check_dialogues.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_check_handlers.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_check_handlers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_specs.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_specs.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_analyse/test_verify_service.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_analyse/test_verify_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,26 +20,32 @@
 """Test `autonomy analyse service` command"""
 
 import logging
 from copy import deepcopy
 from typing import Any, Dict, List, Tuple
 from unittest import mock
 
-import pytest
-from aea.configurations.base import AgentConfig
-from aea.configurations.data_types import ComponentId, ComponentType, PublicId
+from aea.configurations.base import AgentConfig, SkillConfig
+from aea.configurations.data_types import (
+    ComponentId,
+    ComponentType,
+    PackageId,
+    PackageType,
+    PublicId,
+)
 from aea.helpers.cid import to_v0
-from aea_cli_ipfs.ipfs_utils import IPFSTool
+from aea_cli_ipfs.ipfs_utils import IPFSDaemon, IPFSTool
 
 from autonomy.analyse.service import ServiceAnalyser
 from autonomy.configurations.base import Service
 
 from tests.test_autonomy.test_cli.base import BaseCliTest
 
 
+DUMMY_SERVICE_HASH = "bafybeib56ojddzexxbapowofypmpk6zeznqaumwgj7ftneb5ua6sk5k5vj"
 DUMMY_AGENT_HASH = "bafybeib56ojddzexxbapowofypmpk6zeznqaumwgj7ftneb5ua6sk5k5vm"
 DUMMY_LEDGER_CONNECTION_HASH = (
     "bafybeib56ojddzexxbapowofypmpk6zeznqaumwgj7ftneb5ua6sk5k5vn"
 )
 DUMMY_ABCI_CONNECTION_HASH = (
     "bafybeib56ojddzexxbapowofypmpk6zeznqaumwgj7ftneb5ua6sk5k5vo"
 )
@@ -74,14 +80,15 @@
                 "args": {
                     "message": "Hello, World!",
                     "setup": {
                         "safe_contract_address": [
                             ["0xAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA"]
                         ],
                         "all_participants": [["0x"]],
+                        "consensus_threshold": [],
                     },
                     "tendermint_url": "tendermint_url",
                     "tendermint_com_url": "tendermint_com_url",
                     "tendermint_p2p_url": "tendermint_p2p_url",
                     "service_registry_address": "service_registry_address",
                     "share_tm_config_on_startup": "share_tm_config_on_startup",
                     "on_chain_service_id": "on_chain_service_id",
@@ -152,35 +159,95 @@
             "disable_existing_loggers": False,
         },
         "dependencies": {},
         "default_connection": None,
     }
 
 
-@pytest.mark.skip
+def get_dummy_skill_config() -> Dict:
+    """Returns dummy skill config"""
+    return {
+        "name": "abci_skill",
+        "author": "valory",
+        "version": "0.1.0",
+        "type": "skill",
+        "description": "Hello World ABCI application.",
+        "license": "Apache-2.0",
+        "aea_version": ">=1.0.0, <2.0.0",
+        "fingerprint": {},
+        "fingerprint_ignore_patterns": [],
+        "connections": [],
+        "contracts": [],
+        "protocols": [],
+        "skills": [
+            "valory/abstract_round_abci:0.1.0:bafybeiami2y2uwvtmjf76hl3jvfahujdir5docjby6erdyjl66ekoblesi"
+        ],
+        "behaviours": {"main": {"args": {}, "class_name": "DummyBehaviour"}},
+        "handlers": {},
+        "models": {
+            "params": {
+                "args": {
+                    "cleanup_history_depth": 1,
+                    "cleanup_history_depth_current": None,
+                    "drand_public_key": "drand_public_key",
+                    "genesis_config": {},
+                    "keeper_timeout": 30,
+                    "max_attempts": 10,
+                    "max_healthcheck": 120,
+                    "observation_interval": 10,
+                    "on_chain_service_id": None,
+                    "request_retry_delay": 1,
+                    "request_timeout": 10,
+                    "reset_tendermint_after": 2,
+                    "retry_attempts": 400,
+                    "retry_timeout": 3,
+                    "round_timeout_seconds": 30,
+                    "service_id": "hello_world_abci",
+                    "service_registry_address": None,
+                    "setup": {
+                        "all_participants": [
+                            "- '0x0000000000000000000000000000000000000000'"
+                        ],
+                        "safe_contract_address": [
+                            "0x0000000000000000000000000000000000000000"
+                        ],
+                        "consensus_threshold": [None],
+                    },
+                    "share_tm_config_on_startup": False,
+                    "sleep_time": 1,
+                    "tendermint_check_sleep_delay": 3,
+                    "tendermint_com_url": "http://localhost:8080",
+                    "tendermint_max_retries": 5,
+                    "tendermint_p2p_url": "localhost:26656",
+                    "tendermint_url": "http://localhost:26657",
+                    "tx_timeout": 10,
+                },
+                "class_name": "Params",
+            },
+        },
+        "dependencies": {},
+        "is_abstract": False,
+    }
+
+
 class BaseAnalyseServiceTest(BaseCliTest):
     """Base class for service verifier tests"""
 
     cli_options: Tuple[str, ...] = ("analyse", "service")
+    public_id_option = ("--public-id", "valory/service")
+    token_id_option = ("--token-id", "1")
 
     @classmethod
     def setup_class(cls) -> None:
         """Setup class."""
         super().setup_class()
 
         cls.cli_runner.mix_stderr = False
 
     @staticmethod
-    def patch_check_agent_package_published(**kwargs: Any) -> mock._patch:
-        """Patch `ServiceAnalyser.check_agent_package_published` method"""
-        return mock.patch.object(
-            ServiceAnalyser, "check_agent_package_published", **kwargs
-        )
-
-    @staticmethod
     def patch_check_agent_dependencies_published(**kwargs: Any) -> mock._patch:
         """Patch `ServiceAnalyser.check_agent_dependencies_published` method"""
         return mock.patch.object(
             ServiceAnalyser, "check_agent_dependencies_published", **kwargs
         )
 
     @staticmethod
@@ -202,121 +269,164 @@
 
     @staticmethod
     def patch_ipfs_tool(pins: List[str]) -> mock._patch:
         """Patch `ServiceAnalyser.check_skill_override` method"""
         return mock.patch.object(IPFSTool, "all_pins", return_value=pins)
 
     @staticmethod
-    def patch_service_loader(data: List[Dict[str, Any]]) -> mock._patch:
+    def patch_check_on_chain_state(**kwargs: Any) -> mock._patch:
+        """Patch `ServiceAnalyser.check_on_chain_state` method"""
+        return mock.patch.object(ServiceAnalyser, "check_on_chain_state", **kwargs)
+
+    @staticmethod
+    def patch_ipfs_daemon_is_started(**kwargs: Any) -> mock._patch:
+        """Patch IPFSDaemon.is_started method"""
+        return mock.patch.object(
+            IPFSDaemon,
+            "is_started",
+            **kwargs,
+        )
+
+    @staticmethod
+    def patch_loader(
+        service_data: List[Dict[str, Any]],
+        agent_data: List[Dict[str, Any]],
+        skill_data: Dict[str, Any],
+        is_remote: bool = False,
+    ) -> mock._patch:
         """Patch service loader method"""
 
-        config, *overrides = data
-        service = Service.from_json(config)
-        service.overrides = overrides
+        def _loader_patch(package_id: PackageId, **kargs: Any) -> Any:
+            if package_id.package_type == PackageType.SERVICE:
+                config, *overrides = service_data
+                service = Service.from_json(config)
+                service.overrides = overrides
+                return service
+
+            if package_id.package_type == PackageType.AGENT:
+                config, *_overrides = agent_data
+                agent_config = AgentConfig.from_json(config)
+                if len(_overrides) > 0:
+                    processed_overrides = {}
+                    for o in _overrides:
+                        processed_overrides[
+                            ComponentId(
+                                component_type=ComponentType(o.pop("type")),
+                                public_id=PublicId.from_str(o.pop("public_id")),
+                            )
+                        ] = o
+                    agent_config.component_configurations = processed_overrides
+                return agent_config
+
+            if package_id.package_type == PackageType.SKILL:
+                return SkillConfig.from_json(skill_data)
+
+        if is_remote:
+            return mock.patch(
+                "autonomy.cli.helpers.analyse._load_from_ipfs",
+                new=_loader_patch,
+            )
 
         return mock.patch(
-            "autonomy.analyse.service.load_service_config",
-            return_value=service,
+            "autonomy.cli.helpers.analyse._load_from_local",
+            new=_loader_patch,
         )
 
     @staticmethod
-    def patch_agent_loader(data: List[Dict[str, Any]]) -> mock._patch:
-        """Patch agent loader method"""
-        config, *_overrides = data
-        agent_config = AgentConfig.from_json(config)
-        if len(_overrides) > 0:
-            overrides = {}
-            for o in _overrides:
-                overrides[
-                    ComponentId(
-                        component_type=ComponentType(o.pop("type")),
-                        public_id=PublicId.from_str(o.pop("public_id")),
-                    )
-                ] = o
-            agent_config.component_configurations = overrides
+    def patch_get_on_chain_service_id() -> mock._patch:
+        """Patch _get_on_chain_service_id"""
 
         return mock.patch(
-            "autonomy.cli.helpers.analyse._load_agent_from_ipfs",
-            return_value=agent_config,
+            "autonomy.cli.helpers.analyse._get_on_chain_service_id",
+            return_value=PackageId(
+                package_type=PackageType.SERVICE,
+                public_id=PublicId.from_str(f"valory/service:{DUMMY_SERVICE_HASH}"),
+            ),
         )
 
 
 class TestCheckRequiredOverrides(BaseAnalyseServiceTest):
     """Test override verification."""
 
     def test_abci_skill_params_not_defined(self) -> None:
         """Test successful run."""
 
         skill_config = get_dummy_overrides_skill()
         del skill_config["models"]["params"]
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), skill_config]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ):
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[get_dummy_service_config(), skill_config],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]):
+            result = self.run_cli(commands=self.public_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert (
             "ABCI skill validation failed; 'params' is a required property"
             in result.stderr
-        )
+        ), result.stdout
 
-    def test_abci_skill_required_arg_not_defined(self) -> None:
+    def test_abci_skill_required_arg_not_defined(self, caplog: Any) -> None:
         """Test successful run."""
 
         skill_config = get_dummy_overrides_skill()
         del skill_config["models"]["params"]["args"]["tendermint_url"]
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), skill_config]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ):
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[get_dummy_service_config(), skill_config],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]), caplog.at_level(logging.WARNING):
+            result = self.run_cli(commands=self.public_id_option)
 
-        assert result.exit_code == 1, result.stdout
+        assert result.exit_code == 0, result.stdout
         assert (
-            "Error: ABCI skill validation failed; 'tendermint_url' is a required property"
-            in result.stderr
+            "ServiceAnalyser:service.py:284 (agent, valory/dummy_agent:0.1.0) contains configuration which is missing from (service, valory/dummy_service:0.1.0)"
+            in caplog.text
         )
+        assert "Path: models.params.args" in caplog.text
+        assert "Missing parameters: {'tendermint_url'}" in caplog.text
 
     def test_abci_skill_setup_param_not_defined(self) -> None:
         """Test successful run."""
 
         skill_config = get_dummy_overrides_skill()
 
         del skill_config["models"]["params"]["args"]["setup"]["all_participants"]
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), skill_config]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ):
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[get_dummy_service_config(), skill_config],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]):
+            result = self.run_cli(commands=self.public_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert (
             "Error: ABCI skill validation failed; 'all_participants' is a required property"
             in result.stderr
         )
 
     def test_ledger_connection_ledger_not_defined(self) -> None:
         """Test successful run."""
 
         connection_config = get_dummy_overrides_ledger_connection()
         del connection_config["config"]["ledger_apis"]["ethereum"]
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), connection_config]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ):
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[
+                get_dummy_service_config(),
+                get_dummy_overrides_skill(),
+                connection_config,
+            ],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]):
+            result = self.run_cli(commands=self.public_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert (
             "Error: Ledger connection validation failed; {} does not have enough properties"
             in result.stderr
         )
 
@@ -324,178 +434,196 @@
         """Test successful run."""
 
         connection_config = get_dummy_overrides_ledger_connection()
         connection_config["config"]["ledger_apis"]["solana"] = connection_config[
             "config"
         ]["ledger_apis"]["ethereum"]
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), connection_config]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ), caplog.at_level(
-            logging.WARN
-        ):
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[
+                get_dummy_service_config(),
+                get_dummy_overrides_skill(),
+                connection_config,
+            ],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]), caplog.at_level(logging.WARNING):
+            result = self.run_cli(commands=self.public_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert "Unknown ledger configuration found with name `solana`" in caplog.text
 
     def test_ledger_connection_param_not_defined(self) -> None:
         """Test successful run."""
 
         connection_config = get_dummy_overrides_ledger_connection()
         del connection_config["config"]["ledger_apis"]["ethereum"]["address"]
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), connection_config]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ):
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[
+                get_dummy_service_config(),
+                get_dummy_overrides_skill(),
+                connection_config,
+            ],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]):
+            result = self.run_cli(commands=self.public_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert (
             "Error: Ledger connection validation failed; 'address' is a required property"
             in result.stderr
         )
 
     def test_abci_connection_setup_param_not_defined(self) -> None:
         """Test successful run."""
 
         connection_config = get_dummy_overrides_abci_connection()
         del connection_config["config"]["host"]
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), connection_config]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ):
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[
+                get_dummy_service_config(),
+                get_dummy_overrides_skill(),
+                connection_config,
+            ],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]):
+            result = self.run_cli(commands=self.public_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert (
             "Error: ABCI connection validation failed; 'host' is a required property"
             in result.stderr
         )
 
 
-class TestCheckAgentPackagePublished(BaseAnalyseServiceTest):
+class TestCheckAgentDependenciesPublished(BaseAnalyseServiceTest):
     """Test `check_agent_package_published` method."""
 
-    def test_agent_not_found(self) -> None:
+    def test_dependency_not_found(self) -> None:
         """Test failure."""
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), get_dummy_overrides_skill()]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ), self.patch_validate_service_overrides():
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[get_dummy_service_config(), get_dummy_overrides_skill()],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+            is_remote=True,
+        ), self.patch_ipfs_tool(
+            []
+        ), self.patch_validate_service_overrides(), self.patch_ipfs_daemon_is_started(
+            return_value=True,
+        ), self.patch_get_on_chain_service_id(), self.patch_check_on_chain_state():
+            result = self.run_cli(commands=self.token_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert (
-            "Agent package for service valory/dummy_service:0.1.0 not published on the IPFS registry"
+            "Error: Package required for service valory/dummy_service:0.1.0 is not published on the IPFS registry"
             in result.stderr
         )
+        assert "agent: valory/dummy_agent:0.1.0" in result.stderr
 
 
 class TestVerifyOverrides(BaseAnalyseServiceTest):
     """Test verify overrides method."""
 
     def test_missing_override(self) -> None:
         """Test missing override section from agent config."""
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), get_dummy_overrides_skill()]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ), self.patch_validate_service_overrides(), self.patch_check_agent_package_published():
-            result = self.run_cli(commands=(str(self.t),))
-
-        assert result.exit_code == 1, result.stdout
-        assert (
-            "Service config has an overrides which are not defined in the agent config; "
-            "packages with missing overrides={PackageId(skill, valory/abci_skill:0.1.0)}"
-            in result.stderr
-        )
-
-
-class TestCheckAgentDependenciesPublished(BaseAnalyseServiceTest):
-    """Test `check_agent_dependencies_published` method."""
-
-    def test_dependency_missing_from_ipfs(self) -> None:
-        """Test missing dependency"""
-
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), get_dummy_overrides_skill()]
-        ), self.patch_ipfs_tool([]), self.patch_agent_loader(
-            data=[get_dummy_agent_config()]
-        ), self.patch_validate_service_overrides(), self.patch_check_agent_package_published(), self.patch_verify_overrides():
-            result = self.run_cli(commands=(str(self.t),))
+        with self.patch_loader(
+            service_data=[
+                get_dummy_service_config(),
+                get_dummy_overrides_skill(),
+                get_dummy_overrides_ledger_connection(),
+            ],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+        ), self.patch_ipfs_tool([]), self.patch_validate_service_overrides():
+            result = self.run_cli(commands=self.public_id_option)
 
         assert result.exit_code == 1, result.stdout
         assert (
-            "Package required for service valory/dummy_service:0.1.0 is not published on the IPFS registry"
+            "Error: Service config has an overrides which are not defined in the agent config;"
+            " packages with missing overrides={PackageId(connection, valory/ledger:0.1.0)}"
             in result.stderr
         )
 
 
 class TestCheckOnChainState(BaseAnalyseServiceTest):
     """Test `check_on_chain_state` method."""
 
-    def test_on_chain_status_check(self) -> None:
+    def test_on_chain_status_check(self, caplog: Any) -> None:
         """Test `check_on_chain_state` failure"""
 
-        with self.patch_service_loader(
-            data=[get_dummy_service_config(), get_dummy_overrides_skill()]
+        with self.patch_loader(
+            service_data=[get_dummy_service_config(), get_dummy_overrides_skill()],
+            agent_data=[get_dummy_agent_config(), get_dummy_overrides_skill()],
+            skill_data=get_dummy_skill_config(),
+            is_remote=True,
         ), mock.patch(
             "autonomy.analyse.service.get_service_info", return_value=[None, 0, None]
+        ), self.patch_ipfs_tool(
+            []
+        ), self.patch_ipfs_daemon_is_started(
+            return_value=True,
+        ), self.patch_get_on_chain_service_id(), caplog.at_level(
+            logging.WARNING
         ):
-            result = self.run_cli(commands=(str(self.t), "--token-id", "1"))
+            result = self.run_cli(commands=self.token_id_option)
 
         assert result.exit_code == 1, result.stdout
-        assert "Service needs to be in deployed state on-chain" in result.stderr
+        assert (
+            "Service needs to be in deployed state on-chain; Current state=ServiceState.NON_EXISTENT"
+            in caplog.text
+        )
 
 
 class TestCheckSuccessful(BaseAnalyseServiceTest):
     """Test a successful check"""
 
     def test_run(self) -> None:
         """Test run."""
 
         skill_config = get_dummy_overrides_skill()
         models = skill_config.pop("models")
         for i in range(4):
             skill_config[i] = {"models": deepcopy(models)}
 
-        with self.patch_service_loader(
-            data=[
+        with self.patch_loader(
+            service_data=[
                 get_dummy_service_config(),
                 skill_config,
                 get_dummy_overrides_abci_connection(),
                 get_dummy_overrides_ledger_connection(),
-            ]
+            ],
+            agent_data=[
+                get_dummy_agent_config(),
+                get_dummy_overrides_skill(),
+                get_dummy_overrides_abci_connection(),
+                get_dummy_overrides_ledger_connection(),
+            ],
+            skill_data=get_dummy_skill_config(),
+            is_remote=True,
         ), self.patch_ipfs_tool(
             pins=list(
                 map(
                     to_v0,
                     [
                         DUMMY_AGENT_HASH,
                         DUMMY_LEDGER_CONNECTION_HASH,
                         DUMMY_ABCI_CONNECTION_HASH,
                         DUMMY_SKILL_HASH,
                     ],
                 )
             )
-        ), self.patch_agent_loader(
-            data=[
-                get_dummy_agent_config(),
-                get_dummy_overrides_skill(),
-                get_dummy_overrides_abci_connection(),
-                get_dummy_overrides_ledger_connection(),
-            ]
+        ), self.patch_ipfs_daemon_is_started(
+            return_value=True,
+        ), self.patch_get_on_chain_service_id(), mock.patch(
+            "autonomy.analyse.service.get_service_info",
+            return_value=(None, 4, None),
         ):
-            result = self.run_cli(commands=(str(self.t),))
+            result = self.run_cli(commands=self.token_id_option)
 
         assert result.exit_code == 0, result.stderr
         assert "Service is ready to be deployed" in result.output
```

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_build_image.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_build_image.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_build/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_build/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_build/test_deployment.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_build/test_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,22 +469,14 @@
         """Check kubernetes build dir."""
 
         build_tree = list(map(lambda x: x.name, build_dir.iterdir()))
         assert any(
             child in build_tree for child in ["persistent_storage", "build.yaml"]
         )
 
-        kubernetes_config = cls.load_kubernetes_config(path=build_dir)
-        assert all(
-            [
-                resource["metadata"]["name"] != "config-nodes"
-                for resource in kubernetes_config
-            ]
-        )
-
     def test_kubernetes_build(
         self,
     ) -> None:
         """Run tests."""
 
         build_dir = self.t / DEFAULT_BUILD_FOLDER
         with mock.patch("os.chown"):
```

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_from_token.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_from_token.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_deploy/test_run_deployment.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_deploy/test_run_deployment.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_develop/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_develop/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_develop/test_local_service_registry.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_develop/test_local_service_registry.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_fetch.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_fetch.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_hash.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_hash.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/test_chain_helpers.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/test_chain_helpers.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/test_docstrings.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_helpers/test_fsm_spec.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_helpers/test_fsm_spec.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_mint/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_mint/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_mint/test_mint_components.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_mint/test_mint_components.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_packages.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_packages.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_publish.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_push_all.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_push_all.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_replay/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_replay/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_replay/test_agent.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_replay/test_agent.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_replay/test_tendermint.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_replay/test_tendermint.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_scaffold_fsm.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_scaffold_fsm.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_service/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_service/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_service/test_service_manager.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_service/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_utils/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_cli/test_utils/test_click_utils.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_cli/test_utils/test_click_utils.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_configurations.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_configurations.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_constants.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_constants.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_deploy/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_deploy/test_deployment_generators.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_deploy/test_deployment_generators.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_deploy/test_service_specification.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_deploy/test_service_specification.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_images/__init__.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_images/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_images/base.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_images/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,35 +15,44 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 
 """Tools for testing docker images"""
 
+import contextlib
 import json
 from pathlib import Path
-from typing import Dict, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import docker
+from docker.errors import APIError
+from docker.models.containers import Container
 
 
 class BaseImageBuildTest:
     """Test image build and run."""
 
     client: docker
     path: Path
     tag: str
     agent: str
 
+    running_containers: List[Container]
+
     @classmethod
     def setup_class(cls) -> None:
         """Setup class."""
 
         cls.client = docker.from_env()
 
+    def setup(self) -> None:
+        """Setup test."""
+        self.running_containers = []
+
     def build_image(
         self,
         path: Path,
         tag: str,
         buildargs: Optional[Dict[str, str]] = None,
     ) -> Tuple[bool, str]:
         """Build docker image."""
@@ -67,7 +76,15 @@
                     return False, stream_data["errorDetail"]["message"]
                 elif "aux" in stream_data:
                     output += stream_data["aux"]["ID"]
                 elif "status" in stream_data:
                     output += stream_data["status"]
 
         return True, output
+
+    def teardown(self) -> None:
+        """Teardown test."""
+
+        for container in self.running_containers:
+            with contextlib.suppress(APIError):
+                container.kill()
+                container.wait(timeout=30)
```

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_images/test_autonomy.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_images/test_autonomy.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_images/test_runtime.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_images/test_runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,14 +115,16 @@
                 network="host",
                 extra_hosts={
                     DEFAULT_ABCI_HOST: "host-gateway",
                 },
             ),
         )
 
+        self.running_containers += [tm_container, agent_container]
+
         def _check_for_outputs() -> bool:
             """Check for required outputs."""
             return (
                 b"Entered in the 'registration_round' round for period 0"
                 in agent_container.logs()
             )
 
@@ -132,16 +134,10 @@
                 timeout=30,
                 period=1,
             )
             successful = True
         except TimeoutError:
             successful = False
 
-        tm_container.kill()
-        tm_container.wait(timeout=5)
-
-        agent_container.kill()
-        agent_container.wait(timeout=5)
-
         assert (
             successful
-        ), f"Agent runtime failed with {agent_container.logs().decode()}"
+        ), f"Agent runtime failed with error: {agent_container.logs().decode()}"
```

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_images/test_tendermint.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_images/test_tendermint.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,23 +79,26 @@
                     },
                     volumes={
                         temp_dir: {"bind": "/logs", "mode": "rw"},
                     },
                 ),
             )
 
+            self.running_containers = [
+                tm_container,
+            ]
+
             def _check_for_outputs() -> bool:
                 """Check for required outputs."""
                 return "abci.socketClient failed to connect" in log_file.read_text()
 
             try:
                 wait_for_condition(
                     condition_checker=_check_for_outputs,
                     timeout=10,
                     period=1,
                 )
                 successful = True
             except TimeoutError:
                 successful = False
 
-            tm_container.kill()
             assert successful, f"Tendermint runtime failed with {log_file.read_text()}"
```

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_package_manager.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_package_manager.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_autonomy/test_replay.py` & `open-autonomy-0.9.1/tests/test_autonomy/test_replay.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_base.py` & `open-autonomy-0.9.1/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             f"*/{package_type.to_plural()}/*/{PACKAGE_TYPE_TO_CONFIG_FILE[package_type.value]}"
         )
     )
 
 
 def test_version() -> None:
     """Test the version."""
-    assert autonomy.__version__ == "0.9.0"
+    assert autonomy.__version__ == "0.9.1"
 
 
 @pytest.mark.parametrize(
     "component_type,config_file_path",
     itertools.chain.from_iterable(
         [
             itertools.zip_longest([], files, fillvalue=component_type)
```

### Comparing `open-autonomy-0.9.0/tests/test_deployments/__init__.py` & `open-autonomy-0.9.1/tests/test_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_deployments/conftest.py` & `open-autonomy-0.9.1/tests/test_deployments/conftest.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_deployments/test_app.py` & `open-autonomy-0.9.1/tests/test_deployments/test_app.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_deployments/test_deployment_code_identical.py` & `open-autonomy-0.9.1/tests/test_deployments/test_deployment_code_identical.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_deployments/test_deployments.py` & `open-autonomy-0.9.1/tests/test_deployments/test_deployments.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_docs/helper.py` & `open-autonomy-0.9.1/tests/test_docs/helper.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_docs/test_code_blocks.py` & `open-autonomy-0.9.1/tests/test_docs/test_code_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         # },  # flake8: noqa: E800
         "docs/guides/configure_access_external_chains.md": {"skip_blocks": [0]},
     }
 
     skipped_files = [
         "docs/guides/service_configuration_file.md",
         "docs/demos/price_oracle_fsms.md",
+        "docs/advanced_reference/developer_tooling/dev_mode.md",
         "docs/deployment/on-chain_deployment_checklist.md",  # just placeholder examples
     ]
 
 
 class TestPythonSnippets(BaseTestDocCode):
     """Test that all the python snippets in the documentation exist in the repository"""
```

### Comparing `open-autonomy-0.9.0/tests/test_docs/test_commands.py` & `open-autonomy-0.9.1/tests/test_docs/test_commands.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tests/test_scripts/test_check_doc_ipfs_hashes.py` & `open-autonomy-0.9.1/tests/test_scripts/test_check_doc_ipfs_hashes.py`

 * *Files identical despite different names*

### Comparing `open-autonomy-0.9.0/tox.ini` & `open-autonomy-0.9.1/tox.ini`

 * *Files identical despite different names*

