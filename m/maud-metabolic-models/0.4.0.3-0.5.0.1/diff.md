# Comparing `tmp/maud-metabolic-models-0.4.0.3.tar.gz` & `tmp/maud-metabolic-models-0.5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maud-metabolic-models-0.4.0.3.tar", last modified: Tue Jun  6 14:20:48 2023, max compression
+gzip compressed data, was "maud-metabolic-models-0.5.0.1.tar", last modified: Tue Jun  6 14:30:42 2023, max compression
```

## Comparing `maud-metabolic-models-0.4.0.3.tar` & `maud-metabolic-models-0.5.0.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/
--rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/experimental_setup.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/inits.json
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/input_data_train.json
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/expected_stan_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/inits.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/methionine_cycle.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.292125 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.296125 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/experiments.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/parameters.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/priors.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/src/maud/data_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/hardcoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/id_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/kinetic_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/data_model/prior_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_idatas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/getting_stan_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/loading_maud_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/parsing_kinetic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/running_stan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/src/maud/stan/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/debug.stan
--rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/functions.stan
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/model.stan
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/stan/out_of_sample_model.stan
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-06 14:20:35.000000 maud-metabolic-models-0.4.0.3/src/maud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:20:48.300125 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:20:48.000000 maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-06 14:30:42.478769 maud-metabolic-models-0.5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/
+-rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/experimental_setup.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/inits.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/input_data_train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/expected_stan_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.470768 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/inits.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/methionine_cycle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    36103 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.466768 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/experiments.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/priors.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud/data_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/hardcoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/id_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/kinetic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/data_model/prior_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_idatas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/getting_stan_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/loading_maud_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/parsing_kinetic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/running_stan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/debug.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    20773 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/functions.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/stan/out_of_sample_model.stan
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-06 14:30:30.000000 maud-metabolic-models-0.5.0.1/src/maud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:30:42.474769 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:30:42.000000 maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/zip-safe
```

### Comparing `maud-metabolic-models-0.4.0.3/LICENSE` & `maud-metabolic-models-0.5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/PKG-INFO` & `maud-metabolic-models-0.5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.4.0.3
+Version: 0.5.0.1
 Summary: Bayesian statistical models of metabolic networks
 Home-page: https://github.com/biosustain/Maud
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 Author-email: tedgro@dtu.dk
 License: GNU General Public License version 3
 Download-URL: https://pypi.org/project/maud-metabolic-models/
 Platform: UNKNOWN
```

### Comparing `maud-metabolic-models-0.4.0.3/README.rst` & `maud-metabolic-models-0.5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/setup.cfg` & `maud-metabolic-models-0.5.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = maud-metabolic-models
 url = https://github.com/biosustain/Maud
 download_url = https://pypi.org/project/maud-metabolic-models/
 author = Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 author_email = tedgro@dtu.dk
-version = 0.4.0.3
+version = 0.5.0.1
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Natural Language :: English
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `maud-metabolic-models-0.4.0.3/setup.py` & `maud-metabolic-models-0.5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/analysis.py` & `maud-metabolic-models-0.5.0.1/src/maud/analysis.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/cli.py` & `maud-metabolic-models-0.5.0.1/src/maud/cli.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/ODE_solution.xlsx`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/inits.json` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/inits.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/input_data_train.json` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/input_data_train.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/kinetic_model.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/example_ode/priors.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/example_ode/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/expected_stan_input.json` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/expected_stan_input.json`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/experiments.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/kinetic_model.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/parameters.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/linear/priors.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/linear/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/experiments.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/inits.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/inits.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/methionine_cycle.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/methionine_cycle.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/parameters.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_inputs/methionine/priors.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_inputs/methionine/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/experiments.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/experiments.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/kinetic_model.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/parameters.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/parameters.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data/example_outputs/linear/user_input/priors.toml` & `maud-metabolic-models-0.5.0.1/src/maud/data/example_outputs/linear/user_input/priors.toml`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/experiment.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/experiment.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/kinetic_model.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/kinetic_model.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_config.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_config.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_init.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_init.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_input.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/maud_parameter.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/maud_parameter.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/prior.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/prior.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/data_model/prior_input.py` & `maud-metabolic-models-0.5.0.1/src/maud/data_model/prior_input.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/getting_idatas.py` & `maud-metabolic-models-0.5.0.1/src/maud/getting_idatas.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/getting_parameters.py` & `maud-metabolic-models-0.5.0.1/src/maud/getting_parameters.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/getting_priors.py` & `maud-metabolic-models-0.5.0.1/src/maud/getting_priors.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/getting_stan_inputs.py` & `maud-metabolic-models-0.5.0.1/src/maud/getting_stan_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/loading_maud_inputs.py` & `maud-metabolic-models-0.5.0.1/src/maud/loading_maud_inputs.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/parsing_kinetic_models.py` & `maud-metabolic-models-0.5.0.1/src/maud/parsing_kinetic_models.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/running_stan.py` & `maud-metabolic-models-0.5.0.1/src/maud/running_stan.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/stan/functions.stan` & `maud-metabolic-models-0.5.0.1/src/maud/stan/functions.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/stan/model.stan` & `maud-metabolic-models-0.5.0.1/src/maud/stan/model.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/stan/out_of_sample_model.stan` & `maud-metabolic-models-0.5.0.1/src/maud/stan/out_of_sample_model.stan`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud/utils.py` & `maud-metabolic-models-0.5.0.1/src/maud/utils.py`

 * *Files identical despite different names*

### Comparing `maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/PKG-INFO` & `maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maud-metabolic-models
-Version: 0.4.0.3
+Version: 0.5.0.1
 Summary: Bayesian statistical models of metabolic networks
 Home-page: https://github.com/biosustain/Maud
 Author: Novo Nordisk Foundation Center for Biosustainability, Technical University of Denmark
 Author-email: tedgro@dtu.dk
 License: GNU General Public License version 3
 Download-URL: https://pypi.org/project/maud-metabolic-models/
 Platform: UNKNOWN
```

### Comparing `maud-metabolic-models-0.4.0.3/src/maud_metabolic_models.egg-info/SOURCES.txt` & `maud-metabolic-models-0.5.0.1/src/maud_metabolic_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

