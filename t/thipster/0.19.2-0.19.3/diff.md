# Comparing `tmp/thipster-0.19.2.tar.gz` & `tmp/thipster-0.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.19.2.tar", last modified: Fri Jun 23 14:07:38 2023, max compression
+gzip compressed data, was "thipster-0.19.3.tar", last modified: Fri Jun 23 15:12:21 2023, max compression
```

## Comparing `thipster-0.19.2.tar` & `thipster-0.19.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.759747 thipster-0.19.2/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-23 14:07:33.000000 thipster-0.19.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-23 14:07:33.000000 thipster-0.19.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-23 14:07:38.759747 thipster-0.19.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-23 14:07:33.000000 thipster-0.19.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-23 14:07:33.000000 thipster-0.19.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-23 14:07:33.000000 thipster-0.19.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 14:07:38.759747 thipster-0.19.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-23 14:07:34.000000 thipster-0.19.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.747747 thipster-0.19.2/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.747747 thipster-0.19.2/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.747747 thipster-0.19.2/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.747747 thipster-0.19.2/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    16811 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    15104 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.751747 thipster-0.19.2/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     6483 2023-06-23 14:07:33.000000 thipster-0.19.2/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.751747 thipster-0.19.2/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.751747 thipster-0.19.2/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.751747 thipster-0.19.2/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5610 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     5081 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.755747 thipster-0.19.2/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.755747 thipster-0.19.2/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    16910 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    21596 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.755747 thipster-0.19.2/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.759747 thipster-0.19.2/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23588 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-23 14:07:33.000000 thipster-0.19.2/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:07:38.751747 thipster-0.19.2/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-23 14:07:38.000000 thipster-0.19.2/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-23 14:07:38.000000 thipster-0.19.2/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:07:38.000000 thipster-0.19.2/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-23 14:07:38.000000 thipster-0.19.2/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-23 14:07:38.000000 thipster-0.19.2/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.524669 thipster-0.19.3/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-23 15:12:17.000000 thipster-0.19.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-23 15:12:17.000000 thipster-0.19.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-23 15:12:21.524669 thipster-0.19.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-23 15:12:17.000000 thipster-0.19.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-23 15:12:17.000000 thipster-0.19.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-23 15:12:17.000000 thipster-0.19.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:12:21.524669 thipster-0.19.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-23 15:12:18.000000 thipster-0.19.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.512668 thipster-0.19.3/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.512668 thipster-0.19.3/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.512668 thipster-0.19.3/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.516669 thipster-0.19.3/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    16811 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    15104 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.516669 thipster-0.19.3/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2023-06-23 15:12:17.000000 thipster-0.19.3/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.516669 thipster-0.19.3/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.516669 thipster-0.19.3/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.520669 thipster-0.19.3/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5610 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.520669 thipster-0.19.3/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.524669 thipster-0.19.3/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    16910 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    21596 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.524669 thipster-0.19.3/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.524669 thipster-0.19.3/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24574 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-23 15:12:17.000000 thipster-0.19.3/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:12:21.516669 thipster-0.19.3/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-23 15:12:21.000000 thipster-0.19.3/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-23 15:12:21.000000 thipster-0.19.3/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:12:21.000000 thipster-0.19.3/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-23 15:12:21.000000 thipster-0.19.3/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-23 15:12:21.000000 thipster-0.19.3/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.19.2/LICENSE` & `thipster-0.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/PKG-INFO` & `thipster-0.19.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.19.2
+Version: 0.19.3
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
-Metadata-Version: 2.1 Name: thipster Version: 0.19.2 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.19.3 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.19.2/README.md` & `thipster-0.19.3/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/pyproject.toml` & `thipster-0.19.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/setup.py` & `thipster-0.19.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.19.2'
+__version__ = '0.19.3'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.19.2/tests/engine/test_engine.py` & `thipster-0.19.3/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/engine/test_generation.py` & `thipster-0.19.3/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/dsl_parser/test_ast.py` & `thipster-0.19.3/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.19.3/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.19.3/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/dsl_parser/test_token.py` & `thipster-0.19.3/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.19.3/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/test_parsedfile.py` & `thipster-0.19.3/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/test_parserfactory.py` & `thipster-0.19.3/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/parser/test_yamlparser.py` & `thipster-0.19.3/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/repository/test_github_repository.py` & `thipster-0.19.3/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/repository/test_local_repository.py` & `thipster-0.19.3/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/repository/test_resourcemodel.py` & `thipster-0.19.3/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/test_e2e.py` & `thipster-0.19.3/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/tests/test_tools.py` & `thipster-0.19.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/auth/google.py` & `thipster-0.19.3/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/engine/engine.py` & `thipster-0.19.3/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/engine/i_parser.py` & `thipster-0.19.3/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/engine/i_repository.py` & `thipster-0.19.3/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/engine/i_terraform.py` & `thipster-0.19.3/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/engine/parsed_file.py` & `thipster-0.19.3/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/engine/resource_model.py` & `thipster-0.19.3/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/helpers.py` & `thipster-0.19.3/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/ast.py` & `thipster-0.19.3/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.19.3/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.19.3/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/lexer.py` & `thipster-0.19.3/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.19.3/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/parser.py` & `thipster-0.19.3/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/token.py` & `thipster-0.19.3/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.19.3/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/exceptions.py` & `thipster-0.19.3/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/parser_factory.py` & `thipster-0.19.3/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/parser/yaml_parser.py` & `thipster-0.19.3/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/repository/exceptions.py` & `thipster-0.19.3/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/repository/github.py` & `thipster-0.19.3/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/repository/json.py` & `thipster-0.19.3/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/repository/local.py` & `thipster-0.19.3/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster/terraform/cdk.py` & `thipster-0.19.3/thipster/terraform/cdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -542,23 +542,16 @@
     ----------
     ctx: ResourceCreationContext
         Context from which the resource is created
     attribute : ParsedAttribute
         Attribute to process
     """
     if not ctx.no_dependencies and attribute.name in ctx.dependencies:
-        # Test for attribute
-        resource_value, resource_attribute = attribute.value, 'id'
-        if isinstance(resource_value, str):
-            split = resource_value.split('.', maxsplit=1)
-            resource_value = split[0]
-            resource_attribute = split[1] if len(split) > 1 else 'id'
-
         _check_explicit_dependency(
-            ctx, attribute.name, resource_value, resource_attribute,
+            ctx, attribute.name, attribute.value,
         )
         del ctx.dependencies[attribute.name]
         return
 
     # Checks if attribute is an internal object
     if attribute.name in ctx.model.internal_objects:
         _create_internal_object(
@@ -651,26 +644,34 @@
         if 'var_type' in internal_object_model else 'Unknown'
 
     if internal_object_type.startswith('list') or internal_object_model['is_list']:
         if internal_object_name not in ctx.resource_args\
                 and not internal_object_base_ctx.arg_to_complete:
             ctx.resource_args[internal_object_name] = []
 
-        if isinstance(internal_object_args, list) \
-                and isinstance(internal_object_args[0], pf.ParsedDict):
-
+        if isinstance(internal_object_args, list)\
+                and not isinstance(internal_object_args[0], pf.ParsedAttribute):
             for internal_object in internal_object_args:
                 internal_object_ctx = copy.deepcopy(internal_object_base_ctx)
                 internal_object_ctx.regenerate()
-                res = _create_resource(
-                    internal_object_ctx,
-                    internal_object.value,
-                )
-                if not internal_object_base_ctx.arg_to_complete:
-                    ctx.resource_args[internal_object_name] += [res]
+
+                if isinstance(internal_object, pf.ParsedDict):
+                    res = _create_resource(
+                        internal_object_ctx,
+                        internal_object.value,
+                    )
+                    if not internal_object_base_ctx.arg_to_complete:
+                        ctx.resource_args[internal_object_name] += [res]
+
+                elif isinstance(internal_object, pf.ParsedLiteral):
+                    _check_explicit_dependency(
+                        internal_object_ctx,
+                        internal_object_name,
+                        internal_object.value,
+                    )
 
             return True
 
         res = _create_resource(
             internal_object_base_ctx,
             internal_object_args,
         )
@@ -708,62 +709,89 @@
 
     ctx.no_modif = True
 
     # Process attributes
     def attributes(attribute_list: list[pf.ParsedAttribute]):
         for attribute in attribute_list:
             if attribute.name == ctx.model.name_key:
-                ctx.resource_args[ctx.model.name_key] = attribute.name
+                ctx.resource_args[ctx.model.name_key] = attribute.value
             else:
                 _process_attribute(ctx, attribute)
 
     if dependency_attributes:
         attributes(dependency_attributes)
     attributes(CDK._inherited_attributes)
 
     dependency = _instantiate_class(ctx)
     return dependency.id
 
 
 def _check_explicit_dependency(
     ctx: ResourceCreationContext, attribute_name: str, attribute_value: str | dict,
-    resource_attribute: str,
 ):
     """Check if a dependency attribute was explicited before.
 
     If it wasn't : create a default dependency.
 
     Parameters
     ----------
     ctx: ResourceCreationContext
         Context from which the resource is created
     attribute_name: str
         Name of the attribute to check
     attribute_value: str | dict
         Value of the attribute to check
     """
+    resource_attribute = 'id'
+    explicit_value = attribute_value
+    if isinstance(attribute_value, pf.ParsedLiteral):
+        explicit_value = attribute_value.value
+
+    if isinstance(explicit_value, str):
+        split = explicit_value.split('.', maxsplit=1)
+        explicit_value = split[0]
+        resource_attribute = split[1] if len(split) > 1 else 'id'
+
     dependency_type = ctx.dependencies[attribute_name]['resource']
-    created_name = f'{dependency_type}/{attribute_value}'
+    created_name = f'{dependency_type}/{explicit_value}'
 
     # Checks if attribute is an explicit dependency
     if created_name not in CDK._created_resources.keys():
 
-        if isinstance(attribute_value, str):
+        if isinstance(explicit_value, str):
             raise cdk_exceptions.CDKDependencyNotDeclaredError(
                 attribute_name, attribute_value,
             )
 
         dep_ctx = ResourceCreationContext.from_parent(
             ctx,
             resource_type=dependency_type,
         )
 
         # Creates explicit dependency
+        if (
+            isinstance(attribute_value, list)
+            and isinstance(attribute_value[0], pf.ParsedDict)
+        ):
+            ctx.resource_args[attribute_name] = []
+            for dict_value in attribute_value:
+                dep_ctx.regenerate()
+                ctx.resource_args[attribute_name].append(
+                    _create_dependency(
+                        dep_ctx, dict_value.value,
+                    ),
+                )
+            return True
+
         ctx.resource_args[attribute_name] = _create_dependency(
             dep_ctx, attribute_value,
         )
         return True
 
-    ctx.resource_args[attribute_name] = (
-        getattr(CDK._created_resources[created_name], resource_attribute)
+    resource = getattr(
+        CDK._created_resources[created_name], resource_attribute,
     )
+    if attribute_name in ctx.resource_args:
+        ctx.resource_args[attribute_name] += [resource]
+
+    ctx.resource_args[attribute_name] = resource
     return True
```

### Comparing `thipster-0.19.2/thipster/terraform/exceptions.py` & `thipster-0.19.3/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.2/thipster.egg-info/PKG-INFO` & `thipster-0.19.3/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.19.2
+Version: 0.19.3
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
-Metadata-Version: 2.1 Name: thipster Version: 0.19.2 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.19.3 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.19.2/thipster.egg-info/SOURCES.txt` & `thipster-0.19.3/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

