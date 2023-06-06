# Comparing `tmp/datamodel-code-generator-0.9.3.tar.gz` & `tmp/datamodel-code-generator-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamodel-code-generator-0.9.3.tar", last modified: Thu Mar 18 05:53:42 2021, max compression
+gzip compressed data, was "datamodel-code-generator-0.9.4.tar", last modified: Sun Mar 21 09:21:51 2021, max compression
```

## Comparing `datamodel-code-generator-0.9.3.tar` & `datamodel-code-generator-0.9.4.tar`

### file list

```diff
@@ -1,548 +1,555 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.531725 datamodel-code-generator-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.543725 datamodel-code-generator-0.9.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      579 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (116)      595 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.543725 datamodel-code-generator-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      818 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      894 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1928 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2674 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     3350 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1068 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    16751 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    12962 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.543725 datamodel-code-generator-0.9.3/datamodel_code_generator/
--rw-r--r--   0 runner    (1001) docker     (116)    11498 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    14162 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4050 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/api.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2324 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/format.py
--rw-r--r--   0 runner    (1001) docker     (116)      333 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/http.py
--rw-r--r--   0 runner    (1001) docker     (116)     3046 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.543725 datamodel-code-generator-0.9.3/datamodel_code_generator/model/
--rw-r--r--   0 runner    (1001) docker     (116)      131 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8818 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1329 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.543725 datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/
--rw-r--r--   0 runner    (1001) docker     (116)     1202 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5077 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (116)      263 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/custom_root_type.py
--rw-r--r--   0 runner    (1001) docker     (116)      388 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (116)     1741 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/imports.py
--rw-r--r--   0 runner    (1001) docker     (116)    10111 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/types.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.543725 datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/
--rw-r--r--   0 runner    (1001) docker     (116)      253 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/Enum.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/
--rw-r--r--   0 runner    (1001) docker     (116)      776 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/BaseModel.jinja2
--rw-r--r--   0 runner    (1001) docker     (116)      682 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/BaseModel_root.jinja2
--rw-r--r--   0 runner    (1001) docker     (116)      134 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/Config.jinja2
--rw-r--r--   0 runner    (1001) docker     (116)      515 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/dataclass.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/datamodel_code_generator/parser/
--rw-r--r--   0 runner    (1001) docker     (116)      729 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22195 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    44624 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/parser/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (116)     1464 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/parser/openapi.py
--rw-r--r--   0 runner    (1001) docker     (116)    13045 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/reference.py
--rw-r--r--   0 runner    (1001) docker     (116)     9864 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/types.py
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-03-18 05:53:42.000000 datamodel-code-generator-0.9.3/datamodel_code_generator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.543725 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    16751 2021-03-18 05:53:42.000000 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    19954 2021-03-18 05:53:42.000000 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-18 05:53:42.000000 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       78 2021-03-18 05:53:42.000000 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      683 2021-03-18 05:53:42.000000 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       31 2021-03-18 05:53:42.000000 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-18 05:53:41.000000 datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (116)      896 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/development-contributing.md
--rw-r--r--   0 runner    (1001) docker     (116)     1753 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/field-constraints.md
--rw-r--r--   0 runner    (1001) docker     (116)      648 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/formatting.md
--rw-r--r--   0 runner    (1001) docker     (116)    12042 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (116)      797 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/jsondata.md
--rw-r--r--   0 runner    (1001) docker     (116)     1417 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/jsonschema.md
--rw-r--r--   0 runner    (1001) docker     (116)     5283 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/openapi.md
--rw-r--r--   0 runner    (1001) docker     (116)      279 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/pyproject_toml.md
--rw-r--r--   0 runner    (1001) docker     (116)     1311 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/support-data-types.md
--rw-r--r--   0 runner    (1001) docker     (116)     2145 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/docs/using_as_module.md
--rw-r--r--   0 runner    (1001) docker     (116)      919 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      400 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (116)      448 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)      423 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/scripts/format.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      476 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/scripts/lint.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)       71 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/scripts/test.bat
--rwxr-xr-x   0 runner    (1001) docker     (116)       99 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (116)     1950 2021-03-18 05:53:42.587726 datamodel-code-generator-0.9.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)      584 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/csv/
--rw-r--r--   0 runner    (1001) docker     (116)       91 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/csv/simple.csv
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.539725 datamodel-code-generator-0.9.3/tests/data/expected/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.539725 datamodel-code-generator-0.9.3/tests/data/expected/main/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/all_of_ref/
--rw-r--r--   0 runner    (1001) docker     (116)      303 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/all_of_ref/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/allow_population_by_field_name/
--rw-r--r--   0 runner    (1001) docker     (116)     1995 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/allow_population_by_field_name/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/csv_file_simple/
--rw-r--r--   0 runner    (1001) docker     (116)      290 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/csv_file_simple/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/csv_stdin_simple/
--rw-r--r--   0 runner    (1001) docker     (116)      287 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/csv_stdin_simple/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/disable_timestamp/
--rw-r--r--   0 runner    (1001) docker     (116)     1239 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/disable_timestamp/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/enable_faux_immutability/
--rw-r--r--   0 runner    (1001) docker     (116)     1830 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/enable_faux_immutability/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/force_optional/
--rw-r--r--   0 runner    (1001) docker     (116)     1464 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/force_optional/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main/
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_autodetect/
--rw-r--r--   0 runner    (1001) docker     (116)      618 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_autodetect/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_base_class/
--rw-r--r--   0 runner    (1001) docker     (116)     1246 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_base_class/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_circular_reference/
--rw-r--r--   0 runner    (1001) docker     (116)      685 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_circular_reference/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_complicated_enum_default_member/
--rw-r--r--   0 runner    (1001) docker     (116)      642 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_complicated_enum_default_member/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_custom_template_dir/
--rw-r--r--   0 runner    (1001) docker     (116)     1010 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_custom_template_dir/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_disable_appending_item_suffix/
--rw-r--r--   0 runner    (1001) docker     (116)     1790 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_disable_appending_item_suffix/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.547725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_external_definitions/
--rw-r--r--   0 runner    (1001) docker     (116)      313 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_external_definitions/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_external_files_in_directory/
--rw-r--r--   0 runner    (1001) docker     (116)     1530 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_external_files_in_directory/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_invalid_enum_name/
--rw-r--r--   0 runner    (1001) docker     (116)      281 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_invalid_enum_name/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_invalid_model_name/
--rw-r--r--   0 runner    (1001) docker     (116)      638 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_invalid_model_name/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json/
--rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_array_include_null/
--rw-r--r--   0 runner    (1001) docker     (116)      323 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_array_include_null/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_pointer/
--rw-r--r--   0 runner    (1001) docker     (116)      661 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_pointer/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_reuse_enum/
--rw-r--r--   0 runner    (1001) docker     (116)      501 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_reuse_enum/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_reuse_enum_default_member/
--rw-r--r--   0 runner    (1001) docker     (116)      511 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_reuse_enum_default_member/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_reuse_model/
--rw-r--r--   0 runner    (1001) docker     (116)      615 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_reuse_model/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema/
--rw-r--r--   0 runner    (1001) docker     (116)      618 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_external_files/
--rw-r--r--   0 runner    (1001) docker     (116)      346 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_external_files/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_id/
--rw-r--r--   0 runner    (1001) docker     (116)      395 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_id/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_id_stdin/
--rw-r--r--   0 runner    (1001) docker     (116)      395 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_id_stdin/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/
--rw-r--r--   0 runner    (1001) docker     (116)      385 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/ContactPoint.py
--rw-r--r--   0 runner    (1001) docker     (116)      301 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/URI.py
--rw-r--r--   0 runner    (1001) docker     (116)      516 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      297 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/id.py
--rw-r--r--   0 runner    (1001) docker     (116)      539 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/name.py
--rw-r--r--   0 runner    (1001) docker     (116)      540 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/sameAs.py
--rw-r--r--   0 runner    (1001) docker     (116)      284 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/type.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_nested_deep/
--rw-r--r--   0 runner    (1001) docker     (116)      496 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_nested_deep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.535725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_nested_deep/empty_parent/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_nested_deep/empty_parent/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      267 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_nested_deep/empty_parent/nested/deep.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_nested_deep/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      331 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_nested_deep/nested/deep.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/
--rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      943 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/foo/
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      402 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/foo/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      629 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      663 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/nested/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/woo/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/woo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/woo/boo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/
--rw-r--r--   0 runner    (1001) docker     (116)      640 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      943 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/foo/
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      402 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/foo/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      629 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.551725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      553 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/nested/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/woo/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/woo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/woo/boo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/
--rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/
--rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/drink/
--rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/drink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      247 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/drink/coffee.py
--rw-r--r--   0 runner    (1001) docker     (116)      237 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/drink/tea.py
--rw-r--r--   0 runner    (1001) docker     (116)      426 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/food.py
--rw-r--r--   0 runner    (1001) docker     (116)      600 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/friends.py
--rw-r--r--   0 runner    (1001) docker     (116)      247 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/fur.py
--rw-r--r--   0 runner    (1001) docker     (116)      346 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/pet.py
--rw-r--r--   0 runner    (1001) docker     (116)      814 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/person.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_json_pointer/
--rw-r--r--   0 runner    (1001) docker     (116)     1163 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_json_pointer/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_no_file/
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_no_file/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_null_and_array/
--rw-r--r--   0 runner    (1001) docker     (116)      333 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_null_and_array/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_datetime/
--rw-r--r--   0 runner    (1001) docker     (116)      319 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_datetime/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_enum_models_all/
--rw-r--r--   0 runner    (1001) docker     (116)     1375 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_enum_models_all/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_enum_models_one/
--rw-r--r--   0 runner    (1001) docker     (116)     1483 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_enum_models_one/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_http_refs/
--rw-r--r--   0 runner    (1001) docker     (116)     1592 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_http_refs/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_nullable/
--rw-r--r--   0 runner    (1001) docker     (116)     1473 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_nullable/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_nullable_strict_nullable/
--rw-r--r--   0 runner    (1001) docker     (116)     1482 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_nullable_strict_nullable/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_pattern/
--rw-r--r--   0 runner    (1001) docker     (116)      703 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_pattern/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_id/
--rw-r--r--   0 runner    (1001) docker     (116)      841 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_id/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties/
--rw-r--r--   0 runner    (1001) docker     (116)     1356 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_literal/
--rw-r--r--   0 runner    (1001) docker     (116)     1282 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_literal/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_use_generic_container_types/
--rw-r--r--   0 runner    (1001) docker     (116)     1380 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_use_generic_container_types/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_use_standard_collections/
--rw-r--r--   0 runner    (1001) docker     (116)     1350 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_use_standard_collections/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_self_reference/
--rw-r--r--   0 runner    (1001) docker     (116)      424 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_self_reference/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_similar_nested_array/
--rw-r--r--   0 runner    (1001) docker     (116)     1155 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_similar_nested_array/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types/
--rw-r--r--   0 runner    (1001) docker     (116)      739 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types_all/
--rw-r--r--   0 runner    (1001) docker     (116)      914 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types_all/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types_all_field_constraints/
--rw-r--r--   0 runner    (1001) docker     (116)      738 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types_all_field_constraints/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_subclass_enum/
--rw-r--r--   0 runner    (1001) docker     (116)      489 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_subclass_enum/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.555725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/
--rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      963 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/foo/
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      419 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/foo/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      657 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      674 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/nested/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/woo/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/woo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/woo/boo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/
--rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      990 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/foo/
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      446 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/foo/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      684 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      701 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/woo/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/woo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/woo/boo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/
--rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      937 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/foo/
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      390 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/foo/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      617 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      652 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/nested/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/woo/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/woo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/woo/boo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_aliases/
--rw-r--r--   0 runner    (1001) docker     (116)     1410 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_aliases/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_exclusive/
--rw-r--r--   0 runner    (1001) docker     (116)      558 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_exclusive/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_field_constraints/
--rw-r--r--   0 runner    (1001) docker     (116)     1798 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_field_constraints/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_snake_case_field/
--rw-r--r--   0 runner    (1001) docker     (116)     1407 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_snake_case_field/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_strip_default_none/
--rw-r--r--   0 runner    (1001) docker     (116)     1252 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_strip_default_none/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_without_field_constraints/
--rw-r--r--   0 runner    (1001) docker     (116)     1680 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_without_field_constraints/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/main_yaml/
--rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/main_yaml/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files/
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      327 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files/file_a.py
--rw-r--r--   0 runner    (1001) docker     (116)      215 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files/file_b.py
--rw-r--r--   0 runner    (1001) docker     (116)      327 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files/file_c.py
--rw-r--r--   0 runner    (1001) docker     (116)      327 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files/file_d.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.559725 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_json_pointer/
--rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_json_pointer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      391 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_json_pointer/file_a.py
--rw-r--r--   0 runner    (1001) docker     (116)      534 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_json_pointer/file_b.py
--rw-r--r--   0 runner    (1001) docker     (116)      391 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_json_pointer/file_c.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_self_ref/
--rw-r--r--   0 runner    (1001) docker     (116)      114 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_self_ref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      300 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_self_ref/base_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      308 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_self_ref/test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_self_ref_single/
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_self_ref_single/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/pyproject/
--rw-r--r--   0 runner    (1001) docker     (116)     1471 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/pyproject/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/pyproject_not_found/
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/pyproject_not_found/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/simple_json_snake_case_field/
--rw-r--r--   0 runner    (1001) docker     (116)      251 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/simple_json_snake_case_field/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/space_and_special_characters/
--rw-r--r--   0 runner    (1001) docker     (116)     1112 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/space_and_special_characters/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/space_and_special_characters_dict/
--rw-r--r--   0 runner    (1001) docker     (116)     1115 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/space_and_special_characters_dict/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/stdin/
--rw-r--r--   0 runner    (1001) docker     (116)     1279 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/stdin/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/target_python_version/
--rw-r--r--   0 runner    (1001) docker     (116)     1252 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/target_python_version/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/use_default/
--rw-r--r--   0 runner    (1001) docker     (116)     1294 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/use_default/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main/validation/
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main/validation/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.539725 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main/
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_base_class/
--rw-r--r--   0 runner    (1001) docker     (116)     1246 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_base_class/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_custom_template_dir/
--rw-r--r--   0 runner    (1001) docker     (116)     1010 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_custom_template_dir/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/
--rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      943 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/foo/
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      402 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/foo/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      629 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/nested/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      663 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/nested/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/woo/
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/woo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/woo/boo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.563726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_no_file/
--rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_no_file/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_use_schema_description/
--rw-r--r--   0 runner    (1001) docker     (116)     1348 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_use_schema_description/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/pyproject/
--rw-r--r--   0 runner    (1001) docker     (116)     1425 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/pyproject/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/target_python_version/
--rw-r--r--   0 runner    (1001) docker     (116)     1252 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/main_kr/target_python_version/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.539725 datamodel-code-generator-0.9.3/tests/data/expected/parser/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.539725 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/
--rw-r--r--   0 runner    (1001) docker     (116)      759 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/format.py
--rw-r--r--   0 runner    (1001) docker     (116)      868 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/with_import.py
--rw-r--r--   0 runner    (1001) docker     (116)      871 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format.py
--rw-r--r--   0 runner    (1001) docker     (116)      837 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format_custom_module.Base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/
--rw-r--r--   0 runner    (1001) docker     (116)     1099 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/format.py
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     1216 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format.py
--rw-r--r--   0 runner    (1001) docker     (116)     1162 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format_custom_module.Base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/
--rw-r--r--   0 runner    (1001) docker     (116)     1649 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      842 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/collection_s.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/fo_o/
--rw-r--r--   0 runner    (1001) docker     (116)      302 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/fo_o/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      334 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/fo_o/ba_r.py
--rw-r--r--   0 runner    (1001) docker     (116)      525 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/model_s.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/wo_o/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/wo_o/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      354 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/wo_o/bo_o.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_allof/
--rw-r--r--   0 runner    (1001) docker     (116)     1372 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_allof/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_any/
--rw-r--r--   0 runner    (1001) docker     (116)      169 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_any/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_anyof/
--rw-r--r--   0 runner    (1001) docker     (116)      998 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_anyof/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_array_enum/
--rw-r--r--   0 runner    (1001) docker     (116)      316 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_array_enum/with_import_format.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_duplicate_models/
--rw-r--r--   0 runner    (1001) docker     (116)      842 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_duplicate_models/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/
--rw-r--r--   0 runner    (1001) docker     (116)     1467 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py36.py
--rw-r--r--   0 runner    (1001) docker     (116)     1487 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py37.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.567726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/
--rw-r--r--   0 runner    (1001) docker     (116)      541 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      111 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      530 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/foo/
--rw-r--r--   0 runner    (1001) docker     (116)      261 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      298 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/foo/bar.py
--rw-r--r--   0 runner    (1001) docker     (116)      525 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      531 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/woo/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/woo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      305 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/woo/boo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_nested_anyof/
--rw-r--r--   0 runner    (1001) docker     (116)      293 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_nested_anyof/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_nested_oneof/
--rw-r--r--   0 runner    (1001) docker     (116)      293 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_nested_oneof/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_oneof/
--rw-r--r--   0 runner    (1001) docker     (116)      998 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_oneof/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_remote_ref/
--rw-r--r--   0 runner    (1001) docker     (116)      338 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_remote_ref/with_import_format.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_resolved_models/
--rw-r--r--   0 runner    (1001) docker     (116)      358 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_resolved_models/output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.571726 datamodel-code-generator-0.9.3/tests/data/json/
--rw-r--r--   0 runner    (1001) docker     (116)       94 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/json/array_include_null.json
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/json/broken.json
--rw-r--r--   0 runner    (1001) docker     (116)      229 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/json/duplicate_models.json
--rw-r--r--   0 runner    (1001) docker     (116)       50 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/json/pet.json
--rw-r--r--   0 runner    (1001) docker     (116)       19 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/json/simple.json
--rw-r--r--   0 runner    (1001) docker     (116)      566 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/json/space_and_special_characters.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.575726 datamodel-code-generator-0.9.3/tests/data/jsonschema/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.575726 datamodel-code-generator-0.9.3/tests/data/jsonschema/all_of_ref/
--rw-r--r--   0 runner    (1001) docker     (116)      430 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/all_of_ref/base_test.json
--rw-r--r--   0 runner    (1001) docker     (116)      200 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/all_of_ref/test.json
--rw-r--r--   0 runner    (1001) docker     (116)      949 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/circular_reference.json
--rw-r--r--   0 runner    (1001) docker     (116)      809 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/complicated_enum.json
--rw-r--r--   0 runner    (1001) docker     (116)      381 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/datetime.json
--rw-r--r--   0 runner    (1001) docker     (116)      493 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/duplicate_enum.json
--rw-r--r--   0 runner    (1001) docker     (116)      121 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_child.json
--rw-r--r--   0 runner    (1001) docker     (116)       75 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_child.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      198 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_child_root.json
--rw-r--r--   0 runner    (1001) docker     (116)      137 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_definitions.json
--rw-r--r--   0 runner    (1001) docker     (116)      296 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_definitions_root.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.575726 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.575726 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.575726 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/drink/
--rw-r--r--   0 runner    (1001) docker     (116)      180 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/drink/coffee.json
--rw-r--r--   0 runner    (1001) docker     (116)      172 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/drink/tea.json
--rw-r--r--   0 runner    (1001) docker     (116)      333 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/food.json
--rw-r--r--   0 runner    (1001) docker     (116)      625 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/friends.json
--rw-r--r--   0 runner    (1001) docker     (116)      181 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/fur.json
--rw-r--r--   0 runner    (1001) docker     (116)      273 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/pet.json
--rw-r--r--   0 runner    (1001) docker     (116)     1187 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/person.json
--rw-r--r--   0 runner    (1001) docker     (116)      852 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_parent.json
--rw-r--r--   0 runner    (1001) docker     (116)      216 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/external_parent_root.json
--rw-r--r--   0 runner    (1001) docker     (116)      522 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/id.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.575726 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/
--rw-r--r--   0 runner    (1001) docker     (116)      673 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/ContactPoint.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     1018 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/Organization.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      201 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/URI.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      272 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/context.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      185 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/id.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      408 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/name.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      396 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/sameAs.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      198 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/schema.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      176 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/type.schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      167 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/invalid_enum_name.json
--rw-r--r--   0 runner    (1001) docker     (116)      551 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/invalid_model_name.json
--rw-r--r--   0 runner    (1001) docker     (116)     1866 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/json_pointer.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.575726 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files/
--rw-r--r--   0 runner    (1001) docker     (116)      213 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files/file_a.json
--rw-r--r--   0 runner    (1001) docker     (116)      196 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files/file_b.json
--rw-r--r--   0 runner    (1001) docker     (116)      213 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files/file_c.json
--rw-r--r--   0 runner    (1001) docker     (116)      213 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files/file_d.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.579726 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_json_pointer/
--rw-r--r--   0 runner    (1001) docker     (116)      577 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_json_pointer/file_a.json
--rw-r--r--   0 runner    (1001) docker     (116)     1406 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_json_pointer/file_b.json
--rw-r--r--   0 runner    (1001) docker     (116)      578 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_json_pointer/file_c.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.579726 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_self_ref/
--rw-r--r--   0 runner    (1001) docker     (116)      259 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_self_ref/base_test.json
--rw-r--r--   0 runner    (1001) docker     (116)      364 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_self_ref/test.json
--rw-r--r--   0 runner    (1001) docker     (116)      634 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/nested_array.json
--rw-r--r--   0 runner    (1001) docker     (116)      217 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/nested_array.json.snapshot
--rw-r--r--   0 runner    (1001) docker     (116)     3863 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/nested_json_pointer.json
--rw-r--r--   0 runner    (1001) docker     (116)      894 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/nested_person.json
--rw-r--r--   0 runner    (1001) docker     (116)      584 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/null_and_array.json
--rw-r--r--   0 runner    (1001) docker     (116)      427 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/oneof.json
--rw-r--r--   0 runner    (1001) docker     (116)      131 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/oneof.json.snapshot
--rw-r--r--   0 runner    (1001) docker     (116)      519 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/pattern.json
--rw-r--r--   0 runner    (1001) docker     (116)      552 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/person.json
--rw-r--r--   0 runner    (1001) docker     (116)      467 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/root_id.json
--rw-r--r--   0 runner    (1001) docker     (116)     2239 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/root_model_with_additional_properties.json
--rw-r--r--   0 runner    (1001) docker     (116)      435 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/self_reference.json
--rw-r--r--   0 runner    (1001) docker     (116)     1989 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/similar_nested_array.json
--rw-r--r--   0 runner    (1001) docker     (116)      963 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/strict_types.json
--rw-r--r--   0 runner    (1001) docker     (116)      406 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/jsonschema/user.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/data/openapi/
--rw-r--r--   0 runner    (1001) docker     (116)     5083 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/additional_properties.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     8002 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/alias.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       37 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/aliases.json
--rw-r--r--   0 runner    (1001) docker     (116)     6008 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/allof.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      647 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/any.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     4813 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/anyof.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     4686 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/api.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     5206 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/api_constrained.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      288 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/array_enum.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      449 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/datetime.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/definitions.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2741 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/duplicate_models.yaml
--rw-r--r--   0 runner    (1001) docker     (116)        3 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/empty_aliases.json
--rw-r--r--   0 runner    (1001) docker     (116)        3 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/empty_data.json
--rw-r--r--   0 runner    (1001) docker     (116)     2863 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/enum_models.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     4601 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/example.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      867 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/exclusive.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/extra_data.json
--rw-r--r--   0 runner    (1001) docker     (116)       18 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/invalid.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2291 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/lazy_resolved_models.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       42 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/list.json
--rw-r--r--   0 runner    (1001) docker     (116)     6939 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/modular.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      577 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/nested_anyof.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      577 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/nested_oneof.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2976 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/no_components.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       18 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/not.json
--rw-r--r--   0 runner    (1001) docker     (116)     2034 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/nullable.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     4813 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/oneof.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      571 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/pattern.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      144 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/refs.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/resolved_models.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      763 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/subclass_enum.json
--rw-r--r--   0 runner    (1001) docker     (116)     1050 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/openapi/x_enum_varnames.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/data/project/
--rw-r--r--   0 runner    (1001) docker     (116)      408 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/project/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      260 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (116)      567 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/python/space_and_special_characters_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/data/templates/
--rw-r--r--   0 runner    (1001) docker     (116)      420 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/templates/BaseModel.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/data/yaml/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/data/yaml/pet.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/model/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/model/pydantic/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/model/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5814 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/model/pydantic/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     2333 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/model/pydantic/test_custom_root_type.py
--rw-r--r--   0 runner    (1001) docker     (116)     1958 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/model/pydantic/test_data_class.py
--rw-r--r--   0 runner    (1001) docker     (116)     7634 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/model/pydantic/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     8589 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/model/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-18 05:53:42.583726 datamodel-code-generator-0.9.3/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6969 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/parser/test_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    13667 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/parser/test_jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (116)    16469 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/parser/test_openapi.py
--rw-r--r--   0 runner    (1001) docker     (116)      850 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (116)    73281 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (116)     6584 2021-03-18 05:52:59.000000 datamodel-code-generator-0.9.3/tests/test_main_kr.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.728875 datamodel-code-generator-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.676872 datamodel-code-generator-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.688873 datamodel-code-generator-0.9.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)      579 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      595 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.688873 datamodel-code-generator-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      818 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      894 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1928 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2674 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     3350 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1068 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    16751 2021-03-21 09:21:51.728875 datamodel-code-generator-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    12962 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.688873 datamodel-code-generator-0.9.4/datamodel_code_generator/
+-rw-r--r--   0 runner    (1001) docker     (116)    11600 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    13795 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4050 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/api.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     2324 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/format.py
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/http.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3123 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.688873 datamodel-code-generator-0.9.4/datamodel_code_generator/model/
+-rw-r--r--   0 runner    (1001) docker     (116)      131 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8818 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1329 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.688873 datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (116)     1202 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5077 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)      263 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/custom_root_type.py
+-rw-r--r--   0 runner    (1001) docker     (116)      388 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1741 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/imports.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10111 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/types.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.688873 datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/
+-rw-r--r--   0 runner    (1001) docker     (116)      253 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/Enum.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (116)      776 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/BaseModel.jinja2
+-rw-r--r--   0 runner    (1001) docker     (116)      682 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/BaseModel_root.jinja2
+-rw-r--r--   0 runner    (1001) docker     (116)      134 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/Config.jinja2
+-rw-r--r--   0 runner    (1001) docker     (116)      515 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/dataclass.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/datamodel_code_generator/parser/
+-rw-r--r--   0 runner    (1001) docker     (116)      729 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22496 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)    45116 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/parser/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1464 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/parser/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13279 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/reference.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9749 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2021-03-21 09:21:50.000000 datamodel-code-generator-0.9.4/datamodel_code_generator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.688873 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    16751 2021-03-21 09:21:50.000000 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    20220 2021-03-21 09:21:51.000000 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-21 09:21:50.000000 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       78 2021-03-21 09:21:50.000000 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      683 2021-03-21 09:21:50.000000 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       31 2021-03-21 09:21:50.000000 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-21 09:21:49.000000 datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (116)      896 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/development-contributing.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1753 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/field-constraints.md
+-rw-r--r--   0 runner    (1001) docker     (116)      648 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/formatting.md
+-rw-r--r--   0 runner    (1001) docker     (116)    12042 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (116)      797 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/jsondata.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1417 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/jsonschema.md
+-rw-r--r--   0 runner    (1001) docker     (116)     5283 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/openapi.md
+-rw-r--r--   0 runner    (1001) docker     (116)      279 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/pyproject_toml.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1311 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/support-data-types.md
+-rw-r--r--   0 runner    (1001) docker     (116)     2145 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/docs/using_as_module.md
+-rw-r--r--   0 runner    (1001) docker     (116)      919 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      400 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (116)      448 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)      423 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/scripts/format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)      476 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/scripts/lint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)       71 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/scripts/test.bat
+-rwxr-xr-x   0 runner    (1001) docker     (116)       99 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     1950 2021-03-21 09:21:51.728875 datamodel-code-generator-0.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (116)      584 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/csv/
+-rw-r--r--   0 runner    (1001) docker     (116)       91 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/csv/simple.csv
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.684872 datamodel-code-generator-0.9.4/tests/data/expected/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.684872 datamodel-code-generator-0.9.4/tests/data/expected/main/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/all_of_ref/
+-rw-r--r--   0 runner    (1001) docker     (116)      303 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/all_of_ref/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/allow_population_by_field_name/
+-rw-r--r--   0 runner    (1001) docker     (116)     1995 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/allow_population_by_field_name/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/csv_file_simple/
+-rw-r--r--   0 runner    (1001) docker     (116)      290 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/csv_file_simple/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/csv_stdin_simple/
+-rw-r--r--   0 runner    (1001) docker     (116)      287 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/csv_stdin_simple/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/disable_timestamp/
+-rw-r--r--   0 runner    (1001) docker     (116)     1239 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/disable_timestamp/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/enable_faux_immutability/
+-rw-r--r--   0 runner    (1001) docker     (116)     1830 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/enable_faux_immutability/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/force_optional/
+-rw-r--r--   0 runner    (1001) docker     (116)     1464 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/force_optional/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/main/
+-rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_autodetect/
+-rw-r--r--   0 runner    (1001) docker     (116)      618 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_autodetect/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_base_class/
+-rw-r--r--   0 runner    (1001) docker     (116)     1246 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_base_class/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_circular_reference/
+-rw-r--r--   0 runner    (1001) docker     (116)      685 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_circular_reference/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_complicated_enum_default_member/
+-rw-r--r--   0 runner    (1001) docker     (116)      642 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_complicated_enum_default_member/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.692873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_custom_template_dir/
+-rw-r--r--   0 runner    (1001) docker     (116)     1010 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_custom_template_dir/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_disable_appending_item_suffix/
+-rw-r--r--   0 runner    (1001) docker     (116)     1790 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_disable_appending_item_suffix/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_external_definitions/
+-rw-r--r--   0 runner    (1001) docker     (116)      313 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_external_definitions/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_external_files_in_directory/
+-rw-r--r--   0 runner    (1001) docker     (116)     1530 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_external_files_in_directory/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_invalid_enum_name/
+-rw-r--r--   0 runner    (1001) docker     (116)      281 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_invalid_enum_name/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_invalid_model_name/
+-rw-r--r--   0 runner    (1001) docker     (116)      638 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_invalid_model_name/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json/
+-rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_array_include_null/
+-rw-r--r--   0 runner    (1001) docker     (116)      323 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_array_include_null/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_pointer/
+-rw-r--r--   0 runner    (1001) docker     (116)      661 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_pointer/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_reuse_enum/
+-rw-r--r--   0 runner    (1001) docker     (116)      501 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_reuse_enum/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_reuse_enum_default_member/
+-rw-r--r--   0 runner    (1001) docker     (116)      511 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_reuse_enum_default_member/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_reuse_model/
+-rw-r--r--   0 runner    (1001) docker     (116)      615 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_reuse_model/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (116)      618 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_external_files/
+-rw-r--r--   0 runner    (1001) docker     (116)      346 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_external_files/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_id/
+-rw-r--r--   0 runner    (1001) docker     (116)      395 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_id/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_id_stdin/
+-rw-r--r--   0 runner    (1001) docker     (116)      395 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_id_stdin/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/
+-rw-r--r--   0 runner    (1001) docker     (116)      385 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/ContactPoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)      301 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/URI.py
+-rw-r--r--   0 runner    (1001) docker     (116)      516 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      297 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/id.py
+-rw-r--r--   0 runner    (1001) docker     (116)      539 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/name.py
+-rw-r--r--   0 runner    (1001) docker     (116)      540 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/sameAs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      284 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/type.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_nested_deep/
+-rw-r--r--   0 runner    (1001) docker     (116)      496 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_nested_deep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.680872 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_nested_deep/empty_parent/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_nested_deep/empty_parent/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      267 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_nested_deep/empty_parent/nested/deep.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_nested_deep/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      331 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_nested_deep/nested/deep.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_special_enum/
+-rw-r--r--   0 runner    (1001) docker     (116)      442 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_special_enum/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_special_enum_empty_enum_field_name/
+-rw-r--r--   0 runner    (1001) docker     (116)      444 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_special_enum_empty_enum_field_name/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/
+-rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.696873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/foo/
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      402 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/foo/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      629 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      663 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/nested/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/woo/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/woo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/woo/boo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/
+-rw-r--r--   0 runner    (1001) docker     (116)      640 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/foo/
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      402 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/foo/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      629 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      553 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/nested/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/woo/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/woo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/woo/boo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/
+-rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/
+-rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/drink/
+-rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/drink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      247 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/drink/coffee.py
+-rw-r--r--   0 runner    (1001) docker     (116)      237 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/drink/tea.py
+-rw-r--r--   0 runner    (1001) docker     (116)      426 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/food.py
+-rw-r--r--   0 runner    (1001) docker     (116)      600 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/friends.py
+-rw-r--r--   0 runner    (1001) docker     (116)      247 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/fur.py
+-rw-r--r--   0 runner    (1001) docker     (116)      346 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/pet.py
+-rw-r--r--   0 runner    (1001) docker     (116)      814 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/person.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_json_pointer/
+-rw-r--r--   0 runner    (1001) docker     (116)     1163 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_json_pointer/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_no_file/
+-rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_no_file/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_null_and_array/
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_null_and_array/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.700873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_datetime/
+-rw-r--r--   0 runner    (1001) docker     (116)      319 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_datetime/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_all/
+-rw-r--r--   0 runner    (1001) docker     (116)     1375 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_all/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_as_literal_py37/
+-rw-r--r--   0 runner    (1001) docker     (116)     1404 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_as_literal_py37/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_one/
+-rw-r--r--   0 runner    (1001) docker     (116)     1483 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_one/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_http_refs/
+-rw-r--r--   0 runner    (1001) docker     (116)     1592 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_http_refs/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_nullable/
+-rw-r--r--   0 runner    (1001) docker     (116)     1473 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_nullable/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_nullable_strict_nullable/
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_nullable_strict_nullable/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_pattern/
+-rw-r--r--   0 runner    (1001) docker     (116)      703 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_pattern/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_id/
+-rw-r--r--   0 runner    (1001) docker     (116)      841 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_id/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties/
+-rw-r--r--   0 runner    (1001) docker     (116)     1356 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_literal/
+-rw-r--r--   0 runner    (1001) docker     (116)     1282 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_literal/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_use_generic_container_types/
+-rw-r--r--   0 runner    (1001) docker     (116)     1380 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_use_generic_container_types/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_use_standard_collections/
+-rw-r--r--   0 runner    (1001) docker     (116)     1350 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_use_standard_collections/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_self_reference/
+-rw-r--r--   0 runner    (1001) docker     (116)      424 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_self_reference/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_similar_nested_array/
+-rw-r--r--   0 runner    (1001) docker     (116)     1155 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_similar_nested_array/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types/
+-rw-r--r--   0 runner    (1001) docker     (116)      739 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types_all/
+-rw-r--r--   0 runner    (1001) docker     (116)      914 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types_all/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types_all_field_constraints/
+-rw-r--r--   0 runner    (1001) docker     (116)      738 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types_all_field_constraints/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_subclass_enum/
+-rw-r--r--   0 runner    (1001) docker     (116)      489 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_subclass_enum/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/
+-rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      963 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/foo/
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      419 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/foo/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      657 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      674 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/nested/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/woo/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/woo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/woo/boo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/
+-rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      990 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/foo/
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      446 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/foo/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      701 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/woo/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/woo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/woo/boo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.704873 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/
+-rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      937 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/foo/
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      390 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/foo/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      617 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      652 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/nested/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/woo/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/woo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/woo/boo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_aliases/
+-rw-r--r--   0 runner    (1001) docker     (116)     1410 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_aliases/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_exclusive/
+-rw-r--r--   0 runner    (1001) docker     (116)      558 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_exclusive/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_field_constraints/
+-rw-r--r--   0 runner    (1001) docker     (116)     1798 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_field_constraints/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_snake_case_field/
+-rw-r--r--   0 runner    (1001) docker     (116)     1407 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_snake_case_field/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_strip_default_none/
+-rw-r--r--   0 runner    (1001) docker     (116)     1252 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_strip_default_none/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_without_field_constraints/
+-rw-r--r--   0 runner    (1001) docker     (116)     1680 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_without_field_constraints/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/main_yaml/
+-rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/main_yaml/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files/
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      327 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files/file_a.py
+-rw-r--r--   0 runner    (1001) docker     (116)      215 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files/file_b.py
+-rw-r--r--   0 runner    (1001) docker     (116)      327 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files/file_c.py
+-rw-r--r--   0 runner    (1001) docker     (116)      327 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files/file_d.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.708874 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_json_pointer/
+-rw-r--r--   0 runner    (1001) docker     (116)      118 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_json_pointer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      391 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_json_pointer/file_a.py
+-rw-r--r--   0 runner    (1001) docker     (116)      534 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_json_pointer/file_b.py
+-rw-r--r--   0 runner    (1001) docker     (116)      391 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_json_pointer/file_c.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_self_ref/
+-rw-r--r--   0 runner    (1001) docker     (116)      114 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_self_ref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      300 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_self_ref/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      308 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_self_ref/test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_self_ref_single/
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_self_ref_single/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/pyproject/
+-rw-r--r--   0 runner    (1001) docker     (116)     1471 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/pyproject/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/pyproject_not_found/
+-rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/pyproject_not_found/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/simple_json_snake_case_field/
+-rw-r--r--   0 runner    (1001) docker     (116)      251 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/simple_json_snake_case_field/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/space_and_special_characters/
+-rw-r--r--   0 runner    (1001) docker     (116)     1112 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/space_and_special_characters/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/space_and_special_characters_dict/
+-rw-r--r--   0 runner    (1001) docker     (116)     1115 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/space_and_special_characters_dict/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/stdin/
+-rw-r--r--   0 runner    (1001) docker     (116)     1279 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/stdin/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/target_python_version/
+-rw-r--r--   0 runner    (1001) docker     (116)     1252 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/target_python_version/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/use_default/
+-rw-r--r--   0 runner    (1001) docker     (116)     1294 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/use_default/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main/validation/
+-rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main/validation/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.684872 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main/
+-rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_base_class/
+-rw-r--r--   0 runner    (1001) docker     (116)     1246 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_base_class/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_custom_template_dir/
+-rw-r--r--   0 runner    (1001) docker     (116)     1010 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_custom_template_dir/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/
+-rw-r--r--   0 runner    (1001) docker     (116)      645 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      257 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/foo/
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      402 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/foo/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      629 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      663 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/nested/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/woo/
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/woo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/woo/boo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_no_file/
+-rw-r--r--   0 runner    (1001) docker     (116)     1280 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_no_file/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_use_schema_description/
+-rw-r--r--   0 runner    (1001) docker     (116)     1348 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_use_schema_description/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/pyproject/
+-rw-r--r--   0 runner    (1001) docker     (116)     1425 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/pyproject/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/target_python_version/
+-rw-r--r--   0 runner    (1001) docker     (116)     1252 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/main_kr/target_python_version/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.684872 datamodel-code-generator-0.9.4/tests/data/expected/parser/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.684872 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/
+-rw-r--r--   0 runner    (1001) docker     (116)      759 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/format.py
+-rw-r--r--   0 runner    (1001) docker     (116)      868 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/with_import.py
+-rw-r--r--   0 runner    (1001) docker     (116)      871 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format.py
+-rw-r--r--   0 runner    (1001) docker     (116)      837 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format_custom_module.Base.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/
+-rw-r--r--   0 runner    (1001) docker     (116)     1099 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/format.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1216 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1162 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format_custom_module.Base.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.712874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/
+-rw-r--r--   0 runner    (1001) docker     (116)     1649 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      842 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/collection_s.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/fo_o/
+-rw-r--r--   0 runner    (1001) docker     (116)      302 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/fo_o/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      334 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/fo_o/ba_r.py
+-rw-r--r--   0 runner    (1001) docker     (116)      525 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/model_s.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/wo_o/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/wo_o/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      354 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/wo_o/bo_o.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_allof/
+-rw-r--r--   0 runner    (1001) docker     (116)     1372 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_allof/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_any/
+-rw-r--r--   0 runner    (1001) docker     (116)      169 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_any/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_anyof/
+-rw-r--r--   0 runner    (1001) docker     (116)      998 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_anyof/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_array_enum/
+-rw-r--r--   0 runner    (1001) docker     (116)      316 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_array_enum/with_import_format.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_duplicate_models/
+-rw-r--r--   0 runner    (1001) docker     (116)      842 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_duplicate_models/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/
+-rw-r--r--   0 runner    (1001) docker     (116)     1467 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py36.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1487 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py37.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/
+-rw-r--r--   0 runner    (1001) docker     (116)      541 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      111 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      530 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/foo/
+-rw-r--r--   0 runner    (1001) docker     (116)      261 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      298 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/foo/bar.py
+-rw-r--r--   0 runner    (1001) docker     (116)      525 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      531 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/woo/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/woo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      305 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/woo/boo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_nested_anyof/
+-rw-r--r--   0 runner    (1001) docker     (116)      293 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_nested_anyof/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_nested_oneof/
+-rw-r--r--   0 runner    (1001) docker     (116)      293 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_nested_oneof/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_oneof/
+-rw-r--r--   0 runner    (1001) docker     (116)      998 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_oneof/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_remote_ref/
+-rw-r--r--   0 runner    (1001) docker     (116)      338 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_remote_ref/with_import_format.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_resolved_models/
+-rw-r--r--   0 runner    (1001) docker     (116)      358 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_resolved_models/output.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.716874 datamodel-code-generator-0.9.4/tests/data/json/
+-rw-r--r--   0 runner    (1001) docker     (116)       94 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/json/array_include_null.json
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/json/broken.json
+-rw-r--r--   0 runner    (1001) docker     (116)      229 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/json/duplicate_models.json
+-rw-r--r--   0 runner    (1001) docker     (116)       50 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/json/pet.json
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/json/simple.json
+-rw-r--r--   0 runner    (1001) docker     (116)      566 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/json/space_and_special_characters.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/all_of_ref/
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/all_of_ref/base_test.json
+-rw-r--r--   0 runner    (1001) docker     (116)      200 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/all_of_ref/test.json
+-rw-r--r--   0 runner    (1001) docker     (116)      949 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/circular_reference.json
+-rw-r--r--   0 runner    (1001) docker     (116)      809 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/complicated_enum.json
+-rw-r--r--   0 runner    (1001) docker     (116)      381 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/datetime.json
+-rw-r--r--   0 runner    (1001) docker     (116)      493 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/duplicate_enum.json
+-rw-r--r--   0 runner    (1001) docker     (116)      121 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_child.json
+-rw-r--r--   0 runner    (1001) docker     (116)       75 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_child.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      198 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_child_root.json
+-rw-r--r--   0 runner    (1001) docker     (116)      137 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_definitions.json
+-rw-r--r--   0 runner    (1001) docker     (116)      296 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_definitions_root.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/drink/
+-rw-r--r--   0 runner    (1001) docker     (116)      180 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/drink/coffee.json
+-rw-r--r--   0 runner    (1001) docker     (116)      172 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/drink/tea.json
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/food.json
+-rw-r--r--   0 runner    (1001) docker     (116)      625 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/friends.json
+-rw-r--r--   0 runner    (1001) docker     (116)      181 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/fur.json
+-rw-r--r--   0 runner    (1001) docker     (116)      273 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/pet.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1187 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/person.json
+-rw-r--r--   0 runner    (1001) docker     (116)      852 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_parent.json
+-rw-r--r--   0 runner    (1001) docker     (116)      216 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/external_parent_root.json
+-rw-r--r--   0 runner    (1001) docker     (116)      522 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/id.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/
+-rw-r--r--   0 runner    (1001) docker     (116)      673 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/ContactPoint.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1018 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/Organization.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      201 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/URI.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      272 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/context.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      185 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/id.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      408 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/name.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      396 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/sameAs.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      198 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/schema.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      176 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/type.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      167 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/invalid_enum_name.json
+-rw-r--r--   0 runner    (1001) docker     (116)      551 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/invalid_model_name.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1866 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/json_pointer.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files/
+-rw-r--r--   0 runner    (1001) docker     (116)      213 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files/file_a.json
+-rw-r--r--   0 runner    (1001) docker     (116)      196 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files/file_b.json
+-rw-r--r--   0 runner    (1001) docker     (116)      213 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files/file_c.json
+-rw-r--r--   0 runner    (1001) docker     (116)      213 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files/file_d.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.720874 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_json_pointer/
+-rw-r--r--   0 runner    (1001) docker     (116)      577 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_json_pointer/file_a.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1406 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_json_pointer/file_b.json
+-rw-r--r--   0 runner    (1001) docker     (116)      578 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_json_pointer/file_c.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.724874 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_self_ref/
+-rw-r--r--   0 runner    (1001) docker     (116)      259 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_self_ref/base_test.json
+-rw-r--r--   0 runner    (1001) docker     (116)      364 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_self_ref/test.json
+-rw-r--r--   0 runner    (1001) docker     (116)      634 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/nested_array.json
+-rw-r--r--   0 runner    (1001) docker     (116)      217 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/nested_array.json.snapshot
+-rw-r--r--   0 runner    (1001) docker     (116)     3863 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/nested_json_pointer.json
+-rw-r--r--   0 runner    (1001) docker     (116)      894 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/nested_person.json
+-rw-r--r--   0 runner    (1001) docker     (116)      584 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/null_and_array.json
+-rw-r--r--   0 runner    (1001) docker     (116)      427 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/oneof.json
+-rw-r--r--   0 runner    (1001) docker     (116)      131 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/oneof.json.snapshot
+-rw-r--r--   0 runner    (1001) docker     (116)      519 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/pattern.json
+-rw-r--r--   0 runner    (1001) docker     (116)      552 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/person.json
+-rw-r--r--   0 runner    (1001) docker     (116)      467 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/root_id.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2239 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/root_model_with_additional_properties.json
+-rw-r--r--   0 runner    (1001) docker     (116)      435 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/self_reference.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1989 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/similar_nested_array.json
+-rw-r--r--   0 runner    (1001) docker     (116)      185 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/special_enum.json
+-rw-r--r--   0 runner    (1001) docker     (116)      963 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/strict_types.json
+-rw-r--r--   0 runner    (1001) docker     (116)      406 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/jsonschema/user.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.724874 datamodel-code-generator-0.9.4/tests/data/openapi/
+-rw-r--r--   0 runner    (1001) docker     (116)     5083 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/additional_properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     8002 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/alias.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       37 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (116)     6008 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/allof.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      647 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/any.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     4813 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/anyof.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     4686 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/api.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     5206 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/api_constrained.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      288 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/array_enum.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      449 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/datetime.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1516 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/definitions.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     2741 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/duplicate_models.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)        3 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/empty_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (116)        3 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/empty_data.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2863 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/enum_models.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     4601 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      867 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/exclusive.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/extra_data.json
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/invalid.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     2291 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/lazy_resolved_models.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       42 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/list.json
+-rw-r--r--   0 runner    (1001) docker     (116)     6939 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/modular.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      577 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/nested_anyof.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      577 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/nested_oneof.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     2976 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/no_components.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/not.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2034 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/nullable.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     4813 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/oneof.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/pattern.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      144 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/refs.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1962 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/resolved_models.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      763 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/subclass_enum.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1050 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/openapi/x_enum_varnames.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.724874 datamodel-code-generator-0.9.4/tests/data/project/
+-rw-r--r--   0 runner    (1001) docker     (116)      408 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/project/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      260 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.724874 datamodel-code-generator-0.9.4/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (116)      567 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/python/space_and_special_characters_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.724874 datamodel-code-generator-0.9.4/tests/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (116)      420 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/templates/BaseModel.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.724874 datamodel-code-generator-0.9.4/tests/data/yaml/
+-rw-r--r--   0 runner    (1001) docker     (116)       25 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/data/yaml/pet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.724874 datamodel-code-generator-0.9.4/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.728875 datamodel-code-generator-0.9.4/tests/model/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/model/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5814 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/model/pydantic/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2333 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/model/pydantic/test_custom_root_type.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1958 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/model/pydantic/test_data_class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7634 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/model/pydantic/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8589 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/model/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:51.728875 datamodel-code-generator-0.9.4/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6969 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/parser/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13667 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/parser/test_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16469 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/parser/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (116)      850 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (116)    74926 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6584 2021-03-21 09:21:11.000000 datamodel-code-generator-0.9.4/tests/test_main_kr.py
```

### Comparing `datamodel-code-generator-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md` & `datamodel-code-generator-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md` & `datamodel-code-generator-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/.github/workflows/docs.yml` & `datamodel-code-generator-0.9.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/.github/workflows/publish.yml` & `datamodel-code-generator-0.9.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/.github/workflows/test.yml` & `datamodel-code-generator-0.9.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/.gitignore` & `datamodel-code-generator-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/CODE_OF_CONDUCT.md` & `datamodel-code-generator-0.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/LICENSE` & `datamodel-code-generator-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/PKG-INFO` & `datamodel-code-generator-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodel-code-generator
-Version: 0.9.3
+Version: 0.9.4
 Summary: Datamodel Code Generator
 Home-page: https://github.com/koxudaxi/datamodel-code-generator
 Author: Koudai Aono
 Author-email: koxudaxi@gmail.com
 License: UNKNOWN
 Description: # datamodel-code-generator
```

### Comparing `datamodel-code-generator-0.9.3/README.md` & `datamodel-code-generator-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/__init__.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,15 @@
     enum_field_as_literal: Optional[LiteralType] = None,
     set_default_enum_member: bool = False,
     strict_nullable: bool = False,
     use_generic_container_types: bool = False,
     enable_faux_immutability: bool = False,
     disable_appending_item_suffix: bool = False,
     strict_types: Optional[Sequence[StrictTypes]] = None,
+    empty_enum_field_name: Optional[str] = None,
 ) -> None:
     remote_text_cache: DefaultPutDict[str, str] = DefaultPutDict()
     if isinstance(input_, str):
         input_text: Optional[str] = input_
     elif isinstance(input_, ParseResult):
         from .http import get_body
 
@@ -301,14 +302,15 @@
         set_default_enum_member=set_default_enum_member,
         strict_nullable=strict_nullable,
         use_generic_container_types=use_generic_container_types,
         enable_faux_immutability=enable_faux_immutability,
         remote_text_cache=remote_text_cache,
         disable_appending_item_suffix=disable_appending_item_suffix,
         strict_types=strict_types,
+        empty_enum_field_name=empty_enum_field_name,
     )
 
     with chdir(output):
         results = parser.parse()
     if not input_filename:  # pragma: no cover
         if isinstance(input_, str):
             input_filename = '<stdin>'
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/__main__.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,14 +184,21 @@
     '--set-default-enum-member',
     help='Set enum members as default values for enum field',
     action='store_true',
     default=None,
 )
 
 arg_parser.add_argument(
+    '--empty-enum-field-name',
+    help='Set field name when enum value is empty (default:  `_`)',
+    default=None,
+)
+
+
+arg_parser.add_argument(
     '--class-name', help='Set class name of root model', default=None,
 )
 
 arg_parser.add_argument(
     '--custom-template-dir', help='Custom template directory', type=str
 )
 arg_parser.add_argument(
@@ -246,25 +253,14 @@
         elif value is None:  # pragma: no cover
             return None
         raise Error(
             f'This protocol doesn\'t support only http/https. --input={value}'
         )  # pragma: no cover
 
     @root_validator
-    def validate_literal_option(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        if values.get('enum_field_as_literal'):
-            target_python_version: PythonVersion = values['target_python_version']
-            if not target_python_version.has_literal_type:
-                raise Error(
-                    f"`--enum-field-as-literal` isn't compatible with `--target-python-version {target_python_version.value}`.\n"  # type: ignore
-                    f"You have to set `--target-python-version {target_python_version.PY_38.value}` or later version."
-                )
-        return values
-
-    @root_validator
     def validate_use_generic_container_types(
         cls, values: Dict[str, Any]
     ) -> Dict[str, Any]:
         if values.get('use_generic_container_types'):
             target_python_version: PythonVersion = values['target_python_version']
             if target_python_version == target_python_version.PY_36:
                 raise Error(
@@ -299,14 +295,15 @@
     set_default_enum_member: bool = False
     strict_nullable: bool = False
     use_generic_container_types: bool = False
     enable_faux_immutability: bool = False
     url: Optional[ParseResult] = None
     disable_appending_item_suffix: bool = False
     strict_types: List[StrictTypes] = []
+    empty_enum_field_name: Optional[str] = None
 
     def merge_args(self, args: Namespace) -> None:
         for field_name in self.__fields__:
             arg = getattr(args, field_name)
             if arg is None:
                 continue
             setattr(self, field_name, arg)
@@ -418,14 +415,15 @@
             enum_field_as_literal=config.enum_field_as_literal,
             set_default_enum_member=config.set_default_enum_member,
             strict_nullable=config.strict_nullable,
             use_generic_container_types=config.use_generic_container_types,
             enable_faux_immutability=config.enable_faux_immutability,
             disable_appending_item_suffix=config.disable_appending_item_suffix,
             strict_types=config.strict_types,
+            empty_enum_field_name=config.empty_enum_field_name,
         )
         return Exit.OK
     except InvalidClassNameError as e:
         print(f'{e} You have to set `--class-name` option', file=sys.stderr)
         return Exit.ERROR
     except Error as e:
         print(str(e), file=sys.stderr)
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/api.yaml` & `datamodel-code-generator-0.9.4/datamodel_code_generator/api.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/format.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/format.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/imports.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 
 IMPORT_ANY = Import.from_full_path('typing.Any')
 IMPORT_LIST = Import.from_full_path('typing.List')
 IMPORT_UNION = Import.from_full_path('typing.Union')
 IMPORT_OPTIONAL = Import.from_full_path('typing.Optional')
 IMPORT_LITERAL = Import.from_full_path('typing.Literal')
+IMPORT_LITERAL_BACKPORT = Import.from_full_path('typing_extensions.Literal')
 IMPORT_SEQUENCE = Import.from_full_path('typing.Sequence')
 IMPORT_MAPPING = Import.from_full_path('typing.Mapping')
 IMPORT_ABC_SEQUENCE = Import.from_full_path('collections.abc.Sequence')
 IMPORT_ABC_MAPPING = Import.from_full_path('collections.abc.Mapping')
 IMPORT_ENUM = Import.from_full_path('enum.Enum')
 IMPORT_ANNOTATIONS = Import.from_full_path('__future__.annotations')
 IMPORT_DICT = Import.from_full_path('typing.Dict')
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/base.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/base.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/enum.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/enum.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/__init__.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/base_model.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/imports.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/imports.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/pydantic/types.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/BaseModel.jinja2` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/BaseModel.jinja2`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/BaseModel_root.jinja2` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/BaseModel_root.jinja2`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/model/template/pydantic/dataclass.jinja2` & `datamodel-code-generator-0.9.4/datamodel_code_generator/model/template/pydantic/dataclass.jinja2`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/parser/__init__.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/parser/base.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/parser/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,26 @@
 from ..reference import ModelResolver, Reference
 from ..types import DataType, DataTypeManager, StrictTypes
 from . import DefaultPutDict, LiteralType
 
 _UNDER_SCORE_1: Pattern[str] = re.compile(r'(.)([A-Z][a-z]+)')
 _UNDER_SCORE_2: Pattern[str] = re.compile('([a-z0-9])([A-Z])')
 
+escape_characters = str.maketrans(
+    {
+        "\\": r"\\",
+        "'": r"\'",
+        '\b': r'\b',
+        '\f': r'\f',
+        '\n': r'\n',
+        '\r': r'\r',
+        '\t': r'\t',
+    }
+)
+
 
 @lru_cache()
 def camel_to_snake(string: str) -> str:
     subbed = _UNDER_SCORE_1.sub(r'\1_\2', string)
     return _UNDER_SCORE_2.sub(r'\1_\2', subbed).lower()
 
 
@@ -248,14 +260,15 @@
         set_default_enum_member: bool = False,
         strict_nullable: bool = False,
         use_generic_container_types: bool = False,
         enable_faux_immutability: bool = False,
         remote_text_cache: Optional[DefaultPutDict[str, str]] = None,
         disable_appending_item_suffix: bool = False,
         strict_types: Optional[Sequence[StrictTypes]] = None,
+        empty_enum_field_name: Optional[str] = None,
     ):
         self.data_type_manager: DataTypeManager = data_type_manager_type(
             target_python_version,
             use_standard_collections,
             use_generic_container_types,
             strict_types,
         )
@@ -314,14 +327,15 @@
         if enable_faux_immutability:
             self.extra_template_data[ALL_MODEL]['allow_mutation'] = False
 
         self.model_resolver = ModelResolver(
             aliases=aliases,
             base_url=source.geturl() if isinstance(source, ParseResult) else None,
             singular_name_suffix='' if disable_appending_item_suffix else None,
+            empty_field_name=empty_enum_field_name,
         )
         self.field_preprocessors: List[
             Callable[[DataModelFieldBase, DataModel], None]
         ] = []
         if self.snake_case_field:
             self.field_preprocessors.append(snakify_field)
         if self.strip_default_none:
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/parser/jsonschema.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/parser/jsonschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 )
 from datamodel_code_generator.format import PythonVersion
 from datamodel_code_generator.model import DataModel, DataModelFieldBase
 from datamodel_code_generator.model.enum import Enum
 from datamodel_code_generator.parser import DefaultPutDict, LiteralType
 
 from ..model import pydantic as pydantic_model
-from ..parser.base import Parser
+from ..parser.base import Parser, escape_characters
 from ..reference import Reference, is_url
 from ..types import DataType, DataTypeManager, StrictTypes, Types
 
 
 def get_model_by_path(schema: Dict[str, Any], keys: List[str]) -> Dict[str, Any]:
     if not keys:
         return schema
@@ -257,14 +257,15 @@
         set_default_enum_member: bool = False,
         strict_nullable: bool = False,
         use_generic_container_types: bool = False,
         enable_faux_immutability: bool = False,
         remote_text_cache: Optional[DefaultPutDict[str, str]] = None,
         disable_appending_item_suffix: bool = False,
         strict_types: Optional[Sequence[StrictTypes]] = None,
+        empty_enum_field_name: Optional[str] = None,
     ):
         super().__init__(
             source=source,
             data_model_type=data_model_type,
             data_model_root_type=data_model_root_type,
             data_type_manager_type=data_type_manager_type,
             data_model_field_type=data_model_field_type,
@@ -291,14 +292,15 @@
             set_default_enum_member=set_default_enum_member,
             strict_nullable=strict_nullable,
             use_generic_container_types=use_generic_container_types,
             enable_faux_immutability=enable_faux_immutability,
             remote_text_cache=remote_text_cache,
             disable_appending_item_suffix=disable_appending_item_suffix,
             strict_types=strict_types,
+            empty_enum_field_name=empty_enum_field_name,
         )
 
         self.remote_object_cache: DefaultPutDict[str, Dict[str, Any]] = DefaultPutDict()
         self.raw_obj: Dict[Any, Any] = {}
         self._root_id: Optional[str] = None
         self._root_id_base_path: Optional[str] = None
         self.reserved_refs: DefaultDict[Tuple[str], Set[str]] = defaultdict(set)
@@ -516,15 +518,15 @@
                             else field,
                         )
                     elif field.additionalProperties.enum:
                         if self.should_parse_enum_as_literal(
                             field.additionalProperties
                         ):
                             additional_properties_type = self.data_type(
-                                literals=field.additionalProperties.enum
+                                literals=field.additionalProperties.enum,
                             )
                         else:
                             additional_properties_type = self.parse_enum(
                                 field_class_name,
                                 field.additionalProperties,
                                 [*path, field_name],
                             )
@@ -787,40 +789,50 @@
                 f'This argument will be removed in a future version'
             )
         enum_fields: List[DataModelFieldBase] = []
 
         if None in obj.enum and obj.type == 'string':
             # Nullable is valid in only OpenAPI
             nullable: bool = True
-            enum_times = [e for e in obj.enum if e]
+            enum_times = [e for e in obj.enum if e is not None]
         else:
             enum_times = obj.enum
             nullable = False
 
+        exclude_field_names: Set[str] = set()
+
         for i, enum_part in enumerate(enum_times):
             if obj.type == 'string' or isinstance(enum_part, str):
-                default = f"'{enum_part}'"
+                default = (
+                    f"'{enum_part.translate(escape_characters)}'"
+                    if isinstance(enum_part, str)
+                    else enum_part
+                )
                 if obj.x_enum_varnames:
                     field_name = obj.x_enum_varnames[i]
                 else:
-                    field_name = enum_part
+                    field_name = str(enum_part)
             else:
                 default = enum_part
                 if obj.x_enum_varnames:
                     field_name = obj.x_enum_varnames[i]
                 else:
                     prefix = (
                         obj.type
                         if isinstance(obj.type, str)
                         else type(enum_part).__name__
                     )
                     field_name = f'{prefix}_{enum_part}'
+            field_name = self.model_resolver.get_valid_name(
+                field_name, excludes=exclude_field_names
+            )
+            exclude_field_names.add(field_name)
             enum_fields.append(
                 self.data_model_field_type(
-                    name=self.model_resolver.get_valid_name(field_name),
+                    name=field_name,
                     default=default,
                     data_type=self.data_type_manager.get_data_type(Types.any),
                     required=True,
                 )
             )
 
         if not nullable:
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/parser/openapi.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/parser/openapi.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/reference.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,27 +115,29 @@
     def __init__(
         self,
         aliases: Optional[Mapping[str, str]] = None,
         exclude_names: Set[str] = None,
         duplicate_name_suffix: Optional[str] = None,
         base_url: Optional[str] = None,
         singular_name_suffix: Optional[str] = None,
+        empty_field_name: Optional[str] = None,
     ) -> None:
         self.references: Dict[str, Reference] = {}
         self.aliases: Mapping[str, str] = {} if aliases is None else {**aliases}
         self._current_root: Sequence[str] = []
         self._root_id_base_path: Optional[str] = None
         self.ids: DefaultDict[str, Dict[str, str]] = defaultdict(dict)
         self.after_load_files: Set[str] = set()
         self.exclude_names: Set[str] = exclude_names or set()
         self.duplicate_name_suffix: Optional[str] = duplicate_name_suffix
         self._base_url: Optional[str] = base_url
         self.singular_name_suffix: str = singular_name_suffix if isinstance(
             singular_name_suffix, str
         ) else SINGULAR_NAME_SUFFIX
+        self.empty_field_name: str = empty_field_name or '_'
 
     @property
     def base_url(self) -> Optional[str]:
         return self._base_url
 
     def set_base_url(self, base_url: Optional[str]) -> None:
         self._base_url = base_url
@@ -349,27 +351,35 @@
             count += 1
         return uniq_name
 
     @classmethod
     def validate_name(cls, name: str) -> bool:
         return name.isidentifier() and not iskeyword(name)
 
-    @lru_cache()
-    def get_valid_name(self, name: str, camel: bool = False) -> str:
-        if name.isidentifier():
-            return name
+    def get_valid_name(
+        self, name: str, camel: bool = False, excludes: Optional[Set[str]] = None
+    ) -> str:
+        if not name:
+            name = self.empty_field_name
         if name[0] == '#':
             name = name[1:]
         # TODO: when first character is a number
-        replaced_name = re.sub(r'\W', '_', name)
-        if replaced_name[0].isnumeric():
-            replaced_name = f'field_{replaced_name}'
-        # if replaced_name.isidentifier() and not iskeyword(replaced_name):
-        # return self.get_uniq_name(replaced_name, camel)
-        return replaced_name
+        name = re.sub(r'\W', '_', name)
+        if name[0].isnumeric():
+            name = f'field_{name}'
+        count = 1
+        new_name = name
+        while (
+            not new_name.isidentifier()
+            and iskeyword(new_name)
+            or (excludes and new_name in excludes)
+        ):
+            new_name = f'{name}_{count}'
+            count += 1
+        return new_name
 
     def get_valid_field_name_and_alias(
         self, field_name: str
     ) -> Tuple[str, Optional[str]]:
         if field_name in self.aliases:
             return self.aliases[field_name], field_name
         valid_name = self.get_valid_name(field_name)
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator/types.py` & `datamodel-code-generator-0.9.4/datamodel_code_generator/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from itertools import chain
 from typing import (
+    TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
     FrozenSet,
     Iterable,
     Iterator,
     List,
@@ -13,21 +14,24 @@
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
 )
 
+from pydantic import create_model
+
 from datamodel_code_generator.format import PythonVersion
 from datamodel_code_generator.imports import (
     IMPORT_ABC_MAPPING,
     IMPORT_ABC_SEQUENCE,
     IMPORT_DICT,
     IMPORT_LIST,
     IMPORT_LITERAL,
+    IMPORT_LITERAL_BACKPORT,
     IMPORT_MAPPING,
     IMPORT_OPTIONAL,
     IMPORT_SEQUENCE,
     IMPORT_UNION,
     Import,
 )
 from datamodel_code_generator.reference import Reference, _BaseModel
@@ -152,16 +156,26 @@
                         if not (t.type == 'Any' and t.is_optional)
                     ]
                 break
 
         imports: Tuple[Tuple[bool, Import], ...] = (
             (self.is_optional, IMPORT_OPTIONAL),
             (len(self.data_types) > 1, IMPORT_UNION),
-            (any(self.literals), IMPORT_LITERAL),
         )
+        if any(self.literals):
+            import_literal = (
+                IMPORT_LITERAL
+                if self.python_version.has_literal_type
+                else IMPORT_LITERAL_BACKPORT
+            )
+            imports = (
+                *imports,
+                (any(self.literals), import_literal),
+            )
+
         if self.use_generic_container:
             if self.use_standard_collections:
                 imports = (
                     *imports,
                     (self.is_list, IMPORT_ABC_SEQUENCE),
                     (self.is_dict, IMPORT_ABC_MAPPING),
                 )
@@ -234,31 +248,14 @@
             return f'{type_}()'
         return type_
 
 
 DataType.update_forward_refs()
 
 
-class DataTypePy36(DataType):
-    python_version: PythonVersion = PythonVersion.PY_36
-
-
-class DataTypeStandardCollections(DataType):
-    use_standard_collections: bool = True
-
-
-class DataTypeGenericContainer(DataType):
-    use_generic_container: bool = True
-
-
-class DataTypeGenericContainerStandardCollections(DataType):
-    use_standard_collections: bool = True
-    use_generic_container: bool = True
-
-
 class Types(Enum):
     integer = auto()
     int32 = auto()
     int64 = auto()
     number = auto()
     float = auto()
     double = auto()
@@ -297,28 +294,29 @@
         strict_types: Optional[Sequence[StrictTypes]] = None,
     ) -> None:
         self.python_version = python_version
         self.use_standard_collections: bool = use_standard_collections
         self.use_generic_container_types: bool = use_generic_container_types
         self.strict_types: Sequence[StrictTypes] = strict_types or ()
 
-        self.data_type: Type[DataType]
-        if use_generic_container_types:
-            if python_version == PythonVersion.PY_36:  # pragma: no cover
-                raise Exception(
-                    "use_generic_container_types can not be used with target_python_version 3.6.\n"
-                    " The version will be not supported in a future version"
-                )
-            if use_standard_collections:
-                self.data_type = DataTypeGenericContainerStandardCollections
-            else:
-                self.data_type = DataTypeGenericContainer
-        elif use_standard_collections:
-            self.data_type = DataTypeStandardCollections
-        elif python_version == PythonVersion.PY_36:
-            self.data_type = DataTypePy36
+        if (
+            use_generic_container_types and python_version == PythonVersion.PY_36
+        ):  # pragma: no cover
+            raise Exception(
+                "use_generic_container_types can not be used with target_python_version 3.6.\n"
+                " The version will be not supported in a future version"
+            )
+
+        if TYPE_CHECKING:
+            self.data_type: Type[DataType]
         else:
-            self.data_type = DataType
+            self.data_type: Type[DataType] = create_model(
+                'ContextDataType',
+                python_version=python_version,
+                use_standard_collections=use_standard_collections,
+                use_generic_container=use_generic_container_types,
+                __base__=DataType,
+            )
 
     @abstractmethod
     def get_data_type(self, types: Types, **kwargs: Any) -> DataType:
         raise NotImplementedError
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/PKG-INFO` & `datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamodel-code-generator
-Version: 0.9.3
+Version: 0.9.4
 Summary: Datamodel Code Generator
 Home-page: https://github.com/koxudaxi/datamodel-code-generator
 Author: Koudai Aono
 Author-email: koxudaxi@gmail.com
 License: UNKNOWN
 Description: # datamodel-code-generator
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/SOURCES.txt` & `datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,16 @@
 tests/data/expected/main/main_jsonschema_ids/id.py
 tests/data/expected/main/main_jsonschema_ids/name.py
 tests/data/expected/main/main_jsonschema_ids/sameAs.py
 tests/data/expected/main/main_jsonschema_ids/type.py
 tests/data/expected/main/main_jsonschema_nested_deep/__init__.py
 tests/data/expected/main/main_jsonschema_nested_deep/empty_parent/nested/deep.py
 tests/data/expected/main/main_jsonschema_nested_deep/nested/deep.py
+tests/data/expected/main/main_jsonschema_special_enum/output.py
+tests/data/expected/main/main_jsonschema_special_enum_empty_enum_field_name/output.py
 tests/data/expected/main/main_modular/__init__.py
 tests/data/expected/main/main_modular/bar.py
 tests/data/expected/main/main_modular/collections.py
 tests/data/expected/main/main_modular/models.py
 tests/data/expected/main/main_modular/foo/__init__.py
 tests/data/expected/main/main_modular/foo/bar.py
 tests/data/expected/main/main_modular/nested/__init__.py
@@ -137,14 +139,15 @@
 tests/data/expected/main/main_nested_directory/definitions/drink/coffee.py
 tests/data/expected/main/main_nested_directory/definitions/drink/tea.py
 tests/data/expected/main/main_nested_json_pointer/output.py
 tests/data/expected/main/main_no_file/output.py
 tests/data/expected/main/main_null_and_array/output.py
 tests/data/expected/main/main_openapi_datetime/output.py
 tests/data/expected/main/main_openapi_enum_models_all/output.py
+tests/data/expected/main/main_openapi_enum_models_as_literal_py37/output.py
 tests/data/expected/main/main_openapi_enum_models_one/output.py
 tests/data/expected/main/main_openapi_http_refs/output.py
 tests/data/expected/main/main_openapi_nullable/output.py
 tests/data/expected/main/main_openapi_nullable_strict_nullable/output.py
 tests/data/expected/main/main_pattern/output.py
 tests/data/expected/main/main_root_id/output.py
 tests/data/expected/main/main_root_model_with_additional_properties/output.py
@@ -297,14 +300,15 @@
 tests/data/jsonschema/oneof.json.snapshot
 tests/data/jsonschema/pattern.json
 tests/data/jsonschema/person.json
 tests/data/jsonschema/root_id.json
 tests/data/jsonschema/root_model_with_additional_properties.json
 tests/data/jsonschema/self_reference.json
 tests/data/jsonschema/similar_nested_array.json
+tests/data/jsonschema/special_enum.json
 tests/data/jsonschema/strict_types.json
 tests/data/jsonschema/user.json
 tests/data/jsonschema/all_of_ref/base_test.json
 tests/data/jsonschema/all_of_ref/test.json
 tests/data/jsonschema/external_files_in_directory/person.json
 tests/data/jsonschema/external_files_in_directory/definitions/food.json
 tests/data/jsonschema/external_files_in_directory/definitions/friends.json
```

### Comparing `datamodel-code-generator-0.9.3/datamodel_code_generator.egg-info/requires.txt` & `datamodel-code-generator-0.9.4/datamodel_code_generator.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 argcomplete<2.0,>=1.10
 prance<1.0,>=0.18.2
-openapi-spec-validator<0.3,>=0.2.8
+openapi-spec-validator<0.4,>=0.2.8
 jinja2<3.0,>=2.10.1
-inflect<5.0,>=4.1.0
+inflect<6.0,>=4.1.0
 black>=19.10b0
 isort<6.0,>=4.3.21
 PySnooper<1.0.0,>=0.4.1
 toml<1.0.0,>=0.10.0
 genson<2.0,>=1.2.1
 
 [:python_version < "3.9"]
```

### Comparing `datamodel-code-generator-0.9.3/docs/development-contributing.md` & `datamodel-code-generator-0.9.4/docs/development-contributing.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/field-constraints.md` & `datamodel-code-generator-0.9.4/docs/field-constraints.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/formatting.md` & `datamodel-code-generator-0.9.4/docs/formatting.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/index.md` & `datamodel-code-generator-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/jsondata.md` & `datamodel-code-generator-0.9.4/docs/jsondata.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/jsonschema.md` & `datamodel-code-generator-0.9.4/docs/jsonschema.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/openapi.md` & `datamodel-code-generator-0.9.4/docs/openapi.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/support-data-types.md` & `datamodel-code-generator-0.9.4/docs/support-data-types.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/docs/using_as_module.md` & `datamodel-code-generator-0.9.4/docs/using_as_module.md`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/mkdocs.yml` & `datamodel-code-generator-0.9.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/setup.cfg` & `datamodel-code-generator-0.9.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 zip_safe = True
 setup_requires = 
 	pytest-runner
 	setuptools-scm
 install_requires = 
 	argcomplete>=1.10,<2.0
 	prance>=0.18.2,<1.0
-	openapi-spec-validator>=0.2.8,<0.3
+	openapi-spec-validator>=0.2.8,<0.4
 	jinja2>=2.10.1,<3.0
-	inflect>=4.1.0,<5.0
+	inflect>=4.1.0,<6.0
 	pydantic[email]>=1.5.1,<2.0;python_version<'3.9'
 	pydantic[email]>=1.7.2,<2.0;python_version>='3.9'
 	black>=19.10b0
 	isort>=4.3.21,<6.0
 	PySnooper>=0.4.1,<1.0.0
 	toml>=0.10.0,<1.0.0
 	genson>=1.2.1,<2.0
```

### Comparing `datamodel-code-generator-0.9.3/setup.py` & `datamodel-code-generator-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/allow_population_by_field_name/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/allow_population_by_field_name/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/disable_timestamp/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/disable_timestamp/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/enable_faux_immutability/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/enable_faux_immutability/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/force_optional/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/force_optional/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_autodetect/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_autodetect/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_base_class/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_base_class/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_circular_reference/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_circular_reference/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_complicated_enum_default_member/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_complicated_enum_default_member/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_custom_template_dir/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_custom_template_dir/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_disable_appending_item_suffix/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_disable_appending_item_suffix/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_external_files_in_directory/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_external_files_in_directory/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_invalid_model_name/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_invalid_model_name/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_pointer/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_pointer/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_json_reuse_model/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_json_reuse_model/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/name.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/name.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_jsonschema_ids/sameAs.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_jsonschema_ids/sameAs.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/collections.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/collections.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/models.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/models.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular/nested/foo.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular/nested/foo.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/collections.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/collections.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/models.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/models.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_modular_reuse_model/nested/foo.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_modular_reuse_model/nested/foo.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/definitions/friends.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/definitions/friends.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_directory/person.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_directory/person.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_nested_json_pointer/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_nested_json_pointer/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_no_file/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_no_file/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_enum_models_all/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_all/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_enum_models_one/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_enum_models_one/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_http_refs/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_http_refs/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_nullable/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_nullable/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_openapi_nullable_strict_nullable/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_openapi_nullable_strict_nullable/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_pattern/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_pattern/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_id/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_id/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_literal/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_literal/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_use_generic_container_types/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_use_generic_container_types/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_root_model_with_additional_properties_use_standard_collections/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_root_model_with_additional_properties_use_standard_collections/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_similar_nested_array/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_similar_nested_array/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types_all/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types_all/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_strict_types_all_field_constraints/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_strict_types_all_field_constraints/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/collections.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/collections.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/models.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/models.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types/nested/foo.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types/nested/foo.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/collections.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/collections.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/models.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/models.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/foo.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_generic_container_types_standard_collections/nested/foo.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/collections.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/collections.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/models.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/models.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_use_standard_collections/nested/foo.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_use_standard_collections/nested/foo.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_aliases/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_aliases/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_exclusive/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_exclusive/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_field_constraints/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_field_constraints/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_snake_case_field/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_snake_case_field/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_with_strip_default_none/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_with_strip_default_none/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/main_without_field_constraints/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/main_without_field_constraints/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/multiple_files_json_pointer/file_b.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/multiple_files_json_pointer/file_b.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/pyproject/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/pyproject/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/pyproject_not_found/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/pyproject_not_found/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/space_and_special_characters/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/space_and_special_characters/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/space_and_special_characters_dict/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/space_and_special_characters_dict/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/stdin/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/stdin/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/target_python_version/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/target_python_version/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/use_default/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/use_default/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main/validation/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main/validation/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_base_class/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_base_class/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_custom_template_dir/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_custom_template_dir/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/collections.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/collections.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/models.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/models.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_modular/nested/foo.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_modular/nested/foo.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_no_file/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_no_file/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/main_use_schema_description/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/main_use_schema_description/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/pyproject/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/pyproject/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/main_kr/target_python_version/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/main_kr/target_python_version/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/format.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/format.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/with_import.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/with_import.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format_custom_module.Base.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse/with_import_format_custom_module.Base.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/format.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/format.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format_custom_module.Base.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_additional_properties/with_import_format_custom_module.Base.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/collection_s.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/collection_s.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_alias/model_s.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_alias/model_s.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_allof/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_allof/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_anyof/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_anyof/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_duplicate_models/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_duplicate_models/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py36.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py36.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py37.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_enum_models/output_py37.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/__init__.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/__init__.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/collections.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/collections.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/models.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/models.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/foo.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_modular/nested/foo.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/expected/parser/openapi/openapi_parser_parse_oneof/output.py` & `datamodel-code-generator-0.9.4/tests/data/expected/parser/openapi/openapi_parser_parse_oneof/output.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/json/space_and_special_characters.json` & `datamodel-code-generator-0.9.4/tests/data/json/space_and_special_characters.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/circular_reference.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/circular_reference.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/complicated_enum.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/complicated_enum.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/definitions/friends.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/definitions/friends.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/external_files_in_directory/person.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/external_files_in_directory/person.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/external_parent.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/external_parent.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/id.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/id.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/ContactPoint.schema.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/ContactPoint.schema.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/ids/Organization.schema.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/ids/Organization.schema.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/invalid_model_name.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/invalid_model_name.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/json_pointer.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/json_pointer.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_json_pointer/file_a.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_json_pointer/file_a.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_json_pointer/file_b.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_json_pointer/file_b.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/multiple_files_json_pointer/file_c.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/multiple_files_json_pointer/file_c.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/nested_array.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/nested_array.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/nested_json_pointer.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/nested_json_pointer.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/nested_person.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/nested_person.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/null_and_array.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/null_and_array.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/pattern.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/pattern.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/person.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/person.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/root_model_with_additional_properties.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/root_model_with_additional_properties.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/similar_nested_array.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/similar_nested_array.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/jsonschema/strict_types.json` & `datamodel-code-generator-0.9.4/tests/data/jsonschema/strict_types.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/additional_properties.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/additional_properties.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/alias.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/alias.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/allof.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/allof.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/any.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/any.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/anyof.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/anyof.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/api.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/api.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/api_constrained.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/api_constrained.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/definitions.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/definitions.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/duplicate_models.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/duplicate_models.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/enum_models.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/enum_models.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/example.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/example.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/exclusive.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/exclusive.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/lazy_resolved_models.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/lazy_resolved_models.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/modular.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/modular.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/nested_anyof.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/nested_anyof.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/nested_oneof.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/nested_oneof.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/no_components.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/no_components.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/nullable.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/nullable.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/oneof.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/oneof.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/pattern.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/pattern.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/resolved_models.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/resolved_models.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/subclass_enum.json` & `datamodel-code-generator-0.9.4/tests/data/openapi/subclass_enum.json`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/openapi/x_enum_varnames.yaml` & `datamodel-code-generator-0.9.4/tests/data/openapi/x_enum_varnames.yaml`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/data/python/space_and_special_characters_dict.py` & `datamodel-code-generator-0.9.4/tests/data/python/space_and_special_characters_dict.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/model/pydantic/test_base_model.py` & `datamodel-code-generator-0.9.4/tests/model/pydantic/test_base_model.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/model/pydantic/test_custom_root_type.py` & `datamodel-code-generator-0.9.4/tests/model/pydantic/test_custom_root_type.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/model/pydantic/test_data_class.py` & `datamodel-code-generator-0.9.4/tests/model/pydantic/test_data_class.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/model/pydantic/test_types.py` & `datamodel-code-generator-0.9.4/tests/model/pydantic/test_types.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/model/test_base.py` & `datamodel-code-generator-0.9.4/tests/model/test_base.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/parser/test_base.py` & `datamodel-code-generator-0.9.4/tests/parser/test_base.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/parser/test_jsonschema.py` & `datamodel-code-generator-0.9.4/tests/parser/test_jsonschema.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/parser/test_openapi.py` & `datamodel-code-generator-0.9.4/tests/parser/test_openapi.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/test_imports.py` & `datamodel-code-generator-0.9.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `datamodel-code-generator-0.9.3/tests/test_main.py` & `datamodel-code-generator-0.9.4/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1757,21 +1757,25 @@
                 '--input-file-type',
                 'openapi',
                 '--enum-field-as-literal',
                 'all',
             ]
         )
 
-        captured = capsys.readouterr()
-        assert return_code == Exit.ERROR
+        assert return_code == Exit.OK
         assert (
-            captured.err
-            == "`--enum-field-as-literal` isn't compatible with `--target-python-version 3.7`.\n"
-            "You have to set `--target-python-version 3.8` or later version.\n"
+            output_file.read_text()
+            == (
+                EXPECTED_MAIN_PATH
+                / 'main_openapi_enum_models_as_literal_py37'
+                / 'output.py'
+            ).read_text()
         )
+    with pytest.raises(SystemExit):
+        main()
 
 
 @freeze_time('2019-07-26')
 def test_main_root_model_with_additional_properties():
     with TemporaryDirectory() as output_dir:
         output_file: Path = Path(output_dir) / 'output.py'
         return_code: Exit = main(
@@ -2370,7 +2374,61 @@
                 EXPECTED_MAIN_PATH
                 / 'main_strict_types_all_field_constraints'
                 / 'output.py'
             ).read_text()
         )
     with pytest.raises(SystemExit):
         main()
+
+
+@freeze_time('2019-07-26')
+def test_main_jsonschema_special_enum():
+    with TemporaryDirectory() as output_dir:
+        output_file: Path = Path(output_dir) / 'output.py'
+        return_code: Exit = main(
+            [
+                '--input',
+                str(JSON_SCHEMA_DATA_PATH / 'special_enum.json'),
+                '--output',
+                str(output_file),
+                '--input-file-type',
+                'jsonschema',
+            ]
+        )
+        assert return_code == Exit.OK
+        assert (
+            output_file.read_text()
+            == (
+                EXPECTED_MAIN_PATH / 'main_jsonschema_special_enum' / 'output.py'
+            ).read_text()
+        )
+    with pytest.raises(SystemExit):
+        main()
+
+
+@freeze_time('2019-07-26')
+def test_main_jsonschema_special_enum_empty_enum_field_name():
+    with TemporaryDirectory() as output_dir:
+        output_file: Path = Path(output_dir) / 'output.py'
+        return_code: Exit = main(
+            [
+                '--input',
+                str(JSON_SCHEMA_DATA_PATH / 'special_enum.json'),
+                '--output',
+                str(output_file),
+                '--input-file-type',
+                'jsonschema',
+                '--empty-enum-field-name',
+                'empty',
+            ]
+        )
+        assert return_code == Exit.OK
+        assert (
+            output_file.read_text()
+            == (
+                EXPECTED_MAIN_PATH
+                / 'main_jsonschema_special_enum_empty_enum_field_name'
+                / 'output.py'
+            ).read_text()
+        )
+    with pytest.raises(SystemExit):
+        main()
```

### Comparing `datamodel-code-generator-0.9.3/tests/test_main_kr.py` & `datamodel-code-generator-0.9.4/tests/test_main_kr.py`

 * *Files identical despite different names*

