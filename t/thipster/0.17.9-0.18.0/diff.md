# Comparing `tmp/thipster-0.17.9.tar.gz` & `tmp/thipster-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.17.9.tar", last modified: Thu Jun 22 14:29:32 2023, max compression
+gzip compressed data, was "thipster-0.18.0.tar", last modified: Thu Jun 22 15:59:32 2023, max compression
```

## Comparing `thipster-0.17.9.tar` & `thipster-0.18.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.127874 thipster-0.17.9/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 14:29:27.000000 thipster-0.17.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 14:29:27.000000 thipster-0.17.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 14:29:32.127874 thipster-0.17.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-22 14:29:27.000000 thipster-0.17.9/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-22 14:29:27.000000 thipster-0.17.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-22 14:29:27.000000 thipster-0.17.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:29:32.127874 thipster-0.17.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-22 14:29:28.000000 thipster-0.17.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.111874 thipster-0.17.9/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.111874 thipster-0.17.9/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3466 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.111874 thipster-0.17.9/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.115874 thipster-0.17.9/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    16811 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    15104 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.115874 thipster-0.17.9/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     6483 2023-06-22 14:29:27.000000 thipster-0.17.9/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.115874 thipster-0.17.9/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.119874 thipster-0.17.9/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.123874 thipster-0.17.9/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     5081 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.123874 thipster-0.17.9/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.123874 thipster-0.17.9/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    16910 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    21596 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.127874 thipster-0.17.9/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.127874 thipster-0.17.9/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22517 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-22 14:29:27.000000 thipster-0.17.9/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:29:32.119874 thipster-0.17.9/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 14:29:32.000000 thipster-0.17.9/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-22 14:29:32.000000 thipster-0.17.9/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:29:32.000000 thipster-0.17.9/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-22 14:29:32.000000 thipster-0.17.9/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 14:29:32.000000 thipster-0.17.9/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.581946 thipster-0.18.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 15:59:28.000000 thipster-0.18.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 15:59:28.000000 thipster-0.18.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 15:59:32.581946 thipster-0.18.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-22 15:59:28.000000 thipster-0.18.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-22 15:59:28.000000 thipster-0.18.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-22 15:59:28.000000 thipster-0.18.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 15:59:32.581946 thipster-0.18.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-22 15:59:29.000000 thipster-0.18.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.573946 thipster-0.18.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.573946 thipster-0.18.0/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.573946 thipster-0.18.0/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.573946 thipster-0.18.0/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    16811 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    15104 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.573946 thipster-0.18.0/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2023-06-22 15:59:28.000000 thipster-0.18.0/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.573946 thipster-0.18.0/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.577946 thipster-0.18.0/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.577946 thipster-0.18.0/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5610 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.577946 thipster-0.18.0/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.581946 thipster-0.18.0/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    16910 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    21596 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.581946 thipster-0.18.0/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.581946 thipster-0.18.0/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22746 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-22 15:59:28.000000 thipster-0.18.0/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:59:32.577946 thipster-0.18.0/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-22 15:59:32.000000 thipster-0.18.0/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-22 15:59:32.000000 thipster-0.18.0/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 15:59:32.000000 thipster-0.18.0/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-22 15:59:32.000000 thipster-0.18.0/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 15:59:32.000000 thipster-0.18.0/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.17.9/LICENSE` & `thipster-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/PKG-INFO` & `thipster-0.18.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.9
+Version: 0.18.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.9 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.18.0 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.9/README.md` & `thipster-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/pyproject.toml` & `thipster-0.18.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/setup.py` & `thipster-0.18.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.17.9'
+__version__ = '0.18.0'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.17.9/tests/engine/test_engine.py` & `thipster-0.18.0/tests/engine/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,30 +58,30 @@
         return {}
 
 
 class MockTerraform(eng.TerraformPort):
     """Mock engine terraform port."""
 
     @logger('- Terraform:apply')
-    def apply(self):
+    def apply(self, file):
         """Mock the terraform apply method."""
         pass
 
     @logger('- Terraform:generate')
     def generate(self, a, b, auth):
         """Mock the terraform generate method."""
         pass
 
     @logger('- Terraform:init')
     def init(self):
         """Mock the terraform init method."""
         pass
 
     @logger('- Terraform:plan')
-    def plan(self):
+    def plan(self, file):
         """Mock the terraform plan method."""
         pass
 
 
 def test_engine_calls():
     """Test the engine calls."""
     parser = MockParser()
```

### Comparing `thipster-0.17.9/tests/engine/test_generation.py` & `thipster-0.18.0/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/dsl_parser/test_ast.py` & `thipster-0.18.0/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.18.0/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.18.0/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/dsl_parser/test_token.py` & `thipster-0.18.0/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.18.0/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/test_parsedfile.py` & `thipster-0.18.0/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/test_parserfactory.py` & `thipster-0.18.0/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/parser/test_yamlparser.py` & `thipster-0.18.0/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/repository/test_github_repository.py` & `thipster-0.18.0/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/repository/test_local_repository.py` & `thipster-0.18.0/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/repository/test_resourcemodel.py` & `thipster-0.18.0/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/test_e2e.py` & `thipster-0.18.0/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/tests/test_tools.py` & `thipster-0.18.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/auth/google.py` & `thipster-0.18.0/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/engine/engine.py` & `thipster-0.18.0/thipster/engine/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from .i_auth import AuthPort
 from .i_parser import ParserPort
 from .i_repository import RepositoryPort
 from .i_terraform import TerraformPort
 from .resource_model import ResourceModel
 
+terraform_plan_file = 'thipster.tfplan'
+
 
 class Engine():
     """THipster's Engine.
 
     The core of the application, it is used to call and link all
     interfaces together.
     """
@@ -116,15 +118,15 @@
         models = self.get_models(parsed_file)
 
         # Generate Terraform files
         self.generate_tf_files(parsed_file, models)
 
         self.__terraform.init()
 
-        return self.__terraform.plan()
+        return self.__terraform.plan(terraform_plan_file)
 
     def parse_files(self, path: str) -> pf.ParsedFile:
         """Parse the input file or directory.
 
         Parameters
         ----------
         path : str
@@ -172,26 +174,36 @@
         """
         self.__terraform.generate(file, models, self.__auth)
 
     def init_terraform(self) -> None:
         """Initialize Terraform."""
         self.__terraform.init()
 
-    def plan_terraform(self) -> str:
+    def plan_terraform(self, plan_file_path: str = terraform_plan_file) -> str:
         """Plan Terraform.
 
+        Parameters
+        ----------
+        plan_file_path : str, optional
+            The path of the plan file, by default thipster.tfplan
+
         Returns
         -------
         str
             The results of the Terraform plan
         """
-        return self.__terraform.plan()
+        return self.__terraform.plan(plan_file_path)
 
-    def apply_terraform(self) -> str:
+    def apply_terraform(self, plan_file_path: str = terraform_plan_file) -> str:
         """Apply Terraform.
 
+        Parameters
+        ----------
+        plan_file_path : str, optional
+            The path of the plan file, by default thipster.tfplan
+
         Returns
         -------
         str
             The results of the Terraform apply
         """
-        return self.__terraform.apply()
+        return self.__terraform.apply(plan_file_path)
```

### Comparing `thipster-0.17.9/thipster/engine/i_parser.py` & `thipster-0.18.0/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/engine/i_repository.py` & `thipster-0.18.0/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/engine/i_terraform.py` & `thipster-0.18.0/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/engine/parsed_file.py` & `thipster-0.18.0/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/engine/resource_model.py` & `thipster-0.18.0/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/helpers.py` & `thipster-0.18.0/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/ast.py` & `thipster-0.18.0/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.18.0/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.18.0/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/lexer.py` & `thipster-0.18.0/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.18.0/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/parser.py` & `thipster-0.18.0/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/token.py` & `thipster-0.18.0/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.18.0/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/exceptions.py` & `thipster-0.18.0/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/parser_factory.py` & `thipster-0.18.0/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/parser/yaml_parser.py` & `thipster-0.18.0/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/repository/exceptions.py` & `thipster-0.18.0/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/repository/github.py` & `thipster-0.18.0/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/repository/json.py` & `thipster-0.18.0/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/repository/local.py` & `thipster-0.18.0/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster/terraform/cdk.py` & `thipster-0.18.0/thipster/terraform/cdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,30 +132,34 @@
     _resources_to_create: list[ResourceCreationContext] = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = create_logger(__name__)
 
     @classmethod
-    def apply(cls, plan_file_path: str | None = None):
+    def apply(cls, plan_file_path: str):
         """Apply generated Terraform plan.
 
         Parameters
         ----------
-        plan_file_path : str, optional
-            Path to the plan file, default None
+        plan_file_path : str
+            Path to the plan file
 
         Returns
         -------
         str
             Terraform apply output
         """
-        t = Terraform()
-        _, stdout, stderr = t.apply(plan_file_path)
-        return stdout + stderr
+        output = subprocess.run(
+            ['terrraform', 'apply', plan_file_path],
+            shell=True,
+            capture_output=True,
+            encoding='utf-8',
+        )
+        return output.stdout + output.stderr
 
     @classmethod
     def generate(
         cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
         _authenticator: AuthPort,
     ):
         """Generate Terraform file from given parsed file and models.
@@ -241,28 +245,33 @@
 
         Returns
         -------
         str
             Terraform init output
         """
         t = Terraform()
-        _, stdout, stderr = t.init()
+        _, stdout, stderr = t.init(upgrade=True)
         return stdout + stderr
 
     @classmethod
-    def plan(cls):
+    def plan(cls, plan_file_path: str):
         """Get plan from generated terraform code.
 
+        Parameters
+        ----------
+        plan_file_path : str
+            Path and name of the plan file
+
         Returns
         -------
         str
             Terraform plan output
         """
         t = Terraform()
-        _, stdout, stderr = t.plan(out='thipster.tfplan')
+        _, stdout, stderr = t.plan(out=plan_file_path)
         return stdout + stderr
 
     @classmethod
     def _pip_install(cls, package: str):
         """Install a package if it wasn't already installed by thipster.
 
         Parameters
@@ -420,15 +429,15 @@
     ctx.no_modif = True
     ctx.no_dependencies = False
 
     # Process attributes
     def attributes(attribute_list: list[pf.ParsedAttribute]):
         for attribute in attribute_list:
             if attribute.name == ctx.model.name_key:
-                ctx.resource_args[ctx.model.name_key] = attribute.name
+                ctx.resource_args[ctx.model.name_key] = attribute.value
             else:
                 _process_attribute(ctx, attribute)
 
     attributes(input_args)
     attributes(CDK._inherited_attributes)
 
     CDK._inherited_attributes += input_args
@@ -545,15 +554,15 @@
     # Checks if attribute is expected as an attibute
     if attribute.name not in ctx.model.attributes:
         return
 
     # Processes list attribute
     attribute_value = attribute.value
     if ctx.model.attributes[attribute.name].is_list:
-        if type(attribute.value) is list:
+        if isinstance(attribute.value, list):
             attribute_value = [i.value for i in attribute.value]
         else:
             attribute_value = [attribute.value]
 
     # Sets attribute value
     ctx.resource_args[ctx.model.attributes[attribute.name].cdk_name] = attribute_value
```

### Comparing `thipster-0.17.9/thipster/terraform/exceptions.py` & `thipster-0.18.0/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.9/thipster.egg-info/PKG-INFO` & `thipster-0.18.0/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.9
+Version: 0.18.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.9 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.18.0 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.9/thipster.egg-info/SOURCES.txt` & `thipster-0.18.0/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

