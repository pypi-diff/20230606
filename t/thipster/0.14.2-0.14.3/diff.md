# Comparing `tmp/thipster-0.14.2.tar.gz` & `tmp/thipster-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.14.2.tar", last modified: Tue Jun  6 14:16:28 2023, max compression
+gzip compressed data, was "thipster-0.14.3.tar", last modified: Tue Jun  6 15:24:31 2023, max compression
```

## Comparing `thipster-0.14.2.tar` & `thipster-0.14.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-06 14:16:25.000000 thipster-0.14.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-06 14:16:25.000000 thipster-0.14.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-06 14:16:28.663005 thipster-0.14.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3390 2023-06-06 14:16:25.000000 thipster-0.14.2/README.md
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-06 14:16:25.000000 thipster-0.14.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-06 14:16:25.000000 thipster-0.14.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 14:16:28.663005 thipster-0.14.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-06 14:16:25.000000 thipster-0.14.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15549 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6934 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4178 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13710 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17262 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19125 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6276 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15624 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.199558 thipster-0.14.3/
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-06 15:24:28.000000 thipster-0.14.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-06 15:24:28.000000 thipster-0.14.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-06 15:24:31.199558 thipster-0.14.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-06-06 15:24:28.000000 thipster-0.14.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-06 15:24:28.000000 thipster-0.14.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-06 15:24:28.000000 thipster-0.14.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 15:24:31.199558 thipster-0.14.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-06 15:24:28.000000 thipster-0.14.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.195557 thipster-0.14.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.195557 thipster-0.14.3/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.195557 thipster-0.14.3/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.195557 thipster-0.14.3/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15549 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6934 2023-06-06 15:24:28.000000 thipster-0.14.3/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.195557 thipster-0.14.3/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.195557 thipster-0.14.3/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.199558 thipster-0.14.3/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.199558 thipster-0.14.3/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.199558 thipster-0.14.3/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13710 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17262 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19125 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6276 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.199558 thipster-0.14.3/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.199558 thipster-0.14.3/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15624 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-06-06 15:24:28.000000 thipster-0.14.3/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:24:31.195557 thipster-0.14.3/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-06 15:24:31.000000 thipster-0.14.3/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-06 15:24:31.000000 thipster-0.14.3/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:24:31.000000 thipster-0.14.3/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-06 15:24:31.000000 thipster-0.14.3/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-06 15:24:31.000000 thipster-0.14.3/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.14.2/LICENSE` & `thipster-0.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/PKG-INFO` & `thipster-0.14.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.2
+Version: 0.14.3
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.14.2/README.md` & `thipster-0.14.3/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/pyproject.toml` & `thipster-0.14.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/setup.py` & `thipster-0.14.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.14.2'
+__version__ = '0.14.3'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md") as rm:
     readme = rm.read()
```

### Comparing `thipster-0.14.2/tests/engine/test_engine.py` & `thipster-0.14.3/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.14.3/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/dsl_parser/test_ast.py` & `thipster-0.14.3/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.14.3/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/dsl_parser/test_token.py` & `thipster-0.14.3/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.14.3/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/test_ParserFactory.py` & `thipster-0.14.3/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/test_YAMLParser.py` & `thipster-0.14.3/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/parser/test_parsedfile.py` & `thipster-0.14.3/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/tests/test_e2e.py` & `thipster-0.14.3/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/auth/google.py` & `thipster-0.14.3/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/engine/engine.py` & `thipster-0.14.3/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/engine/i_parser.py` & `thipster-0.14.3/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/engine/i_repository.py` & `thipster-0.14.3/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/engine/i_terraform.py` & `thipster-0.14.3/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/engine/parsed_file.py` & `thipster-0.14.3/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/engine/resource_model.py` & `thipster-0.14.3/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/ast.py` & `thipster-0.14.3/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.14.3/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.14.3/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/lexer.py` & `thipster-0.14.3/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.14.3/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/parser.py` & `thipster-0.14.3/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/token.py` & `thipster-0.14.3/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.14.3/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/parser_factory.py` & `thipster-0.14.3/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/parser/yaml_parser.py` & `thipster-0.14.3/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/repository/github.py` & `thipster-0.14.3/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/repository/json.py` & `thipster-0.14.3/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/terraform/cdk.py` & `thipster-0.14.3/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster/terraform/exceptions.py` & `thipster-0.14.3/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.2/thipster.egg-info/PKG-INFO` & `thipster-0.14.3/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.2
+Version: 0.14.3
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.14.2/thipster.egg-info/SOURCES.txt` & `thipster-0.14.3/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

