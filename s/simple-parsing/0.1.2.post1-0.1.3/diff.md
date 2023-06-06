# Comparing `tmp/simple_parsing-0.1.2.post1.tar.gz` & `tmp/simple_parsing-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_parsing-0.1.2.post1.tar", last modified: Thu Apr 27 19:03:25 2023, max compression
+gzip compressed data, was "simple_parsing-0.1.3.tar", last modified: Tue Jun  6 21:40:02 2023, max compression
```

## Comparing `simple_parsing-0.1.2.post1.tar` & `simple_parsing-0.1.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/simple_parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/simple_parsing/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.707081 simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/get_field_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/help_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/flatten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hparam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/nested_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    33395 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/yaml_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/helpers/subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/replace.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.711081 simple_parsing-0.1.2.post1/simple_parsing/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/dataclass_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_metavar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/simple_parsing/wrappers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.707081 simple_parsing-0.1.2.post1/simple_parsing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 19:03:25.000000 simple_parsing-0.1.2.post1/simple_parsing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:03:25.715081 simple_parsing-0.1.2.post1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_bools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_custom_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_default_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_future_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_generation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_huggingface_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_initvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue64.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_107.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_132.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_144.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_46.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_48.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_issue_96.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_optional_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_optional_union.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_positional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_set_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_suppress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_tuples.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/test/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-04-27 19:03:06.000000 simple_parsing-0.1.2.post1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/simple_parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/simple_parsing/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.568274 simple_parsing-0.1.3/simple_parsing/annotation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/annotation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/annotation_utils/get_field_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/help_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.568274 simple_parsing-0.1.3/simple_parsing/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/flatten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.572275 simple_parsing-0.1.3/simple_parsing/helpers/hparams/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/hparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/nested_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.572275 simple_parsing-0.1.3/simple_parsing/helpers/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33185 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/yaml_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28879 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.572275 simple_parsing-0.1.3/simple_parsing/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/dataclass_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/field_metavar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/field_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/field_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.568274 simple_parsing-0.1.3/simple_parsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_bools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_custom_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_default_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_future_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_generation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_huggingface_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_initvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_132.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_46.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_96.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_optional_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_optional_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_positional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_set_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_suppress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/versioneer.py
```

### Comparing `simple_parsing-0.1.2.post1/LICENSE` & `simple_parsing-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/PKG-INFO` & `simple_parsing-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_parsing
-Version: 0.1.2.post1
+Version: 0.1.3
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.2.post1/README.md` & `simple_parsing-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/setup.py` & `simple_parsing-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     install_requires = req_file.read().splitlines(keepends=False)
 
 extras_require: dict[str, list[str]] = {
     "test": [
         "pytest",
         "pytest-xdist",
         "pytest-regressions",
+        "numpy",
+        "torch",
     ],
     "yaml": ["pyyaml"],
 }
 extras_require["all"] = list(set(sum(extras_require.values(), [])))
 
 
 setuptools.setup(
```

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/__init__.py` & `simple_parsing-0.1.3/simple_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/annotation_utils/get_field_annotations.py` & `simple_parsing-0.1.3/simple_parsing/annotation_utils/get_field_annotations.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/conflicts.py` & `simple_parsing-0.1.3/simple_parsing/conflicts.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/decorators.py` & `simple_parsing-0.1.3/simple_parsing/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/docstring.py` & `simple_parsing-0.1.3/simple_parsing/docstring.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/help_formatter.py` & `simple_parsing-0.1.3/simple_parsing/help_formatter.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/custom_actions.py` & `simple_parsing-0.1.3/simple_parsing/helpers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/fields.py` & `simple_parsing-0.1.3/simple_parsing/helpers/fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/flatten.py` & `simple_parsing-0.1.3/simple_parsing/helpers/flatten.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hparam.py` & `simple_parsing-0.1.3/simple_parsing/helpers/hparams/hparam.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters.py` & `simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/hyperparameters_test.py` & `simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors.py` & `simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/hparams/priors_test.py` & `simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/nested_partial.py` & `simple_parsing-0.1.3/simple_parsing/helpers/nested_partial.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/partial.py` & `simple_parsing-0.1.3/simple_parsing/helpers/partial.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/decoding.py` & `simple_parsing-0.1.3/simple_parsing/helpers/serialization/decoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/encoding.py` & `simple_parsing-0.1.3/simple_parsing/helpers/serialization/encoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/serializable.py` & `simple_parsing-0.1.3/simple_parsing/helpers/serialization/serializable.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from importlib import import_module
 from itertools import chain
 from logging import getLogger
 from pathlib import Path
 from types import ModuleType
 from typing import IO, Any, Callable, ClassVar, TypeVar, Union
 
+from typing_extensions import Protocol
+
 from simple_parsing.utils import (
     DataclassT,
     all_subclasses,
     get_args,
     get_forward_arg,
     is_optional,
 )
@@ -53,14 +55,105 @@
         ordered_dict_constructor,
     )
 
 except ImportError:
     pass
 
 
+class FormatExtension(Protocol):
+    binary: ClassVar[bool] = False
+
+    @staticmethod
+    def load(fp: IO) -> Any:
+        ...
+
+    @staticmethod
+    def dump(obj: Any, io: IO) -> None:
+        ...
+
+
+class JSONExtension(FormatExtension):
+    load = staticmethod(json.load)
+    dump = staticmethod(json.dump)
+
+
+class PickleExtension(FormatExtension):
+    binary: ClassVar[bool] = True
+    load: ClassVar[Callable[[IO], Any]] = staticmethod(pickle.load)
+    dump: ClassVar[Callable[[Any, IO[bytes]], None]] = staticmethod(pickle.dump)
+
+
+class YamlExtension(FormatExtension):
+    def load(self, io: IO) -> Any:
+        import yaml
+
+        return yaml.safe_load(io)
+
+    def dump(self, obj: Any, io: IO, **kwargs) -> None:
+        import yaml
+
+        return yaml.dump(obj, io, **kwargs)
+
+
+class NumpyExtension(FormatExtension):
+    binary: bool = True
+
+    def load(self, io: IO) -> Any:
+        import numpy
+
+        obj = numpy.load(io, allow_pickle=True)
+        if isinstance(obj, numpy.ndarray) and obj.dtype == object:
+            obj = obj.item()
+        return obj
+
+    def dump(self, obj: Any, io: IO[bytes], **kwargs) -> None:
+        import numpy
+
+        return numpy.save(io, obj, **kwargs)
+
+
+class TorchExtension(FormatExtension):
+    binary: bool = True
+
+    def load(self, io: IO) -> None:
+        import torch  # type: ignore
+
+        return torch.load(io)
+
+    def dump(self, obj: Any, io: IO, **kwargs) -> None:
+        import torch  # type: ignore
+
+        return torch.save(obj, io, **kwargs)
+
+
+json_extension = JSONExtension()
+yaml_extension = YamlExtension()
+
+
+extensions: dict[str, FormatExtension] = {
+    ".json": JSONExtension(),
+    ".pkl": PickleExtension(),
+    ".yaml": YamlExtension(),
+    ".yml": YamlExtension(),
+    ".npy": NumpyExtension(),
+    ".pth": TorchExtension(),
+}
+
+
+def get_extension(path: str | Path) -> FormatExtension:
+    path = Path(path)
+    if path.suffix in extensions:
+        return extensions[path.suffix]
+    else:
+        raise RuntimeError(
+            f"Cannot load to/save from a {path.suffix} file because "
+            "this extension is not registered in the extensions dictionary."
+        )
+
+
 class SerializableMixin:
     """Makes a dataclass serializable to and from dictionaries.
 
     Supports JSON and YAML files for now.
 
     >>> from dataclasses import dataclass
     >>> from simple_parsing.helpers import Serializable
@@ -244,25 +337,25 @@
                 None, in which case `yaml.safe_load` is used.
 
         Returns:
             D: an instance of the dataclass.
         """
         return load_yaml(cls, path, load_fn=load_fn, drop_extra_fields=drop_extra_fields, **kwargs)
 
-    def save(self, path: str | Path, dump_fn=None) -> None:
-        save(self, path=path, dump_fn=dump_fn)
+    def save(self, path: str | Path, format: FormatExtension | None = None) -> None:
+        save(self, path=path, format=format)
 
-    def _save(self, path: str | Path, dump_fn: DumpFn = json.dump, **kwargs) -> None:
-        save(self, path=path, dump_fn=partial(dump_fn, **kwargs))
+    def _save(self, path: str | Path, format: FormatExtension = json_extension, **kwargs) -> None:
+        save(self, path=path, format=format, **kwargs)
 
     def save_yaml(self, path: str | Path, dump_fn: DumpFn | None = None, **kwargs) -> None:
-        save_yaml(self, path, dump_fn=dump_fn, **kwargs)
+        save_yaml(self, path, **kwargs)
 
-    def save_json(self, path: str | Path, dump_fn=json.dump, **kwargs) -> None:
-        save_json(self, path, dump_fn=dump_fn, **kwargs)
+    def save_json(self, path: str | Path, **kwargs) -> None:
+        save_json(self, path, **kwargs)
 
     @classmethod
     def loads(
         cls: type[D],
         s: str,
         drop_extra_fields: bool | None = None,
         load_fn: LoadsFn = json.loads,
@@ -480,130 +573,52 @@
 ) -> DataclassT:
     import yaml
 
     load_fn = load_fn or yaml.safe_load
     return loads(cls, s, drop_extra_fields=drop_extra_fields, load_fn=partial(load_fn, **kwargs))
 
 
-extensions_to_loading_fn: dict[str, Callable[[IO], Any]] = {
-    ".json": json.load,
-    ".pkl": pickle.load,
-}
-extensions_to_read_mode: dict[str, str] = {".pkl": "rb"}
-
-extensions_to_write_mode: dict[str, str] = {".pkl": "wb"}
-extensions_to_dump_fn: dict[str, Callable[[Any, IO], None]] = {
-    ".json": json.dump,
-    ".pkl": pickle.dump,
-}
-try:
-    import yaml
-
-    extensions_to_loading_fn[".yaml"] = yaml.safe_load
-    extensions_to_loading_fn[".yml"] = yaml.safe_load
-    extensions_to_dump_fn[".yaml"] = yaml.dump
-    extensions_to_dump_fn[".yml"] = yaml.dump
-
-
-except ImportError:
-    pass
-
-try:
-    import numpy  # type: ignore
-
-    extensions_to_loading_fn[".npy"] = numpy.load
-    extensions_to_dump_fn[".npy"] = numpy.save
-    extensions_to_read_mode[".npy"] = "rb"
-    extensions_to_write_mode[".npy"] = "wb"
-
-except ImportError:
-    pass
-
-try:
-    import torch  # type: ignore
-
-    extensions_to_loading_fn[".pth"] = torch.load
-    extensions_to_dump_fn[".pth"] = torch.save
-    extensions_to_read_mode[".pth"] = "rb"
-    extensions_to_write_mode[".pth"] = "wb"
-except ImportError:
-    pass
-
-
 def read_file(path: str | Path) -> dict:
     """Returns the contents of the given file as a dictionary.
     Uses the right function depending on `path.suffix`:
     {
         ".yml": yaml.safe_load,
         ".yaml": yaml.safe_load,
         ".json": json.load,
         ".pth": torch.load,
         ".pkl": pickle.load,
     }
     """
-    path = Path(path)
-    if path.suffix in extensions_to_loading_fn:
-        load_fn = extensions_to_loading_fn[path.suffix]
-    else:
-        raise RuntimeError(
-            f"Unable to determine what function to use in order to load "
-            f"path {path} into a dictionary since the path's extension isn't registered in the "
-            f"`extensions_to_loading_fn` dictionary..."
-        )
-    mode = extensions_to_read_mode.get(path.suffix, "r")
-    with open(path, mode=mode) as f:
-        return load_fn(f)
+    format = get_extension(path)
+    with open(path, mode="rb" if format.binary else "r") as f:
+        return format.load(f)
 
 
 def save(
     obj: Any,
     path: str | Path,
-    dump_fn: Callable[[dict, IO], None] | None = None,
+    format: FormatExtension | None = None,
     save_dc_types: bool = False,
+    **kwargs,
 ) -> None:
-    """Save the given dataclass or dictionary to the given file.
-
-    Note: The `encode` function is applied to all the object fields to get serializable values,
-    like so:
-    - obj -> encode -> "raw" values (dicts, strings, ints, etc) -> `dump_fn` ([json/yaml/etc].dumps) -> string
-    """
-    path = Path(path)
-
+    """Save the given dataclass or dictionary to the given file."""
     if not isinstance(obj, dict):
         obj = to_dict(obj, save_dc_types=save_dc_types)
+    if format is None:
+        format = get_extension(path)
+    with open(path, mode="wb" if format.binary else "w") as f:
+        return format.dump(obj, f, **kwargs)
 
-    if dump_fn:
-        save_fn = dump_fn
-    elif path.suffix in extensions_to_dump_fn:
-        save_fn = extensions_to_dump_fn[path.suffix]
-    else:
-        raise RuntimeError(
-            f"Unable to determine what function to use in order to save obj {obj} to path {path},"
-            f"since the path's extension isn't registered in the "
-            f"`extensions_to_dump_fn` dictionary..."
-        )
-    mode = extensions_to_write_mode.get(path.suffix, "w")
-    with open(path, mode=mode) as f:
-        return save_fn(obj, f)
 
+def save_yaml(obj, path: str | Path, **kwargs) -> None:
+    save(obj, path, format=yaml_extension, **kwargs)
 
-def save_yaml(
-    obj, path: str | Path, dump_fn: DumpFn | None = None, save_dc_types: bool = False, **kwargs
-) -> None:
-    import yaml
-
-    if dump_fn is None:
-        dump_fn = yaml.dump
-    save(obj, path, dump_fn=partial(dump_fn, **kwargs), save_dc_types=save_dc_types)
 
-
-def save_json(
-    obj, path: str | Path, dump_fn: DumpFn = json.dump, save_dc_types: bool = False, **kwargs
-) -> None:
-    save(obj, path, dump_fn=partial(dump_fn, **kwargs), save_dc_types=save_dc_types)
+def save_json(obj, path: str | Path, **kwargs) -> None:
+    save(obj, path, format=json_extension, **kwargs)
 
 
 def load_yaml(
     cls: type[T],
     path: str | Path,
     drop_extra_fields: bool | None = None,
     load_fn: LoadFn | None = None,
```

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/serialization/yaml_serialization.py` & `simple_parsing-0.1.3/simple_parsing/helpers/serialization/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/helpers/subgroups.py` & `simple_parsing-0.1.3/simple_parsing/helpers/subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/parsing.py` & `simple_parsing-0.1.3/simple_parsing/parsing.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/replace.py` & `simple_parsing-0.1.3/simple_parsing/replace.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/utils.py` & `simple_parsing-0.1.3/simple_parsing/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     TypeVar,
     Union,
     overload,
 )
 
 from typing_extensions import Literal, Protocol, TypeGuard, get_args, get_origin
 
+# There are cases where typing.Literal doesn't match typing_extensions.Literal:
+# https://github.com/python/typing_extensions/pull/148
+try:
+    from typing import Literal as LiteralAlt
+except ImportError:
+    LiteralAlt = Literal  # type: ignore
+
 
 # NOTE: Copied from typing_inspect.
 def is_typevar(t) -> bool:
     return type(t) is TypeVar
 
 
 def get_bound(t):
@@ -258,15 +265,15 @@
     >>> is_literal(Literal[1,2,3])
     True
     >>> is_literal(Literal["foo", "bar"])
     True
     >>> is_literal(Optional[Literal[1,2]])
     False
     """
-    return get_origin(t) is Literal
+    return get_origin(t) in (Literal, LiteralAlt)
 
 
 def is_list(t: type) -> bool:
     """returns True when `t` is a List type.
 
     Args:
         t (Type): a type.
```

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/wrappers/dataclass_wrapper.py` & `simple_parsing-0.1.3/simple_parsing/wrappers/dataclass_wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_metavar.py` & `simple_parsing-0.1.3/simple_parsing/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_parsing.py` & `simple_parsing-0.1.3/simple_parsing/wrappers/field_parsing.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/wrappers/field_wrapper.py` & `simple_parsing-0.1.3/simple_parsing/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing/wrappers/wrapper.py` & `simple_parsing-0.1.3/simple_parsing/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/simple_parsing.egg-info/PKG-INFO` & `simple_parsing-0.1.3/simple_parsing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-parsing
-Version: 0.1.2.post1
+Version: 0.1.3
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.2.post1/simple_parsing.egg-info/SOURCES.txt` & `simple_parsing-0.1.3/simple_parsing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_aliases.py` & `simple_parsing-0.1.3/test/test_aliases.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_base.py` & `simple_parsing-0.1.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_bools.py` & `simple_parsing-0.1.3/test/test_bools.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_choice.py` & `simple_parsing-0.1.3/test/test_choice.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_conflicts.py` & `simple_parsing-0.1.3/test/test_conflicts.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_custom_args.py` & `simple_parsing-0.1.3/test/test_custom_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_decoding.py` & `simple_parsing-0.1.3/test/test_decoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_decorator.py` & `simple_parsing-0.1.3/test/test_decorator.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_default_args.py` & `simple_parsing-0.1.3/test/test_default_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_docstrings.py` & `simple_parsing-0.1.3/test/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_examples.py` & `simple_parsing-0.1.3/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_fields.py` & `simple_parsing-0.1.3/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_forward_ref.py` & `simple_parsing-0.1.3/test/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_future_annotations.py` & `simple_parsing-0.1.3/test/test_future_annotations.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_generation_mode.py` & `simple_parsing-0.1.3/test/test_generation_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 
 import pytest
 
 from simple_parsing.wrappers.field_wrapper import ArgumentGenerationMode, NestedMode
 
-from . import TestSetup
+from .testutils import TestSetup
 
 
 @dataclass
 class ModelOptions:
     path: str
     device: str
```

### Comparing `simple_parsing-0.1.2.post1/test/test_huggingface_compat.py` & `simple_parsing-0.1.3/test/test_huggingface_compat.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_inheritance.py` & `simple_parsing-0.1.3/test/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_initvar.py` & `simple_parsing-0.1.3/test/test_initvar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_issue64.py` & `simple_parsing-0.1.3/test/test_issue64.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_issue_107.py` & `simple_parsing-0.1.3/test/test_issue_107.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_issue_132.py` & `simple_parsing-0.1.3/test/test_issue_132.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_issue_144.py` & `simple_parsing-0.1.3/test/test_issue_144.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_issue_46.py` & `simple_parsing-0.1.3/test/test_issue_46.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_issue_48.py` & `simple_parsing-0.1.3/test/test_issue_48.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_issue_96.py` & `simple_parsing-0.1.3/test/test_issue_96.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_lists.py` & `simple_parsing-0.1.3/test/test_lists.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_literal.py` & `simple_parsing-0.1.3/test/test_literal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import enum
+import sys
 from dataclasses import dataclass
 from typing import Any, List, NamedTuple, Optional
 
 import pytest
 from typing_extensions import Literal
 
 from .testutils import (
     TestSetup,
+    exits_and_writes_to_stderr,
     raises_invalid_choice,
     raises_missing_required_arg,
     xfail_param,
 )
 
 
 class FieldComponents(NamedTuple):
@@ -94,7 +96,25 @@
         Foo.setup("")
 
     assert Foo.setup(f"--values {passed_value} {passed_value}") == Foo(
         values=[parsed_value, parsed_value]
     )
     with raises_invalid_choice():
         assert Foo.setup(f"--values {incorrect_value}")
+
+
+@dataclass
+class SomeFoo(TestSetup):
+    param: Literal["bar", "biz"] = "biz"
+
+
+@pytest.mark.skipif(sys.version_info != (3, 9), reason="Bug is only in 3.9")
+@pytest.mark.xfail(strict=True, reason="This bug was fixed by #260")
+def test_reproduce_issue_259_parsing_literal_py39():
+    """Reproduces https://github.com/lebrice/SimpleParsing/issues/259"""
+    # $ python issue.py
+    # usage: issue.py [-h] [--param typing.Literal['bar', 'biz']]
+    # issue.py: error: argument --param: invalid typing.Literal['bar', 'biz'] value: 'biz'
+    with exits_and_writes_to_stderr(
+        "argument --param: invalid typing.Literal['bar', 'biz'] value: 'biz'"
+    ):
+        assert SomeFoo.setup("").param == "biz"
```

### Comparing `simple_parsing-0.1.2.post1/test/test_multiple.py` & `simple_parsing-0.1.3/test/test_multiple.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_optional.py` & `simple_parsing-0.1.3/test/test_optional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_optional_subparsers.py` & `simple_parsing-0.1.3/test/test_optional_subparsers.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_positional.py` & `simple_parsing-0.1.3/test/test_positional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_replace.py` & `simple_parsing-0.1.3/test/test_replace.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_set_defaults.py` & `simple_parsing-0.1.3/test/test_set_defaults.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_subgroups.py` & `simple_parsing-0.1.3/test/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_subparsers.py` & `simple_parsing-0.1.3/test/test_subparsers.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_suppress.py` & `simple_parsing-0.1.3/test/test_suppress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import shlex
 from dataclasses import dataclass
-from test import raises_missing_required_arg
+from test.testutils import raises_missing_required_arg
 
 from simple_parsing import ArgumentParser
 from simple_parsing.utils import str2bool
 
 
 def test_suppress_default(simple_attribute, silent):
     some_type, passed_value, expected_value = simple_attribute
```

### Comparing `simple_parsing-0.1.2.post1/test/test_tuples.py` & `simple_parsing-0.1.3/test/test_tuples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_union.py` & `simple_parsing-0.1.3/test/test_union.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/test_utils.py` & `simple_parsing-0.1.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/test/testutils.py` & `simple_parsing-0.1.3/test/testutils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.2.post1/versioneer.py` & `simple_parsing-0.1.3/versioneer.py`

 * *Files identical despite different names*

