# Comparing `tmp/akerbp.mlops-3.1.2a5.tar.gz` & `tmp/akerbp.mlops-3.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-d56omjt1/akerbp.mlops-3.1.2a5.tar", last modified: Fri May 26 13:39:38 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-tzxwcl13/akerbp.mlops-3.2.0a0.tar", last modified: Tue Jun  6 15:06:31 2023, max compression
```

## Comparing `akerbp.mlops-3.1.2a5.tar` & `akerbp.mlops-3.2.0a0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.460501 akerbp.mlops-3.1.2a5/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-26 13:39:38.460501 akerbp.mlops-3.1.2a5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35941 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4240 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.452501 akerbp.mlops-3.1.2a5/bitbucket_pipeline_helpers/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3739 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/install.sh
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.452501 akerbp.mlops-3.1.2a5/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/model_artifact/mlpet_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.452501 akerbp.mlops-3.1.2a5/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     9932 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     5427 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-26 13:39:38.460501 akerbp.mlops-3.1.2a5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.448501 akerbp.mlops-3.1.2a5/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.448501 akerbp.mlops-3.1.2a5/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.452501 akerbp.mlops-3.1.2a5/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-26 13:39:38.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.456501 akerbp.mlops-3.1.2a5/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38633 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.456501 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16951 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.456501 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     6555 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21689 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.456501 akerbp.mlops-3.1.2a5/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22521 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.456501 akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.452501 akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-05-26 13:39:38.000000 akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-26 13:39:38.000000 akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-26 13:39:38.000000 akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-26 13:39:38.000000 akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-26 13:39:38.000000 akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-26 13:39:38.000000 akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.456501 akerbp.mlops-3.1.2a5/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:39:38.460501 akerbp.mlops-3.1.2a5/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-05-26 13:39:15.000000 akerbp.mlops-3.1.2a5/test/test_version_increment.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35467 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4908 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.417051 akerbp.mlops-3.2.0a0/bitbucket_pipeline_helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.417051 akerbp.mlops-3.2.0a0/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/model_artifact/mlpet_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.421051 akerbp.mlops-3.2.0a0/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     5427 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.417051 akerbp.mlops-3.2.0a0/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.417051 akerbp.mlops-3.2.0a0/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.421051 akerbp.mlops-3.2.0a0/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-06 15:06:31.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.421051 akerbp.mlops-3.2.0a0/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    37962 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.421051 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16504 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21442 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22658 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.421051 akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-06 15:06:31.000000 akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-06-06 15:06:31.000000 akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-06 15:06:31.000000 akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-06 15:06:31.000000 akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-06 15:06:31.000000 akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-06 15:06:31.000000 akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 15:06:31.425051 akerbp.mlops-3.2.0a0/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-06-06 15:06:00.000000 akerbp.mlops-3.2.0a0/test/test_version_increment.py
```

### Comparing `akerbp.mlops-3.1.2a5/.flake8` & `akerbp.mlops-3.2.0a0/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/.pre-commit-config.yaml` & `akerbp.mlops-3.2.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/LICENSE` & `akerbp.mlops-3.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/PKG-INFO` & `akerbp.mlops-3.2.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.1.2a5
+Version: 3.2.0a0
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -724,35 +724,31 @@
 ## Local Testing and Deployment
 It's possible to tests the functions locally, which can help you debug errors
 quickly. This is recommended before a deployment.
 
 Define the following environmental variables (e.g. in `.bashrc`):
 ```bash
 export MODEL_ENV=dev
-export COGNITE_API_KEY_PERSONAL=xxx
-export COGNITE_API_KEY_FUNCTIONS=$COGNITE_API_KEY_PERSONAL
-export COGNITE_API_KEY_DATA=$COGNITE_API_KEY_PERSONAL
-export COGNITE_API_KEY_FILES=$COGNITE_API_KEY_PERSONAL
+export COGNITE_OIDC_BASE_URL=https://api.cognitedata.com
+export COGNITE_TENANT_ID=<tenant id>
+export COGNITE_CLIENT_ID_WRITE=<write access client id>
+export COGNITE_CLIENT_SECRET_WRITE=<write access client secret>
+export COGNITE_CLIENT_ID_READ=<read access client id>
+export COGNITE_CLIENT_SECRET_READ=<read access client secret>
 ```
 
 From your repo's root folder:
 - `python -m pytest model_code` (replace `model_code` by your model code folder
   name)
 - `deploy_prediction_service`
 - `deploy_training_service` (if there's a training service)
 
 The first one will run your model tests. The last two run model tests but also
 the service tests implemented in the framework and simulate deployment.
 
-If you really want to deploy from your development environment, you can run
-this: `LOCAL_DEPLOYMENT=True deploy_prediction_service`
-
-Note that, in case of emergency, it's possible to deploy to test or production
-from your local environment, e.g. : `LOCAL_DEPLOYMENT=True MODEL_ENV=test deploy_prediction_service`
-
 If you want to run tests only you need to set `TESTING_ONLY=True` before calling the deployment script.
 
 ## Automated Deployments from Bitbucket
 Deployments to the test environment are triggered by commits (you need to push
 them). Deployments to the production environment are enabled manually from the
 Bitbucket pipeline dashboard. Branches that match 'deploy/*' behave as master.
 Branches that match `feature/*` run tests only (i.e. do not deploy).
@@ -765,15 +761,15 @@
 It is possible to schedule the training service in CDF, and then it can make
 sense to schedule the deployment pipeline of the model service (as often as new
 models are trained)
 
 NOTE: Previous version of akerbp.mlops assumes that calling
 `LOCAL_DEPLOYMENT=True deploy_prediction_service` will not deploy models and run tests.
 The package is now refactored to only trigger tests when the environment variable
-`TESTING_ONLY` is set to `True`, and allows to deploy locally when setting `LOCAL_DEPLOYMENT=True`.
+`TESTING_ONLY` is set to `True`.
 Make sure to update the pipeline definition for branches with prefix `feature/`to call
 `TESTING_ONLY=True deploy_prediction_service` instead.
 
 ## Bitbucket Setup
 The following environments need to be defined in `repository settings >
 deployments`:
 - test deployments: `test-prediction` and `test-training`, each with `MODEL_ENV=test`
@@ -842,17 +838,15 @@
 - Bash scripts will be installed in a `bin` folder in the `PATH`.
 
 The pipeline is setup to build the library from Bitbucket, but it's possible to
 build and upload the library from the development environment as well:
 ```bash
 bash build.sh
 ```
-In general this is required before `LOCAL_DEPLOYMENT=True deploy_xxx_service`. The exception is if local changes affect only the
-deployment part of the library, and the library has been installed in developer
-mode with:
+
 ```
 pip install -e .
 ```
 In this mode, the installed package links to the source code, so that it can be
 modified without the need to reinstall.
 
 ## Bitbucket Setup
```

### Comparing `akerbp.mlops-3.1.2a5/README.md` & `akerbp.mlops-3.2.0a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -505,35 +505,31 @@
 ## Local Testing and Deployment
 It's possible to tests the functions locally, which can help you debug errors
 quickly. This is recommended before a deployment.
 
 Define the following environmental variables (e.g. in `.bashrc`):
 ```bash
 export MODEL_ENV=dev
-export COGNITE_API_KEY_PERSONAL=xxx
-export COGNITE_API_KEY_FUNCTIONS=$COGNITE_API_KEY_PERSONAL
-export COGNITE_API_KEY_DATA=$COGNITE_API_KEY_PERSONAL
-export COGNITE_API_KEY_FILES=$COGNITE_API_KEY_PERSONAL
+export COGNITE_OIDC_BASE_URL=https://api.cognitedata.com
+export COGNITE_TENANT_ID=<tenant id>
+export COGNITE_CLIENT_ID_WRITE=<write access client id>
+export COGNITE_CLIENT_SECRET_WRITE=<write access client secret>
+export COGNITE_CLIENT_ID_READ=<read access client id>
+export COGNITE_CLIENT_SECRET_READ=<read access client secret>
 ```
 
 From your repo's root folder:
 - `python -m pytest model_code` (replace `model_code` by your model code folder
   name)
 - `deploy_prediction_service`
 - `deploy_training_service` (if there's a training service)
 
 The first one will run your model tests. The last two run model tests but also
 the service tests implemented in the framework and simulate deployment.
 
-If you really want to deploy from your development environment, you can run
-this: `LOCAL_DEPLOYMENT=True deploy_prediction_service`
-
-Note that, in case of emergency, it's possible to deploy to test or production
-from your local environment, e.g. : `LOCAL_DEPLOYMENT=True MODEL_ENV=test deploy_prediction_service`
-
 If you want to run tests only you need to set `TESTING_ONLY=True` before calling the deployment script.
 
 ## Automated Deployments from Bitbucket
 Deployments to the test environment are triggered by commits (you need to push
 them). Deployments to the production environment are enabled manually from the
 Bitbucket pipeline dashboard. Branches that match 'deploy/*' behave as master.
 Branches that match `feature/*` run tests only (i.e. do not deploy).
@@ -546,15 +542,15 @@
 It is possible to schedule the training service in CDF, and then it can make
 sense to schedule the deployment pipeline of the model service (as often as new
 models are trained)
 
 NOTE: Previous version of akerbp.mlops assumes that calling
 `LOCAL_DEPLOYMENT=True deploy_prediction_service` will not deploy models and run tests.
 The package is now refactored to only trigger tests when the environment variable
-`TESTING_ONLY` is set to `True`, and allows to deploy locally when setting `LOCAL_DEPLOYMENT=True`.
+`TESTING_ONLY` is set to `True`.
 Make sure to update the pipeline definition for branches with prefix `feature/`to call
 `TESTING_ONLY=True deploy_prediction_service` instead.
 
 ## Bitbucket Setup
 The following environments need to be defined in `repository settings >
 deployments`:
 - test deployments: `test-prediction` and `test-training`, each with `MODEL_ENV=test`
@@ -623,17 +619,15 @@
 - Bash scripts will be installed in a `bin` folder in the `PATH`.
 
 The pipeline is setup to build the library from Bitbucket, but it's possible to
 build and upload the library from the development environment as well:
 ```bash
 bash build.sh
 ```
-In general this is required before `LOCAL_DEPLOYMENT=True deploy_xxx_service`. The exception is if local changes affect only the
-deployment part of the library, and the library has been installed in developer
-mode with:
+
 ```
 pip install -e .
 ```
 In this mode, the installed package links to the source code, so that it can be
 modified without the need to reinstall.
 
 ## Bitbucket Setup
```

### Comparing `akerbp.mlops-3.1.2a5/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.0a0/bitbucket-pipelines.yml`

 * *Files 12% similar despite different names*

```diff
@@ -10,45 +10,49 @@
 image: python:3.8.5
 
 clone:
   depth: full
   lfs: true
 
 definitions:
+  .set-environment-dev: &set-environment-dev |
+    export MODEL_ENV=dev
+    export SERVICE_NAME=prediction
+
   .set-environment-test: &set-environment-test |
     export MODEL_ENV=test
     export SERVICE_NAME=prediction
 
   .install-mlops: &install-mlops |
     git pull
     bash -ex install.sh
 
   steps:
+    - step: &deploy-dev-prediction-service
+        name: Deploy Prediction Service to Dev
+        deployment: dev-prediction
+        caches:
+          - pip
+        script:
+          - *install-mlops
+          - deploy_prediction_service
     - step: &deploy-test-package
-        name: Deploy Pre-release to Test
+        name: Deploy Pre-release Package to PyPI
         deployment: test-pypi
         caches:
           - pip
         script:
           - git pull
           - bash -ex build.sh
-    - step: &deploy-test-prediction-service
-        name: Deploy Prediction Service to Test
-        deployment: test-prediction
-        caches:
-          - pip
-        script:
-          - *install-mlops
-          - deploy_prediction_service
     - step: &run-tests-without-deploying
-        name: Run tests without deploying
+        name: Run Tests Without Deploying
         caches:
           - pip
         script:
-          - *set-environment-test
+          - *set-environment-dev
           - *install-mlops
           - python bitbucket_pipeline_helpers/upload_dummy_artifacts.py
           - TESTING_ONLY=True deploy_prediction_service
           - python bitbucket_pipeline_helpers/remove_dummy_artifacts.py
     - step: &unit-testing
         name: Unit Testing
         caches:
@@ -91,44 +95,54 @@
           - chmod +x ./snyk
           - mv ./snyk /usr/local/bin
           - snyk auth $SNYK_TOKEN
           - snyk test --fail-on=all --print-deps
 
 pipelines:
   pull-requests:
-    "**": # Run for PRs on all branches - Deploy pre-release package and prediction services to test
+    "**": # Run for PRs on all branches
       - parallel:
           - step: *unit-testing
           - step: *flake8-linting
           - step: *mypy-type-checking
           - step: *security-scan-secrets
           - step: *snyk-scan
+      # TODO: if not restricted by cognite, figure out how to install wheels from private repo and run integration tests before deploying pre-release to PyPI
       - step: *deploy-test-package
       - step: *run-tests-without-deploying
-      - step: *deploy-test-prediction-service
+      - step: *deploy-dev-prediction-service
       - step:
-          name: Promote Artifacts to Production
+          name: Promote Artifacts to Test and Prod
           script:
-            - *set-environment-test
+            - *set-environment-dev
             - *install-mlops
             - python bitbucket_pipeline_helpers/upload_dummy_artifacts.py
             - python bitbucket_pipeline_helpers/promote_dummy_artifacts.py
             - python bitbucket_pipeline_helpers/remove_dummy_artifacts.py
+            - *set-environment-test
+            - python bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+            - python bitbucket_pipeline_helpers/remove_dummy_artifacts.py
       - step:
-          <<: *deploy-test-prediction-service
-          name: Deploy Prediction Service to Production
+          <<: *deploy-dev-prediction-service
+          name: Deploy Prediction Service to Test
+          deployment: test-prediction
+      - step:
+          <<: *deploy-dev-prediction-service
+          name: Deploy Prediction Service to Prod
           deployment: production-prediction
 
+
   branches:
     master: # Mirror to public repo and choose to manually deploy package, training and production services to prod
       - step: *unit-testing
       - step:
           name: Mirror Latest Version to Public Repo
           script:
             - git remote add public git@bitbucket.org:akerbp/akerbp.mlops.git
             - git pull
             - git push public master
+      # TODO: Add a step for downloading the pre-release from PyPI and run all the above tests before deploying the stable release
       - step:
           <<: *deploy-test-package
-          name: Deploy Package to Production
+          name: Deploy Stable Version to PyPI
           deployment: production-pypi
           trigger: manual
```

### Comparing `akerbp.mlops-3.1.2a5/build.sh` & `akerbp.mlops-3.2.0a0/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/increment_package_version.py` & `akerbp.mlops-3.2.0a0/increment_package_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         words_in_commit_msg = commit_msg.split()
 
         # Remove special characters from commit message
         for i, word in enumerate(words_in_commit_msg):
             alphanumeric = [char for char in word if char.isalnum()]
             word = "".join(alphanumeric)
             words_in_commit_msg[i] = word
+
         # Increment version based on commit message; Avoid incrementing if we specify to increment a pre-release
         if "prerelease" not in words_in_commit_msg:
             if "major" in words_in_commit_msg:
                 major = str(int(major) + 1)
                 minor, patch = "0", "0"
             elif "minor" in words_in_commit_msg:
                 minor = str(int(minor) + 1)
```

### Comparing `akerbp.mlops-3.1.2a5/mlops_settings.yaml` & `akerbp.mlops-3.2.0a0/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/model_code/model.py` & `akerbp.mlops-3.2.0a0/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/model_code/test_model.py` & `akerbp.mlops-3.2.0a0/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/pyproject.toml` & `akerbp.mlops-3.2.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/cdf/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -983,69 +983,57 @@
         latest_artifact_version = artifact_versions.loc[
             artifact_versions["uploaded_time"].argmax()
         ].metadata["version"]
 
     return int(latest_artifact_version)
 
 
-def get_arguments_for_redeploying_latest_model_version(
+def get_arguments_for_redeploying_numbered_models(
     external_id: str,
 ) -> Tuple[str, str, str, Dict[str, str], str]:
     """Extract data needed to redeploy the latest function from CDF files using a predictable external id,
     i.e. witout the model version number. In this way the client does not have to care about version numbers.
-    In addition to copying the data fields of the function, the description of the function is tagged with (LATEST VERSION),
-    and the version number is added to the metadata (set to 1 if it does not exist)
+    In addition to copying the data fields of the function, the version number is added to the metadata (set to 1 if it does not exist)
 
     Args:
         external_id (str): external id of the deployed function in CDF
 
     Returns:
         (tuple): tuple containing the data needed for redeploying the latest function with a predictable external id
     """
     client = global_client["read"]
     latest_function = client.functions.retrieve(external_id=external_id)
     name = latest_function.name  # type: ignore
     file_id = latest_function.file_id  # type: ignore
-    description = latest_function.description + " (LATEST VERSION)"  # type: ignore
+    description = latest_function.description  # type: ignore
     owner = latest_function.owner  # type: ignore
     metadata = latest_function.metadata  # type: ignore
-    if len(stripped_external_id := latest_function.external_id.split("-")) > 3:  # type: ignore
-        version_number = str(stripped_external_id[-1])  # type: ignore
-    else:
-        version_number = "1"
-    metadata["version"] = version_number  # type: ignore
-    metadata["akerbp.mlops_version"] = mlops_version  # type: ignore
-    try:
-        mlpet_version = package_version("akerbp.mlpet")
-    except PackageNotFoundError:
-        mlpet_version = "not found"
-    metadata["akerbp.mlpet_version"] = mlpet_version  # type: ignore
     return name, file_id, description, metadata, owner  # type: ignore
 
 
 def setup_schedule_for_latest_model_in_prod(
-    predictable_external_id: str,
+    external_id: str,
     client: Optional[CogniteClient] = None,
 ) -> None:
     if client is None:
         client = global_client["write"]
     schedules = client.functions.schedules.list(
-        function_external_id=predictable_external_id,
+        function_external_id=external_id,
     )
     if len(schedules) > 0:
         logger.info("A schedule already exist and will be overwritten")
         for schedule in schedules:
             schedule_id = schedule.id
             client.functions.schedules.delete(id=schedule_id)
 
     _ = client.functions.schedules.create(
         name="Keep warm schedule",
         description="Keep the function warm by calling it with an empty payload every 30 minutes during extended working hours on weekdays",
         cron_expression="*/30 5-17 * * 1-5",
-        function_external_id=predictable_external_id,
+        function_external_id=external_id,
         data={},
     )
     logger.info("Schedule created")
 
 
 def garbage_collection(
     c: config.ServiceSettings,
```

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,19 @@
 class EnvVar:
     """Dataclass for keeping track of environmental variables
 
     Attributes:
         model_env (Optional[str]): environment. Defaults to None
         service_name (Optional[str]): service name. Defaults to None
         platform (Optional[str]): platform. Defaults to None
-        local_deployment (Optional[Union[str, bool]]): local deployment. Defaults to False
     """
 
     model_env: Optional[str] = None
     service_name: Optional[str] = None
     platform: Optional[str] = None
-    local_deployment: Optional[Union[str, bool]] = False
     testing_only: Optional[Union[str, bool]] = False
 
     def __post_init__(self):
         """Post initialization function of the dataclass that validates the attributes env, platform and service_name
         Allowed values for attributes:
             model_env: 'dev', 'test', 'prod'
             platform: 'cdf', 'local'
@@ -71,35 +69,28 @@
 
 
 def read_env_vars() -> EnvVar:
     """
     Read environmental variables and initialize EnvVar object with those that
     were set (i.e. ignored those with None value). Note that
     Default values:
-        LOCAL_DEPLOYMENT: 'False'
         DEPLOYMENT_PLATFORM: 'cdf'
         TESTING_ONLY: 'False'
     """
     envs = dict(
         model_env=os.getenv("MODEL_ENV"),
         service_name=os.getenv("SERVICE_NAME"),
-        local_deployment=os.getenv("LOCAL_DEPLOYMENT", "False"),
         platform=os.getenv("DEPLOYMENT_PLATFORM", "cdf"),
         testing_only=os.getenv("TESTING_ONLY", "False"),
     )
     envs = {k: v for k, v in envs.items() if v is not None}
 
-    # For local testing
-    if envs["local_deployment"] == "False" and envs["model_env"] == "dev":
-        envs["platform"] = "local"
-
     return EnvVar(
         model_env=envs.get("model_env"),
         service_name=envs.get("service_name"),
-        local_deployment=envs.get("local_deployment", "False"),
         platform=envs.get("platform"),
         testing_only=envs.get("testing_only"),
     )
 
 
 ENV_VARS = read_env_vars()
 
@@ -428,15 +419,14 @@
     ]
 
     metadata = settings["info"]["prediction"]["metadata"]
     metadata_fields = metadata.keys()
 
     missing_fields = []
     for field in required_fields:
-
         if field == "petrel_exposure":
             try:
                 petrel_exposure = metadata[field]
                 if petrel_exposure:
                     for petrel_field in required_fields_petrel:
                         if petrel_field not in metadata_fields:
                             missing_fields.append(petrel_field)
```

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/deploy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 deploy.py
 
 Deploy services in either Google Cloud Run or CDF Functions.
 Model registry uses CDF Files.
 """
 import os
+import ast
 import traceback
 from pathlib import Path
 from typing import List
 
 import akerbp.mlops.model_manager as mm
 from akerbp.mlops import __version__ as package_version
 from akerbp.mlops.core import config
@@ -42,26 +43,25 @@
     """
     c = model_settings
     try:
         original_req_file = c.req_file
         envs = config.ENV_VARS
         env = envs.model_env
         testing_only = eval(envs.testing_only)
-        local_deployment = eval(envs.local_deployment)
         service_name = envs.service_name
         platform = envs.platform
         if service_name is None:
             raise ValueError(
                 "SERVICE_NAME environment variable must be set to either 'prediction' or 'training'"
             )
         deployment_folder = helpers.deployment_folder_path(c.model_name)
         function_name = f"{c.model_name}-{service_name}-{env}"
 
         # Handle mlops internal testing settings
-        mlops_testing = os.environ.get("LOCAL_MLOPS_TESTING", False)
+        mlops_testing = ast.literal_eval(os.environ.get("LOCAL_MLOPS_TESTING", "False"))  # type: ignore
 
         logger.info(
             f"Starting deployment and/or testing of model {c.human_friendly_model_name}"
         )
 
         if (service_name == "prediction") and c.artifact_folder:
             if platform == "cdf" or platform == "local":
@@ -85,53 +85,30 @@
             deployment_folder=deployment_folder if mlops_testing else None,
         )
         helpers.copy_to_deployment_folder(c.files, deployment_folder)
 
         logger.info(f"cd {deployment_folder}")
         os.chdir(deployment_folder)
 
-        # Local testing - for MODEL_ENV=dev and LOCAL_DEPLOYMENT=False
-        if envs.model_env == "dev" and envs.local_deployment == "False":
-            c.platform = "local"
-        if c.platform == "local":
-            if c.test_file:
-                logger.info("Performing local testing")
-                helpers.run_tests(
-                    c,
-                    setup_venv=True,
-                    deploy=False,
-                )
-            else:
-                logger.warning(
-                    "No test file specified in the settings, skipping local tests."
-                )
-
         # Deploy to CDF
-        elif c.platform == "cdf":
-            if (env == "test" or env == "prod") and testing_only:
-
+        if c.platform == "cdf":
+            if testing_only:
                 logger.info(
                     f"Running tests for model {c.human_friendly_model_name} in {env}, will not deploy"
                 )
                 helpers.run_tests(c, setup_venv=True, deploy=False)
-            elif (
-                (env == "test" or env == "prod") and not testing_only
-            ) or local_deployment:
+            else:
                 helpers.do_deploy(
                     c,
                     env,
                     service_name,
                     function_name,
                     deployment_folder,
                     setup_venv=True,
                 )
-            else:
-                logger.warning(
-                    f"Will not run tests nor deploy model(s), check your environment variables: {config.ENV_VARS}"
-                )
         return "OK"
     except (Exception, KeyboardInterrupt):
         # Remove deployment folder if it exists
         helpers.rm_deployment_folder(c.model_name)
         # Remove temporary requirements file if it exists
         if c.req_file != original_req_file:
             req_file = Path(c.req_file).resolve()
@@ -172,17 +149,20 @@
         for model, message in failed_models.items():
             logger.warning(f"Model {model} failed: {message}")
         raise Exception("At least one model failed.")
 
 
 def main() -> None:
     logger = get_logger(name="akerbp.mlops.deployment.deploy.py")
-    logger.info(
-        f"Deploying prediction service using MLOps framework version {package_version}"
-    )
+    if ast.literal_eval(os.environ.get("LOCAL_MLOPS_TESTING", "FALSE")):
+        message = "Deploying prediction service using the built wheel for testing purposes before releasing"
+    else:
+        message = f"Deploying prediction service using MLOps framework version {package_version}"
+
+    logger.info(message)
     mm.setup()
     settings = config.read_project_settings()
     deploy(settings)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -513,44 +513,49 @@
     # Log deployment folder content - at this point we are already inside the deployment folder
     deployment_folder_content = get_deployment_folder_content(
         deployment_folder=Path(".")
     )
     logger.info(
         f"Deployment folder '{deployment_folder}' now contains the following: {deployment_folder_content}"
     )
-
+    external_id = function_name
     platform = c.platform
     deploy_function, _, test_function = platform_methods[platform]
     logger.info(f"Starting deployment of model {c.model_name} to {env}")
+    # Get the latest artifact version uploaded to CDF Files and tag the model metadata with this version number
     if platform == "cdf":
         latest_artifact_version = cdf.get_latest_artifact_version(
-            external_id=function_name
+            external_id=external_id
         )
         if c.artifact_version is None:
             logger.info(
                 f"Latest artifact version in {env} is {latest_artifact_version}"
             )
             artifact_version = latest_artifact_version
         else:
             artifact_version = c.artifact_version
-
-        external_id = function_name + "-" + str(artifact_version)
     elif platform == "gc":
-        external_id = function_name  # Revisions are automatically created by GC
+        pass
     else:
         raise NotImplementedError(
             f"Functionality for deploying models to platform {platform} is not implemented!"
         )
 
     logger.info(
         f"Deploying function {c.human_friendly_model_name} with external id {external_id} to {platform}"
     )
+
+    # Tag model metadata with version number
+    model_info = c.info[service_name]
+    model_info["metadata"]["version"] = str(artifact_version)
     try:
         deploy_function(
-            c.human_friendly_model_name, external_id, info=c.info[service_name]
+            c.human_friendly_model_name,
+            external_id,
+            info=model_info,
         )
     except Exception as e:
         raise DeploymentError(f"Deployment failed with message: \n{str(e)}") from e
     if c.test_file:
         logger.info(f"Make a test call to function with external id {external_id}")
         try:
             test_function(external_id, test_payload)
@@ -559,86 +564,77 @@
                 f"Test of deployed model failed with message: \n{str(e)}"
             ) from e
     else:
         logger.warning(
             f"No test file was set up. End-to-end test skipped for function {external_id}"
         )
 
-    # Redeploy latest function with a predictable external id (model-service-env)
-    if artifact_version == latest_artifact_version and platform == "cdf":
+    if platform == "cdf" and env == "prod":
+        # Create a schedule for keeping the latest function warm in prod
         logger.info(
-            f"Redeploying latest model {c.human_friendly_model_name} with predictable external id {function_name} to {platform}"
+            f"Creating a schedule for keeping the function {external_id} warm on weekdays during extended working hours"
         )
-        redeploy_model_with_predictable_external_id(
+        cdf.setup_schedule_for_latest_model_in_prod(
+            external_id=function_name,
+        )
+        # Redeploy latest function with a predictable external id (model-service-env)
+        numbered_external_id = function_name + "-" + str(latest_artifact_version)
+        logger.info(
+            f"Redeploying numbered model {c.human_friendly_model_name} with external id {external_id} to {platform} in {env}"
+        )
+        redeploy_model_with_numbered_external_id(
             c,
             external_id=external_id,
-            predictable_external_id=function_name,
+            numbered_external_id=numbered_external_id,
             test_payload=test_payload,
         )
 
-        # Create a schedule for keeping the latest function warm in prod
-        if env == "prod":
-            logger.info(
-                f"Creating a schedule for keeping the function {function_name} warm on weekdays during extended working hours"
-            )
-            cdf.setup_schedule_for_latest_model_in_prod(
-                predictable_external_id=function_name,
-            )
-    else:
-        logger.info(
-            f"Deployment is based on an old artifact version ({artifact_version}/{latest_artifact_version})."
-        )
-        logger.info("Skipping redeployment with a predictable external id.")
-        if env == "prod" and platform == "cdf":
-            logger.info(
-                f"Will not setup a schedule for keeping this version in {env} warm"
-            )
     if platform == "cdf":
-        logger.info("Initiating garbage collection of old model versions")
+        logger.info("Initiating garbage collection of old, numbered model versions")
         cdf.garbage_collection(
             c,
             function_name,
             env,
             remove_artifacts=c.model_name == "mlopsdemo",
         )
 
 
-def redeploy_model_with_predictable_external_id(
+def redeploy_model_with_numbered_external_id(
     c: ServiceSettings,
     external_id: str,
-    predictable_external_id: str,
+    numbered_external_id: str,
     test_payload: Any,
     platform_methods: Dict = platform_methods,
 ) -> None:
     _, redeploy_function, test_function = platform_methods[c.platform]
     (
         name,
         file_id,
         description,
         metadata,
         owner,
-    ) = cdf.get_arguments_for_redeploying_latest_model_version(external_id=external_id)
+    ) = cdf.get_arguments_for_redeploying_numbered_models(external_id=external_id)
 
     try:
         redeploy_function(
             name,
-            predictable_external_id,
+            numbered_external_id,
             file_id,
             description,
             metadata,
             owner,
         )
     except Exception as e:
         raise DeploymentError(
-            f"Redeployment of latest model failed with message:  \n{str(e)}"
+            f"Redeployment of numbered model failed with message:  \n{str(e)}"
         ) from e
 
     if c.test_file:
         try:
-            test_function(predictable_external_id, test_payload)
+            test_function(numbered_external_id, test_payload)
         except Exception as e:
             raise TestError(
                 f"Testing the newly redeployed latest model failed with message: \n{str(e)}"
             ) from e
     else:
         logger.warning("No test file was specified in the settings, skipping tests")
```

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,17 @@
         folder: (Path) path to folder whose content will be uploaded
         metadata: dictionary with metadata (it should not contain a 'version' key)
 
     Returns:
         (dict): model metadata
     """
     specified_version = kwargs.get("version", None)
-    # TODO: when migrating to dev->test->prod release cycle, add check for test as well
-    if env == "prod":
+    if env == "prod" or env == "test":
         raise ValueError(
-            "You are not allowed to upload artifacts directly to prod, use promote_model instead to promote artifacts from test to prod"
+            f"You are not allowed to upload artifacts directly to {env}, use promote_model instead to promote artifacts dev to test and henceforth from test to prod"
         )
     if specified_version is None:
         file_list = cdf.query_file_versions(
             external_id_prefix=f"{model_name}/{env}/",
             directory_prefix="/mlops",
             uploaded=None,  # count any file
             dataset_id=dataset_id,
@@ -255,22 +254,16 @@
     Args:
         artifact_folder (Path):
         model_name: str
 
     Returns:
         (str): model id provided by the model manager or an existing folder in dev
     """
-    if artifact_folder.exists():
-        if env == "dev":
-            logger.info(f"Use model artifacts in {artifact_folder=}")
-            model_id = f"{model_name}/dev/1"
-            return model_id
-        else:
-            message = f"Existing, local artifacts won't be used ({env=}). Download uploaded artifacts from CDF Files"
-            logger.info(message)
+    message = f"Existing, local artifacts won't be used ({env=}). Download uploaded artifacts from CDF Files"
+    logger.info(message)
 
     logger.info("Downloading serialized model")
     model_id = download_model_version(model_name, env, artifact_folder)
     return model_id
 
 
 def get_model_version_overview(
@@ -423,70 +416,79 @@
                 env=environment,
                 folder=folder,
                 metadata=metadata,
                 version=version,
             )
 
 
-def promote_model(model_name: str, **kwargs) -> None:
+def promote_model(model_name: str, promote_to: str, **kwargs) -> None:
     """
     Promote a model version from test to prod
 
     Keyword Args:
         confirm (bool): Whether to confirm the promotion, defaults to True
         version (int): Version number. Defaults to None,
             where the latest version number is queried from CDF.
     Args:
         model_name (str): name of model
+        promote_to (str): environment to promote to, either 'test' or 'prod'
     """
     version = kwargs.get("version", None)
     confirm = kwargs.get("confirm", True)
+
+    if promote_to == "test":
+        promote_from = "dev"
+    elif promote_to == "prod":
+        promote_from = "test"
+    else:
+        raise ValueError("promote_to must be either 'test' or 'prod'")
+
     if version is None:
         logger.info(
-            "No version number specified, will query CDF for the latest version uploaded to test"
+            f"No version number specified, will query CDF for the latest version uploaded to {promote_from}"
         )
-        external_id_function = f"{model_name}-prediction-test"
+        external_id_function = f"{model_name}-prediction-{promote_from}"
         version = cdf.get_latest_artifact_version(external_id=external_id_function)
-        logger.info(f"Latest uploaded model version in test is {version}")
-    external_id = f"{model_name}/test/{version}"
+        logger.info(f"Latest uploaded model version in {promote_from} is {version}")
+    external_id = f"{model_name}/{promote_from}/{version}"
     if not cdf.file_exists(external_id, "/mlops", dataset_id):
         logger.warning(
-            f"Model version {external_id} doesn't exist in test, nothing to promote."
+            f"Model version {external_id} doesn't exist in {promote_from}, nothing to promote."
         )
         return
 
     confirmed = False
     if confirm:
-        question = f"Promote {model_name=}, environment=test, {version=} to production?"
+        question = f"Promote artifacts for {model_name} from {promote_from}, {version=},  to {promote_to}?"
         confirmed = confirm_prompt(question)
 
-    target_ext_id = f"{model_name}/prod/{version}"
+    target_ext_id = f"{model_name}/{promote_to}/{version}"
     if cdf.file_exists(
         external_id=target_ext_id, directory="/mlops", dataset_id=dataset_id
     ):
         logger.info(
-            f"Model version {target_ext_id} already exists in production, nothing new to promote."
+            f"Model version {target_ext_id} already exists in {promote_to}, nothing new to promote."
         )
         return
 
     if not confirm or confirmed:
         try:
             client = cdf.global_client["read"]
         except KeyError as e:
             raise MissingClientError(
-                "Set up model manager before promoting artifacts"
+                "Set up model manager by running 'mm.setup()' before promoting artifacts"
             ) from e
 
         old_filename = client.files.retrieve(external_id=external_id).name
         cdf.copy_file(
             external_id,
             target_ext_id,
             dataset_id=dataset_id,
             overwrite_name=True,
-            name=old_filename.replace("test", "prod"),
+            name=old_filename.replace(promote_from, promote_to),
         )
 
 
 def get_latest_model_in_env(model_name: str, env: str, deployed: bool = False) -> int:
     """Return the number of uploaded artifact versions for a given model in a given environment.
     If deployed is set to True, this function will try to return the version number of the latest deployed
     model in env. This requires that the deployed model has a metadata field 'version'. If not, and deployed is True,
```

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/prediction.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.2.0a0/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.1.2a5
+Version: 3.2.0a0
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -724,35 +724,31 @@
 ## Local Testing and Deployment
 It's possible to tests the functions locally, which can help you debug errors
 quickly. This is recommended before a deployment.
 
 Define the following environmental variables (e.g. in `.bashrc`):
 ```bash
 export MODEL_ENV=dev
-export COGNITE_API_KEY_PERSONAL=xxx
-export COGNITE_API_KEY_FUNCTIONS=$COGNITE_API_KEY_PERSONAL
-export COGNITE_API_KEY_DATA=$COGNITE_API_KEY_PERSONAL
-export COGNITE_API_KEY_FILES=$COGNITE_API_KEY_PERSONAL
+export COGNITE_OIDC_BASE_URL=https://api.cognitedata.com
+export COGNITE_TENANT_ID=<tenant id>
+export COGNITE_CLIENT_ID_WRITE=<write access client id>
+export COGNITE_CLIENT_SECRET_WRITE=<write access client secret>
+export COGNITE_CLIENT_ID_READ=<read access client id>
+export COGNITE_CLIENT_SECRET_READ=<read access client secret>
 ```
 
 From your repo's root folder:
 - `python -m pytest model_code` (replace `model_code` by your model code folder
   name)
 - `deploy_prediction_service`
 - `deploy_training_service` (if there's a training service)
 
 The first one will run your model tests. The last two run model tests but also
 the service tests implemented in the framework and simulate deployment.
 
-If you really want to deploy from your development environment, you can run
-this: `LOCAL_DEPLOYMENT=True deploy_prediction_service`
-
-Note that, in case of emergency, it's possible to deploy to test or production
-from your local environment, e.g. : `LOCAL_DEPLOYMENT=True MODEL_ENV=test deploy_prediction_service`
-
 If you want to run tests only you need to set `TESTING_ONLY=True` before calling the deployment script.
 
 ## Automated Deployments from Bitbucket
 Deployments to the test environment are triggered by commits (you need to push
 them). Deployments to the production environment are enabled manually from the
 Bitbucket pipeline dashboard. Branches that match 'deploy/*' behave as master.
 Branches that match `feature/*` run tests only (i.e. do not deploy).
@@ -765,15 +761,15 @@
 It is possible to schedule the training service in CDF, and then it can make
 sense to schedule the deployment pipeline of the model service (as often as new
 models are trained)
 
 NOTE: Previous version of akerbp.mlops assumes that calling
 `LOCAL_DEPLOYMENT=True deploy_prediction_service` will not deploy models and run tests.
 The package is now refactored to only trigger tests when the environment variable
-`TESTING_ONLY` is set to `True`, and allows to deploy locally when setting `LOCAL_DEPLOYMENT=True`.
+`TESTING_ONLY` is set to `True`.
 Make sure to update the pipeline definition for branches with prefix `feature/`to call
 `TESTING_ONLY=True deploy_prediction_service` instead.
 
 ## Bitbucket Setup
 The following environments need to be defined in `repository settings >
 deployments`:
 - test deployments: `test-prediction` and `test-training`, each with `MODEL_ENV=test`
@@ -842,17 +838,15 @@
 - Bash scripts will be installed in a `bin` folder in the `PATH`.
 
 The pipeline is setup to build the library from Bitbucket, but it's possible to
 build and upload the library from the development environment as well:
 ```bash
 bash build.sh
 ```
-In general this is required before `LOCAL_DEPLOYMENT=True deploy_xxx_service`. The exception is if local changes affect only the
-deployment part of the library, and the library has been installed in developer
-mode with:
+
 ```
 pip install -e .
 ```
 In this mode, the installed package links to the source code, so that it can be
 modified without the need to reinstall.
 
 ## Bitbucket Setup
```

### Comparing `akerbp.mlops-3.1.2a5/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.2.0a0/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_data_validation.py` & `akerbp.mlops-3.2.0a0/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_install_requirements.py` & `akerbp.mlops-3.2.0a0/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_metadata_validation.py` & `akerbp.mlops-3.2.0a0/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.2.0a0/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.1.2a5/test/test_version_increment.py` & `akerbp.mlops-3.2.0a0/test/test_version_increment.py`

 * *Files identical despite different names*

