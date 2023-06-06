# Comparing `tmp/dev-gpt-0.18.42.dev8.tar.gz` & `tmp/dev-gpt-0.18.42.dev87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.42.dev8.tar", last modified: Tue May 23 15:10:26 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.42.dev87.tar", last modified: Tue Jun  6 13:40:05 2023, max compression
```

## Comparing `dev-gpt-0.18.42.dev8.tar` & `dev-gpt-0.18.42.dev87.tar`

### file list

```diff
@@ -1,96 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.902459 dev-gpt-0.18.42.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-05-23 15:10:26.902459 dev-gpt-0.18.42.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.894459 dev-gpt-0.18.42.dev8/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 15:10:26.000000 dev-gpt-0.18.42.dev8/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.894459 dev-gpt-0.18.42.dev8/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.894459 dev-gpt-0.18.42.dev8/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.894459 dev-gpt-0.18.42.dev8/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.894459 dev-gpt-0.18.42.dev8/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/auto_refine_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/extract_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/get_user_input_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/conversation_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31796 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/pm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/pm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/pm/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/pm/task_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/prompt_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.894459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/app_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/google_custom_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/templates_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.894459 dev-gpt-0.18.42.dev8/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-05-23 15:10:26.000000 dev-gpt-0.18.42.dev8/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-23 15:10:26.000000 dev-gpt-0.18.42.dev8/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:10:26.000000 dev-gpt-0.18.42.dev8/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 15:10:26.000000 dev-gpt-0.18.42.dev8/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 15:10:26.000000 dev-gpt-0.18.42.dev8/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 15:10:26.000000 dev-gpt-0.18.42.dev8/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:10:26.902459 dev-gpt-0.18.42.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:26.898459 dev-gpt-0.18.42.dev8/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/unit/test_construct_sub_task_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/unit/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/unit/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-23 15:10:22.000000 dev-gpt-0.18.42.dev8/test/unit/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.838458 dev-gpt-0.18.42.dev87/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-06-06 13:40:05.838458 dev-gpt-0.18.42.dev87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20820 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.830458 dev-gpt-0.18.42.dev87/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 13:40:05.000000 dev-gpt-0.18.42.dev87/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/auto_refine_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/extract_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/fix_based_on_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/get_user_input_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/conversation_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32257 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/pm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/pm/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/pm/task_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/prompt_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.830458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/app_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/google_custom_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/templates_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.830458 dev-gpt-0.18.42.dev87/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-06-06 13:40:05.000000 dev-gpt-0.18.42.dev87/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-06 13:40:05.000000 dev-gpt-0.18.42.dev87/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:40:05.000000 dev-gpt-0.18.42.dev87/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 13:40:05.000000 dev-gpt-0.18.42.dev87/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-06 13:40:05.000000 dev-gpt-0.18.42.dev87/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 13:40:05.000000 dev-gpt-0.18.42.dev87/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:40:05.838458 dev-gpt-0.18.42.dev87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.834458 dev-gpt-0.18.42.dev87/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:40:05.838458 dev-gpt-0.18.42.dev87/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_construct_sub_task_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_error_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_self_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-06 13:39:58.000000 dev-gpt-0.18.42.dev87/test/unit/test_yes_no_question.py
```

### Comparing `dev-gpt-0.18.42.dev8/LICENSE` & `dev-gpt-0.18.42.dev87/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/PKG-INFO` & `dev-gpt-0.18.42.dev87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.42.dev8
+Version: 0.18.42.dev87
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
-Author: Florian Hönicke
-Author-email: florian.hoenicke@jina.ai
-License: UNKNOWN
+Author: Jina AI
+Author-email: hello@jina.ai
+License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
-Dev GPT: Your Automated Development Team
+Dev-GPT: Your Automated Development Team
 </h1>
 
 <p align="center" style="color: red; font-weight: bold;">
 ⚠️ This is an experimental version. ⚠️
 </p>
 
 <div align="center">
@@ -88,16 +88,16 @@
 ### Requirements
 - OpenAI key with access to gpt-3.5-turbo or gpt-4
 - if you want to enable your microservice to search for web content, 
 you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID environment variables.
 More information can be found [here](https://developers.google.com/custom-search/v1/overview).
 ```bash
 dev-gpt configure --openai_api_key <your openai api key>
-dev-gpt configure --google_api_key <google api key> (optional if you want to use google search)
-dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google search)
+dev-gpt configure --google_api_key <google api key> (optional if you want to use google custom search)
+dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google custom search)
 ```
 
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ## Docs
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.42.dev8 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.42.dev87 Summary: Use natural
 language interface to generate, deploy and update your microservice
-infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
-HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE
-            ****** Dev GPT: Your Automated Development Team ******
+infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Jina AI
+Author-email: hello@jina.ai License: Apache 2.0 Platform: UNKNOWN Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
+            ****** Dev-GPT: Your Automated Development Team ******
                 â ï¸ This is an experimental version. â ï¸
                     [Product Manager] [Developer] [DevOps]
                      Product Manager   Developer   DevOps
 Tell your AI team what microservice you want to build, and they will do it for
                       you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
             platforms] [Downloads] [https://img.shields.io/discord/
@@ -26,20 +25,20 @@
 project is covered, from concept to deployment. ## Quickstart ```bash pip
 install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
 to gpt-3.5-turbo or gpt-4 - if you want to enable your microservice to search
 for web content, you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID
 environment variables. More information can be found [here](https://
 developers.google.com/custom-search/v1/overview). ```bash dev-gpt configure --
 openai_api_key  dev-gpt configure --google_api_key  (optional if you want to
-use google search) dev-gpt configure --google_cse_id  (optional if you want to
-use google search) ``` If you set the environment variable `OPENAI_API_KEY`,
-the configuration step can be skipped. Your api key must have access to gpt-
-4 to use this tool. We are working on a way to use gpt-3.5-turbo as well. ##
-Docs ### Generate Microservice ```bash dev-gpt generate \ --description "" \ --
-model
+use google custom search) dev-gpt configure --google_cse_id  (optional if you
+want to use google custom search) ``` If you set the environment variable
+`OPENAI_API_KEY`, the configuration step can be skipped. Your api key must have
+access to gpt-4 to use this tool. We are working on a way to use gpt-3.5-turbo
+as well. ## Docs ### Generate Microservice ```bash dev-gpt generate \ --
+description "" \ --model
 5-turbo or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5-turbo` or `gpt-4`. `gpt-3.5-
 turbo` is ~10x cheaper, but will not be able to generate as complex
 microservices. (default: largest you have access to) - A `path` on the local
 drive where the microservice will be generated. (default: ./microservice) The
```

### Comparing `dev-gpt-0.18.42.dev8/README.md` & `dev-gpt-0.18.42.dev87/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-Dev GPT: Your Automated Development Team
+Dev-GPT: Your Automated Development Team
 </h1>
 
 <p align="center" style="color: red; font-weight: bold;">
 ⚠️ This is an experimental version. ⚠️
 </p>
 
 <div align="center">
@@ -68,16 +68,16 @@
 ### Requirements
 - OpenAI key with access to gpt-3.5-turbo or gpt-4
 - if you want to enable your microservice to search for web content, 
 you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID environment variables.
 More information can be found [here](https://developers.google.com/custom-search/v1/overview).
 ```bash
 dev-gpt configure --openai_api_key <your openai api key>
-dev-gpt configure --google_api_key <google api key> (optional if you want to use google search)
-dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google search)
+dev-gpt configure --google_api_key <google api key> (optional if you want to use google custom search)
+dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google custom search)
 ```
 
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ## Docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-            ****** Dev GPT: Your Automated Development Team ******
+            ****** Dev-GPT: Your Automated Development Team ******
                 â ï¸ This is an experimental version. â ï¸
                     [Product Manager] [Developer] [DevOps]
                      Product Manager   Developer   DevOps
 Tell your AI team what microservice you want to build, and they will do it for
                       you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
             platforms] [Downloads] [https://img.shields.io/discord/
@@ -15,20 +15,20 @@
 project is covered, from concept to deployment. ## Quickstart ```bash pip
 install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
 to gpt-3.5-turbo or gpt-4 - if you want to enable your microservice to search
 for web content, you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID
 environment variables. More information can be found [here](https://
 developers.google.com/custom-search/v1/overview). ```bash dev-gpt configure --
 openai_api_key  dev-gpt configure --google_api_key  (optional if you want to
-use google search) dev-gpt configure --google_cse_id  (optional if you want to
-use google search) ``` If you set the environment variable `OPENAI_API_KEY`,
-the configuration step can be skipped. Your api key must have access to gpt-
-4 to use this tool. We are working on a way to use gpt-3.5-turbo as well. ##
-Docs ### Generate Microservice ```bash dev-gpt generate \ --description "" \ --
-model
+use google custom search) dev-gpt configure --google_cse_id  (optional if you
+want to use google custom search) ``` If you set the environment variable
+`OPENAI_API_KEY`, the configuration step can be skipped. Your api key must have
+access to gpt-4 to use this tool. We are working on a way to use gpt-3.5-turbo
+as well. ## Docs ### Generate Microservice ```bash dev-gpt generate \ --
+description "" \ --model
 5-turbo or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5-turbo` or `gpt-4`. `gpt-3.5-
 turbo` is ~10x cheaper, but will not be able to generate as complex
 microservices. (default: largest you have access to) - A `path` on the local
 drive where the microservice will be generated. (default: ./microservice) The
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.42.dev87/dev_gpt/apis/gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from langchain.schema import HumanMessage, SystemMessage, BaseMessage, AIMessage
 from openai.error import RateLimitError, APIError
 from requests.exceptions import ConnectionError, ChunkedEncodingError
 from urllib3.exceptions import InvalidChunkLength
 
 from dev_gpt.constants import PRICING_GPT4_PROMPT, PRICING_GPT4_GENERATION, PRICING_GPT3_5_TURBO_PROMPT, \
     PRICING_GPT3_5_TURBO_GENERATION, CHARS_PER_TOKEN
-from dev_gpt.options.generate.conversation_logger import ConversationLogger
+from dev_gpt.options.generate.conversation_logger import ConversationLogger, Timer
+from dev_gpt.options.generate.parser import identity_parser
 from dev_gpt.options.generate.templates_system import template_system_message_base
 from dev_gpt.utils.string_tools import print_colored, get_template_parameters
 
 
 def configure_openai_api_key():
     if 'OPENAI_API_KEY' not in os.environ:
         print_colored('You need to set OPENAI_API_KEY in your environment.', '''
@@ -78,15 +79,15 @@
                         model="gpt-4",
                         messages=[{
                             "role": 'system',
                             "content": 'you respond nothing'
                         }]
                     )
                     break
-                except (RateLimitError, openai.error.APIError):
+                except (RateLimitError, openai.error.APIError, ConnectionError, InvalidChunkLength, ChunkedEncodingError, APIError, openai.error.Timeout):
                     sleep(1)
                     continue
             return True
         except openai.error.InvalidRequestError:
             return False
 
     def cost_callback(self, chars_prompt, chars_generation, print_costs: bool = True):
@@ -113,78 +114,80 @@
 
 class _GPTConversation:
     def __init__(self, model: str, cost_callback, messages: List[BaseMessage], print_stream, print_costs, conversation_logger: ConversationLogger = None):
         self._chat = ChatOpenAI(
             model_name=model,
             streaming=True,
             callback_manager=CallbackManager([AssistantStreamingStdOutCallbackHandler()] if print_stream else []),
+            request_timeout=10,
             verbose=True,
             temperature=0,
         )
         self.cost_callback = cost_callback
         self.messages = messages
         self.print_stream = print_stream
         self.print_costs = print_costs
         self.conversation_logger = conversation_logger
 
     def print_messages(self, messages):
+        t = Timer().get_time_since_start()
         for i, message in enumerate(messages):
             if os.environ['VERBOSE'].lower() == 'true':
                 if isinstance(message, SystemMessage):
-                    print_colored(f'({i}) system - prompt', message.content, 'magenta')
+                    print_colored(f'{t} - ({i}) system - prompt', message.content, 'magenta')
                 elif isinstance(message, HumanMessage):
-                    print_colored(f'({i}) user - prompt', message.content, 'blue')
+                    print_colored(f'{t} - ({i}) user - prompt', message.content, 'blue')
                 elif isinstance(message, AIMessage):
-                    print_colored(f'({i}) assistant - prompt', message.content, 'green')
+                    print_colored(f'{t} - ({i}) assistant - prompt', message.content, 'green')
 
     def chat(self, prompt: str, role: str = 'user'):
         MassageClass = HumanMessage if role == 'user' else SystemMessage
         chat_message = MassageClass(content=prompt)
         self.messages.append(chat_message)
         self.print_messages(self.messages)
         if self.print_stream:
-            print_colored('assistant', '', 'green', end='')
+            print_colored(f'{Timer().get_time_since_start()} - assistant', '', 'green', end='')
         print('thinking...')
         for i in range(10):
             try:
                 response = self._chat(self.messages)
                 self.conversation_logger.log(self.messages, response)
                 break
-            except (ConnectionError, InvalidChunkLength, ChunkedEncodingError, APIError) as e:
+            except (RateLimitError, openai.error.APIError, ConnectionError, InvalidChunkLength, ChunkedEncodingError, APIError, openai.error.Timeout) as e:
                 print('There was a connection error. Retrying...')
                 if i == 9:
                     raise e
                 sleep(10)
 
         if os.environ['VERBOSE'].lower() == 'true':
             print()
         self.cost_callback(sum([len(m.content) for m in self.messages]), len(response.content), self.print_costs)
         self.messages.append(response)
         return response.content
 
     @staticmethod
     def _create_system_message(task_description, test_description) -> SystemMessage:
         system_message = PromptTemplate.from_template(template_system_message_base).format(
-            task_description=task_description,
-            test_description=test_description,
+            # task_description=task_description,
+            # test_description=test_description,
         )
         return SystemMessage(content=system_message)
 
 
-def ask_gpt(prompt_template, parser, **kwargs):
+def ask_gpt(prompt_template: str, parser=identity_parser, **kwargs):
     template_parameters = get_template_parameters(prompt_template)
     if set(template_parameters) != set(kwargs.keys()):
         raise ValueError(
             f'Prompt template parameters {set(template_parameters)} do not match provided parameters {set(kwargs.keys())}'
         )
     for key, value in kwargs.items():
         if isinstance(value, dict):
             kwargs[key] = json.dumps(value, indent=4)
     prompt = prompt_template.format(**kwargs)
     conversation = GPTSession._instance.get_conversation(
-        [],
+        [SystemMessage(content='You are a helpful AI assistant that follows instructions from the user exactly.')],
         print_stream=os.environ['VERBOSE'].lower() == 'true',
         print_costs=False
     )
     agent_response_raw = conversation.chat(prompt, role='user')
     agent_response = parser(agent_response_raw)
     return agent_response
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.42.dev87/dev_gpt/apis/jina_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import requests
 from hubble.executor.helper import upload_file, archive_package, get_full_version
 from jcloud.flow import CloudFlow
 from jina import Flow
 
 from dev_gpt.constants import DEMO_TOKEN
 from dev_gpt.utils.io import suppress_stdout, is_docker_running
-from dev_gpt.utils.string_tools import print_colored
+from dev_gpt.utils.string_tools import print_colored, clean_large_words
 
 
 def wait_until_app_is_ready(url):
     is_app_ready = False
     while not is_app_ready:
         try:
             response = requests.get(url)
@@ -97,21 +97,21 @@
     form_data = {
         'public': 'True',
         'private': 'False',
         'verbose': 'True',
         'buildEnv': f'{{"OPENAI_API_KEY": "{os.environ["OPENAI_API_KEY"]}", "GOOGLE_API_KEY": "{os.environ.get("GOOGLE_API_KEY","")}", "GOOGLE_CSE_ID": "{os.environ.get("GOOGLE_CSE_ID","")}"}}',
         'md5sum': md5_digest,
     }
-    with suppress_stdout():
-        headers = get_request_header()
-        headers['jinameta-platform'] = 'Darwin'
-        headers['jinameta-platform-release'] = '21.1.0'
-        headers['jinameta-platform-version'] = 'Darwin Kernel Version 21.1.0: Wed Oct 13 17:33:23 PDT 2021; root:xnu-8019.41.5~1/RELEASE_X86_64'
-        headers['jinameta-architecture'] = 'x86_64'
-        headers['jinameta-processor'] = 'i386'
+    # with suppress_stdout():
+    headers = get_request_header()
+    headers['jinameta-platform'] = 'Darwin'
+    headers['jinameta-platform-release'] = '21.1.0'
+    headers['jinameta-platform-version'] = 'Darwin Kernel Version 21.1.0: Wed Oct 13 17:33:23 PDT 2021; root:xnu-8019.41.5~1/RELEASE_X86_64'
+    headers['jinameta-architecture'] = 'x86_64'
+    headers['jinameta-processor'] = 'i386'
 
     resp = upload_file(
         'https://api.hubble.jina.ai/v2/rpc/executor.push',
         'filename',
         content,
         dict_data=form_data,
         headers=headers,
@@ -305,14 +305,15 @@
     return relevant_lines
 
 
 def clean_color_codes(response):
     response = re.sub(r'\x1b\[[0-9;]*m', '', response)
     return response
 
+
 def process_error_message(error_message):
     lines = error_message.split('\n')
 
     relevant_lines = []
 
     pattern = re.compile(r"^#\d+ \[[ \d]+/[ \d]+\]")  # Pattern to match lines like "#11 [7/8]"
     last_matching_line_index = None
@@ -326,15 +327,17 @@
 
     relevant_lines = shorten_logs(relevant_lines)
 
     response = '\n'.join(relevant_lines[-100:]).strip()
 
     response = clean_color_codes(response)
 
+    # the following code makes sure that the error message is cleaned from irrelevant sequences of e.g. base64 strings.
+    response = clean_large_words(response)
+
     # the following code tests the case that the docker file is corrupted and can not be parsed
     # the method above will not return a relevant error message in this case
     # but the last line of the error message will start with "error"
-
     last_line = lines[-1]
     if not response and last_line.startswith('error: '):
         return last_line
     return response
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.42.dev87/dev_gpt/apis/pypi.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,33 +31,44 @@
     for v, release_info in releases.items():
         if not release_info:
             continue
         upload_time = datetime.strptime(release_info[0]['upload_time'], '%Y-%m-%dT%H:%M:%S')
         if upload_time.year <= 2020 or (upload_time.year == 2021 and upload_time.month <= 9):  # knowledge cutoff 2021-09 (including september)
             valid_versions.append(v)
 
-    v = max(valid_versions, key=version.parse) if valid_versions else None
+    v = max(valid_versions, key=parse_version) if valid_versions else None
     return v
 
+def parse_version(version_string):
+    """
+    Parses a version string and returns a tuple of integers.
+    """
+    try:
+        return version.parse(version_string)
+    except version.InvalidVersion:
+        return version.parse("0.0.0")
 
 def clean_requirements_txt(previous_microservice_path):
     """
     It can happen that the generated requirements.txt contains packages that are not on PyPI (like base64).
     In this case, we remove the requirement from requirements.txt.
     In case the package is on PyPI, but the version is not, we update the version to the latest version that is still not older than 2021.
     """
     requirements_txt_path = os.path.join(previous_microservice_path, 'requirements.txt')
     with open(requirements_txt_path, 'r', encoding='utf-8') as f:
         requirements_txt = f.read()
 
     updated_requirements = []
 
     for line in requirements_txt.split('\n'):
+        # replace comment at the end of the line
+        pattern = r'#.+'
+        line = re.sub(pattern, '', line)
         line = line.strip()
-        if not line or line.startswith('#'):
+        if not line:
             continue
 
         split = re.split(r'==|>=|<=|>|<|~=', line)
         if len(split) == 1 or len(split) > 2:
             version = None
             package_name = split[0]
         else:
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/cli.py` & `dev-gpt-0.18.42.dev87/dev_gpt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 
 import click
 
 from dev_gpt.apis.gpt import configure_openai_api_key
 from dev_gpt.apis.jina_cloud import jina_auth_login
 from dev_gpt.options.configure.key_handling import set_api_key
+from dev_gpt.options.generate.conversation_logger import Timer
+
 
 def openai_api_key_needed(func):
     def wrapper(*args, **kwargs):
         configure_openai_api_key()
         return func(*args, **kwargs)
     return wrapper
 
@@ -40,14 +42,15 @@
     return wrapper
 
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 @exception_interceptor
 def main(ctx):
+    Timer() # start timer
     if ctx.invoked_subcommand is None:
         click.echo(ctx.get_help())
 
 
 @openai_api_key_needed
 @main.command()
 @click.option('--description', required=False, help='Description of the microservice.')
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/constants.py` & `dev-gpt-0.18.42.dev87/dev_gpt/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DOCKER_BASE_IMAGE_VERSION = '0.0.6'
+DOCKER_BASE_IMAGE_VERSION = '0.0.8'
 
 EXECUTOR_FILE_NAME = '__init__.py'
 IMPLEMENTATION_FILE_NAME = 'microservice.py'
 TEST_EXECUTOR_FILE_NAME = 'test_microservice.py'
 REQUIREMENTS_FILE_NAME = 'requirements.txt'
 DOCKER_FILE_NAME = 'Dockerfile'
 CLIENT_FILE_NAME = 'client.py'
@@ -46,24 +46,33 @@
 MAX_DEBUGGING_ITERATIONS = 10
 
 DEMO_TOKEN = '45372338e04f5a41af949024db929d46'
 
 BLACKLISTED_PACKAGES = [
     'moderngl', 'pyopengl', 'pyglet', 'pythreejs', 'panda3d',  # because they need a screen,
     'tika',  # because it needs java
-    'clearbit'  # because of installation issues on latest version
+    'clearbit',  # because of installation issues on latest version
+    'pyttsx3',  # after engine.save_to_file(summarized_text, "summarized_audio.wav"); engine.runAndWait() "summarized_audio.wav" does not exist
 ]
+
 UNNECESSARY_PACKAGES = [
-    'fastapi', 'uvicorn', 'starlette'  # because the wrappers are used instead
+    'jinja2', 'werkzeug', 'flask', 'flask_restful', 'http.server', 'flask_json', 'flask_cors', 'fastapi', 'uvicorn', 'starlette',  # because the wrappers are used instead
+    'pypng', # if we provide access to the documentation all should be fine but for now it is too hard to use since the import is png
+
 ]
 
 LANGUAGE_PACKAGES = [
-    'allennlp', 'bertopic', 'GPT-3', 'fasttext', 'flair', 'gensim', 'nltk', 'openai',
+    'allennlp', 'bert-for-tf2', 'bertopic', 'gpt-3', 'fasttext', 'flair', 'gensim', 'nltk', 'openai',
     'pattern', 'polyglot', 'pytorch-transformers', 'rasa', 'sentence-transformers',
     'spacy', 'stanza', 'summarizer', 'sumy', 'textblob', 'textstat', 'transformers',
-    'vadersentiment'
+    'vadersentiment', 'language-tool-python'
 ]
 
 SEARCH_PACKAGES = [
     'googlesearch-python', 'google', 'googlesearch', 'google-api-python-client', 'pygooglenews', 'google-cloud'
 ]
 
+TOOL_TO_ALIASES = {
+    'gpt_3_5_turbo': ['gpt-3', 'GPT-3'],
+    'google_custom_search': ['Google Custom Search API']
+}
+
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/__init__.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/auto_refine_description.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/auto_refine_description.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,84 @@
 import json
 
 from dev_gpt.apis.gpt import ask_gpt
-from dev_gpt.options.generate.parser import identity_parser
+from dev_gpt.constants import TOOL_TO_ALIASES
+from dev_gpt.options.generate.parser import identity_parser, optional_tripple_back_tick_parser
 from dev_gpt.options.generate.prompt_factory import context_to_string
 from dev_gpt.options.generate.tools.tools import get_available_tools
 
 
-def auto_refine_description(context):
-    context['microservice_description'] = ask_gpt(
+def enhance_description(context):
+    enhanced_description = ask_gpt(
         better_description_prompt,
         identity_parser,
         context_string=context_to_string(context)
     )
+    for tool_name, aliases in TOOL_TO_ALIASES.items():
+        for alias in aliases:
+            enhanced_description = enhanced_description.replace(alias, tool_name)
+    return enhanced_description
+
+
+def auto_refine_description(context):
+    context['microservice_description'] = enhance_description(context)
     context['request_schema'] = ask_gpt(
         generate_request_schema_prompt,
-        identity_parser,
+        optional_tripple_back_tick_parser,
         context_string=context_to_string(context)
     )
     context['response_schema'] = ask_gpt(
         generate_output_schema_prompt,
-        identity_parser,
+        optional_tripple_back_tick_parser,
         context_string=context_to_string(context)
     )
     context['microservice_description'] = ask_gpt(
         summarize_description_and_schemas_prompt,
         identity_parser,
         context_string=context_to_string(context)
     )
     # details = extract_information(context['microservice_description'], ['database connection details', 'URL', 'secret'])
     # if details:
     #     context['microservice_description'] += '\n\nAdditional information:' + json.dumps(details, indent=4)
     # del context['details']
 
 
 better_description_prompt = f'''{{context_string}}
-Update the description of the Microservice to make it more precise without adding or removing information.
-Note: the output must be a list of tasks the Microservice has to perform.
-Note: you can uses two tools if necessary:
+Based on this description, update the tasks for the Microservice to be more precise. This update should neither add nor remove information.
+
+Constraints:
+
+- The output must be a list of tasks that the Microservice has to perform.
+- The updated description must be unambiguous, using precise language and direct instructions.
+- Use of non-specific formulations, such as 'like', 'such as', is strictly not allowed.
+- The tools that can be used in the updated description:
 {get_available_tools()}
-Example for the description: "return a description of the average temperature of the 5 days weather forecast for a given location."
-1. get the 5 days weather forcast from the https://openweathermap.org/ API
-2. extract the temperature from the response
-3. calculate the average temperature'''
+- Note: You are not required to use all tools for every task. Use them only when necessary.
+Example for the description: "return an image representing the current weather for a given location." \
+when the tools gpt_3_5_turbo and google_custom_search are available:
+1. get the current weather information from the https://openweathermap.org/ API
+2. generate a Google search query to find the image matching the weather information and the location by using gpt_3_5_turbo (a)
+3. find the image by using the google_custom_search (b)
+4. return the image as a base64 encoded string'''
 
 generate_request_schema_prompt = '''{context_string}
 Generate the lean request json schema of the Microservice.
-Note: If you are not sure about the details, then come up with the minimal number of parameters possible.'''
+Note: If you are not sure about the details, then come up with the minimal number of parameters possible (could be even no parameters).
+Note: If you can decide to receive files as URLs or as base64 encoded strings, then choose the base64 encoded strings.'''
 
 generate_output_schema_prompt = '''{context_string}
 Generate the lean response json schema for the Microservice.
 Note: If you are not sure about the details, then come up with the minimal number of parameters possible.
 Note: If you can decide to return files as URLs or as base64 encoded strings, then choose the base64 encoded strings.'''
 
 summarize_description_and_schemas_prompt = '''{context_string}
-Write an updated microservice description by incorporating information about the request and response parameters in a concise way without losing any information.
-Note: You must not mention any details about algorithms or the technical implementation.
-Note: You must not mention that there is a request and response JSON schema
-Note: You must not use any formatting like triple backticks.
-Note: If an external API is mentioned in the description, then you must mention the API in the updated description as well.'''
+Please write an updated microservice description by incorporating information about the request and response parameters in a concise manner, ensuring all information from the existing description is maintained.
+
+Constraints:
+
+- Do not mention any details about algorithms or the technical implementation.
+- Refrain from indicating there is a request and response JSON schema.
+- Avoid using any special formatting such as triple backticks.
+- If a specific tool or API (e.g. google_custom_search, gpt_3_5_turbo) is referred to in the original description, \
+include it in the updated description using the exact name given. \
+For instance, if the original description mentions 'gpt_3_5_turbo', \
+the updated description should also specify 'gpt_3_5_turbo'.'''
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/extract_information.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/extract_information.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/get_user_input_if_needed.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/get_user_input_if_needed.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/question_answering.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/question_answering.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,36 +11,38 @@
 
 def is_question_false(question):
     return lambda context: not is_question_true(question)(context)
 
 
 def answer_yes_no_question(text, question):
     pros_and_cons = ask_gpt(
-        pros_and_cons_prompt.format(
-            question=question,
-            text=text,
-        ),
-        identity_parser,
+        pros_and_cons_prompt,
+        question=question,
+        text=text,
     )
 
     return ask_gpt(
-        question_prompt.format(
-            text=text,
-            question=question,
-            pros_and_cons=pros_and_cons,
-        ),
-        boolean_parser)
+        question_prompt,
+        boolean_parser,
+        text=text,
+        question=question,
+        pros_and_cons=pros_and_cons,
+    )
 
 pros_and_cons_prompt = '''\
 # Context
 {text}
 # Question
 {question}
-Note: You must not answer the question. Instead, give up to 5 bullet points (10 words) arguing why the question should be answered with true or false.'''
+Note: You must not answer the question. Instead, give between 1 and 5 bullet points (5 words each) arguing why the question should be answered with yes or no.'''
 
 question_prompt = '''\
 # Context
 {text}
+
+# Pros and Cons
+{pros_and_cons}
+
 # Question
-{question}
-Note: You must answer "yes" or "no".
+Based on the pros and cons, answer the following question: {question}
+Note: You must answer the question correctly by saying something like "since <explanagion>, the answer is yes" or "since <explanagion>, the answer is no".
 '''
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/translation.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/translation.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from dev_gpt.apis.gpt import ask_gpt
 from dev_gpt.options.generate.parser import identity_parser
 
 
-def user_feedback_loop(context, current_description):
+def user_feedback_loop(current_description):
     while (user_feedback := get_user_feedback(current_description)):
-        context['user_feedback'] = user_feedback
         current_description = ask_gpt(
             add_feedback_prompt,
             identity_parser,
-            **context
+            microservice_description=current_description,
+            user_feedback=user_feedback,
         )
-        del context['user_feedback']
     return current_description
 
 def get_user_feedback(microservice_description):
     while True:
         user_feedback = input(
             f'I suggest that we implement the following microservice:\n{microservice_description}\nDo you agree? [y/n]')
         if user_feedback.lower() in ['y', 'yes', 'yeah', 'yep', 'yup', 'sure', 'ok', 'okay']:
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from typing import List, Text, Optional
 
 from langchain import PromptTemplate
 from langchain.schema import SystemMessage, AIMessage
 from pydantic.dataclasses import dataclass
 
 from dev_gpt.apis import gpt
-from dev_gpt.apis.gpt import _GPTConversation
+from dev_gpt.apis.gpt import _GPTConversation, ask_gpt
 from dev_gpt.apis.jina_cloud import process_error_message, push_executor, is_executor_in_hub
 from dev_gpt.apis.pypi import is_package_on_pypi, clean_requirements_txt
 from dev_gpt.constants import FILE_AND_TAG_PAIRS, NUM_IMPLEMENTATION_STRATEGIES, MAX_DEBUGGING_ITERATIONS, \
     BLACKLISTED_PACKAGES, EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_TAG, \
     REQUIREMENTS_FILE_NAME, REQUIREMENTS_FILE_TAG, DOCKER_FILE_NAME, IMPLEMENTATION_FILE_NAME, \
     IMPLEMENTATION_FILE_TAG, LANGUAGE_PACKAGES, UNNECESSARY_PACKAGES, DOCKER_BASE_IMAGE_VERSION, SEARCH_PACKAGES, \
     INDICATOR_TO_IMPORT_STATEMENT
+from dev_gpt.options.generate.conversation_logger import Timer
+from dev_gpt.options.generate.parser import json_parser, self_healing_json_parser
 from dev_gpt.options.generate.pm.pm import PM
 from dev_gpt.options.generate.templates_user import template_generate_microservice_name, \
     template_generate_possible_packages, \
     template_implement_solution_code_issue, \
     template_solve_pip_dependency_issue, template_is_dependency_issue, template_generate_playground, \
     template_generate_function_constructor, template_generate_test, template_generate_requirements, \
     template_chain_of_thought, template_summarize_error, \
@@ -280,14 +282,20 @@
         json_string = self.extract_content_from_result(content_raw, 'apt-get-packages.json', match_single_block=True)
         packages = ' '.join(json.loads(json_string)['packages'])
 
         docker_file_template = self.read_docker_template()
         return {DOCKER_FILE_NAME: docker_file_template.replace('{{APT_GET_PACKAGES}}', '{APT_GET_PACKAGES}').replace('{{DOCKER_BASE_IMAGE_VERSION}}', DOCKER_BASE_IMAGE_VERSION).format(
             APT_GET_PACKAGES=packages)}
 
+    def get_parse_result_fn_dockerfile_json_parser(self, file_name):
+        def parse_result_fn_self_healing_json_parser(content_raw: str):
+            json_string = self_healing_json_parser(content_raw)
+            return {file_name: json_string}
+        return parse_result_fn_self_healing_json_parser
+
     def parse_result_fn_requirements(self, content_raw: str):
         content_parsed = self.extract_content_from_result(content_raw, 'requirements.txt', match_single_block=True)
 
         lines = content_parsed.split('\n')
         lines = [line for line in lines if
                  not any([pkg in line for pkg in ['jina', 'docarray', 'openai', 'pytest', 'gpt_3_5_turbo']])]
         content_modified = f'''jina==3.15.1.dev14
@@ -351,18 +359,22 @@
         if not is_executor_in_hub(gateway_name):
             raise Exception(f'{self.microservice_name} not in hub. Hubble logs: {hubble_log}')
 
     def debug_microservice(self, num_approach, packages, self_healing):
         for i in range(1, MAX_DEBUGGING_ITERATIONS):
             print('Debugging iteration', i)
             print('Trying to debug the microservice. Might take a while...')
+            print(f'{Timer().get_time_since_start()} - Clean requirements.txt...')
             clean_requirements_txt(self.cur_microservice_path)
+            print(f'{Timer().get_time_since_start()} - Build executor...')
             log_hubble = push_executor(self.cur_microservice_path)
+            print(f'{Timer().get_time_since_start()} - Analyze logs...')
             error = process_error_message(log_hubble)
             if error:
+                print('Handling error...')
                 if not self_healing:
                     print(error)
                     raise Exception('Self-healing is disabled. Please fix the error manually.')
                 print('An error occurred during the build process. Feeding the error back to the assistant...')
                 self.previous_microservice_path = self.cur_microservice_path
                 self.cur_microservice_path = get_microservice_path(
                     self.microservice_root_path, self.microservice_name, packages, num_approach, i + 1
@@ -430,25 +442,21 @@
                     suggested_solution=suggested_solution,
                 )
 
                 self.previous_errors.append(summarized_error)
                 self.previous_solutions.append(suggested_solution)
 
     def generate_solution_suggestion(self, summarized_error, all_files_string):
-        suggested_solutions = json.loads(
-            self.generate_and_persist_file(
-                section_title='Suggest solution for code issue',
-                template=template_suggest_solutions_code_issue,
-                file_name_s=['solutions.json'],
-                summarized_error=summarized_error,
-                task_description=self.microservice_specification.task,
-                test_description=self.microservice_specification.test,
-                all_files_string=all_files_string,
-                response_format_example=response_format_suggest_solutions,
-            )['solutions.json']
+        suggested_solutions = ask_gpt(
+            template_suggest_solutions_code_issue,
+            self_healing_json_parser,
+            task_description=self.microservice_specification.task,
+            test_description=self.microservice_specification.test,
+            all_files_string=all_files_string,
+            summarized_error=summarized_error,
         )
 
         if len(self.previous_errors) > 0:
             was_error_seen_before = json.loads(
                 self.generate_and_persist_file(
                     section_title='Check if error was seen before',
                     template=template_was_error_seen_before,
@@ -508,42 +516,34 @@
                                                                                           package_manager)
         )
         answer_json_string = self.extract_content_from_result(answer_raw, 'response.json', match_single_block=True, )
         answer = json.loads(answer_json_string)['dependency_installation_failure']
         return 'yes' in answer.lower()
 
     def generate_microservice_name(self, description):
-        name = self.generate_and_persist_file(
-            section_title='Generate microservice name',
-            template=template_generate_microservice_name,
-            destination_folder=self.microservice_root_path,
-            file_name_s=['name.txt'],
-            description=description
-        )['name.txt']
-        return name
+        return ask_gpt(template_generate_microservice_name, description=description)
 
     def get_possible_packages(self):
         print_colored('', '\n\n############# What packages to use? #############', 'blue')
-        packages_json_string = self.generate_and_persist_file(
-            section_title='Generate possible packages',
-            template=template_generate_possible_packages,
-            destination_folder=self.microservice_root_path,
-            file_name_s=['strategies.json'],
-            description=self.microservice_specification.task
-        )['strategies.json']
-        packages_list = [[pkg.strip().lower() for pkg in packages] for packages in json.loads(packages_json_string)]
-        packages_list = [[self.replace_with_tool_if_possible(pkg) for pkg in packages] for packages in
+        packages_json = ask_gpt(template_generate_possible_packages, self_healing_json_parser, description=self.microservice_specification.task)
+        packages_list = self.process_packages_json_string(packages_json, self.microservice_specification.task)
+        return packages_list
+
+    @staticmethod
+    def process_packages_json_string(packages_json, task_description):
+        packages_list = [[pkg.strip().lower().replace('-', '_') for pkg in packages] for packages in packages_json]
+        packages_list = [[Generator.replace_with_tool_if_possible(pkg) for pkg in packages] for packages in
                          packages_list]
 
-        packages_list = self.filter_packages_list(packages_list)
-        packages_list = self.remove_duplicates_from_packages_list(packages_list)
+        packages_list = Generator.filter_packages_list(packages_list)
+        packages_list = Generator.remove_duplicates_from_packages_list(packages_list)
+        packages_list = Generator.add_tools_if_missing(packages_list, task_description)
         packages_list = packages_list[:NUM_IMPLEMENTATION_STRATEGIES]
         return packages_list
-    # '/private/var/folders/f5/whmffl4d7q79s29jpyb6719m0000gn/T/pytest-of-florianhonicke/pytest-128/test_generation_level_0_mock_i0'
-    # '/private/var/folders/f5/whmffl4d7q79s29jpyb6719m0000gn/T/pytest-of-florianhonicke/pytest-129/test_generation_level_0_mock_i0'
+
     def generate(self):
         os.makedirs(self.microservice_root_path)
         self.microservice_specification.task, self.microservice_specification.test = PM().refine_specification(self.microservice_specification.task)
         generated_name = self.generate_microservice_name(self.microservice_specification.task)
         self.microservice_name = f'{generated_name}{random.randint(0, 10_000_000)}'
         packages_list = self.get_possible_packages()
         for num_approach, packages in enumerate(packages_list):
@@ -595,23 +595,32 @@
         packages_list = [
             [
                 package for package in packages
                 if (package not in UNNECESSARY_PACKAGES)
                    and (  # all packages must be on pypi or it is gpt_3_5_turbo
                            is_package_on_pypi(package)
                            or package == 'gpt_3_5_turbo'
+                           or package == 'google_custom_search'
                    )
             ] for packages in packages_list
         ]
         return packages_list
 
     @staticmethod
     def remove_duplicates_from_packages_list(packages_list):
         return [list(set(packages)) for packages in packages_list]
 
+    @classmethod
+    def add_tools_if_missing(cls, packages_list, task_description):
+        for packages in packages_list:
+            for tool in ['gpt_3_5_turbo', 'google_custom_search']:
+                if tool not in packages and tool in task_description:
+                    packages.append(tool)
+        return packages_list
+
 #     def create_prototype_implementation(self):
 #         microservice_py_lines = ['''\
 # Class {microservice_name}:''']
 #         for sub_task in self.pm.iterate_over_sub_tasks_pydantic(self.sub_task_tree):
 #             microservice_py_lines.append(f'    {sub_task.python_fn_signature}')
 #             microservice_py_lines.append(f'        """')
 #             microservice_py_lines.append(f'        {sub_task.python_fn_docstring}')
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/pm/pm.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/pm/pm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from dev_gpt.apis import gpt
 from dev_gpt.apis.gpt import ask_gpt
 from dev_gpt.options.generate.chains.auto_refine_description import auto_refine_description
+from dev_gpt.options.generate.chains.get_user_input_if_needed import get_user_input_if_needed
 from dev_gpt.options.generate.chains.question_answering import is_question_true
 from dev_gpt.options.generate.chains.translation import translation
 from dev_gpt.options.generate.chains.user_confirmation_feedback_loop import user_feedback_loop
-from dev_gpt.options.generate.chains.get_user_input_if_needed import get_user_input_if_needed
-from dev_gpt.options.generate.parser import identity_parser, json_parser
+from dev_gpt.options.generate.parser import identity_parser, json_parser, self_healing_json_parser
 from dev_gpt.options.generate.pm.task_tree_schema import TaskTree
 from dev_gpt.options.generate.prompt_factory import make_prompt_friendly
+from dev_gpt.options.generate.templates_user import generate_used_apis_prompt
 from dev_gpt.options.generate.ui import get_random_employee
 
 
 class PM:
     def refine_specification(self, microservice_description):
         pm = get_random_employee('pm')
         print(f'{pm.emoji}👋 Hi, I\'m {pm.name}, a PM at Jina AI. Gathering the requirements for our engineers.')
@@ -39,58 +40,71 @@
         # sub_task_tree = construct_sub_task_tree(microservice_description)
         # return sub_task_tree
         return microservice_description, test_description
 
     def refine_description(self, microservice_description):
         context = {'microservice_description': microservice_description}
         auto_refine_description(context)
-        microservice_description = user_feedback_loop(context, context['microservice_description'])
+        microservice_description = user_feedback_loop(context['microservice_description'])
 
         test_description = ask_gpt(
             generate_test_assertion_prompt,
             identity_parser,
             **context
         )
 
         test_description += self.user_input_extension_if_needed(
-            context,
-            microservice_description,
-            condition_question='Does the request schema provided include a property that represents a file?',
+            {
+                'Microservice description': microservice_description,
+                'Request schema': context['request_schema'],
+                'Response schema': context['response_schema'],
+            },
+            conditions = [
+                is_question_true('Does the request schema provided include a property that represents a file?'),
+            ],
             question_gen='Generate a question that requests for an example file url.',
             extension_name='Input Example',
         )
-        microservice_description += self.user_input_extension_if_needed(
-            context,
-            microservice_description,
-            condition_question='''\
-Does the microservice send requests to an API beside the Google Custom Search API and gpt-3.5-turbo?''',
-            question_gen='Generate a question that asks for the endpoint of the external API and an example of a request and response when interacting with the external API.',
-            extension_name='Example of API usage',
-            post_transformation_fn=translation(from_format='api instruction', to_format='python code snippet raw without formatting')
-        )
+        used_apis_beside_tools = [
+            x for x in self.get_used_apis(microservice_description) if not any(t in x.lower() for t in ['gpt', 'search', 'google'])
+        ]
+        for api in used_apis_beside_tools:
+            microservice_description += self.user_input_extension_if_needed(
+                {
+                    'Microservice description': microservice_description,
+                },
+                conditions=[
+                    lambda _:True
+                ],
+                question_gen=f'Generate a question that asks for the endpoint for {api} and an example of a request and response when interacting with the API.',
+                extension_name=f'Instructions for {api}',
+                post_transformation_fn=translation(from_format='api instruction',
+                                                   to_format='python code snippet raw without formatting')
+            )
         return microservice_description, test_description
 
+    @staticmethod
+    def get_used_apis(microservice_description):
+        return ask_gpt(
+            generate_used_apis_prompt,
+            self_healing_json_parser,
+            microservice_description=microservice_description
+        )['mentioned_apis']
+
     def user_input_extension_if_needed(
             self,
             context,
-            microservice_description,
-            condition_question,
+            conditions,
             question_gen,
             extension_name,
             post_transformation_fn=None
     ):
         user_answer = get_user_input_if_needed(
-            context={
-                'Microservice description': microservice_description,
-                'Request schema': context['request_schema'],
-                'Response schema': context['response_schema'],
-            },
-            conditions=[
-                is_question_true(condition_question),
-            ],
+            context=context,
+            conditions=conditions,
             question_gen_prompt_part=question_gen,
         )
         if user_answer:
             if post_transformation_fn:
                 user_answer = make_prompt_friendly(user_answer)
                 user_answer = post_transformation_fn(user_answer)
             return f'\n{extension_name}: {user_answer}'
@@ -100,16 +114,14 @@
 
 client_description = '''\
 Microservice description:
 ```
 {microservice_description}
 ```'''
 
-
-
 generate_test_assertion_prompt = client_description + '''
 Request json schema:
 ```
 {request_schema}
 ```
 Response json schema:
 ```
@@ -118,14 +130,15 @@
 Generate the description of the weak test assertion for the microservice. The weak assertion only checks if the output of func is of the correct type (e.g. str, int, bool, etc.). Nothing else.
 Note: you must only output the test description - nothing else.
 Note: you must not use any formatting like triple backticks.
 Note: the generated description must be less than 30 words long.
 Example:
 "Input for func is a base64 encoded image. The test asserts that the output of func is of type 'str'".'''
 
+
 # def get_nlp_fns(self, microservice_description):
 #     return ask_gpt(
 #         get_nlp_fns_prompt,
 #         json_parser,
 #         microservice_description=microservice_description
 #     )
 #
@@ -153,25 +166,26 @@
         sub_task_tree_solutions_prompt, identity_parser,
         # nlp_fns=nlp_fns,
         microservice_description=microservice_description, sub_task_tree=sub_task_tree_dict,
         reflections=reflections,
     )
     sub_task_tree_updated = ask_gpt(
         sub_task_tree_update_prompt,
-        json_parser,
+        self_healing_json_parser,
         microservice_description=microservice_description,
         # nlp_fns=nlp_fns,
         sub_task_tree=sub_task_tree_dict, solutions=solutions
     )
     # for task_dict in self.iterate_over_sub_tasks(sub_task_tree_updated):
     #     task_dict.update(self.get_additional_task_info(task_dict['task']))
 
     sub_task_tree = TaskTree.parse_obj(sub_task_tree_updated)
     return sub_task_tree
 
+
 # def get_additional_task_info(self, sub_task_description):
 #     additional_info_dict = self.get_additional_infos(
 #         description=sub_task_description,
 #         parameter={
 #             'display_name': 'Task description',
 #             'text': sub_task_description,
 #         },
@@ -254,15 +268,14 @@
 #         if ask_gpt(is_feedback_valuable_prompt, boolean_parser, user_feedback=user_feedback,
 #                         microservice_description=microservice_description):
 #             return user_feedback
 #         else:
 #             print('Sorry, I can not handle this feedback. Please formulate it more precisely.')
 
 
-
 # better_description_prompt = client_description + '''
 # Update the description of the Microservice to make it more precise without adding or removing information.'''
 
 
 # If we want to activate this back, then it first needs to work. Currently, it outputs "no" for too many cases.
 # is_feedback_valuable_prompt = client_description + '''
 # User feedback:
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/pm/task_tree_schema.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/pm/task_tree_schema.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/app_template.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/app_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,70 @@
 import json
 import os
 
 import streamlit as st
 from jina import Client, Document, DocumentArray
-import io
 
-st.set_page_config(
-    page_title="<page title here>",
-    page_icon="<page icon here>",
-    layout="centered",
-    initial_sidebar_state="auto",
-)
-
-st.title("<thematic emoji here> <header title here>")
-st.markdown(
-    "<10 word description here>"
-    "To generate and deploy your own microservice, click [here](https://github.com/jina-ai/dev-gpt)."
-)
-st.subheader("<a unique thematic emoji here> <sub header title here>")  # only if input parameters are needed
-with st.form(key="input_form"):
-    # <input parameter definition here>
-    input_json_dict = {} #
+def main():
+    set_page_config()
+    st.title("<thematic emoji here> <header title here>")
+    st.markdown(
+        "<10 word description here>"
+        "To generate and deploy your own microservice, click [here](https://github.com/jina-ai/dev-gpt)."
+    )
+    st.subheader("<a unique thematic emoji here> <sub header title here>")  # only if input parameters are needed
+    is_submitted, input_json_dict = get_input_parameters()
 
     input_json_dict_string = json.dumps(input_json_dict)
-    submitted = st.form_submit_button("<submit button text>")
+    # call microservice
+    if is_submitted:
+        output_data = make_api_call(input_json_dict_string)
+        # <visualization of results here>
 
-# Process input and call microservice
-if submitted:
+    display_curl_command(input_json_dict_string)
+
+def make_api_call(input_json_dict_string):
     with st.spinner("<spinner text here>..."):
         client = Client(host="http://localhost:8080")
         d = Document(text=input_json_dict_string)
         response = client.post("/", inputs=DocumentArray([d]))
 
         output_data = json.loads(response[0].text)
-        # <visualization of results here>
+    return output_data
 
-# Display curl command
-deployment_id = os.environ.get("K8S_NAMESPACE_NAME", "")
-api_endpoint = (
-    f"https://dev-gpt-{deployment_id.split('-')[1]}.wolf.jina.ai/post"
-    if deployment_id
-    else "http://localhost:8080/post"
-)
-
-with st.expander("See curl command"):
-    st.markdown("You can use the following curl command to send a request to the microservice from the command line:")
-    escaped_input_json_dict_string = input_json_dict_string.replace('"', '\\"')
-
-    st.code(
-        f'curl -X "POST" "{api_endpoint}" -H "accept: application/json" -H "Content-Type: application/json" -d \'{{"data": [{{"text": "{escaped_input_json_dict_string}"}}]}}\'',
-        language="bash",
+def display_curl_command(input_json_dict_string):
+    # Display curl command
+    deployment_id = os.environ.get("K8S_NAMESPACE_NAME", "")
+    api_endpoint = (
+        f"https://dev-gpt-{deployment_id.split('-')[1]}.wolf.jina.ai/post"
+        if deployment_id
+        else "http://localhost:8080/post"
     )
+
+    with st.expander("See curl command"):
+        st.markdown(
+            "You can use the following curl command to send a request to the microservice from the command line:")
+        escaped_input_json_dict_string = input_json_dict_string.replace('"', '\\"')
+
+        st.code(
+            f'curl -X "POST" "{api_endpoint}" -H "accept: application/json" -H "Content-Type: application/json" -d \'{{"data": [{{"text": "{escaped_input_json_dict_string}"}}]}}\'',
+            language="bash",
+        )
+
+def get_input_parameters():
+    with st.form(key="input_form"):
+        # <input parameter definition here>
+        input_json_dict = {}  # <input parameter dictionary here>
+        is_submitted = st.form_submit_button("<submit button text>")
+    return is_submitted, input_json_dict
+
+
+def set_page_config():
+    st.set_page_config(
+        page_title="<page title here>",
+        page_icon="<page icon here>",
+        layout="centered",
+        initial_sidebar_state="auto",
+    )
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/google_custom_search.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/google_custom_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,13 +16,28 @@
         'num': top_n
     }
     response = requests.get(url, params=params)
     response.raise_for_status()
     return response.json()
 
 def search_images(search_term, top_n):
-    response = google_search(search_term, search_type="image", top_n=top_n)
-    return [item["link"] for item in response["items"]]
+    """
+    Returns only images that have a 200 response code.
+    """
+    response = google_search(search_term, search_type="image", top_n=10)
+    image_urls = []
+    for item in response["items"]:
+        if len(image_urls) >= top_n:
+            break
+        try:
+            response = requests.head(item["link"], timeout=2)
+            if response.status_code == 200:
+                image_urls.append(
+                    item["link"]
+                )
+        except requests.exceptions.RequestException:
+            pass
+    return image_urls
 
 def search_web(search_term, top_n):
     response = google_search(search_term, search_type="web", top_n=top_n)
     return [item["snippet"] for item in response["items"]]
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/templates_system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 from dev_gpt.options.generate.templates_user import not_allowed_docker_string, not_allowed_function_string
 
 
 template_system_message_base = f'''It is September 2021. 
-You are a principal engineer working at Jina - an open source company.
+You are a helpful assistant.
 You accurately satisfy all of the user's requirements.
-To be more specific, you help the user to build a microservice with the following requirements:
-```
-{{task_description}}
-```
-and the following test scenario:
-```
-{{test_description}}
-```
-
 You must obey the following rules:
 {not_allowed_function_string}
 {not_allowed_docker_string}'''
 
 system_task_introduction = f'''
 You are a product manager who refines the requirements of a client who wants to create a microservice.
 '''
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/templates_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from langchain import PromptTemplate
 
 from dev_gpt.constants import IMPLEMENTATION_FILE_NAME
 
-general_guidelines_string = '''The code you write is production ready. Every file starts with comments describing what the code is doing before the first import. Comments can only be written within code blocks.
-Then all imports are listed.
-
-Start from top-level and then fully implement all methods.'''
+general_guidelines_string = '''\
+The code you write is production ready. 
+Every file starts with comments describing what the code is doing before the first import. 
+Comments can only be written within code blocks.'''
 
 
 not_allowed_docker_string = '''Note that the Dockerfile only has access to the files: microservice.py, requirements.txt, config.yml, test_microservice.py.
 Note that the Dockerfile runs the test_microservice.py during the build process.
 The Dockerfile must not attach a virtual display when running test_microservice.py.'''
 
 
@@ -19,95 +19,81 @@
 The implemented function and the test must not access external apis unless it is explicitly mentioned.
 The implemented function and the test must not be based on a large collection of hard-coded strings.
 The implemented function and the test must not open files from the local file system unless it was created by the implemented function itself.
 The implemented function and the test must not use a pre-trained model unless it is explicitly mentioned in the description.
 The implemented function and the test must not train a model.
 The implemented function and the test must not contain prototype or placeholder implementations.
 The implemented function and the test must run in a docker container based on debian.
-The implemented function and the test must not use libraries like Flask.
 The implemented function and the test must not have a __main__ function.
 The implemented function and the test must use gpt_3_5_turbo if the task requires the processing of language (e.g., understanding, generation, summarization, transformation, translation, modification or classification). Other language models are not allowed.
 The implemented function must follow a clean and elegant coding style.'''
 
+plain_response_format_prompt = '''The response must be raw text and not fenced by markdown or html'''
 
-template_generate_microservice_name = PromptTemplate.from_template(
-    '''Generate a name for the executor matching the description:
-"{description}"
+template_generate_microservice_name = f'''\
+Generate a name for the executor matching the description:
+"{{description}}"
 The executor name must fulfill the following criteria:
 - camel case
 - start with a capital letter
 - only consists of lower and upper case characters
 - end with Executor.
-
-Your response must exactly match the following block code format (double asterisks for the file name and triple backticks for the file block):
-**name.txt**
-```
-<name here>
-```
-Example for: "Get a png as input and return a vectorized version as svg.":
-**name.txt**
+{plain_response_format_prompt}
+Positive example:
+PngToSvgExecutor
+Negative example:
 ```
 PngToSvgExecutor
-```'''
-)
+```
+'''
+
 
 # todo split into multiple calls. One for brainstorming - one for the final answer
-template_generate_possible_packages = PromptTemplate.from_template(
-    '''Here is the task description of the problem you need to solve:
+template_generate_possible_packages = '''\
+Here is the task description of the problem you need to solve:
 "{description}"
 1. Write down up to 3 different strategies to solve the task. For each strategy write down how it solves the core problems.
-Note that packages are preferred over external apis except if it is mentioned in the description.
-2. For each strategy list up to 3 Python packages that are specifically designed or have functionalities to solve the complete core problems.
-3. For each package think if it fulfills the following requirements:
-a) specifically designed or have functionalities to solve the complete core problem.
-b) has a stable api among different versions
-c) does not have system requirements
-d) can solve the task when running in a docker container
-e) the implementation of the core problem using the package would obey the following rules:
-''' + not_allowed_function_string + '''
-
-When answering, just write "yes" or "no".
-
-4. For each approach, list the required python package combinations as discibed in the following.
-You must output the package combinations as json wrapped into triple backticks ``` and name it **strategies.json**. \
+Note that packages are preferred over external apis except they are mentioned in the description.
+2. Write down the strategies.json which is a list of required python package combinations.
 Note that you can also leave a list empty to indicate that one of the strategies does not require any package and can be done in plain python.
-Write the output using double asterisks and triple backticks like this:
+Note that if gpt_3_5_turbo or google_custom_search are mentioned in the description, then they must be part of each strategy in strategies.json.
+Example:
 **strategies.json**
 ```
 [
   ["package1", "package2", "package3"],
   ["package4", "package5"],
-  ["package6", "package7", "package8", "package9"],
+  ["package6", "package7", "gpt_3_5_turbo"],
   [],
-  ["package10"]
+  ["google_custom_search"]
 ]
-```''')
+```'''
 
 
 template_code_wrapping_string = '''The code will go into {file_name_purpose}.
 Note that you must obey the double asterisk and triple backtick syntax from like this:
 **{file_name}**
 ```{tag_name}
 ...code...
 ```
 You must provide the complete {file_name} wrapped with the exact syntax shown above.'''
 
 
-gpt_35_turbo_usage_string = """If you need to use gpt_3_5_turbo, then use it like shown in the following example:
+gpt_35_turbo_usage_string = """Use the gpt_3_5_turbo like shown in the following example:
 ```
 from .gpt_3_5_turbo import GPT_3_5_Turbo
 
 gpt_3_5_turbo = GPT_3_5_Turbo(
     system_string=\'\'\'
 You are a tv-reporter who is specialized in C-list celebrities.
 When you get asked something like 'Who was having a date with <X>?', then you answer with a string like "<y>, <z> were having a date with <x>"'. 
 You must not answer something else - only the json.
 \'\'\')
 
-generated_string = gpt_3_5_turbo(prompt_string="example user prompt") # prompt_string is the only parameter
+generated_string = gpt_3_5_turbo("example user prompt") # prompt_string is the only parameter
 ```
 """
 
 google_custom_search_usage_string = """If you need to use google_custom_search, then use it like shown in the following example:
 a) when searching for text:
 ```
 from .google_custom_search import search_web
@@ -133,30 +119,25 @@
 
 Write a python function which receives as \
 input json dictionary string (that can be parsed with the python function json.loads) and \
 outputs a json dictionary string (that can be parsed with the python function json.loads). \
 The function is called 'func' and has the following signature:
 def func(input_json_dict_string: str) -> str:
 The function must fulfill the following description: '{{microservice_description}}'.
-It will be tested with the following scenario: '{{test_description}}'.
+The function must pass the following test condition: '{{test_description}}'.
 For the implementation use the following package(s): '{{packages}}'.
 
 The code must start with the following imports:
 ```{linebreak +'from .gpt_3_5_turbo import GPT_3_5_Turbo' if is_using_gpt_3_5_turbo else ""}{linebreak + 'from .google_custom_search import search_web, search_images' if is_using_google_custom_search else ""}
 import json
 import requests
 ```
 Obey the following rules:
 {not_allowed_function_string}
 
-Your approach:
-1. Identify the core challenge when implementing the function.
-2. Think about solutions for these challenges.
-3. Decide for one of the solutions.
-4. Write the code for the function. Don't write code for the test.
 {gpt_35_turbo_usage_string if is_using_gpt_3_5_turbo else ''}
 {google_custom_search_usage_string if is_using_google_custom_search else ''}
 {template_code_wrapping_string}'''
     )
 
 
 template_generate_test = PromptTemplate.from_template(
@@ -236,15 +217,15 @@
 
 
 template_summarize_error = PromptTemplate.from_template(
     '''Your task is to condense an error encountered during the docker build process. The error message is as follows:
 "{error}"
 Your task is to summarize the error message as compact and informative as possible \
 while maintaining all information necessary to debug the core issue (100 words).
-It should also provide some additional context regarding the specific file and line number where the error occurred. \
+It should also provide some additional context regarding the specific file. \
 Note that you must not suggest a solution to the error.
 Warnings are not worth mentioning.'''
 )
 
 
 template_is_dependency_issue = PromptTemplate.from_template(
     '''Your task is to assist in identifying the root cause of a Docker build error for a python application.
@@ -314,67 +295,77 @@
 
 To solve this error, you should determine the list of packages that need to be installed via `apt-get install` in the Dockerfile.
 Output the apt-get packages that need to be placed at {{APT_GET_PACKAGES}} as json in the following format:
 **apt-get-packages.json**
 ```json
 {{"packages": ["<package1>", "<package2>"]}}
 ```
-Example:
-Error is about missing package `libgl1-mesa-glx`.
-The output is:
+
+Example output for an error is about missing package `libgl1-mesa-glx`:
 **apt-get-packages.json**
 ```json
 {{"packages": [libgl1-mesa-glx]}}
 ```
-Only output content of the apt-get-packages.json file. Ensure the response can be parsed by Python json.loads
+
+Negative example1:
+```json
+{{"packages": [libgl1-mesa-glx]}}
+```
+
+Negative example2:
+{{"packages": [libgl1-mesa-glx]}}
+
+Note: Only output content of the apt-get-packages.json file.
 Note: you must not output the content of any other. Especially don't output the Dockerfile or requirements.txt. 
 Note: the first line you output must be: **apt-get-packages.json**
 '''
 )
 
 
-response_format_suggest_solutions = '''**solutions.json**
+response_format_suggest_solutions = '''\
 ```json
 {{
     "1": "<best solution>",
     "2": "<2nd best solution>"
 }}
 ```'''
 
 
-template_suggest_solutions_code_issue = PromptTemplate.from_template(
-    '''General rules:
-''' + not_allowed_function_string + '''
+template_suggest_solutions_code_issue = f'''\
+General rules:
+{not_allowed_function_string}
 
 Here is the description of the task the function must solve:
-{task_description}
+{{task_description}}
 
 Here is the test scenario the function must pass:
-{test_description}
+{{test_description}}
 Here are all the files I use:
-{all_files_string}
+{{all_files_string}}
 
 
 Here is the summary of the error that occurred:
-{summarized_error}
+{{summarized_error}}
 
 You should suggest 3 to 5 possible solution approaches on how to solve it.
 Obey the following rules:
 Do not implement the solution.
 You have no access to the documentation of the package.
 You must not change the Dockerfile.
-Note that any changes needed to make the test pass must be written under the constraint that ''' + IMPLEMENTATION_FILE_NAME +  ''' will be used in a different file as well.
-''' + f'{not_allowed_function_string}\n{not_allowed_docker_string}\n{gpt_35_turbo_usage_string}' + '''
+Note that any changes needed to make the test pass must be written under the constraint that {IMPLEMENTATION_FILE_NAME} will be used in a different file as well.
+{not_allowed_function_string}
+{not_allowed_docker_string}
+{gpt_35_turbo_usage_string}
 
 
 After thinking about the possible solutions, output them as JSON ranked from best to worst.
 You must use the following format:
-''' + response_format_suggest_solutions + '''
-Ensure the response starts with **solutions.json** and can be parsed by Python json.loads'''
-)
+{response_format_suggest_solutions}
+Ensure the response can be parsed by Python json.loads'''
+
 
 
 response_format_was_error_seen_before = '''**was_error_seen_before.json**
 ```json
 {{"was_error_seen_before": "<yes/no>"}}
 ```'''
 
@@ -552,7 +543,32 @@
 Note that you must obey the double asterisk and triple backtick syntax from above.
 Note that the last sequence of characters in your response must be ``` (triple backtick).
 Note that your response must start with the character sequence ** (double asterisk).
 Note that prompt.json must only contain one question.
 {custom_suffix}
 '''
 )
+
+generate_used_apis_prompt = '''\
+Microservice description: 
+{microservice_description}
+
+Question:
+Respond with a list as JSON indicating which web APIs (e.g. google_custom_search, gpt_3_5_turbo) are mentioned in the description.
+Note that local libraries are not web APIs and must not be mentioned. 
+Positive Example 1:
+{{
+  "mentioned_apis": ["google_custom_search", "gpt_3_5_turbo"]
+}}
+Positive Example 2:
+{{
+    "mentioned_apis": ["google_custom_search"]
+}}
+Positive Example 3:
+{{
+    "mentioned_apis": ["gpt_3_5_turbo"]
+}}
+Positive Example 4:
+{{
+    "mentioned_apis": []
+}}
+'''
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.42.dev87/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt/utils/io.py` & `dev-gpt-0.18.42.dev87/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.42.dev87/dev_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.42.dev8
+Version: 0.18.42.dev87
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
-Author: Florian Hönicke
-Author-email: florian.hoenicke@jina.ai
-License: UNKNOWN
+Author: Jina AI
+Author-email: hello@jina.ai
+License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
-Dev GPT: Your Automated Development Team
+Dev-GPT: Your Automated Development Team
 </h1>
 
 <p align="center" style="color: red; font-weight: bold;">
 ⚠️ This is an experimental version. ⚠️
 </p>
 
 <div align="center">
@@ -88,16 +88,16 @@
 ### Requirements
 - OpenAI key with access to gpt-3.5-turbo or gpt-4
 - if you want to enable your microservice to search for web content, 
 you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID environment variables.
 More information can be found [here](https://developers.google.com/custom-search/v1/overview).
 ```bash
 dev-gpt configure --openai_api_key <your openai api key>
-dev-gpt configure --google_api_key <google api key> (optional if you want to use google search)
-dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google search)
+dev-gpt configure --google_api_key <google api key> (optional if you want to use google custom search)
+dev-gpt configure --google_cse_id <google cse id> (optional if you want to use google custom search)
 ```
 
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ## Docs
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.42.dev8 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.42.dev87 Summary: Use natural
 language interface to generate, deploy and update your microservice
-infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
-HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE
-            ****** Dev GPT: Your Automated Development Team ******
+infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Jina AI
+Author-email: hello@jina.ai License: Apache 2.0 Platform: UNKNOWN Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
+            ****** Dev-GPT: Your Automated Development Team ******
                 â ï¸ This is an experimental version. â ï¸
                     [Product Manager] [Developer] [DevOps]
                      Product Manager   Developer   DevOps
 Tell your AI team what microservice you want to build, and they will do it for
                       you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
             platforms] [Downloads] [https://img.shields.io/discord/
@@ -26,20 +25,20 @@
 project is covered, from concept to deployment. ## Quickstart ```bash pip
 install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
 to gpt-3.5-turbo or gpt-4 - if you want to enable your microservice to search
 for web content, you need to set the GOOGLE_API_KEY and GOOGLE_CSE_ID
 environment variables. More information can be found [here](https://
 developers.google.com/custom-search/v1/overview). ```bash dev-gpt configure --
 openai_api_key  dev-gpt configure --google_api_key  (optional if you want to
-use google search) dev-gpt configure --google_cse_id  (optional if you want to
-use google search) ``` If you set the environment variable `OPENAI_API_KEY`,
-the configuration step can be skipped. Your api key must have access to gpt-
-4 to use this tool. We are working on a way to use gpt-3.5-turbo as well. ##
-Docs ### Generate Microservice ```bash dev-gpt generate \ --description "" \ --
-model
+use google custom search) dev-gpt configure --google_cse_id  (optional if you
+want to use google custom search) ``` If you set the environment variable
+`OPENAI_API_KEY`, the configuration step can be skipped. Your api key must have
+access to gpt-4 to use this tool. We are working on a way to use gpt-3.5-turbo
+as well. ## Docs ### Generate Microservice ```bash dev-gpt generate \ --
+description "" \ --model
 5-turbo or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5-turbo` or `gpt-4`. `gpt-3.5-
 turbo` is ~10x cheaper, but will not be able to generate as complex
 microservices. (default: largest you have access to) - A `path` on the local
 drive where the microservice will be generated. (default: ./microservice) The
```

### Comparing `dev-gpt-0.18.42.dev8/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.42.dev87/dev_gpt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 dev_gpt/options/generate/prompt_factory.py
 dev_gpt/options/generate/templates_system.py
 dev_gpt/options/generate/templates_user.py
 dev_gpt/options/generate/ui.py
 dev_gpt/options/generate/chains/__init__.py
 dev_gpt/options/generate/chains/auto_refine_description.py
 dev_gpt/options/generate/chains/extract_information.py
+dev_gpt/options/generate/chains/fix_based_on_error.py
 dev_gpt/options/generate/chains/get_user_input_if_needed.py
 dev_gpt/options/generate/chains/question_answering.py
 dev_gpt/options/generate/chains/translation.py
 dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
 dev_gpt/options/generate/pm/__init__.py
 dev_gpt/options/generate/pm/pm.py
 dev_gpt/options/generate/pm/task_tree_schema.py
@@ -64,11 +65,15 @@
 test/__init__.py
 test/conftest.py
 test/integration/__init__.py
 test/integration/test_generator.py
 test/unit/__init__.py
 test/unit/test_api.py
 test/unit/test_construct_sub_task_tree.py
+test/unit/test_error_summarization.py
+test/unit/test_packages.py
 test/unit/test_response_parsing.py
 test/unit/test_search.py
+test/unit/test_self_refinement.py
 test/unit/test_strings.py
-test/unit/test_tools.py
+test/unit/test_tools.py
+test/unit/test_yes_no_question.py
```

### Comparing `dev-gpt-0.18.42.dev8/setup.py` & `dev-gpt-0.18.42.dev87/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 setup(
     name='dev-gpt',
     version=__version__,
     description='Use natural language interface to generate, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    author='Florian Hönicke',
-    author_email='florian.hoenicke@jina.ai',
+    author='Jina AI',
+    author_email='hello@jina.ai',
+    license='Apache 2.0',
     url='https://github.com/jina-ai/dev-gpt',
     packages=find_packages(),
     include_package_data=True,
     install_requires=read_requirements(),
     scripts=['main.py'],
     entry_points={
         'console_scripts': [
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dev-gpt-0.18.42.dev8/test/conftest.py` & `dev-gpt-0.18.42.dev87/test/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from typing import List, Generator
 
 import pytest
 
+from dev_gpt.apis.gpt import GPTSession
+
 
 def input_generator(input_sequence: list) -> Generator[str, None, None]:
     """
     Creates a generator that yields input strings from the given sequence.
 
     :param input_sequence: A list of input strings.
     :return: A generator that yields input strings.
@@ -30,7 +32,11 @@
     Creates a temporary directory for a microservice.
 
     :param tmpdir: A temporary directory.
     :return: The path of the temporary directory.
     """
     return os.path.join(str(tmpdir), "microservice")
 
+@pytest.fixture
+def init_gpt(tmpdir):
+    os.environ['VERBOSE'] = 'true'
+    GPTSession(os.path.join(str(tmpdir), 'log.json'), model='gpt-3.5-turbo')
```

### Comparing `dev-gpt-0.18.42.dev8/test/integration/test_generator.py` & `dev-gpt-0.18.42.dev87/test/integration/test_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Databases: ❌
     """
     os.environ['VERBOSE'] = 'true'
     generator = Generator(
         "The microservice is very simple, it does not take anything as input and only outputs the word 'test'",
         microservice_dir,
         'gpt-3.5-turbo',
-        self_healing=False,
+        # self_healing=False,
     )
     assert generator.generate() == 0
 
 
 @pytest.mark.parametrize('mock_input_sequence', [['y']], indirect=True)
 def test_generation_level_1(microservice_dir, mock_input_sequence):
     """
@@ -37,18 +37,15 @@
     environment: ❌
     GPT-3.5-turbo: ✅ (for summarizing the text)
     APIs: ❌
     Databases: ❌
     """
     os.environ['VERBOSE'] = 'true'
     generator = Generator(
-        '''Input is a tweet that might contain passive aggressive language. The output is the positive version of that tweet.
-Example tweet: 
-\'When your coworker microwaves fish in the break room... AGAIN. 🐟🤢 
-But hey, at least SOMEONE's enjoying their lunch. #officelife\'''',
+        '''Input is a tweet that contains passive aggressive language. The output is the positive version of that tweet.''',
         str(microservice_dir),
         'gpt-3.5-turbo',
         # self_healing=False,
     )
     assert generator.generate() == 0
 
 
@@ -62,15 +59,15 @@
     environment: ❌
     GPT-3.5-turbo: ✅ (for summarizing the text)
     APIs: ❌
     Databases: ❌
     """
     os.environ['VERBOSE'] = 'true'
     generator = Generator(
-        "The input is a PDF and the output the summarized text (50 words).",
+        "The input is a PDF and the output the summarized text.",
         str(microservice_dir),
         'gpt-3.5-turbo',
         # self_healing=False,
     )
     assert generator.generate() == 0
 
 
@@ -92,15 +89,15 @@
         str(microservice_dir),
         'gpt-3.5-turbo',
         # self_healing=False,
     )
     assert generator.generate() == 0
 
 
-@pytest.mark.parametrize('mock_input_sequence', [['y', 'yfinance.Ticker("MSFT").info']], indirect=True)
+@pytest.mark.parametrize('mock_input_sequence', [['y', 'ticker = yf.Ticker(symbol); data = ticker.history(start=start_date, end=end_date); [row[\'Close\'] for row in data.to_dict(\'records\')]']], indirect=True)
 def test_generation_level_3(microservice_dir, mock_input_sequence):
     """
     Requirements:
     coding challenge: ✅ (calculate the average closing price)
     pip packages: ❌
     environment: ❌
     GPT-3.5-turbo: ✅ (for processing the text)
@@ -118,71 +115,76 @@
 ''',
         str(microservice_dir),
         'gpt-3.5-turbo',
         # self_healing=False,
     )
     assert generator.generate() == 0
 
-
-@pytest.mark.parametrize(
-    'mock_input_sequence', [
-        [
-            'y',
-            'https://www2.cs.uic.edu/~i101/SoundFiles/taunt.wav',
-            f'''\
-import requests
-url = "https://transcribe.whisperapi.com"
-headers = {{
-'Authorization': 'Bearer {os.environ['WHISPER_API_KEY']}'
-}}
-data = {{
-  "url": "URL_OF_STORED_AUDIO_FILE"
-}}
-response = requests.post(url, headers=headers, data=data)
-assert response.status_code == 200
-print('This is the text from the audio file:', response.text)'''
-        ]
-    ],
-    indirect=True
-)
-def test_generation_level_4(microservice_dir, mock_input_sequence):
-    """
-    Requirements:
-    coding challenge: ❌
-    pip packages: ✅ (text to speech)
-    environment: ✅ (tts library)
-    GPT-3.5-turbo: ✅ (summarizing the text)
-    APIs: ✅ (whisper for speech to text)
-    Databases: ❌
-    """
-    os.environ['VERBOSE'] = 'true'
-    generator = Generator(
-        f'''Given an audio file (1min wav) of speech, 
-1. convert it to text using the Whisper API.
-2. Summarize the text (~50 words) while still maintaining the key facts.
-3. Create an audio file of the summarized text using a tts library.
-4. Return the the audio file as base64 encoded binary.
-''',
-        str(microservice_dir),
-        'gpt-4',
-        # self_healing=False,
-    )
-    assert generator.generate() == 0
+#
+# @pytest.mark.parametrize(
+#     'mock_input_sequence', [
+#         [
+#             'y',
+#             'https://www2.cs.uic.edu/~i101/SoundFiles/taunt.wav',
+#             f'''\
+# import requests
+# url = "https://transcribe.whisperapi.com"
+# headers = {{
+# 'Authorization': 'Bearer {os.environ['WHISPER_API_KEY']}'
+# }}
+# data = {{
+#   "url": "URL_OF_STORED_AUDIO_FILE"
+# }}
+# response = requests.post(url, headers=headers, data=data)
+# assert response.status_code == 200
+# print('This is the text from the audio file:', response.text)''',
+#             'use any library',
+#             #             f'''\
+#             # import openai
+#             # audio_file= open("/path/to/file/audio.mp3", "rb")
+#             # transcript = openai.Audio.transcribe("whisper-1", audio_file)'''
+#         ]
+#     ],
+#     indirect=True
+# )
+# def test_generation_level_4(microservice_dir, mock_input_sequence):
+#     """
+#     Requirements:
+#     coding challenge: ❌
+#     pip packages: ✅ (text to speech)
+#     environment: ✅ (tts library)
+#     GPT-3.5-turbo: ✅ (summarizing the text)
+#     APIs: ✅ (whisper for speech to text)
+#     Databases: ❌
+#     """
+#     os.environ['VERBOSE'] = 'true'
+#     generator = Generator(
+#         f'''Given an audio file (1min wav) of speech,
+# 1. convert it to text using the Whisper API.
+# 2. Summarize the text (~50 words) while still maintaining the key facts.
+# 3. Create an audio file of the summarized text using a tts library.
+# 4. Return the the audio file as base64 encoded binary.
+# ''',
+#         str(microservice_dir),
+#         # 'gpt-3.5-turbo',
+#         'gpt-4',
+#         # self_healing=False,
+#     )
+#     assert generator.generate() == 0
 
 
 @pytest.mark.parametrize('mock_input_sequence', [['y']], indirect=True)
 def test_generation_level_5_company_logos(microservice_dir, mock_input_sequence):
     os.environ['VERBOSE'] = 'true'
     generator = Generator(
         f'''\
-Given a list of email addresses, get all company names from them.
+Given a list of email addresses, get all unique company names from them.
 For all companies, get the company logo.
 All logos need to be arranged on a square.
-The square is returned as png.
-''',
+The square is returned as png.''',
         str(microservice_dir),
         'gpt-3.5-turbo',
         # self_healing=False,
     )
     assert generator.generate() == 0
```

### Comparing `dev-gpt-0.18.42.dev8/test/unit/test_api.py` & `dev-gpt-0.18.42.dev87/test/unit/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,23 +52,29 @@
 io~=0.0.1
 # not parsable version
 pdfminer.six>=20201018,<20211018
 # existing package without version
 requests
 # another existing package without version
 streamlit
+# invalid version 1.0beta5prerelease
+google-api-python-client
+# with comment
+language-tool-python==2.5.3  # requires Java
 """
     requirements_clean = """\
 jina==111.222.333
 docarray==111.222.333
 gtts~=2.2.3
 pydub~=0.25.1
 pdfminer.six~=20201018
 requests~=2.26.0
-streamlit~=0.89.0"""
+streamlit~=0.89.0
+google-api-python-client~=2.23.0
+language-tool-python==2.5.3"""
     requirements_txt_path = os.path.join(tmpdir, "requirements.txt")
     with open(requirements_txt_path, "w", encoding="utf-8") as f:
         f.write(requirements_content)
 
     clean_requirements_txt(tmpdir)
 
     with open(requirements_txt_path, "r", encoding="utf-8") as f:
```

