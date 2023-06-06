# Comparing `tmp/maud-metabolic-models-0.4.0.2.tar.gz` & `tmp/maud-metabolic-models-0.4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maud-metabolic-models-0.4.0.2.tar", last modified: Fri Feb  3 12:22:23 2023, max compression
+gzip compressed data, was "maud-metabolic-models-0.4.0.3.tar", last modified: Tue Jun  6 14:20:48 2023, max compression
```

## Comparing `maud-metabolic-models-0.4.0.2.tar` & `maud-metabolic-models-0.4.0.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.536732 maud-metabolic-models-0.4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-03 12:22:23.536732 maud-metabolic-models-0.4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-03 12:22:23.536732 maud-metabolic-models-0.4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.520732 maud-metabolic-models-0.4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.528732 maud-metabolic-models-0.4.0.2/src/maud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.520732 maud-metabolic-models-0.4.0.2/src/maud/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.520732 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.528732 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/
--rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/experimental_setup.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/inits.json
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/input_data_train.json
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.532732 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/expected_stan_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.532732 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)    30603 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/inits.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/methionine_cycle.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.520732 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.520732 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.532732 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.536732 maud-metabolic-models-0.4.0.2/src/maud/data_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/hardcoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/id_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/kinetic_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/data_model/prior_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/getting_idatas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/getting_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/getting_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/getting_stan_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/loading_maud_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/parsing_kinetic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/running_stan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.536732 maud-metabolic-models-0.4.0.2/src/maud/stan/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/stan/debug.stan
--rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/stan/functions.stan
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/stan/model.stan
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/stan/out_of_sample_model.stan
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-02-03 12:22:13.000000 maud-metabolic-models-0.4.0.2/src/maud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 12:22:23.536732 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-03 12:22:23.000000 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-02-03 12:22:23.000000 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 12:22:23.000000 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-03 12:22:23.000000 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-03 12:22:23.000000 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-03 12:22:23.000000 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 12:22:23.000000 maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/
+-rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/experimental_setup.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/inits.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/input_data_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/expected_stan_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/inits.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/methionine_cycle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/src/maud/data_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/hardcoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/id_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/kinetic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/prior_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_idatas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_stan_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/loading_maud_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/parsing_kinetic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/running_stan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/src/maud/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/debug.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/functions.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/out_of_sample_model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/zip-safe
```

### Comparing `maud-metabolic-models-0.4.0.2/LICENSE` & `maud-metabolic-models-0.4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/PKG-INFO` & `maud-metabolic-models-0.4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.4.0.2
+Version: 0.4.0.3
 Summary: Bayesian statistical models of metabolic networks
 Home-page: https://github.com/biosustain/Maud
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 Author-email: tedgro@dtu.dk
 License: GNU General Public License version 3
 Download-URL: https://pypi.org/project/maud-metabolic-models/
 Platform: UNKNOWN
```

### Comparing `maud-metabolic-models-0.4.0.2/README.rst` & `maud-metabolic-models-0.4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/setup.cfg` & `maud-metabolic-models-0.4.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = maud-metabolic-models
 url = https://github.com/biosustain/Maud
 download_url = https://pypi.org/project/maud-metabolic-models/
 author = Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 author_email = tedgro@dtu.dk
-version = 0.4.0.2
+version = 0.4.0.3
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Natural Language :: English
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `maud-metabolic-models-0.4.0.2/setup.py` & `maud-metabolic-models-0.4.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/analysis.py` & `maud-metabolic-models-0.4.0.3/src/maud/analysis.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/cli.py` & `maud-metabolic-models-0.4.0.3/src/maud/cli.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/inits.json` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/inits.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/input_data_train.json` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/input_data_train.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/kinetic_model.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/example_ode/priors.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/expected_stan_input.json` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/expected_stan_input.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/experiments.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/kinetic_model.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/parameters.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/linear/priors.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/experiments.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/inits.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/inits.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 km = [
   {metabolite = "adn", compartment = "c", enzyme = "AHC1", reaction = "AHC", init = 5.66E-06},
   {metabolite = "ahcys", compartment = "c", enzyme = "AHC1", reaction = "AHC", init = 2.32E-05},
   {metabolite = "hcys-L", compartment = "c", enzyme = "AHC1", reaction = "AHC", init = 1.06E-05},
-  {metabolite = "glyb", compartment = "c", ennnnnzyme = "BHMT1", reaction = "BHMT", init = 0.00845898},
+  {metabolite = "glyb", compartment = "c", enzyme = "BHMT1", reaction = "BHMT", init = 0.00845898},
   {metabolite = "hcys-L", compartment = "c", enzyme = "BHMT1", reaction = "BHMT", init = 1.98E-05},
   {metabolite = "hcys-L", compartment = "c", enzyme = "CBS1", reaction = "CBS", init = 4.24E-05},
   {metabolite = "ser-L", compartment = "c", enzyme = "CBS1", reaction = "CBS", init = 2.83E-06},
   {metabolite = "amet", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", init = 0.000520015},
   {metabolite = "gly", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", init = 0.00253545},
   {metabolite = "atp", compartment = "c", enzyme = "MAT1", reaction = "METAT", init = 0.00203015},
   {metabolite = "met-L", compartment = "c", enzyme = "MAT1", reaction = "METAT", init = 0.000106919},
@@ -38,21 +38,21 @@
 ki = [
   {metabolite = "ahcys", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", init = 5.31E-05},
   {metabolite = "amet", compartment = "c", enzyme = "MAT1", reaction = "METAT", init = 0.000346704},
   {metabolite = "ahcys", compartment = "c", enzyme = "METH-Gen", reaction = "METH", init = 5.56E-06}
 ]
 
 dissociation_constant = [
-  {metabolite = "mlthf", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", init = 0.000228576},
-  {metabolite = "amet", compartment = "c", enzyme = "MTHFR1", reaction = "MTHFR", init = 1.46E-05},
-  {metabolite = "amet", compartment = "c", enzyme = "CBS1", reaction = "CBS", init = 9.30E-05},
-  {metabolite = "amet", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", init = 1.98E-05},
-  {metabolite = "amet", compartment = "c", enzyme = "MAT3", reaction = "METAT", init = 0.000316641},
-  {metabolite = "met-L", compartment = "c", enzyme = "MAT3", reaction = "METAT", init = 0.00059999},
-  {metabolite = "ahcys", compartment = "c", enzyme = "MTHFR1", reaction = "MTHFR", init = 2.45E-06},
+  {metabolite = "mlthf", compartment = "c", enzyme = "GNMT1", init = 0.000228576, modification_type = "inhibition"},
+  {metabolite = "amet", compartment = "c", enzyme = "MTHFR1", init = 1.46E-05, modification_type = "inhibition"},
+  {metabolite = "amet", compartment = "c", enzyme = "CBS1", init = 9.30E-05, modification_type = "activation"},
+  {metabolite = "amet", compartment = "c", enzyme = "GNMT1", init = 1.98E-05, modification_type = "activation"},
+  {metabolite = "amet", compartment = "c", enzyme = "MAT3", init = 0.000316641, modification_type = "activation"},
+  {metabolite = "met-L", compartment = "c", enzyme = "MAT3", init = 0.00059999, modification_type = "activation"},
+  {metabolite = "ahcys", compartment = "c", enzyme = "MTHFR1", init = 2.45E-06, modification_type = "activation"},
 ]
 
 transfer_constant = [
   {enzyme = "CBS1", reaction = "CBS", init = 1.03452},
   {enzyme = "GNMT1", reaction = "GNMT", init = 131.207},
   {enzyme = "MAT3", reaction = "METAT", init = 0.107657},
   {enzyme = "MTHFR1", reaction = "MTHFR", init = 0.392035},
```

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/methionine_cycle.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/methionine_cycle.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/parameters.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_inputs/methionine/priors.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/priors.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 ki = [
   {metabolite = "ahcys", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", exploc = 0.000052, scale = 2},
   {metabolite = "amet", compartment = "c", enzyme = "MAT1", reaction = "METAT", exploc = 0.0003, scale = 0.0004},
   {metabolite = "ahcys", compartment = "c", enzyme = "METH-Gen", reaction = "METH", exploc = 0.000001, scale = 0.00003},  # Based on ahyc_c intracellular
 ]
 
 dissociation_constant = [
-  {metabolite = "amet" ,compartment = "c", enzyme = "MAT3", reaction = "METAT", exploc = 0.0001,scale = 0.001, modification_type = "inhibition"},
-  {metabolite = "met-L", compartment = "c", enzyme = "MAT3", reaction = "METAT", exploc = 0.00045,scale = 0.0008, modification_type = "inhibition"},# Based on met_c conc
-  {metabolite = "amet", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", exploc = 0.00003,scale = 0.002, modification_type = "inhibition"},
-  {metabolite = "mlthf", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", exploc = 0.0003,scale = 2, modification_type = "activation"},
-  {metabolite = "amet", compartment = "c", enzyme = "CBS1", reaction = "CBS", exploc = 9.22e-05,scale = 2, modification_type = "inhibition"},
-  {metabolite = "ahcys", compartment = "c", enzyme = "MTHFR1", reaction = "MTHFR", exploc = 0.000003,scale = 2, modification_type = "inhibition"},
-  {metabolite = "amet", compartment = "c", enzyme = "MTHFR1", reaction = "MTHFR", exploc = 0.000003,scale = 2, modification_type = "activation"},
+  {metabolite = "amet" ,compartment = "c", enzyme = "MAT3", reaction = "METAT", exploc = 0.0001,scale = 0.001, modification_type = "activation"},
+  {metabolite = "met-L", compartment = "c", enzyme = "MAT3", reaction = "METAT", exploc = 0.00045,scale = 0.0008, modification_type = "activation"},# Based on met_c conc
+  {metabolite = "amet", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", exploc = 0.00003,scale = 0.002, modification_type = "activation"},
+  {metabolite = "mlthf", compartment = "c", enzyme = "GNMT1", reaction = "GNMT", exploc = 0.0003,scale = 2, modification_type = "inhibition"},
+  {metabolite = "amet", compartment = "c", enzyme = "CBS1", reaction = "CBS", exploc = 9.22e-05,scale = 2, modification_type = "activation"},
+  {metabolite = "ahcys", compartment = "c", enzyme = "MTHFR1", reaction = "MTHFR", exploc = 0.000003,scale = 2, modification_type = "activation"},
+  {metabolite = "amet", compartment = "c", enzyme = "MTHFR1", reaction = "MTHFR", exploc = 0.000003,scale = 2, modification_type = "inhibition"},
 ]
 
 transfer_constant = [
   {enzyme = "MAT3", reaction = "METAT", exploc = 0.1, scale = 2},
   {enzyme = "GNMT1", reaction = "GNMT", exploc = 1, scale = 2},
   {enzyme = "CBS1", reaction = "CBS", exploc = 1, scale = 2},
   {enzyme = "MTHFR1", reaction = "MTHFR", exploc = 3, scale = 2},
```

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/experiments.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/parameters.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data/example_outputs/linear/user_input/priors.toml` & `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/experiment.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/experiment.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/kinetic_model.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/kinetic_model.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_config.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provides dataclass MaudConfig."""
 from typing import Optional
 
-from pydantic.dataclasses import dataclass
+from pydantic.dataclasses import Field, dataclass
 
 
-@dataclass
+@dataclass(frozen=True)
 class ODEConfig:
     """Config that is specific to the ODE solver."""
 
     rel_tol: float = 1e-9
     abs_tol: float = 1e-9
     max_num_steps: int = int(1e9)
     timepoint: float = 500
@@ -28,27 +28,34 @@
     :param ode_config: Configuration for Stan's ode solver.
     :param stanc_options: Valid choices for CmdStanModel argument `stanc_options`.
     :param cpp_options: Valid choices for CmdStanModel `cpp_options`.
     :param variational_options: Arguments for CmdStanModel.variational.
     :param user_inits_file: path to a csv file of initial values.
     :param steady_state_threshold_abs: absolute threshold for Sv=0 be at steady state
     :param steady_state_threshold_rel: relative threshold for Sv=0 be at steady state
-    :param: drain_small_conc_corrector: number for correcting small conc drains
+    :param default_initial_concentration: in molecule_unit per volume_unit
+    :param drain_small_conc_corrector: number for correcting small conc drains
+    :param molecule_unit: A unit for counting molecules, like 'mol' or 'mmol'
+    :param volume_unit: A unit for measuring volume, like 'L'
+    :param energy_unit: A unit for measuring energy, like 'J' or 'kJ'
     """
 
     name: str
     kinetic_model_file: str
     priors_file: str
     experiments_file: str
     likelihood: bool
     cmdstanpy_config: Optional[dict] = None
     cmdstanpy_config_predict: Optional[dict] = None
     stanc_options: Optional[dict] = None
     cpp_options: Optional[dict] = None
     variational_options: Optional[dict] = None
     user_inits_file: Optional[str] = None
-    ode_config: ODEConfig = ODEConfig()
+    ode_config: ODEConfig = Field(default_factory=ODEConfig)
     reject_non_steady: bool = True
     steady_state_threshold_abs: float = 1e-8
     steady_state_threshold_rel: float = 1e-3
     default_initial_concentration: float = 0.01
     drain_small_conc_corrector: float = 1e-6
+    molecule_unit: str = "mmol"
+    volume_unit: str = "L"
+    energy_unit: str = "kJ"
```

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_init.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_init.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_input.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 @dataclass
 class MaudInput:
     """Everything that is needed to run Maud."""
 
     config: MaudConfig
     kinetic_model: KineticModel
     experiments: List[Experiment]
-    prior_input: PriorInput = PriorInput()
-    init_input: InitInput = InitInput()
+    prior_input: PriorInput = Field(default_factory=PriorInput)
+    init_input: InitInput = Field(default_factory=InitInput)
     parameters: ParameterSet = Field(init=False, exclude=True)
     stan_input_train: Dict = Field(init=False, exclude=True)
     stan_input_test: Dict = Field(init=False, exclude=True)
 
     def __post_init__(self):
         """Add attributes that depend on other ones."""
         self.parameters = get_maud_parameters(
```

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/maud_parameter.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_parameter.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/prior.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/prior.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/data_model/prior_input.py` & `maud-metabolic-models-0.4.0.3/src/maud/data_model/prior_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/getting_idatas.py` & `maud-metabolic-models-0.4.0.3/src/maud/getting_idatas.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/getting_parameters.py` & `maud-metabolic-models-0.4.0.3/src/maud/getting_parameters.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/getting_priors.py` & `maud-metabolic-models-0.4.0.3/src/maud/getting_priors.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/getting_stan_inputs.py` & `maud-metabolic-models-0.4.0.3/src/maud/getting_stan_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/loading_maud_inputs.py` & `maud-metabolic-models-0.4.0.3/src/maud/loading_maud_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/parsing_kinetic_models.py` & `maud-metabolic-models-0.4.0.3/src/maud/parsing_kinetic_models.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/running_stan.py` & `maud-metabolic-models-0.4.0.3/src/maud/running_stan.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/stan/functions.stan` & `maud-metabolic-models-0.4.0.3/src/maud/stan/functions.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/stan/model.stan` & `maud-metabolic-models-0.4.0.3/src/maud/stan/model.stan`

 * *Files 3% similar despite different names*

```diff
@@ -247,25 +247,36 @@
     if (reject_non_steady == 1 &&
         check_steady_state((S * edge_flux)[balanced_mic_ix], conc_balanced_experiment[1], steady_state_threshold_abs, steady_state_threshold_rel) == 0){
         print("Non-steady state in experiment ", e);
         print("Balanced metabolite concentration", conc_balanced_experiment[1]);
         print("flux_train: ", flux_train[e]);
         print("conc_init: ", conc_init);
         print("conc_unbalanced_train: ", conc_unbalanced_train[e]);
+        print("log_conc_unbalanced_train_z: ", log_conc_unbalanced_train_z[e]);
         print("conc_enzyme_experiment: ", conc_enzyme_experiment);
+        print("log_conc_enzyme_train_z: ", log_conc_enzyme_train_z[e]);
         print("km: ", km);
+        print("log_km_z: ", log_km_z);
         print("drain_train: ", drain_train[e]);
+        print("drain_train_z: ", drain_train_z[e]);
         print("kcat: ", kcat);
+        print("log_kcat_z: ", log_kcat_z);
         print("dgr_train: ", dgr_train[e]);
         print("ki: ", ki);
+        print("log_ki_z: ", log_ki_z);
         print("dissociation_constant: ", dissociation_constant);
+        print("log_dissociation_constant_z: ", log_dissociation_constant_z);
         print("transfer_constant: ", transfer_constant);
+        print("log_transfer_constant_z: ", log_transfer_constant_z);
         print("kcat_pme: ", kcat_pme);
+        print("log_kcat_pme_z: ", log_kcat_pme_z);
         print("conc_pme_experiment: ", conc_pme_experiment);
+        print("log_conc_pme_train_z: ", log_conc_pme_train_z[e]);
         print("psi_train: ", psi_train);
+        print("psi_train_z: ", psi_train_z);
         reject("Rejecting");
       }
     }
   }
 }
 model {
   log_kcat_z ~ std_normal();
```

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/stan/out_of_sample_model.stan` & `maud-metabolic-models-0.4.0.3/src/maud/stan/out_of_sample_model.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud/utils.py` & `maud-metabolic-models-0.4.0.3/src/maud/utils.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/PKG-INFO` & `maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.4.0.2
+Version: 0.4.0.3
 Summary: Bayesian statistical models of metabolic networks
 Home-page: https://github.com/biosustain/Maud
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 Author-email: tedgro@dtu.dk
 License: GNU General Public License version 3
 Download-URL: https://pypi.org/project/maud-metabolic-models/
 Platform: UNKNOWN
```

### Comparing `maud-metabolic-models-0.4.0.2/src/maud_metabolic_models.egg-info/SOURCES.txt` & `maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

