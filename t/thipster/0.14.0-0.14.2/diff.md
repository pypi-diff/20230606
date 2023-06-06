# Comparing `tmp/thipster-0.14.0.tar.gz` & `tmp/thipster-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.14.0.tar", last modified: Tue Jun  6 08:10:01 2023, max compression
+gzip compressed data, was "thipster-0.14.2.tar", last modified: Tue Jun  6 14:16:28 2023, max compression
```

## Comparing `thipster-0.14.0.tar` & `thipster-0.14.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-06 08:09:58.000000 thipster-0.14.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-06 08:09:58.000000 thipster-0.14.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3883 2023-06-06 08:10:01.380800 thipster-0.14.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3270 2023-06-06 08:09:58.000000 thipster-0.14.0/README.md
--rw-r--r--   0 root         (0) root         (0)      867 2023-06-06 08:09:58.000000 thipster-0.14.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-06 08:09:58.000000 thipster-0.14.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 08:10:01.380800 thipster-0.14.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-06 08:09:59.000000 thipster-0.14.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.372800 thipster-0.14.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.372800 thipster-0.14.0/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.372800 thipster-0.14.0/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13247 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/auth/Google.py
--rw-r--r--   0 root         (0) root         (0)      173 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)     3340 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/Engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Auth.py
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Parser.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Repository.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/ParsedFile.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/ResourceModel.py
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     6283 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)    10350 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/AST.py
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/DSLExceptions.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/DSLParser.py
--rw-r--r--   0 root         (0) root         (0)    13788 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/Interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17548 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/Lexer.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/LexerPosition.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/Token.py
--rw-r--r--   0 root         (0) root         (0)    20153 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/TokenParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/GithubRepo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/JSONRepo.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/LocalRepo.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)    12057 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/terraform/CDK.py
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/terraform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3883 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1637 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-06 14:16:25.000000 thipster-0.14.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-06 14:16:25.000000 thipster-0.14.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-06 14:16:28.663005 thipster-0.14.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-06-06 14:16:25.000000 thipster-0.14.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-06 14:16:25.000000 thipster-0.14.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-06 14:16:25.000000 thipster-0.14.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 14:16:28.663005 thipster-0.14.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-06 14:16:25.000000 thipster-0.14.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15549 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6934 2023-06-06 14:16:25.000000 thipster-0.14.2/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.655005 thipster-0.14.2/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13710 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17262 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19125 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6276 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.663005 thipster-0.14.2/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15624 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-06-06 14:16:25.000000 thipster-0.14.2/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 14:16:28.659005 thipster-0.14.2/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-06 14:16:28.000000 thipster-0.14.2/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.14.0/LICENSE` & `thipster-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.14.0/PKG-INFO` & `thipster-0.14.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.0
+Version: 0.14.2
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -19,15 +19,15 @@
 
 Written entirely in Python, it leverages the Python CDK for Terraform to create Terraform files and apply them to the chosen provider.
 
 ## Technology Stack
 Written in Python 3.11, thipster is designed as a python package, to be used either as a standalone tool, or as a module inside a running process like a CI/CD pipeline.
 
 ## Project Status
-THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](CHANGELOG.md) for more details.
+THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for more details.
 
 ## Dependencies
 
 In order to user THipster, you will need to have the following installed:
 - [Python](https://www.python.org/downloads/) (3.11+)
 - [pipenv](https://pipenv.pypa.io/en/latest/) v2021.5+
 - [Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) (1.2+)
@@ -89,20 +89,19 @@
 To install the project for development, you can use the following command:
 
 ```console
 pip install -r requirements.txt && pip install -e .[dev,test,doc]
 pre-commit install && pre-commit run --all-files
 ```
 
-For more information on how to help out, please check the [CONTRIBUTING](CONTRIBUTING.md) file.
+For more information on how to help out, please check the [CONTRIBUTING](https://github.com/THipster/THipster/blob/main/CONTRIBUTING.md) file.
 
 ## Open source licensing info
-1. [TERMS](TERMS.md)
-2. [LICENSE](LICENSE)
-3. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
+1. [LICENSE](https://github.com/THipster/THipster/blob/main/LICENSE)
+2. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
 
 ## Credits and references
 
 1. Projects that inspired you
     - [AWS Application Composer](https://aws.amazon.com/application-composer/?nc1=h_ls)
 2. Related projects
     - [Wing Programming Language](https://www.winglang.io/)
```

### Comparing `thipster-0.14.0/README.md` & `thipster-0.14.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Written entirely in Python, it leverages the Python CDK for Terraform to create Terraform files and apply them to the chosen provider.
 
 ## Technology Stack
 Written in Python 3.11, thipster is designed as a python package, to be used either as a standalone tool, or as a module inside a running process like a CI/CD pipeline.
 
 ## Project Status
-THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](CHANGELOG.md) for more details.
+THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for more details.
 
 ## Dependencies
 
 In order to user THipster, you will need to have the following installed:
 - [Python](https://www.python.org/downloads/) (3.11+)
 - [pipenv](https://pipenv.pypa.io/en/latest/) v2021.5+
 - [Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) (1.2+)
@@ -75,20 +75,19 @@
 To install the project for development, you can use the following command:
 
 ```console
 pip install -r requirements.txt && pip install -e .[dev,test,doc]
 pre-commit install && pre-commit run --all-files
 ```
 
-For more information on how to help out, please check the [CONTRIBUTING](CONTRIBUTING.md) file.
+For more information on how to help out, please check the [CONTRIBUTING](https://github.com/THipster/THipster/blob/main/CONTRIBUTING.md) file.
 
 ## Open source licensing info
-1. [TERMS](TERMS.md)
-2. [LICENSE](LICENSE)
-3. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
+1. [LICENSE](https://github.com/THipster/THipster/blob/main/LICENSE)
+2. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
 
 ## Credits and references
 
 1. Projects that inspired you
     - [AWS Application Composer](https://aws.amazon.com/application-composer/?nc1=h_ls)
 2. Related projects
     - [Wing Programming Language](https://www.winglang.io/)
```

### Comparing `thipster-0.14.0/pyproject.toml` & `thipster-0.14.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -23,7 +23,10 @@
 repository_url = "https://upload.pypi.org/legacy/"
 
 commit_subject = ":bookmark: {version}"
 major_on_zero = false
 
 [pytest]
 mock_use_standalone_module = true
+
+[tool.ruff]
+exclude = ["__init__.py"]
```

### Comparing `thipster-0.14.0/setup.py` & `thipster-0.14.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.14.0'
+__version__ = '0.14.2'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md") as rm:
     readme = rm.read()
```

### Comparing `thipster-0.14.0/tests/engine/test_engine.py` & `thipster-0.14.2/tests/engine/test_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import thipster.engine.Engine as eng
-from thipster.engine.ParsedFile import ParsedFile
-from thipster.engine.ResourceModel import ResourceModel
+import os
 
 import pytest
-import os
+
+import thipster.engine as eng
+from thipster.engine.parsed_file import ParsedFile
+from thipster.engine.resource_model import ResourceModel
 
 
 def logger(name: str):
     def wrapper(function):
         def internal_wrapper(*args, **kwargs):
             print(f'{name} starting')
             res = function(*args, **kwargs)
```

### Comparing `thipster-0.14.0/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.14.2/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-from thipster.engine.ParsedFile import ParsedDict, ParsedFile, ParsedList, ParsedLiteral
-from thipster.parser.dsl_parser.DSLParser import DSLParser
-from thipster.parser.dsl_parser.DSLParser import DSLParserPathNotFound
-from thipster.parser.dsl_parser.Token import TOKENTYPES as TT
 import os
-from thipster.parser.dsl_parser.TokenParser import DSLConditionException,\
-    DSLSyntaxException, DSLUnexpectedEOF
+
 import pytest
 
+import thipster.engine.parsed_file as pf
+from thipster.parser import DSLParser
+from thipster.parser.dsl_parser.exceptions import DSLParserPathNotFound
+from thipster.parser.dsl_parser.token import TOKENTYPES as TT
+from thipster.parser.dsl_parser.token_parser import (
+    DSLConditionException,
+    DSLSyntaxException,
+    DSLUnexpectedEOF,
+)
+
 
 def create_dir(dirname: str, files: dict[str, str]):
     if not os.path.isdir(dirname):
         os.mkdir(dirname)
 
     dirname = os.path.abspath(dirname)
     for name, content in files.items():
@@ -72,15 +77,15 @@
         },
     )
 
     parser = DSLParser
     try:
         output = parser.run(path_input)
 
-        assert type(output) == ParsedFile
+        assert isinstance(output, pf.ParsedFile)
     except Exception as e:
         raise e
     finally:
         _destroy_dir()
 
     return output
 
@@ -97,15 +102,15 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
-    assert type(region._ParsedAttribute__value) == ParsedLiteral
+    assert isinstance(region._ParsedAttribute__value, pf.ParsedLiteral)
     assert region.value == 'euw'
 
 
 def test_parse_empty_file():
     out = __test_file(
         file="""""",
     )
@@ -177,15 +182,15 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
-    assert type(region._ParsedAttribute__value) == ParsedList
+    assert isinstance(region._ParsedAttribute__value, pf.ParsedList)
     assert len(region.value) == 3
 
     out = __test_file(
         file="""bucket my-bucket:
 \tregion: [toto, titi, tata]
 """,
     )
@@ -195,15 +200,15 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
-    assert type(region._ParsedAttribute__value) == ParsedList
+    assert isinstance(region._ParsedAttribute__value, pf.ParsedList)
     assert len(region.value) == 3
 
     out = __test_file(
         file="""bucket my-bucket:
 \tregion: []
 """,
     )
@@ -213,15 +218,15 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
-    assert type(region._ParsedAttribute__value) == ParsedList
+    assert isinstance(region._ParsedAttribute__value, pf.ParsedList)
     assert len(region.value) == 0
 
 
 def test_parse_dict_list_in_dict():
     out = __test_file(
         file="""bucket my-bucket:
 \ttoto:
@@ -238,18 +243,18 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 2
 
     toto = bucket.attributes[0]
     assert toto.name == 'toto'
-    assert type(toto._ParsedAttribute__value) == ParsedDict
+    assert isinstance(toto._ParsedAttribute__value, pf.ParsedDict)
     tata = bucket.attributes[1]
     assert tata.name == 'tata'
-    assert type(tata._ParsedAttribute__value) == ParsedList
+    assert isinstance(tata._ParsedAttribute__value, pf.ParsedList)
 
 
 def test_parse_if_else():
     # IN DICT
     out = __test_file(
         file="""bucket my-bucket:
 \tregion: euw if 1 == 1 else us
@@ -298,15 +303,15 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
-    assert type(region._ParsedAttribute__value) == ParsedList
+    assert isinstance(region._ParsedAttribute__value, pf.ParsedList)
 
     assert len(region.value) == 1
     r = region.value[0]
     assert r.value == 'euw'
 
 
 def test_parse_literal_types():
```

### Comparing `thipster-0.14.0/tests/parser/dsl_parser/test_ast.py` & `thipster-0.14.2/tests/parser/dsl_parser/test_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from thipster.engine.ParsedFile import Position
-from thipster.parser.dsl_parser.Token import Token
-import thipster.parser.dsl_parser.AST as ast
+import thipster.parser.dsl_parser.ast as ast
+from thipster.engine.parsed_file import Position
+from thipster.parser.dsl_parser.token import Token
 
 
 def test_create_AST():
     # bucket nom-#test \n\t toto: tata
     tree = ast.FileNode()
 
     tree.add(
```

### Comparing `thipster-0.14.0/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.14.2/tests/parser/dsl_parser/test_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from thipster.parser.dsl_parser.Lexer import Lexer, DSLParserNoEndingQuotes
-from thipster.parser.dsl_parser.Token import TOKENTYPES as TT
 import pytest
 
+from thipster.parser.dsl_parser.exceptions import DSLParserNoEndingQuotes
+from thipster.parser.dsl_parser.lexer import Lexer
+from thipster.parser.dsl_parser.token import TOKENTYPES as TT
+
 
 def __getTokenString(
     fileName: str,
     ln: int,
     col: int,
     tokenType: TT,
     value: str | None = None,
```

### Comparing `thipster-0.14.0/tests/parser/dsl_parser/test_token.py` & `thipster-0.14.2/tests/parser/dsl_parser/test_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from thipster.parser.dsl_parser.Token import Token
-from thipster.engine.ParsedFile import Position
+from thipster.engine.parsed_file import Position
+from thipster.parser.dsl_parser.token import Token
 
 
 def test_create_token():
     position = Position(fileName='testFile', ln=2, col=6)
     tokenType = 'test_type'
     value = 'test_value'
```

### Comparing `thipster-0.14.0/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.14.2/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from thipster.engine.ParsedFile import Position
-from thipster.parser.dsl_parser.TokenParser import TokenParser
-from thipster.parser.dsl_parser.Token import Token, TOKENTYPES as TT
+from thipster.engine.parsed_file import Position
+from thipster.parser.dsl_parser.token import TOKENTYPES as TT
+from thipster.parser.dsl_parser.token import Token
+from thipster.parser.dsl_parser.token_parser import TokenParser
 
 
 def test_simple_file():
     input = [
         Token(Position('file', 1, 1), TT.STRING, 'bucket'),
         Token(Position('file', 1, 7), TT.WHITESPACE),
         Token(Position('file', 1, 8), TT.STRING, 'nom'),
```

### Comparing `thipster-0.14.0/tests/parser/test_ParserFactory.py` & `thipster-0.14.2/tests/parser/test_ParserFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from thipster.engine.ParsedFile import ParsedFile
 
-from thipster.parser.ParserFactory import ParserFactory
+from thipster.engine.parsed_file import ParsedFile
+from thipster.parser import ParserFactory
 
 
 def create_dir(dirname: str, files: dict[str, str]):
     if not os.path.isdir(dirname):
         os.mkdir(dirname)
 
     dirname = os.path.abspath(dirname)
```

### Comparing `thipster-0.14.0/tests/parser/test_YAMLParser.py` & `thipster-0.14.2/tests/parser/test_YAMLParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import thipster.engine.ParsedFile as pf
-from thipster.parser.YAMLParser import YAMLParser, YAMLParserNoName
 import os
+
 import pytest
 
+import thipster.engine.parsed_file as pf
+from thipster.parser import YAMLParser
+from thipster.parser.yaml_parser import YAMLParserNoName
+
 
 def __test_parser_raises(mocker, input: str, exception: Exception)\
         -> pytest.ExceptionInfo:
     with pytest.raises(exception) as exc_info:
         __test_file(
             file=input,
         )
```

### Comparing `thipster-0.14.0/tests/parser/test_parsedfile.py` & `thipster-0.14.2/tests/parser/test_parsedfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import thipster.engine.ParsedFile as pf
+import thipster.engine.parsed_file as pf
 
 
 def test_create_parsed_file():
     file = pf.ParsedFile()
 
     assert isinstance(file, pf.ParsedFile)
```

### Comparing `thipster-0.14.0/tests/test_e2e.py` & `thipster-0.14.2/tests/test_e2e.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import json
 import os
 import shutil
-from cdktf_cdktf_provider_google.provider import GoogleProvider
 
-from thipster.engine.Engine import Engine
-from thipster.engine.I_Auth import I_Auth
-from thipster.parser.ParserFactory import ParserFactory
 import pytest
-from thipster.repository.LocalRepo import LocalRepo
-import thipster.terraform.CDK as cdk
+from cdktf_cdktf_provider_google.provider import GoogleProvider
+
+from thipster.engine.engine import Engine
+from thipster.engine.i_auth import I_Auth
+from thipster.parser.parser_factory import ParserFactory
+from thipster.repository.local import LocalRepo
+from thipster.terraform import Terraform
+from thipster.terraform.exceptions import (
+    CDKCyclicDependencies,
+    CDKDependencyNotDeclared,
+    CDKMissingAttributeInDependency,
+)
 
 LOCAL_REPO = 'tests/resources/e2e/models'
 REMOTE_REPO = 'THipster/models'
 
 
 class MockAuth(I_Auth):
     def authenticate(app):
@@ -44,79 +50,116 @@
 
     file = open(f'{dirname}/{filename}', 'w')
     file.write(content)
     file.close()
 
 
 def __test_file(file: str, local_repo: str = LOCAL_REPO, file_type: str = 'thips'):
-
     path_input = 'test'
     __destroy_dir = create_dir(
         path_input,
         {
             f'test_file.{file_type}':
             file,
         },
     )
 
     engine = Engine(
         ParserFactory(),
         LocalRepo(local_repo),
         MockAuth,
-        cdk.CDK(),
+        Terraform(),
     )
     try:
         output = engine.run(path_input)
     except Exception as e:
         raise e
     finally:
         __destroy_dir()
 
         if os.path.exists('cdktf.out'):
             shutil.rmtree('cdktf.out')
 
     return output
 
 
-def assert_resource_created(res_type: str, name: str):
+def get_output():
     with open("thipster.tf.json") as f:
-        output = json.load(f)
+        file_contents = json.load(f)
         f.close()
+    return file_contents
+
+
+def get_resource(resource_data: tuple):
+    output = get_output()
+
+    resources_of_type = output.get("resource").get(resource_data[0])
+    resource = None
+    for r in resources_of_type.values():
+        if r.get("name") == resource_data[1]:
+            resource = r
 
+    assert resource is not None
+
+    return resource
+
+
+def assert_resource_created(
+    resource_type: str,
+    resource_name: str,
+):
+    output = get_output()
     assert output.get("resource") is not None
     resources = output.get("resource")
 
-    assert resources.get(res_type) is not None
+    assert resources.get(resource_type) is not None
 
-    names = [x.get("name") for _, x in resources.get(res_type).items()]
-    assert name in names
+    names = [x.get("name") for _, x in resources.get(resource_type).items()]
+    assert resource_name in names
 
+    return (resource_type, resource_name)
 
-def assert_number_of_resource_type_is(res_type: str, amount: str):
-    with open("thipster.tf.json") as f:
-        output = json.load(f)
-        f.close()
 
+def assert_number_of_resource_type_is(
+    resource_type: str,
+    amount: str,
+):
+    output = get_output()
     assert output.get("resource") is not None
     resources = output.get("resource")
 
-    assert resources.get(res_type) is not None
-    assert len(resources.get(res_type)) == amount
+    assert resources.get(resource_type) is not None
+    assert len(resources.get(resource_type)) == amount
+
+
+def assert_resource_parameters_are(resource_data: tuple, parameters: list[str]):
+    resource = get_resource(resource_data)
+
+    for parameter in parameters:
+        assert parameter in resource.keys()
+
+
+def get_resource_parameter(resource_data: tuple, parameter: str):
+    resource = get_resource(resource_data)
+
+    assert parameter in resource.keys()
+    return resource.get(parameter)
 
 
 def test_bucket():
     __test_file(
         file="""
 bucket my-bucket:
 \tregion : euw
     """,
     )
 
     assert_number_of_resource_type_is("google_storage_bucket", 1)
-    assert_resource_created("google_storage_bucket", "my-bucket")
+    bucket = assert_resource_created("google_storage_bucket", "my-bucket")
+    assert_resource_parameters_are(bucket, ["location"])
 
 
 def test_empty_bucket():
     __test_file(
         file="""
 bucket dzvhvzarbazkhr:
 
@@ -137,25 +180,25 @@
 
     assert_number_of_resource_type_is("google_storage_bucket", 2)
     assert_resource_created("google_storage_bucket", "dzvhvzarbazkhr")
     assert_resource_created("google_storage_bucket", "ezezeaz")
 
 
 def test_dep_with_no_options():
-    with pytest.raises(cdk.CDKMissingAttributeInDependency):
+    with pytest.raises(CDKMissingAttributeInDependency):
         __test_file(
             file="""
 bucket_bad_dep_parent my-bucket:
 \tregion : euw
         """,
         )
 
 
 def test_cyclic_deps():
-    with pytest.raises(cdk.CDKCyclicDependencies):
+    with pytest.raises(CDKCyclicDependencies):
         __test_file(
             file="""
 bucket_bad_dep_cyclic my-bucket:
 \tregion : euw
         """,
         )
 
@@ -178,29 +221,14 @@
     assert_number_of_resource_type_is("google_compute_network", 3)
     assert_resource_created("google_compute_network", "lb-net")
 
     assert_number_of_resource_type_is("google_compute_subnetwork", 1)
     assert_resource_created("google_compute_subnetwork", "lb-subnet")
 
 
-def test_lb_single_file():
-    __test_file(
-        file="""
-network lb-net:
-
-subnetwork lb-subnet:
-\tregion: europe-west1b
-\tip_range: 10.0.1.0/24
-
-loadbalancer my-lb:
-\tload_balancing_scheme: EXTERNAL
-    """,
-    )
-
-
 def test_internal_object():
     __test_file(
         file="""
 firewall testParent:
 \tdirection: EGRESS
         """,
     )
@@ -212,14 +240,39 @@
 
 \tallow:
 \t\tprotocol: http
         """,
     )
 
 
+def test_missing_explicit_dependency():
+    with pytest.raises(CDKDependencyNotDeclared):
+        __test_file(
+            file="""
+subnetwork lb-subnet:
+\tnetwork: lb-net
+\tregion: europe-west1b
+\tip_range: 10.0.1.0/24
+            """,
+        )
+
+
+def test_explicit_dependency():
+    __test_file(
+        file="""
+network lb-net:
+
+subnetwork lb-subnet:
+\tnetwork: lb-net
+\tregion: europe-west1b
+\tip_range: 10.0.1.0/24
+        """,
+    )
+
+
 def test_bucket_cors():
     __test_file(
         file="""
 bucket corsBucket:
     cors:
         origin:
             - "http://example.com"
@@ -256,8 +309,11 @@
       - "*"
       maxAge: 600
 """,
         file_type='yaml',
     )
 
     assert_number_of_resource_type_is("google_storage_bucket", 1)
-    assert_resource_created("google_storage_bucket", "corsBucket")
+    bucket = assert_resource_created("google_storage_bucket", "corsBucket")
+    cors_block = get_resource_parameter(bucket, "cors")
+
+    assert len(cors_block) == 2
```

### Comparing `thipster-0.14.0/thipster/auth/Google.py` & `thipster-0.14.2/thipster/auth/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import google.auth
-from thipster.engine.I_Auth import I_Auth
 from cdktf_cdktf_provider_google.provider import GoogleProvider
 
+from thipster.engine import I_Auth
+
 
 class GoogleAuth(I_Auth):
     """Authentication to GCP Projects
     """
 
     def __init__(self) -> None:
         return GoogleAuth
```

### Comparing `thipster-0.14.0/thipster/engine/Engine.py` & `thipster-0.14.2/thipster/engine/engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """_Engine.py module.
 """
 import time
 
-from thipster.engine.I_Parser import I_Parser
-from thipster.engine.I_Repository import I_Repository
-from thipster.engine.I_Auth import I_Auth
-from thipster.engine.I_Terraform import I_Terraform
-import thipster.engine.ParsedFile as pf
-from thipster.engine.ResourceModel import ResourceModel
+import thipster.engine.parsed_file as pf
+
+from .i_auth import I_Auth
+from .i_parser import I_Parser
+from .i_repository import I_Repository
+from .i_terraform import I_Terraform
+from .resource_model import ResourceModel
 
 
 class Engine():
     """The engine of thipster
 
     The core of the application, it is used to call and link all
     interfaces together.
@@ -39,14 +40,58 @@
 
         """
         self.__parser = parser
         self.__repository = repository
         self.__auth = auth
         self.__terraform = terraform
 
+    @property
+    def parser(self):
+        return self.__parser
+
+    @parser.setter
+    def parser(self, value):
+        if not isinstance(value, I_Parser):
+            raise Exception()
+
+        self.__parser = value
+
+    @property
+    def repository(self):
+        return self.__repository
+
+    @repository.setter
+    def repository(self, value):
+        if not isinstance(value, I_Repository):
+            raise Exception()
+
+        self.__repository = value
+
+    @property
+    def auth(self):
+        return self.__auth
+
+    @auth.setter
+    def auth(self, value):
+        if not isinstance(value, I_Auth):
+            raise Exception()
+
+        self.__auth = value
+
+    @property
+    def terraform(self):
+        return self.__terraform
+
+    @terraform.setter
+    def terraform(self, value):
+        if not isinstance(value, I_Terraform):
+            raise Exception()
+
+        self.__terraform = value
+
     def run(self, path: str) -> tuple[list[str], str]:
         """Returns json Terraform files from the input file name
 
         Calls the different run methods of the parser, repository,
         auth and terraform modules.
         Transforms the inputed filename into a Cloud architecture plan.
```

### Comparing `thipster-0.14.0/thipster/engine/I_Parser.py` & `thipster-0.14.2/thipster/engine/i_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
-from thipster.engine.ParsedFile import ParsedFile
+
+from thipster.engine.parsed_file import ParsedFile
 
 
 class I_Parser(ABC):
     """Parser module interface
     """
     @abstractmethod
     def run(self, path: str) -> ParsedFile:
```

### Comparing `thipster-0.14.0/thipster/engine/I_Repository.py` & `thipster-0.14.2/thipster/engine/i_repository.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
-from thipster.engine.ResourceModel import ResourceModel
+
+from thipster.engine.resource_model import ResourceModel
 
 
 class I_Repository(ABC):
     """Repository module interface
     """
     @abstractmethod
     def get(self, resourceNames: list[str]) -> dict[str, ResourceModel]:
```

### Comparing `thipster-0.14.0/thipster/engine/I_Terraform.py` & `thipster-0.14.2/thipster/engine/i_terraform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
-import thipster.engine.ResourceModel as rm
-import thipster.engine.ParsedFile as pf
+
+import thipster.engine.parsed_file as pf
+import thipster.engine.resource_model as rm
 
 
 class I_Terraform(ABC):
     """Terraform module interface
     """
     @abstractmethod
     def apply(self):
```

### Comparing `thipster-0.14.0/thipster/engine/ParsedFile.py` & `thipster-0.14.2/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.0/thipster/engine/ResourceModel.py` & `thipster-0.14.2/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.0/thipster/parser/ParserFactory.py` & `thipster-0.14.2/thipster/parser/dsl_parser/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,76 @@
 import os
-from thipster.engine.I_Parser import I_Parser
-from thipster.engine.ParsedFile import ParsedFile
-from thipster.parser.YAMLParser import YAMLParser
-from thipster.parser.dsl_parser.DSLParser import DSLParser
 
+from thipster.engine import I_Parser
+from thipster.engine.parsed_file import ParsedFile
 
-class ParserPathNotFound(Exception):
-    def __init__(self, path, *args: object) -> None:
-        super().__init__(*args)
+from .exceptions import DSLParserBaseException, DSLParserPathNotFound
+from .interpreter import Interpreter
+from .lexer import Lexer
+from .token_parser import TokenParser
 
-        self.__message = f'Path not found : {path}'
 
-    @property
-    def message(self):
-        return self.__message
+class DSLParser(I_Parser):
 
-
-class ParserFactory(I_Parser):
-
-    def __getfiles(self, path: str) -> list[str]:
-        """Recursively get all files names in the requested directory and its\
-              sudirectories
+    def __getfiles(path: str) -> dict[str, str]:
+        """Recursively get all files in the requested directory and its sudirectories
         Can be run on a path file aswell
 
         Parameters
         ----------
         path: str
             Path to run this function into
 
         Returns
         -------
-        list[str]
-            A list of all the filenames 
+        dict[str, str]
+            A dictionary that links a filename to its content, fileName : fileContent
         """
 
         path = os.path.abspath(path)
 
         if not os.path.exists(path):
-            raise ParserPathNotFound(path)
+            raise DSLParserPathNotFound(path)
 
-        files = []
+        files = {}
 
         if os.path.isdir(path):
             for content in os.listdir(path):
-                files += self.__getfiles(f'{path}/{content}')
+                files.update(DSLParser.__getfiles(f'{path}/{content}'))
 
         if os.path.isfile(path):
-            return [path]
-
-        return files
+            with open(path, 'r') as f:
+                files.update({path: f.read()})
 
-    def __yamlParser(self) -> YAMLParser:
-        return YAMLParser
+                f.close()
 
-    def __dslParser(self) -> DSLParser:
-        return DSLParser
-
-    def __noParser(self):
-        raise Exception()
+        return files
 
-    def run(self, path: str) -> ParsedFile:
-        """Run the ParserFactory
+    def run(path: str) -> ParsedFile:
+        """Run the DSLParser
 
         Parameters
         ----------
         path: str
             Path to run the parser into
 
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
-        files = self.__getfiles(path)
-
-        res = ParsedFile()
-        for file in files:
-            parsedFile = self.__getParser(file).run(file)
-            res.resources += parsedFile.resources
-
-        return res
-
-    def __getParser(self, path) -> I_Parser:
-        __parsers = {
-            '.yaml': self.__yamlParser,
-            '.yml': self.__yamlParser,
-            '.jinja': self.__yamlParser,
-            '.thips': self.__dslParser,
-        }
-
-        _, pathExtension = os.path.splitext(path)
 
-        return __parsers.get(pathExtension, self.__noParser)()
+        try:
+            files = DSLParser.__getfiles(path)
+            lexer = Lexer(files)
+            token_list = lexer.run()
+            parser = TokenParser(token_list)
+            ast = parser.run()
+
+            interpreter = Interpreter()
+            parsedFile = interpreter.run(ast)
+
+            return parsedFile
+        except DSLParserBaseException as e:
+            raise e
+        except Exception as e:
+            raise e
```

### Comparing `thipster-0.14.0/thipster/parser/YAMLParser.py` & `thipster-0.14.2/thipster/parser/yaml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from thipster.engine.I_Parser import I_Parser
-import thipster.engine.ParsedFile as pf
-from jinja2 import Environment, FileSystemLoader
-
 import os
+
 import yaml
+from jinja2 import Environment, FileSystemLoader
+
+import thipster.engine.parsed_file as pf
+from thipster.engine import I_Parser
 
 
 class YAMLParserBaseException(Exception):
     def __init__(self, message, *args: object) -> None:
         super().__init__(*args)
 
         self.__message = message
```

### Comparing `thipster-0.14.0/thipster/parser/dsl_parser/AST.py` & `thipster-0.14.2/thipster/parser/dsl_parser/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
-from thipster.engine.ParsedFile import Position
 
-from thipster.parser.dsl_parser.Token import Token
+from thipster.engine.parsed_file import Position
+
+from .token import Token
 
 
 class Node(ABC):
 
     @abstractmethod
     def accept(self, visitor):
         raise NotImplementedError()
```

### Comparing `thipster-0.14.0/thipster/parser/dsl_parser/DSLParser.py` & `thipster-0.14.2/thipster/parser/parser_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,93 @@
-from thipster.engine.I_Parser import I_Parser
-from thipster.engine.ParsedFile import ParsedFile
-
 import os
-from thipster.parser.dsl_parser.Interpreter import Interpreter
-from thipster.parser.dsl_parser.Lexer import Lexer
-from thipster.parser.dsl_parser.TokenParser import TokenParser
 
-from thipster.parser.dsl_parser.DSLExceptions import DSLParserPathNotFound, \
-    DSLParserBaseException
+from thipster.engine import I_Parser
+from thipster.engine.parsed_file import ParsedFile
+from .dsl_parser import DSLParser
+from .yaml_parser import YAMLParser
+
+
+class ParserPathNotFound(Exception):
+    def __init__(self, path, *args: object) -> None:
+        super().__init__(*args)
+
+        self.__message = f'Path not found : {path}'
+
+    @property
+    def message(self):
+        return self.__message
+
+
+class ParserFactory(I_Parser):
 
+    __parsers = {
+        '.yaml': YAMLParser,
+        '.yml': YAMLParser,
+        '.jinja': YAMLParser,
+        '.thips': DSLParser,
+    }
 
-class DSLParser(I_Parser):
+    def addParser(parser: I_Parser, extensions: list[str]):
+        ParserFactory.__parsers.update({e: parser for e in extensions})
 
-    def __getfiles(path: str) -> dict[str, str]:
-        """Recursively get all files in the requested directory and its sudirectories
+    def __getfiles(self, path: str) -> list[str]:
+        """Recursively get all files names in the requested directory and its\
+              sudirectories
         Can be run on a path file aswell
 
         Parameters
         ----------
         path: str
             Path to run this function into
 
         Returns
         -------
-        dict[str, str]
-            A dictionary that links a filename to its content, fileName : fileContent
+        list[str]
+            A list of all the filenames 
         """
 
         path = os.path.abspath(path)
 
         if not os.path.exists(path):
-            raise DSLParserPathNotFound(path)
+            raise ParserPathNotFound(path)
 
-        files = {}
+        files = []
 
         if os.path.isdir(path):
             for content in os.listdir(path):
-                files.update(DSLParser.__getfiles(f'{path}/{content}'))
+                files += self.__getfiles(f'{path}/{content}')
 
         if os.path.isfile(path):
-            with open(path, 'r') as f:
-                files.update({path: f.read()})
-
-                f.close()
+            return [path]
 
         return files
 
-    def run(path: str) -> ParsedFile:
-        """Run the DSLParser
+    def __noParser(self):
+        raise Exception()
+
+    def run(self, path: str) -> ParsedFile:
+        """Run the ParserFactory
 
         Parameters
         ----------
         path: str
             Path to run the parser into
 
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
+        files = self.__getfiles(path)
+
+        res = ParsedFile()
+        for file in files:
+            parsedFile = self.__getParser(file).run(file)
+            res.resources += parsedFile.resources
+
+        return res
+
+    def __getParser(self, path) -> I_Parser:
+
+        _, pathExtension = os.path.splitext(path)
 
-        try:
-            files = DSLParser.__getfiles(path)
-            lexer = Lexer(files)
-            token_list = lexer.run()
-            parser = TokenParser(token_list)
-            ast = parser.run()
-
-            interpreter = Interpreter()
-            parsedFile = interpreter.run(ast)
-
-            return parsedFile
-        except DSLParserBaseException as e:
-            raise e
-        except Exception as e:
-            raise e
+        return ParserFactory.__parsers.get(pathExtension, self.__noParser)
```

### Comparing `thipster-0.14.0/thipster/parser/dsl_parser/Interpreter.py` & `thipster-0.14.2/thipster/parser/dsl_parser/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import thipster.engine.ParsedFile as pf
-import thipster.parser.dsl_parser.AST as ast
-from thipster.parser.dsl_parser.Token import TOKENTYPES as TT
-from thipster.parser.dsl_parser.DSLExceptions import DSLParserBaseException
-from thipster.parser.dsl_parser.TokenParser import DSLSyntaxException
+import thipster.engine.parsed_file as pf
+import thipster.parser.dsl_parser.ast as ast
+
+from .exceptions import DSLParserBaseException
+from .token import TOKENTYPES as TT
+from .token_parser import DSLSyntaxException
 
 
 class DSLParserVariableAlreadyUsed(DSLParserBaseException):
     def __init__(self, var: str, *args: object) -> None:
         super().__init__(f'Variable already used : {var}', *args)
```

### Comparing `thipster-0.14.0/thipster/parser/dsl_parser/Lexer.py` & `thipster-0.14.2/thipster/parser/dsl_parser/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-from thipster.parser.dsl_parser.Token import Token, TOKENTYPES as TT
-from thipster.engine.ParsedFile import Position
+from thipster.engine.parsed_file import Position
 from thipster.helpers import createLogger
-from thipster.parser.dsl_parser.DSLExceptions import DSLParserBaseException
-from thipster.parser.dsl_parser.LexerPosition import LexerPosition
 
-
-class DSLParserNoEndingQuotes(DSLParserBaseException):
-    def __init__(self, position, *args: object) -> None:
-        super().__init__(
-            f'Invalid syntax, missing ending quotes at : {position}', *args,
-        )
+from .exceptions import DSLParserNoEndingQuotes
+from .lexer_position import LexerPosition
+from .token import TOKENTYPES as TT
+from .token import Token
 
 
 class Lexer():
     """Lexer class for the DSL Parser
     """
 
     def __init__(self, files: dict[str, str]):
```

### Comparing `thipster-0.14.0/thipster/parser/dsl_parser/LexerPosition.py` & `thipster-0.14.2/thipster/parser/dsl_parser/lexer_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thipster.engine.ParsedFile import Position
+from thipster.engine.parsed_file import Position
 
 
 class LexerPosition():
     def __init__(
         self,
         fileName: str = '',
         startLine: int = 1,
```

### Comparing `thipster-0.14.0/thipster/parser/dsl_parser/Token.py` & `thipster-0.14.2/thipster/parser/dsl_parser/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from thipster.engine.ParsedFile import Position
 from enum import Enum
 
+from thipster.engine.parsed_file import Position
+
 
 class TOKENTYPES(Enum):
     AMOUNT = 'AMOUNT'
     AND = 'AND'
     BOOLEAN = 'BOOLEAN'
     BRACKETS_START = 'BRACKETS_START'
     BRACKETS_END = 'BRACKETS_END'
```

### Comparing `thipster-0.14.0/thipster/parser/dsl_parser/TokenParser.py` & `thipster-0.14.2/thipster/parser/dsl_parser/token_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,16 @@
-from thipster.parser.dsl_parser.Token import Token, TOKENTYPES as TT
-import thipster.parser.dsl_parser.AST as ast
+import thipster.parser.dsl_parser.ast as ast
 
-
-class DSLSyntaxException(Exception):
-    def __init__(self, token: Token, expected: TT | list[TT], *args: object) -> None:
-        super().__init__(*args)
-        self.__tok = token
-        self.__exp = expected
-
-    def __repr__(self) -> str:
-
-        if type(self.__exp) is TT:
-            return f"""{str(self.__tok.position)} :\n\tSyntax error : Expected \
-{str(self.__exp.value)}, got {str(self.__tok.tokenType)}"""
-        else:
-            return f"""{str(self.__tok.position)} :\n\tSyntax error : Expected \
-{str(' or '.join(list(map(lambda x : str(x), self.__exp))))}, got {
-    str(self.__tok.tokenType)}"""
-
-    @property
-    def tok(self):
-        return self.__tok
-
-
-class DSLConditionException(Exception):
-    def __init__(self, token: Token, *args: object) -> None:
-        super().__init__(*args)
-        self.__tok = token
-
-    def __repr__(self) -> str:
-        return f"""{str(self.__tok.position)} :\n\tBad condition"""
-
-
-class DSLUnexpectedEOF(Exception):
-    def __init__(self, *args: object) -> None:
-        super().__init__(*args)
-
-    def __repr__(self) -> str:
-        return 'Unexpected EOF'
+from .exceptions import (
+    DSLConditionException,
+    DSLSyntaxException,
+    DSLUnexpectedEOF,
+)
+from .token import TOKENTYPES as TT
+from .token import Token
 
 
 class TokenParser():
     def __init__(self, tokens: list[Token]) -> None:
         self.__tokens = tokens
 
     def run(self) -> ast.FileNode:
```

### Comparing `thipster-0.14.0/thipster/repository/GithubRepo.py` & `thipster-0.14.2/thipster/repository/github.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """GithubRepo.py module
 """
 
-from thipster.repository.JSONRepo import JSONRepo
 import requests
 
+from .json import JSONRepo
+
 
 class GithubRepo(JSONRepo):
     """Class representing a GitHub resources Repository
 
     JSON Models of resources and services offered by supported cloud providers are
     stored in a repository.
     This class is used to access those models if they are located in a GitHub repo.
```

### Comparing `thipster-0.14.0/thipster/repository/JSONRepo.py` & `thipster-0.14.2/thipster/repository/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """JSONRepo.py module.
 """
 
-from abc import ABC, abstractmethod
 import json
-from thipster.engine.I_Repository import I_Repository
+from abc import ABC, abstractmethod
 
-import thipster.engine.ResourceModel as rm
+import thipster.engine.resource_model as rm
+from thipster.engine import I_Repository
 
 
 class JSONRepo(I_Repository, ABC):
     _parentStack = []
     """Class representing a JSON resources Repository
 
     JSON Models of resources and services offered by supported cloud providers are
```

### Comparing `thipster-0.14.0/thipster/terraform/CDK.py` & `thipster-0.14.2/thipster/terraform/cdk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,26 @@
 import copy
+import importlib
+import os
 import shutil
 import subprocess
 import sys
-import os
-import importlib
 import uuid
-from thipster.engine.I_Auth import I_Auth
 
-from python_terraform import Terraform
+from cdktf import App, TerraformOutput, TerraformStack
 from constructs import Construct
-from cdktf import App, TerraformStack, TerraformOutput
+from python_terraform import Terraform
 
-import thipster.engine.ResourceModel as rm
-import thipster.engine.ParsedFile as pf
-from thipster.engine.I_Terraform import I_Terraform
+import thipster.engine.parsed_file as pf
+import thipster.engine.resource_model as rm
+import thipster.terraform.exceptions as cdk_exceptions
+from thipster.engine import I_Auth, I_Terraform
 from thipster.helpers import createLogger as Logger
 
 
-class CDKException(Exception):
-    @property
-    def message(self):
-        return str(self)
-
-
-class CDKInvalidAttribute(CDKException):
-    def __init__(self, attr: str, modelType: str, **args: object) -> None:
-        super().__init__(*args)
-        self.__attr = attr
-        self.__modelType = modelType
-
-    def __str__(self) -> str:
-        return f'{self.__attr} in {self.__modelType} but not useful'
-
-
-class CDKMissingAttribute(CDKException):
-    pass
-
-
-class CDKMissingAttributeInDependency(CDKMissingAttribute):
-    pass
-
-
-class CDKDependencyNotDeclared(CDKException):
-    def __init__(self, depType: str, depName: str, **args: object) -> None:
-        super().__init__(*args)
-        self.__name = depName
-        self.__type = depType
-
-    def __str__(self) -> str:
-        return f'{self.__type} {self.__name} not declared \
-(be sure to declare it before using it)'
-
-
-class CDKCyclicDependencies(CDKException):
-    def __init__(self, stack: list[str], **args: object) -> None:
-        super().__init__(*args)
-        self.__stack = stack
-
-    def __str__(self) -> str:
-        return ','.join(self.__stack)
-
-
 class CDK(I_Terraform):
     _models = []
     _parentStack = []
     _importedPackages = []
 
     _created_resources = {}
     _logger = Logger(__name__)
@@ -82,16 +38,17 @@
         _, stdout, stderr = t.apply()
         return stdout + stderr
 
     def generate(
         self, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
         _auth: I_Auth,
     ):
-
+        CDK._created_resources = {}
         CDK._models = models
+        CDK._parentStack = []
         # Init CDK
         app = App()
 
         f_position = file.resources[0].position
         file_name = f_position.fileName if f_position else 'thipster_infrastructure'
 
         CDK._logger.debug('Creating tf code for file %s', file_name)
@@ -188,23 +145,23 @@
     def _create_default_resource(
         self, typ: str, parentName: str | None = None,
         noModif: bool = True, noDependencies: bool = False,
     ):
         # Checks for cyclic dependency
         if typ in CDK._parentStack:
             CDK._logger.error('%s already present in parent Stack', typ)
-            raise CDKCyclicDependencies(CDK._parentStack)
+            raise cdk_exceptions.CDKCyclicDependencies(CDK._parentStack)
 
         CDK._parentStack.append(typ)
 
         model = CDK._models[typ]
 
         # Checks that all attributes are optional
         if noModif and not all(map(lambda x: x.optional, model.attributes.values())):
-            raise CDKMissingAttributeInDependency(typ)
+            raise cdk_exceptions.CDKMissingAttributeInDependency(typ)
 
         # Import package and class
         CDK._pip_install(model.cdk_provider)
         resourceClass = CDK._import(
             model.cdk_provider, model.cdk_module, model.cdk_name,
         )
 
@@ -217,15 +174,30 @@
             resource_args[model.name_key] = name
 
         for _, v in model.attributes.items():
             resource_args[v.cdk_name] = v.default
 
         # Create default defendencies if needed
         if not noDependencies:
-            CDK._create_dependencies(self, deps, resource_args, name)
+            for depName, depValue in deps.items():
+                CDK._create_dependency(
+                    self, depName, depValue, resource_args, parentName,
+                )
+
+            # Create default internal objects if needed
+            for objName, internalObject in model.internalObjects.items():
+                if objName not in resource_args:
+                    for defaultArg in internalObject['defaults']:
+                        CDK._create_internal_object(
+                            self,
+                            model.internalObjects[objName],
+                            objName,
+                            defaultArg,
+                            resource_args,
+                        )
 
         CDK._logger.debug('Created default %s named %s', resourceClass, name)
 
         return (resourceClass, name, resource_args)
 
     def _create_resource_from_args(
         self, typ: str, args: list[pf.ParsedAttribute] | None,
@@ -249,25 +221,97 @@
                 model=model,
                 attribute=attribute,
                 resource_args=resource_args,
                 deps=deps,
             )
 
         # Create missing dependencies
-        CDK._create_dependencies(self, deps, resource_args, resourceName)
+        for depName, depValue in deps.items():
+            CDK._create_dependency(
+                self, depName, depValue, resource_args, resourceName,
+            )
+
+        # Create default internal objects if needed
+        for objName, internalObject in model.internalObjects.items():
+            if objName not in resource_args:
+                for defaultArg in internalObject['defaults']:
+                    CDK._create_internal_object(
+                        self,
+                        model.internalObjects[objName],
+                        objName,
+                        defaultArg,
+                        resource_args,
+                    )
 
         # Create resource
         CDK._parentStack.remove(typ)
+
+        CDK._logger.debug(
+            'Created default %s named %s',
+            resourceClass, resourceName,
+        )
+
         if not model.name_key:
             return resourceClass(**resource_args)
+        return resourceClass(self, resourceName, **resource_args)
+
+    def _create_resource_from_dict(
+        self, typ: str, args: dict | None,
+    ):
+        resourceClass, resourceName, resource_args = CDK._create_default_resource(
+            self,
+            typ,
+            noModif=False,
+            noDependencies=True,
+        )
+        model = CDK._models[typ]
+
+        # Process attributes
+        deps = copy.deepcopy(model.dependencies)
+        for name, value in args.items():
+            if name and model.name_key:
+                resource_args[model.name_key] = name
+
+            resource_args, deps = CDK._process_attribute(
+                self,
+                model=model,
+                attribute=pf.ParsedAttribute(
+                    name, None, pf.ParsedLiteral(value),
+                ),
+                resource_args=resource_args,
+                deps=deps,
+            )
+
+        # Create missing dependencies
+        for depName, depValue in deps.items():
+            CDK._create_dependency(
+                self, depName, depValue, resource_args, resourceName,
+            )
+
+        # Create default internal objects if needed
+        for objName, internalObject in model.internalObjects.items():
+            if objName not in resource_args:
+                for defaultArg in internalObject['defaults']:
+                    CDK._create_internal_object(
+                        self,
+                        model.internalObjects[objName],
+                        objName,
+                        defaultArg,
+                        resource_args,
+                    )
+        # Create resource
+        CDK._parentStack.remove(typ)
 
         CDK._logger.debug(
             'Created default %s named %s',
             resourceClass, resourceName,
         )
+
+        if not model.name_key:
+            return resourceClass(**resource_args)
         return resourceClass(self, resourceName, **resource_args)
 
     def _create_resource_from_resource(self, resource: pf.ParsedResource):
         # Create resource with default values
         resourceClass, _, resource_args = CDK._create_default_resource(
             self,
             resource.type,
@@ -287,15 +331,30 @@
                 model=model,
                 attribute=attribute,
                 resource_args=resource_args,
                 deps=deps,
             )
 
         # Create missing dependencies
-        CDK._create_dependencies(self, deps, resource_args, resource.name)
+        for depName, depValue in deps.items():
+            CDK._create_dependency(
+                self, depName, depValue, resource_args, resource.name,
+            )
+
+        # Create default internal objects if needed
+        for objName, internalObject in model.internalObjects.items():
+            if objName not in resource_args:
+                for defaultArg in internalObject['defaults']:
+                    CDK._create_internal_object(
+                        self,
+                        model.internalObjects[objName],
+                        objName,
+                        defaultArg,
+                        resource_args,
+                    )
 
         # Create resource
         CDK._parentStack.remove(resource.type)
 
         CDK._logger.debug(
             'Created resource %s named %s',
             resourceClass, resource.name,
@@ -306,85 +365,116 @@
     def _process_attribute(
         self,
         model: rm.ResourceModel,
         attribute: pf.ParsedAttribute,
         resource_args: dict[str, object],
         deps: dict[str, dict[str, object]] | None,
     ):
-        # Checks if attribute is an explicit dependency
         if attribute.name in deps:
             created_name = f"{deps[attribute.name]['resource']}/{attribute.value}"
 
-            if created_name not in CDK._created_resources:
-                raise CDKDependencyNotDeclared(attribute.name, attribute.value)
+            # Checks if attribute is an explicit dependency
+            if created_name not in CDK._created_resources.keys():
+
+                if isinstance(attribute.value, str):
+                    raise cdk_exceptions.CDKDependencyNotDeclared(
+                        attribute.name, attribute.value,
+                    )
+
+                # Creates explicit dependency
+                CDK._create_dependency(
+                    self, attribute.name, attribute.value,
+                    resource_args, attribute.name,
+                )
 
             resource_args[attribute.name] = CDK._created_resources[created_name]
+
             del deps[attribute.name]
             return resource_args, deps
 
         # Checks if attribute is an internal object
         if attribute.name in model.internalObjects:
-            resource_args = CDK._handle_internal_object(
+            resource_args = CDK._create_internal_object(
                 self,
-                model=model,
-                attribute=attribute,
-                resource_args=resource_args,
+                model.internalObjects[attribute.name],
+                attribute.name,
+                attribute.value,
+                resource_args,
             )
             return resource_args, deps
 
         # Checks if attribute is expected as an attibute
         if attribute.name not in model.attributes:
-            raise CDKInvalidAttribute(attribute.name, model.type)
+            raise cdk_exceptions.CDKInvalidAttribute(
+                attribute.name, model.type,
+            )
 
         # Processes list attribute
         attribute_value = attribute.value
         if model.attributes[attribute.name].is_list:
             if type(attribute.value) is list:
                 attribute_value = [i.value for i in attribute.value]
             else:
                 attribute_value = [attribute.value]
 
         # Sets attribute value
         resource_args[model.attributes[attribute.name].cdk_name] = attribute_value
 
         return resource_args, deps
 
-    def _handle_internal_object(
+    def _create_internal_object(
         self,
-        model: rm.ResourceModel,
-        attribute: pf.ParsedAttribute,
+        internalObjectModel,
+        name: str,
+        args,
         resource_args: dict,
     ):
-        int_obj = model.internalObjects[attribute.name]
+        int_obj = internalObjectModel
         var_type = int_obj['var_type'] if 'var_type' in int_obj else 'Unknown'
 
-        if 'list' in var_type:
-            if attribute.name not in resource_args:
-                resource_args[attribute.name] = []
-
-            if isinstance(attribute.value[0], pf.ParsedDict):
-                for internalObject in attribute.value:
-                    res = CDK._create_resource_from_args(
+        if var_type.startswith('list'):
+            if name not in resource_args:
+                resource_args[name] = []
+
+            if isinstance(args, list) and isinstance(args[0], pf.ParsedDict):
+                for internalObject in args:
+                    res = CDK._handle_internal_object(
                         self,
-                        model.internalObjects[attribute.name]['resource'],
+                        internalObjectModel['resource'],
                         internalObject.value,
                     )
+                    resource_args[name] += [res]
+
+                return resource_args
 
-                    resource_args[attribute.name] += [res]
-        else:
-            res = CDK._create_resource_from_args(
+            res = CDK._handle_internal_object(
                 self,
-                model.internalObjects[attribute.name]['resource'],
-                attribute.value,
+                internalObjectModel['resource'],
+                args,
             )
-            resource_args[attribute.name] = res
+            resource_args[name] += [res]
+            return resource_args
+
+        res = CDK._handle_internal_object(
+            self,
+            internalObjectModel['resource'],
+            args,
+        )
+        resource_args[name] = res
 
         return resource_args
 
-    def _create_dependencies(self, deps, resource_args, name):
-        for k, d in deps.items():
-            c, n, a = CDK._create_default_resource(self, d['resource'], name)
-            id = c(self, n, **a).id
-            if k:
-                resource_args[k] = id
+    def _handle_internal_object(self, objectType: str, args: object):
+        if isinstance(args, dict):
+            return CDK._create_resource_from_dict(self, objectType, args)
+
+        return CDK._create_resource_from_args(self, objectType, args)
+
+    def _create_dependency(self, depName, depValue, resource_args, parentName):
+        _class, _className, _classAttributes = CDK._create_default_resource(
+            self, depValue['resource'], parentName,
+        )
+        id = _class(self, _className, **_classAttributes).id
+        if depName:
+            resource_args[depName] = id
 
-            CDK._parentStack.remove(d['resource'])
+        CDK._parentStack.remove(depValue['resource'])
```

### Comparing `thipster-0.14.0/thipster.egg-info/PKG-INFO` & `thipster-0.14.2/thipster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.0
+Version: 0.14.2
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -19,15 +19,15 @@
 
 Written entirely in Python, it leverages the Python CDK for Terraform to create Terraform files and apply them to the chosen provider.
 
 ## Technology Stack
 Written in Python 3.11, thipster is designed as a python package, to be used either as a standalone tool, or as a module inside a running process like a CI/CD pipeline.
 
 ## Project Status
-THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](CHANGELOG.md) for more details.
+THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster/blob/main/CHANGELOG.md) for more details.
 
 ## Dependencies
 
 In order to user THipster, you will need to have the following installed:
 - [Python](https://www.python.org/downloads/) (3.11+)
 - [pipenv](https://pipenv.pypa.io/en/latest/) v2021.5+
 - [Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) (1.2+)
@@ -89,20 +89,19 @@
 To install the project for development, you can use the following command:
 
 ```console
 pip install -r requirements.txt && pip install -e .[dev,test,doc]
 pre-commit install && pre-commit run --all-files
 ```
 
-For more information on how to help out, please check the [CONTRIBUTING](CONTRIBUTING.md) file.
+For more information on how to help out, please check the [CONTRIBUTING](https://github.com/THipster/THipster/blob/main/CONTRIBUTING.md) file.
 
 ## Open source licensing info
-1. [TERMS](TERMS.md)
-2. [LICENSE](LICENSE)
-3. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
+1. [LICENSE](https://github.com/THipster/THipster/blob/main/LICENSE)
+2. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
 
 ## Credits and references
 
 1. Projects that inspired you
     - [AWS Application Composer](https://aws.amazon.com/application-composer/?nc1=h_ls)
 2. Related projects
     - [Wing Programming Language](https://www.winglang.io/)
```

### Comparing `thipster-0.14.0/thipster.egg-info/SOURCES.txt` & `thipster-0.14.2/thipster.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,35 +21,36 @@
 thipster/__init__.py
 thipster/helpers.py
 thipster.egg-info/PKG-INFO
 thipster.egg-info/SOURCES.txt
 thipster.egg-info/dependency_links.txt
 thipster.egg-info/requires.txt
 thipster.egg-info/top_level.txt
-thipster/auth/Google.py
 thipster/auth/__init__.py
-thipster/engine/Engine.py
-thipster/engine/I_Auth.py
-thipster/engine/I_Parser.py
-thipster/engine/I_Repository.py
-thipster/engine/I_Terraform.py
-thipster/engine/ParsedFile.py
-thipster/engine/ResourceModel.py
+thipster/auth/google.py
 thipster/engine/__init__.py
-thipster/parser/ParserFactory.py
-thipster/parser/YAMLParser.py
+thipster/engine/engine.py
+thipster/engine/i_auth.py
+thipster/engine/i_parser.py
+thipster/engine/i_repository.py
+thipster/engine/i_terraform.py
+thipster/engine/parsed_file.py
+thipster/engine/resource_model.py
 thipster/parser/__init__.py
-thipster/parser/dsl_parser/AST.py
-thipster/parser/dsl_parser/DSLExceptions.py
-thipster/parser/dsl_parser/DSLParser.py
-thipster/parser/dsl_parser/Interpreter.py
-thipster/parser/dsl_parser/Lexer.py
-thipster/parser/dsl_parser/LexerPosition.py
-thipster/parser/dsl_parser/Token.py
-thipster/parser/dsl_parser/TokenParser.py
+thipster/parser/parser_factory.py
+thipster/parser/yaml_parser.py
 thipster/parser/dsl_parser/__init__.py
-thipster/repository/GithubRepo.py
-thipster/repository/JSONRepo.py
-thipster/repository/LocalRepo.py
+thipster/parser/dsl_parser/ast.py
+thipster/parser/dsl_parser/exceptions.py
+thipster/parser/dsl_parser/interpreter.py
+thipster/parser/dsl_parser/lexer.py
+thipster/parser/dsl_parser/lexer_position.py
+thipster/parser/dsl_parser/parser.py
+thipster/parser/dsl_parser/token.py
+thipster/parser/dsl_parser/token_parser.py
 thipster/repository/__init__.py
-thipster/terraform/CDK.py
-thipster/terraform/__init__.py
+thipster/repository/github.py
+thipster/repository/json.py
+thipster/repository/local.py
+thipster/terraform/__init__.py
+thipster/terraform/cdk.py
+thipster/terraform/exceptions.py
```

