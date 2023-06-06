# Comparing `tmp/thipster-0.13.6.tar.gz` & `tmp/thipster-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.13.6.tar", last modified: Wed May 31 13:17:02 2023, max compression
+gzip compressed data, was "thipster-0.14.0.tar", last modified: Tue Jun  6 08:10:01 2023, max compression
```

## Comparing `thipster-0.13.6.tar` & `thipster-0.14.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.670935 thipster-0.13.6/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-31 13:17:00.000000 thipster-0.13.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 13:17:02.670935 thipster-0.13.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-31 13:17:00.000000 thipster-0.13.6/README.md
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-31 13:17:00.000000 thipster-0.13.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-31 13:17:00.000000 thipster-0.13.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 13:17:02.670935 thipster-0.13.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1057 2023-05-31 13:17:00.000000 thipster-0.13.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13247 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/thipster/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      799 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/auth/Google.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.666935 thipster-0.13.6/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)     3472 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/Engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Auth.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Parser.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Repository.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Terraform.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/ParsedFile.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/ResourceModel.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.666935 thipster-0.13.6/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.666935 thipster-0.13.6/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)    10350 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/AST.py
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/DSLExceptions.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/DSLParser.py
--rw-r--r--   0 root         (0) root         (0)    13788 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/Interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17548 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/Lexer.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/LexerPosition.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/Token.py
--rw-r--r--   0 root         (0) root         (0)    20153 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/TokenParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.670935 thipster-0.13.6/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/GithubRepo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/JSONRepo.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/LocalRepo.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.670935 thipster-0.13.6/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)    11680 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/terraform/CDK.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/terraform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      225 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-06 08:09:58.000000 thipster-0.14.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-06 08:09:58.000000 thipster-0.14.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-06-06 08:10:01.380800 thipster-0.14.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-06-06 08:09:58.000000 thipster-0.14.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      867 2023-06-06 08:09:58.000000 thipster-0.14.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-06 08:09:58.000000 thipster-0.14.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 08:10:01.380800 thipster-0.14.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-06 08:09:59.000000 thipster-0.14.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.372800 thipster-0.14.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.372800 thipster-0.14.0/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.372800 thipster-0.14.0/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13247 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-06-06 08:09:58.000000 thipster-0.14.0/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/auth/Google.py
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)     3340 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/Engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Auth.py
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Parser.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Repository.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/I_Terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/ParsedFile.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/ResourceModel.py
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     6283 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/AST.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/DSLExceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/DSLParser.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/Interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/Lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/LexerPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/Token.py
+-rw-r--r--   0 root         (0) root         (0)    20153 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/TokenParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/parser/dsl_parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/GithubRepo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/JSONRepo.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/LocalRepo.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.380800 thipster-0.14.0/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)    12057 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/terraform/CDK.py
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-06 08:09:58.000000 thipster-0.14.0/thipster/terraform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:10:01.376800 thipster-0.14.0/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-06 08:10:01.000000 thipster-0.14.0/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.13.6/PKG-INFO` & `thipster-0.14.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,94 @@
-Metadata-Version: 2.1
-Name: thipster
-Version: 0.13.6
-Home-page: https://github.com/THipster/THipster
-Download-URL: https://github.com/THipster/THipster.git
-Classifier: Development Status :: 1 - Planning
-Classifier: Programming Language :: Python
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: doc
-
 # THipster
 
-THipster is a CLI tool dedicated to simplifying the ordeal associated with writing Terraform files.
+THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files.
 It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 
 Written entirely in Python, it leverages the Python CDK for Terraform to create Terraform files and apply them to the chosen provider.
 
-### Table of contents
-[Technology Stack](#technology-stack)
-
-[Project Status](#project-status)
-
-[Dependencies](#dependencies)
-
-[Installation](#installation)
-
-[Usage](#usage)
-
-[Test the software](#how-to-test-the-software)
-
-[Known issues](#knwon-issues)
-
-[Getting help](#getting-help)
-
-[Getting involved](#getting-involved)
-
 ## Technology Stack
 Written in Python 3.11, thipster is designed as a python package, to be used either as a standalone tool, or as a module inside a running process like a CI/CD pipeline.
 
 ## Project Status
 THipster is currently in an active development state. If you want to know more, please check the [CHANGELOG](CHANGELOG.md) for more details.
 
 ## Dependencies
 
-*Describe any dependencies that must be installed for this software to work.
-This includes programming languages, databases or other storage mechanisms, build tools, frameworks, and so forth.
-If specific versions of other software are required, or known not to work, call that out.*
+In order to user THipster, you will need to have the following installed:
+- [Python](https://www.python.org/downloads/) (3.11+)
+- [pipenv](https://pipenv.pypa.io/en/latest/) v2021.5+
+- [Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) (1.2+)
+- [Node.js](https://nodejs.org/) and npm v16+.
 
 ## Installation
 
-*Detailed instructions on how to install, configure, and get the project running.
-This should be frequently tested to ensure reliability. Alternatively, link to
-a separate [INSTALL](INSTALL.md) document.*
+To use THipster, you can simply install the package with pip:
+
+```console
+pip install thipster
+```
+
+The list of available versions can be found on [PyPI](https://pypi.org/project/thipster/).
 
 ## Usage
 
-*Show users how to use the software.
-Be specific.
-Use appropriate formatting when showing code snippets.*
+You can use THipster in two ways:
+- By leveraging the [THipster CLI](https://github.com/THipster/THipster-cli)
+- By directly using the [THipster Python package](https://pypi.org/project/thipster/) in your own code
+
+Main feature:
+- Generate Terraform files from a YAML+JINJA or THIPS file:
+```python
+from thipster.engine.Engine import Engine as ThipsterEngine
+from thipster.repository.GithubRepo import GithubRepo
+from thipster.parser.ParserFactory import ParserFactory
+from thipster.auth.Google import GoogleAuth
+from thipster.terraform.CDK import CDK
+
+# create new THipster engine
+engine = ThipsterEngine(ParserFactory(), GithubRepo('THipster/models'), GoogleAuth, CDK())
+
+# generate Terraform files and plan from a YAML+JINJA file
+
+list_dir, tf_plan = engine.run('path/to/file/or/directory')
+print(tf_plan)
+```
 
 ## How to test the software
 
-*If the software includes automated tests, detail how to run those tests.*
+To run the tests, you can use the following command:
+
+```console
+pip install -e .[test]
+pytest tests
+```
 
 ## Known issues
 
-*Document any known significant shortcomings with the software.*
+All known issues, bugs, and feature requests are tracked in the [Issue tracker](https://github.com/THipster/THipster/issues).
 
 ## Getting help
 
-If you have questions, concerns, bug reports, etc, please file an issue in this repository's Issue Tracker.
+If you have questions, concerns, bug reports, etc, please file an issue in this repository's [Issue tracker](https://github.com/THipster/THipster/issues).
 
 ## Getting involved
 
-*This section should detail why people should get involved and describe key areas you are
-currently focusing on; e.g., trying to get feedback on features, fixing certain bugs, building
-important pieces, etc.*
-
-*General instructions on _how_ to contribute should be stated with a link to [CONTRIBUTING](CONTRIBUTING.md).*
+To install the project for development, you can use the following command:
 
+```console
+pip install -r requirements.txt && pip install -e .[dev,test,doc]
+pre-commit install && pre-commit run --all-files
+```
 
-----
+For more information on how to help out, please check the [CONTRIBUTING](CONTRIBUTING.md) file.
 
 ## Open source licensing info
-*1. [TERMS](TERMS.md)
+1. [TERMS](TERMS.md)
 2. [LICENSE](LICENSE)
-3. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)*
-
-
-----
+3. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
 
 ## Credits and references
 
-*1. Projects that inspired you
+1. Projects that inspired you
+    - [AWS Application Composer](https://aws.amazon.com/application-composer/?nc1=h_ls)
 2. Related projects
-3. Books, papers, talks, or other sources that have meaningful impact or influence on this project*
+    - [Wing Programming Language](https://www.winglang.io/)
```

### Comparing `thipster-0.13.6/pyproject.toml` & `thipster-0.14.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/setup.py` & `thipster-0.14.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.13.6'
+__version__ = '0.14.0'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md") as rm:
     readme = rm.read()
 
 setup(
     name="thipster",
     authors=[
         {"name": "rcattin", "email": "rafa.cattin+thipster@gmail.com"},
         {"name": "gsuquet", "email": "gsuquet@ippon.fr"},
     ],
-    description="",
+    description="THipster is a tool dedicated to simplifying the difficulty associated \
+with writing Terraform files. It allows users to write infrastructure as code in a \
+simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.",
     long_description=readme,
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python",
     ],
 
     download_url="https://github.com/THipster/THipster.git",
     url="https://github.com/THipster/THipster",
@@ -38,10 +41,11 @@
             'pytest',
             'pytest-mock',
             'dagger.io',
             'pre-commit',
         ],
         'doc': [
             'sphinx',
+            'myst-parser',
         ],
     },
 )
```

### Comparing `thipster-0.13.6/tests/engine/test_engine.py` & `thipster-0.14.0/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.14.0/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/dsl_parser/test_ast.py` & `thipster-0.14.0/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.14.0/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/dsl_parser/test_token.py` & `thipster-0.14.0/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.14.0/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/test_ParserFactory.py` & `thipster-0.14.0/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/test_YAMLParser.py` & `thipster-0.14.0/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/tests/parser/test_parsedfile.py` & `thipster-0.14.0/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/auth/Google.py` & `thipster-0.14.0/thipster/auth/Google.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import google.auth
 from thipster.engine.I_Auth import I_Auth
 from cdktf_cdktf_provider_google.provider import GoogleProvider
 
 
 class GoogleAuth(I_Auth):
     """Authentication to GCP Projects
-
-    Methods
-    -------
-    authenticate(app: Construct)
-        Generates the google provider in terraform
-
     """
 
     def __init__(self) -> None:
         return GoogleAuth
 
     def authenticate(app):
         """Generates the google provider block for the Terraform CDK
```

### Comparing `thipster-0.13.6/thipster/engine/Engine.py` & `thipster-0.14.0/thipster/engine/Engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 
 
 class Engine():
     """The engine of thipster
 
     The core of the application, it is used to call and link all
     interfaces together.
-
-    Methods
-    -------
-    run(filename: str)
-        Processes a fileName and creates the corresponding Cloud architecture plan
-
     """
 
     importedPackages = []
 
     def __init__(
             self, parser: I_Parser,
             repository: I_Repository,
```

### Comparing `thipster-0.13.6/thipster/engine/I_Terraform.py` & `thipster-0.14.0/thipster/engine/I_Terraform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 from abc import ABC, abstractmethod
 import thipster.engine.ResourceModel as rm
 import thipster.engine.ParsedFile as pf
 
 
 class I_Terraform(ABC):
     """Terraform module interface
-
-    Methods
-    -------
-    generate()
-        Generates Terraform code from parsed file and models
-    plan()
-        Get plan from generated terraform code
-    apply()
-        Apply generated terraform code
-
     """
     @abstractmethod
     def apply(self):
         """Apply generated terraform code
 
         Raises
         ------
```

### Comparing `thipster-0.13.6/thipster/engine/ParsedFile.py` & `thipster-0.14.0/thipster/engine/ParsedFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 """
 
 from abc import ABC, abstractmethod
 
 
 class I_ParsedValue(ABC):
     """Parsed Value Interface
-
-    Attributes
-    ----------
-    value
     """
 
     @property
     @abstractmethod
     def value(self):
         """Abstract value attribute
         """
@@ -22,20 +18,14 @@
 
 
 class Position():
     """Class representing the position of a token
 
     Indicates the initial position of a token, resource or character in the input files.
     It includes the file name, line and column numbers of the designated element.
-
-    Attributes
-    ----------
-    fileName
-    ln
-    col
     """
 
     def __init__(self, fileName: str, ln: int, col: int):
         """
         Parameters
         ----------
         fileName : str
```

### Comparing `thipster-0.13.6/thipster/engine/ResourceModel.py` & `thipster-0.14.0/thipster/engine/ResourceModel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/ParserFactory.py` & `thipster-0.14.0/thipster/parser/ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/YAMLParser.py` & `thipster-0.14.0/thipster/parser/YAMLParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             A ParsedAttribute object with wanted value type
         """
         if type(value) == dict:
             val = YAMLParser.__get_dict(value)
         elif type(value) == list:
             val = YAMLParser.__get_list(value)
         else:
-            val = pf.ParsedLiteral(str(value))
+            val = pf.ParsedLiteral(value)
 
         return pf.ParsedAttribute(
             name=name,
             value=val,
             position=None,
         )
```

### Comparing `thipster-0.13.6/thipster/parser/dsl_parser/AST.py` & `thipster-0.14.0/thipster/parser/dsl_parser/AST.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/dsl_parser/DSLParser.py` & `thipster-0.14.0/thipster/parser/dsl_parser/DSLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/dsl_parser/Interpreter.py` & `thipster-0.14.0/thipster/parser/dsl_parser/Interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/dsl_parser/Lexer.py` & `thipster-0.14.0/thipster/parser/dsl_parser/Lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/dsl_parser/LexerPosition.py` & `thipster-0.14.0/thipster/parser/dsl_parser/LexerPosition.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/dsl_parser/Token.py` & `thipster-0.14.0/thipster/parser/dsl_parser/Token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/parser/dsl_parser/TokenParser.py` & `thipster-0.14.0/thipster/parser/dsl_parser/TokenParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/repository/GithubRepo.py` & `thipster-0.14.0/thipster/repository/GithubRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/repository/JSONRepo.py` & `thipster-0.14.0/thipster/repository/JSONRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.6/thipster/terraform/CDK.py` & `thipster-0.14.0/thipster/terraform/CDK.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,28 +350,36 @@
 
     def _handle_internal_object(
         self,
         model: rm.ResourceModel,
         attribute: pf.ParsedAttribute,
         resource_args: dict,
     ):
-        res = CDK._create_resource_from_args(
-            self,
-            model.internalObjects[attribute.name]['resource'],
-            attribute.value,
-        )
-
         int_obj = model.internalObjects[attribute.name]
         var_type = int_obj['var_type'] if 'var_type' in int_obj else 'Unknown'
 
         if 'list' in var_type:
             if attribute.name not in resource_args:
                 resource_args[attribute.name] = []
-            resource_args[attribute.name] += [res]
+
+            if isinstance(attribute.value[0], pf.ParsedDict):
+                for internalObject in attribute.value:
+                    res = CDK._create_resource_from_args(
+                        self,
+                        model.internalObjects[attribute.name]['resource'],
+                        internalObject.value,
+                    )
+
+                    resource_args[attribute.name] += [res]
         else:
+            res = CDK._create_resource_from_args(
+                self,
+                model.internalObjects[attribute.name]['resource'],
+                attribute.value,
+            )
             resource_args[attribute.name] = res
 
         return resource_args
 
     def _create_dependencies(self, deps, resource_args, name):
         for k, d in deps.items():
             c, n, a = CDK._create_default_resource(self, d['resource'], name)
```

### Comparing `thipster-0.13.6/thipster.egg-info/SOURCES.txt` & `thipster-0.14.0/thipster.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 tests/__init__.py
 tests/test_e2e.py
```

