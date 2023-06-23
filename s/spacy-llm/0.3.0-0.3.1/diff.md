# Comparing `tmp/spacy-llm-0.3.0.tar.gz` & `tmp/spacy-llm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.3.0.tar", last modified: Wed Jun 14 09:34:09 2023, max compression
+gzip compressed data, was "spacy-llm-0.3.1.tar", last modified: Fri Jun 23 13:19:00 2023, max compression
```

## Comparing `spacy-llm-0.3.0.tar` & `spacy-llm-0.3.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    62271 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    61027 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      698 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1810 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.618001 spacy-llm-0.3.0/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      234 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)      502 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/
--rw-r--r--   0 vsts      (1001) docker     (122)      279 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4712 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2583 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3435 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4715 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/
--rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1256 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/minichain.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4784 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4157 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/openai.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1901 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10806 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8011 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7790 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8788 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/spancat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/lemma.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)    15017 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      223 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4009 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4722 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/span.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2294 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1682 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_minichain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_stablelm.py
--rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6951 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/ner_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/ner_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/ner_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/rel_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/lemma_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/ner_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/textcat_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)     7949 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21901 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5203 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16700 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23397 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5934 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8724 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    62271 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4685 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      149 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/ner_minichain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_minichain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_minichain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3509 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    62605 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    61361 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      736 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1810 2023-06-23 13:19:00.737381 spacy-llm-0.3.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      234 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm/backends/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)      502 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      279 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4712 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2583 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3435 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4715 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/
+-rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1256 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/minichain.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/backends/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4784 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4157 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/openai.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1901 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11318 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7947 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7901 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8724 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/spancat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/lemma.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)    15128 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      223 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4009 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4826 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/span.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2294 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1682 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_minichain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_stablelm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8027 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/ner_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/ner_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/ner_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/lemma_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/ner_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/textcat_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)     7949 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22403 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5704 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17202 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23835 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5934 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8941 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    62605 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4685 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      149 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/ner_minichain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_minichain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_minichain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3509 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.3.0/LICENSE` & `spacy-llm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/PKG-INFO` & `spacy-llm-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -247,20 +247,18 @@
 
 spacy_llm.logger.addHandler(logging.StreamHandler())
 spacy_llm.logger.setLevel(logging.DEBUG)
 ```
 
 > NOTE: Any `logging` handler will work here so you probably want to use some sort of rotating `FileHandler` as the generated prompts can be quite long, especially for tasks with few-shot examples.
 
-
 Then when using the pipeline you'll be able to view the prompt and response.
 
 E.g. with the config and code from [Example 1](##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
 
-
 ```python
 from spacy_llm.util import assemble
 
 
 nlp = assemble("config.cfg")
 doc = nlp("You look gorgeous!")
 print(doc.cats)
@@ -298,20 +296,21 @@
 {'COMPLIMENT': 1.0, 'INSULT': 0.0}
 ```
 
 ## 📓 API
 
 `spacy-llm` exposes a `llm` factory that accepts the following configuration options:
 
-| Argument  | Type                                        | Description                                                                         |
-| --------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
-| `task`    | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
-| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
-| `cache`   | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
-| `save_io` | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`                  |
+| Argument         | Type                                        | Description                                                                         |
+| ---------------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
+| `task`           | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
+| `backend`        | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
+| `cache`          | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
+| `save_io`        | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`.                 |
+| `validate_types` | `bool`                                      | Whether to check if signatures of configured backend and task are consistent.       |
 
 An `llm` component is defined by two main settings:
 
 - A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
 - A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
@@ -321,14 +320,18 @@
 
 Finally, you can choose to save a stringified version of LLM prompts/responses
 within the `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
 `Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM component
 within the spaCy pipeline. Each entry is itself a dictionary, with two keys:
 `prompt` and `response`.
 
+A note on `validate_types`: by default, `spacy-llm` checks whether the signatures of the `backend` and `task` callables
+are consistent with each other and emits a warning if they don't. `validate_types` can be set to `False` if you want to
+disable this behavior.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -683,35 +686,36 @@
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.Lemma.v1"
 examples = null
 ```
 
-| Argument                  | Type                                    | Default                                                   | Description                                                                                                                                           |
-| ------------------------- | --------------------------------------- |-----------------------------------------------------------| ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `template`                | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
-| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                    | Optional function that generates examples for few-shot learning.                                                                                      |
+| Argument   | Type                                    | Default                                                | Description                                                                                                                              |
+| ---------- | --------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
+| `template` | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                 | Optional function that generates examples for few-shot learning.                                                                         |
 
 `Lemma.v1` prompts the LLM to lemmatize the passed text and return the lemmatized version as a list of tokens and their
-corresponding lemma. E. g. the text 
+corresponding lemma. E. g. the text
 `I'm buying ice cream for my friends` should invoke the response
+
 ```
 I: I
 'm: be
 buying: buy
 ice: ice
 cream: cream
 for: for
 my: my
 friends: friend
 .: .
 ```
 
-If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized 
+If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized
 by spaCy, no lemmas are stored in the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is updated with
 the lemma suggested by the LLM.
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
 The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
 
 ```yaml
@@ -721,15 +725,15 @@
     - "'m": "be"
     - "buying": "buy"
     - "ice": "ice"
     - "cream": "cream"
     - ".": "."
 
 - text: I've watered the plants.
-  lemmas: 
+  lemmas:
     - "I": "I"
     - "'ve": "have"
     - "watered": "water"
     - "the": "the"
     - "plants": "plant"
     - ".": "."
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.0 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.1 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -153,39 +153,44 @@
 example: Label1, Label2, Label3. Do not put any other text in your answer, only
 one or more of the provided labels with nothing before or after. If the text
 cannot be classified into any of the provided labels, answer `==NONE==`. Here
 is the text that needs classification Text: ''' You look gorgeous! ''' Backend
 response for doc: You look gorgeous! COMPLIMENT ``` `print(doc.cats)` to
 standard output should look like: ``` {'COMPLIMENT': 1.0, 'INSULT': 0.0} ``` ##
 ð API `spacy-llm` exposes a `llm` factory that accepts the following
-configuration options: | Argument | Type | Description | | --------- | --------
------------------------------------ | -----------------------------------------
------------------------------------------- | | `task` | `Optional[LLMTask]` |
-An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks). |
-| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a
-specific LLM API. See [docs](#backends). | | `cache` | `Cache` | Cache to use
-for caching prompts and responses per doc (batch). See [docs](#cache). | |
-`save_io` | `bool` | Whether to save prompts/responses within `Doc.user_data
-["llm_io"]` | An `llm` component is defined by two main settings: - A
-[**task**](#tasks), defining the prompt to send to the LLM as well as the
-functionality to parse the resulting response back into structured fields on
-spaCy's [Doc](https://spacy.io/api/doc) objects. - A [**backend**](#backends)
-defining the model to use and how to connect to it. Note that `spacy-llm`
-supports both access to external APIs (such as OpenAI) as well as access to
-self-hosted open-source LLMs (such as using Dolly through Hugging Face).
-Moreover, `spacy-llm` exposes a customizable [**caching**](#cache)
-functionality to avoid running the same document through an LLM service (be it
-local or through a REST API) more than once. Finally, you can choose to save a
-stringified version of LLM prompts/responses within the `Doc.user_data
-["llm_io"]` attribute by setting `save_io` to `True`. `Doc.user_data["llm_io"]`
-is a dictionary containing one entry for every LLM component within the spaCy
-pipeline. Each entry is itself a dictionary, with two keys: `prompt` and
-`response`. ### Tasks A _task_ defines an NLP problem or question, that will be
-sent to the LLM via a prompt. Further, the task defines how to parse the LLM's
-responses back into structured information. All tasks are registered in spaCy's
+configuration options: | Argument | Type | Description | | ---------------- | -
+------------------------------------------ | ----------------------------------
+------------------------------------------------- | | `task` | `Optional
+[LLMTask]` | An LLMTask can generate prompts and parse LLM responses. See
+[docs](#tasks). | | `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` |
+Callable querying a specific LLM API. See [docs](#backends). | | `cache` |
+`Cache` | Cache to use for caching prompts and responses per doc (batch). See
+[docs](#cache). | | `save_io` | `bool` | Whether to save prompts/responses
+within `Doc.user_data["llm_io"]`. | | `validate_types` | `bool` | Whether to
+check if signatures of configured backend and task are consistent. | An `llm`
+component is defined by two main settings: - A [**task**](#tasks), defining the
+prompt to send to the LLM as well as the functionality to parse the resulting
+response back into structured fields on spaCy's [Doc](https://spacy.io/api/doc)
+objects. - A [**backend**](#backends) defining the model to use and how to
+connect to it. Note that `spacy-llm` supports both access to external APIs
+(such as OpenAI) as well as access to self-hosted open-source LLMs (such as
+using Dolly through Hugging Face). Moreover, `spacy-llm` exposes a customizable
+[**caching**](#cache) functionality to avoid running the same document through
+an LLM service (be it local or through a REST API) more than once. Finally, you
+can choose to save a stringified version of LLM prompts/responses within the
+`Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
+`Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM
+component within the spaCy pipeline. Each entry is itself a dictionary, with
+two keys: `prompt` and `response`. A note on `validate_types`: by default,
+`spacy-llm` checks whether the signatures of the `backend` and `task` callables
+are consistent with each other and emits a warning if they don't.
+`validate_types` can be set to `False` if you want to disable this behavior.
+### Tasks A _task_ defines an NLP problem or question, that will be sent to the
+LLM via a prompt. Further, the task defines how to parse the LLM's responses
+back into structured information. All tasks are registered in spaCy's
 `llm_tasks` registry. Practically speaking, a task should adhere to the
 `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py). It needs to define
 a `generate_prompts` function and a `parse_responses` function. Moreover, the
 task may define an optional [`scorer` method](https://spacy.io/api/
 scorer#score). It should accept an iterable of `Example`s as input and return a
 score dictionary. If the `scorer` method is defined, `spacy-llm` will call it
 to evaluate the component. #### function `task.generate_prompts` Takes a
@@ -441,148 +446,148 @@
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
 [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
 "Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
 = "rel_examples.jsonl" ``` #### spacy.Lemma.v1 The `Lemma.v1` task lemmatizes
 the provided text and updates the `lemma_` attribute in the doc's tokens
 accordingly. ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
-examples = null ``` | Argument | Type | Default | Description | | -------------
------------- | --------------------------------------- |-----------------------
-------------------------------------| -----------------------------------------
+examples = null ``` | Argument | Type | Default | Description | | ---------- |
+--------------------------------------- | -------------------------------------
+----------------- | -----------------------------------------------------------
+----------------------------------------------------------------------------- |
+| `template` | `str` | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) |
+Custom prompt template to send to LLM backend. Default templates for each task
+are located in the `spacy_llm/tasks/templates` directory. | | `examples` |
+`Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
+generates examples for few-shot learning. | `Lemma.v1` prompts the LLM to
+lemmatize the passed text and return the lemmatized version as a list of tokens
+and their corresponding lemma. E. g. the text `I'm buying ice cream for my
+friends` should invoke the response ``` I: I 'm: be buying: buy ice: ice cream:
+cream for: for my: my friends: friend .: . ``` If for any given text/doc
+instance the number of lemmas returned by the LLM doesn't match the number of
+tokens recognized by spaCy, no lemmas are stored in the corresponding doc's
+tokens. Otherwise the tokens `.lemma_` property is updated with the lemma
+suggested by the LLM. To perform few-shot learning, you can write down a few
+examples in a separate file, and provide these to be injected into the prompt
+to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+`.yaml`, `.json` and `.jsonl`. ```yaml - text: I'm buying ice cream. lemmas: -
+"I": "I" - "'m": "be" - "buying": "buy" - "ice": "ice" - "cream": "cream" -
+".": "." - text: I've watered the plants. lemmas: - "I": "I" - "'ve": "have" -
+"watered": "water" - "the": "the" - "plants": "plant" - ".": "." ``` ```ini
+[components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"lemma_examples.yml" ``` #### spacy.NoOp.v1 This task is only useful for
+testing - it tells the LLM to do nothing, and does not set any fields on the
+`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
+Backends A _backend_ defines which LLM model to query, and how to query it. It
+can be a simple function taking a collection of prompts (consistent with the
+output type of `task.generate_prompts()`) and returning a collection of
+responses (consistent with the expected input of `parse_responses`). Generally
+speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
+but specific implementations can have other signatures, like `Callable[
+[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
+`llm_backends`. If no backend is specified, the repo currently connects to the
+[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
+accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
+third-party libraries in addition to a native REST backend and which should > I
+choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
+prompt management, integration of many different LLM > APIs, and other related
+features such as conversational memory or agents. `spacy-llm` on the other hand
+emphasizes > features we consider useful in the context of NLP pipelines
+utilizing LLMs to process documents (mostly) independent > from each other. It
+makes sense that the feature set of such third-party libraries and `spacy-llm`
+is not identical - > and users might want to take advantage of features not
+available in `spacy-llm`. > > The advantage of offering our own REST backend is
+that we can ensure a larger degree of stability of robustness, as > we can
+guarantee backwards-compatibility and more smoothly integrated error handling.
+> > Ultimately we recommend trying to implement your use case using the REST
+backend first (which is configured as the > default backend). If however there
+are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
+> backend of a third-party library - and easy to customize the prompting
+mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
+to get an API key from openai.com, and ensure that the keys are set as
+environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
+OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
+`requests` and a simple retry mechanism to access an API. ```ini
+[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
+= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
+Default | Description | | ----------- | ---------------- | ------- | ----------
 -------------------------------------------------------------------------------
------------------------------ | | `template` | `str` | [lemma.jinja](./
-spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM
-backend. Default templates for each task are located in the `spacy_llm/tasks/
-templates` directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
-| `None` | Optional function that generates examples for few-shot learning. |
-`Lemma.v1` prompts the LLM to lemmatize the passed text and return the
-lemmatized version as a list of tokens and their corresponding lemma. E. g. the
-text `I'm buying ice cream for my friends` should invoke the response ``` I: I
-'m: be buying: buy ice: ice cream: cream for: for my: my friends: friend .: .
-``` If for any given text/doc instance the number of lemmas returned by the LLM
-doesn't match the number of tokens recognized by spaCy, no lemmas are stored in
-the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is
-updated with the lemma suggested by the LLM. To perform few-shot learning, you
-can write down a few examples in a separate file, and provide these to be
-injected into the prompt to the LLM. The default reader
-`spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
-```yaml - text: I'm buying ice cream. lemmas: - "I": "I" - "'m": "be" -
-"buying": "buy" - "ice": "ice" - "cream": "cream" - ".": "." - text: I've
-watered the plants. lemmas: - "I": "I" - "'ve": "have" - "watered": "water" -
-"the": "the" - "plants": "plant" - ".": "." ``` ```ini [components.llm.task]
-@llm_tasks = "spacy.Lemma.v1" [components.llm.task.examples] @misc =
-"spacy.FewShotReader.v1" path = "lemma_examples.yml" ``` #### spacy.NoOp.v1
-This task is only useful for testing - it tells the LLM to do nothing, and does
-not set any fields on the `docs`. ```ini [components.llm.task] @llm_tasks =
-"spacy.NoOp.v1" ``` ### Backends A _backend_ defines which LLM model to query,
-and how to query it. It can be a simple function taking a collection of prompts
-(consistent with the output type of `task.generate_prompts()`) and returning a
-collection of responses (consistent with the expected input of
-`parse_responses`). Generally speaking, it's a function of type `Callable[
-[Iterable[Any]], Iterable[Any]]`, but specific implementations can have other
-signatures, like `Callable[[Iterable[str]], Iterable[str]]`. All built-in
-backends are registered in `llm_backends`. If no backend is specified, the repo
-currently connects to the [`OpenAI` API](#openai) by default, using the built-
-in REST protocol, and accesses the `"gpt-3.5-turbo"` model. > :question: _Why
-are there backends for third-party libraries in addition to a native REST
-backend and which should > I choose?_ > > Third-party libraries like
-`langchain` or `minichain` focus on prompt management, integration of many
-different LLM > APIs, and other related features such as conversational memory
-or agents. `spacy-llm` on the other hand emphasizes > features we consider
-useful in the context of NLP pipelines utilizing LLMs to process documents
-(mostly) independent > from each other. It makes sense that the feature set of
-such third-party libraries and `spacy-llm` is not identical - > and users might
-want to take advantage of features not available in `spacy-llm`. > > The
-advantage of offering our own REST backend is that we can ensure a larger
-degree of stability of robustness, as > we can guarantee backwards-
-compatibility and more smoothly integrated error handling. > > Ultimately we
-recommend trying to implement your use case using the REST backend first (which
-is configured as the > default backend). If however there are features or APIs
-not covered by `spacy-llm`, it's trivial to switch to the > backend of a third-
-party library - and easy to customize the prompting mechanism, if so required.
-#### OpenAI When the backend uses OpenAI, you have to get an API key from
-openai.com, and ensure that the keys are set as environmental variables:
-```shell export OPENAI_API_KEY="sk-..." export OPENAI_API_ORG="org-..." ```
-#### spacy.REST.v1 This default backend uses `requests` and a simple retry
-mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
-"spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-turbo",
-"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
--- | ---------------- | ------- | ---------------------------------------------
------------------------------------------------------------------------ | |
-`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
-supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
-passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
-error if the LLM API returns a malformed response. Otherwise, return the error
-responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
-request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
-When `api` is set to `OpenAI`, the following settings can be defined in the
-`config` dictionary: - `model`: one of the following list of supported models:
-- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
-turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
-- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
-`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
-api.openai.com/v1/completions`. For models requiring the chat endpoint, use
-`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
-[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
-make sure you have installed it first: ```shell python -m pip install
-"minichain>=0.3,<0.4" # Or install with spacy-llm directly python -m pip
-install "spacy-llm[minichain]" ``` Note that MiniChain currently only supports
-Python 3.8, 3.9 and 3.10. Example config blocks: ```ini
-[components.llm.backend] @llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
-[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
-Argument | Type | Default | Description | | -------- | ------------------------
---------------------------------------------------------- | ------- | ---------
--------------------------------------------------------------------------- | |
-`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
-`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
-backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
-Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
-If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
-(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
-for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
-(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
-you have installed it first: ```shell python -m pip install
-"langchain>=0.0.144,<0.1" # Or install with spacy-llm directly python -m pip
-install "spacy-llm[langchain]" ``` Note that LangChain currently only supports
-Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
-@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
-"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
-Default | Description | | -------- | ------------------------------------------
------------------------------------- | ------- | ------------------------------
------------------------------------------------------- | | `api` | `str` | |
-The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
-[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
-`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
-Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
-defaults to `spacy.CallLangChain.v1`. | The default `query`
-(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
-each given textual prompt. #### spacy.Dolly_HF.v1 To use this backend, ideally
-you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
-your virtual environment. This allows you to have the setting `device=cuda:0`
-in your config, which ensures that the model is loaded entirely on the GPU (and
-fails otherwise). You can do so with ```shell python -m pip install "spacy-llm
-[transformers]" "transformers[sentencepiece]" ``` If you don't have access to a
-GPU, you can install `accelerate` and set`device_map=auto` instead, but be
-aware that this may result in some layers getting distributed to the CPU or
-even the hard drive, which may ultimately result in extremely slow queries.
-```shell python -m pip install "accelerate>=0.16.0,<1.0" ``` Example config
-block: ```ini [components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1"
-model = "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description
-| | ------------- | ---------------- | ------- | ------------------------------
------------------------------------------------------------------- | | `model`
-| `str` | | The name of a Dolly model that is supported. | | `config_init` |
-`Dict[str, Any]` | `{}` | Further configuration passed on to the construction
-of the model with `transformers.pipeline()`. | | `config_run` | `Dict[str,
-Any]` | `{}` | Further configuration used during model inference. | Supported
-models (see the [Databricks models page](https://huggingface.co/databricks) on
-Hugging Face for details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-
-v2-7b"` - `"databricks/dolly-v2-12b"` Note that Hugging Face will download this
-model the first time you use it - you can [define the cached directory](https:/
-/huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting
-the environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
+--------------------------- | | `api` | `str` | | The name of a supported API.
+In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
+| Further configuration passed on to the backend. | | `strict` | `bool` |
+`True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
+following settings can be defined in the `config` dictionary: - `model`: one of
+the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
+32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
+`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
+babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
+`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
+For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
+completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
+srush/MiniChain) for the API retrieval part, make sure you have installed it
+first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
+spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
+MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
+blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
+api = "OpenAI" [components.llm.backend.query] @llm_queries =
+"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
+--- | -------------------------------------------------------------------------
+-------- | ------- | ----------------------------------------------------------
+------------------------- | | `api` | `str` | | The name of an API supported by
+MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
+Function that executes the prompts. If `None`, defaults to
+`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
+executes the prompts by running `model(text).run()` for each given textual
+prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
+hwchase17/langchain) for the API retrieval part, make sure you have installed
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
+with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
+that LangChain currently only supports Python 3.9 and beyond. Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
+= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
+- | ---------------------------------------------------------------------------
+--- | ------- | ---------------------------------------------------------------
+--------------------- | | `api` | `str` | | The name of an API supported by
+LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
+that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
+`model(text)` for each given textual prompt. #### spacy.Dolly_HF.v1 To use this
+backend, ideally you have a GPU enabled and have installed `transformers`,
+`torch` and CUDA in your virtual environment. This allows you to have the
+setting `device=cuda:0` in your config, which ensures that the model is loaded
+entirely on the GPU (and fails otherwise). You can do so with ```shell python -
+m pip install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If
+you don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" model =
+"databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
+--------- | ---------------- | ------- | --------------------------------------
+---------------------------------------------------------- | | `model` | `str`
+| | The name of a Dolly model that is supported. | | `config_init` | `Dict[str,
+Any]` | `{}` | Further configuration passed on to the construction of the model
+with `transformers.pipeline()`. | | `config_run` | `Dict[str, Any]` | `{}` |
+Further configuration used during model inference. | Supported models (see the
+[Databricks models page](https://huggingface.co/databricks) on Hugging Face for
+details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` -
+`"databricks/dolly-v2-12b"` Note that Hugging Face will download this model the
+first time you use it - you can [define the cached directory](https://
+huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
+environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
 `torch` and CUDA in your virtual environment. You can do so with ```shell
 python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ``` If you don't have access to a GPU, you can install `accelerate` and
 set`device_map=auto` instead, but be aware that this may result in some layers
 getting distributed to the CPU or even the hard drive, which may ultimately
 result in extremely slow queries. ```shell python -m pip install
```

### Comparing `spacy-llm-0.3.0/README.md` & `spacy-llm-0.3.1/spacy_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: spacy-llm
+Version: 0.3.1
+Summary: Integrating LLMs into structured NLP pipelines
+Author: Explosion
+Author-email: contact@explosion.ai
+License: MIT
+Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
+Project-URL: Source, https://github.com/explosion/spacy-llm
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: minichain
+Provides-Extra: langchain
+Provides-Extra: transformers
+License-File: LICENSE
+
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
@@ -215,20 +247,18 @@
 
 spacy_llm.logger.addHandler(logging.StreamHandler())
 spacy_llm.logger.setLevel(logging.DEBUG)
 ```
 
 > NOTE: Any `logging` handler will work here so you probably want to use some sort of rotating `FileHandler` as the generated prompts can be quite long, especially for tasks with few-shot examples.
 
-
 Then when using the pipeline you'll be able to view the prompt and response.
 
 E.g. with the config and code from [Example 1](##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
 
-
 ```python
 from spacy_llm.util import assemble
 
 
 nlp = assemble("config.cfg")
 doc = nlp("You look gorgeous!")
 print(doc.cats)
@@ -266,20 +296,21 @@
 {'COMPLIMENT': 1.0, 'INSULT': 0.0}
 ```
 
 ## 📓 API
 
 `spacy-llm` exposes a `llm` factory that accepts the following configuration options:
 
-| Argument  | Type                                        | Description                                                                         |
-| --------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
-| `task`    | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
-| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
-| `cache`   | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
-| `save_io` | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`                  |
+| Argument         | Type                                        | Description                                                                         |
+| ---------------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
+| `task`           | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
+| `backend`        | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
+| `cache`          | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
+| `save_io`        | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`.                 |
+| `validate_types` | `bool`                                      | Whether to check if signatures of configured backend and task are consistent.       |
 
 An `llm` component is defined by two main settings:
 
 - A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
 - A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
@@ -289,14 +320,18 @@
 
 Finally, you can choose to save a stringified version of LLM prompts/responses
 within the `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
 `Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM component
 within the spaCy pipeline. Each entry is itself a dictionary, with two keys:
 `prompt` and `response`.
 
+A note on `validate_types`: by default, `spacy-llm` checks whether the signatures of the `backend` and `task` callables
+are consistent with each other and emits a warning if they don't. `validate_types` can be set to `False` if you want to
+disable this behavior.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -651,35 +686,36 @@
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.Lemma.v1"
 examples = null
 ```
 
-| Argument                  | Type                                    | Default                                                   | Description                                                                                                                                           |
-| ------------------------- | --------------------------------------- |-----------------------------------------------------------| ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `template`                | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
-| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                    | Optional function that generates examples for few-shot learning.                                                                                      |
+| Argument   | Type                                    | Default                                                | Description                                                                                                                              |
+| ---------- | --------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
+| `template` | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                 | Optional function that generates examples for few-shot learning.                                                                         |
 
 `Lemma.v1` prompts the LLM to lemmatize the passed text and return the lemmatized version as a list of tokens and their
-corresponding lemma. E. g. the text 
+corresponding lemma. E. g. the text
 `I'm buying ice cream for my friends` should invoke the response
+
 ```
 I: I
 'm: be
 buying: buy
 ice: ice
 cream: cream
 for: for
 my: my
 friends: friend
 .: .
 ```
 
-If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized 
+If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized
 by spaCy, no lemmas are stored in the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is updated with
 the lemma suggested by the LLM.
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
 The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
 
 ```yaml
@@ -689,15 +725,15 @@
     - "'m": "be"
     - "buying": "buy"
     - "ice": "ice"
     - "cream": "cream"
     - ".": "."
 
 - text: I've watered the plants.
-  lemmas: 
+  lemmas:
     - "I": "I"
     - "'ve": "have"
     - "watered": "water"
     - "the": "the"
     - "plants": "plant"
     - ".": "."
 ```
```

#### html2text {}

```diff
@@ -1,12 +1,29 @@
-[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
-structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
-github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
-(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
-Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.1 Summary: Integrating LLMs
+into structured NLP pipelines Author: Explosion Author-email:
+contact@explosion.ai License: MIT Project-URL: Release notes, https://
+github.com/explosion/spacy-llm/releases Project-URL: Source, https://
+github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
+Content-Type: text/markdown Provides-Extra: minichain Provides-Extra: langchain
+Provides-Extra: transformers License-File: LICENSE [https://explosion.ai/
+assets/img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP
+pipelines [![GitHub Workflow Status](https://img.shields.io/github/actions/
+workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/
+explosion/spacy-llm/actions/workflows/test.yml) [![pypi Version](https://
+img.shields.io/pypi/v/spacy-llm.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/ambv/black) This package
 integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
 featuring a modular system for **fast prototyping** and **prompting**, and
 turning unstructured responses into **robust outputs** for various NLP tasks,
 **no training data** required. - Serializable `llm` **component** to integrate
@@ -136,39 +153,44 @@
 example: Label1, Label2, Label3. Do not put any other text in your answer, only
 one or more of the provided labels with nothing before or after. If the text
 cannot be classified into any of the provided labels, answer `==NONE==`. Here
 is the text that needs classification Text: ''' You look gorgeous! ''' Backend
 response for doc: You look gorgeous! COMPLIMENT ``` `print(doc.cats)` to
 standard output should look like: ``` {'COMPLIMENT': 1.0, 'INSULT': 0.0} ``` ##
 ð API `spacy-llm` exposes a `llm` factory that accepts the following
-configuration options: | Argument | Type | Description | | --------- | --------
------------------------------------ | -----------------------------------------
------------------------------------------- | | `task` | `Optional[LLMTask]` |
-An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks). |
-| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a
-specific LLM API. See [docs](#backends). | | `cache` | `Cache` | Cache to use
-for caching prompts and responses per doc (batch). See [docs](#cache). | |
-`save_io` | `bool` | Whether to save prompts/responses within `Doc.user_data
-["llm_io"]` | An `llm` component is defined by two main settings: - A
-[**task**](#tasks), defining the prompt to send to the LLM as well as the
-functionality to parse the resulting response back into structured fields on
-spaCy's [Doc](https://spacy.io/api/doc) objects. - A [**backend**](#backends)
-defining the model to use and how to connect to it. Note that `spacy-llm`
-supports both access to external APIs (such as OpenAI) as well as access to
-self-hosted open-source LLMs (such as using Dolly through Hugging Face).
-Moreover, `spacy-llm` exposes a customizable [**caching**](#cache)
-functionality to avoid running the same document through an LLM service (be it
-local or through a REST API) more than once. Finally, you can choose to save a
-stringified version of LLM prompts/responses within the `Doc.user_data
-["llm_io"]` attribute by setting `save_io` to `True`. `Doc.user_data["llm_io"]`
-is a dictionary containing one entry for every LLM component within the spaCy
-pipeline. Each entry is itself a dictionary, with two keys: `prompt` and
-`response`. ### Tasks A _task_ defines an NLP problem or question, that will be
-sent to the LLM via a prompt. Further, the task defines how to parse the LLM's
-responses back into structured information. All tasks are registered in spaCy's
+configuration options: | Argument | Type | Description | | ---------------- | -
+------------------------------------------ | ----------------------------------
+------------------------------------------------- | | `task` | `Optional
+[LLMTask]` | An LLMTask can generate prompts and parse LLM responses. See
+[docs](#tasks). | | `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` |
+Callable querying a specific LLM API. See [docs](#backends). | | `cache` |
+`Cache` | Cache to use for caching prompts and responses per doc (batch). See
+[docs](#cache). | | `save_io` | `bool` | Whether to save prompts/responses
+within `Doc.user_data["llm_io"]`. | | `validate_types` | `bool` | Whether to
+check if signatures of configured backend and task are consistent. | An `llm`
+component is defined by two main settings: - A [**task**](#tasks), defining the
+prompt to send to the LLM as well as the functionality to parse the resulting
+response back into structured fields on spaCy's [Doc](https://spacy.io/api/doc)
+objects. - A [**backend**](#backends) defining the model to use and how to
+connect to it. Note that `spacy-llm` supports both access to external APIs
+(such as OpenAI) as well as access to self-hosted open-source LLMs (such as
+using Dolly through Hugging Face). Moreover, `spacy-llm` exposes a customizable
+[**caching**](#cache) functionality to avoid running the same document through
+an LLM service (be it local or through a REST API) more than once. Finally, you
+can choose to save a stringified version of LLM prompts/responses within the
+`Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
+`Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM
+component within the spaCy pipeline. Each entry is itself a dictionary, with
+two keys: `prompt` and `response`. A note on `validate_types`: by default,
+`spacy-llm` checks whether the signatures of the `backend` and `task` callables
+are consistent with each other and emits a warning if they don't.
+`validate_types` can be set to `False` if you want to disable this behavior.
+### Tasks A _task_ defines an NLP problem or question, that will be sent to the
+LLM via a prompt. Further, the task defines how to parse the LLM's responses
+back into structured information. All tasks are registered in spaCy's
 `llm_tasks` registry. Practically speaking, a task should adhere to the
 `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py). It needs to define
 a `generate_prompts` function and a `parse_responses` function. Moreover, the
 task may define an optional [`scorer` method](https://spacy.io/api/
 scorer#score). It should accept an iterable of `Example`s as input and return a
 score dictionary. If the `scorer` method is defined, `spacy-llm` will call it
 to evaluate the component. #### function `task.generate_prompts` Takes a
@@ -424,148 +446,148 @@
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
 [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
 "Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
 = "rel_examples.jsonl" ``` #### spacy.Lemma.v1 The `Lemma.v1` task lemmatizes
 the provided text and updates the `lemma_` attribute in the doc's tokens
 accordingly. ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
-examples = null ``` | Argument | Type | Default | Description | | -------------
------------- | --------------------------------------- |-----------------------
-------------------------------------| -----------------------------------------
+examples = null ``` | Argument | Type | Default | Description | | ---------- |
+--------------------------------------- | -------------------------------------
+----------------- | -----------------------------------------------------------
+----------------------------------------------------------------------------- |
+| `template` | `str` | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) |
+Custom prompt template to send to LLM backend. Default templates for each task
+are located in the `spacy_llm/tasks/templates` directory. | | `examples` |
+`Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
+generates examples for few-shot learning. | `Lemma.v1` prompts the LLM to
+lemmatize the passed text and return the lemmatized version as a list of tokens
+and their corresponding lemma. E. g. the text `I'm buying ice cream for my
+friends` should invoke the response ``` I: I 'm: be buying: buy ice: ice cream:
+cream for: for my: my friends: friend .: . ``` If for any given text/doc
+instance the number of lemmas returned by the LLM doesn't match the number of
+tokens recognized by spaCy, no lemmas are stored in the corresponding doc's
+tokens. Otherwise the tokens `.lemma_` property is updated with the lemma
+suggested by the LLM. To perform few-shot learning, you can write down a few
+examples in a separate file, and provide these to be injected into the prompt
+to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+`.yaml`, `.json` and `.jsonl`. ```yaml - text: I'm buying ice cream. lemmas: -
+"I": "I" - "'m": "be" - "buying": "buy" - "ice": "ice" - "cream": "cream" -
+".": "." - text: I've watered the plants. lemmas: - "I": "I" - "'ve": "have" -
+"watered": "water" - "the": "the" - "plants": "plant" - ".": "." ``` ```ini
+[components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"lemma_examples.yml" ``` #### spacy.NoOp.v1 This task is only useful for
+testing - it tells the LLM to do nothing, and does not set any fields on the
+`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
+Backends A _backend_ defines which LLM model to query, and how to query it. It
+can be a simple function taking a collection of prompts (consistent with the
+output type of `task.generate_prompts()`) and returning a collection of
+responses (consistent with the expected input of `parse_responses`). Generally
+speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
+but specific implementations can have other signatures, like `Callable[
+[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
+`llm_backends`. If no backend is specified, the repo currently connects to the
+[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
+accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
+third-party libraries in addition to a native REST backend and which should > I
+choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
+prompt management, integration of many different LLM > APIs, and other related
+features such as conversational memory or agents. `spacy-llm` on the other hand
+emphasizes > features we consider useful in the context of NLP pipelines
+utilizing LLMs to process documents (mostly) independent > from each other. It
+makes sense that the feature set of such third-party libraries and `spacy-llm`
+is not identical - > and users might want to take advantage of features not
+available in `spacy-llm`. > > The advantage of offering our own REST backend is
+that we can ensure a larger degree of stability of robustness, as > we can
+guarantee backwards-compatibility and more smoothly integrated error handling.
+> > Ultimately we recommend trying to implement your use case using the REST
+backend first (which is configured as the > default backend). If however there
+are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
+> backend of a third-party library - and easy to customize the prompting
+mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
+to get an API key from openai.com, and ensure that the keys are set as
+environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
+OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
+`requests` and a simple retry mechanism to access an API. ```ini
+[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
+= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
+Default | Description | | ----------- | ---------------- | ------- | ----------
 -------------------------------------------------------------------------------
------------------------------ | | `template` | `str` | [lemma.jinja](./
-spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM
-backend. Default templates for each task are located in the `spacy_llm/tasks/
-templates` directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
-| `None` | Optional function that generates examples for few-shot learning. |
-`Lemma.v1` prompts the LLM to lemmatize the passed text and return the
-lemmatized version as a list of tokens and their corresponding lemma. E. g. the
-text `I'm buying ice cream for my friends` should invoke the response ``` I: I
-'m: be buying: buy ice: ice cream: cream for: for my: my friends: friend .: .
-``` If for any given text/doc instance the number of lemmas returned by the LLM
-doesn't match the number of tokens recognized by spaCy, no lemmas are stored in
-the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is
-updated with the lemma suggested by the LLM. To perform few-shot learning, you
-can write down a few examples in a separate file, and provide these to be
-injected into the prompt to the LLM. The default reader
-`spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
-```yaml - text: I'm buying ice cream. lemmas: - "I": "I" - "'m": "be" -
-"buying": "buy" - "ice": "ice" - "cream": "cream" - ".": "." - text: I've
-watered the plants. lemmas: - "I": "I" - "'ve": "have" - "watered": "water" -
-"the": "the" - "plants": "plant" - ".": "." ``` ```ini [components.llm.task]
-@llm_tasks = "spacy.Lemma.v1" [components.llm.task.examples] @misc =
-"spacy.FewShotReader.v1" path = "lemma_examples.yml" ``` #### spacy.NoOp.v1
-This task is only useful for testing - it tells the LLM to do nothing, and does
-not set any fields on the `docs`. ```ini [components.llm.task] @llm_tasks =
-"spacy.NoOp.v1" ``` ### Backends A _backend_ defines which LLM model to query,
-and how to query it. It can be a simple function taking a collection of prompts
-(consistent with the output type of `task.generate_prompts()`) and returning a
-collection of responses (consistent with the expected input of
-`parse_responses`). Generally speaking, it's a function of type `Callable[
-[Iterable[Any]], Iterable[Any]]`, but specific implementations can have other
-signatures, like `Callable[[Iterable[str]], Iterable[str]]`. All built-in
-backends are registered in `llm_backends`. If no backend is specified, the repo
-currently connects to the [`OpenAI` API](#openai) by default, using the built-
-in REST protocol, and accesses the `"gpt-3.5-turbo"` model. > :question: _Why
-are there backends for third-party libraries in addition to a native REST
-backend and which should > I choose?_ > > Third-party libraries like
-`langchain` or `minichain` focus on prompt management, integration of many
-different LLM > APIs, and other related features such as conversational memory
-or agents. `spacy-llm` on the other hand emphasizes > features we consider
-useful in the context of NLP pipelines utilizing LLMs to process documents
-(mostly) independent > from each other. It makes sense that the feature set of
-such third-party libraries and `spacy-llm` is not identical - > and users might
-want to take advantage of features not available in `spacy-llm`. > > The
-advantage of offering our own REST backend is that we can ensure a larger
-degree of stability of robustness, as > we can guarantee backwards-
-compatibility and more smoothly integrated error handling. > > Ultimately we
-recommend trying to implement your use case using the REST backend first (which
-is configured as the > default backend). If however there are features or APIs
-not covered by `spacy-llm`, it's trivial to switch to the > backend of a third-
-party library - and easy to customize the prompting mechanism, if so required.
-#### OpenAI When the backend uses OpenAI, you have to get an API key from
-openai.com, and ensure that the keys are set as environmental variables:
-```shell export OPENAI_API_KEY="sk-..." export OPENAI_API_ORG="org-..." ```
-#### spacy.REST.v1 This default backend uses `requests` and a simple retry
-mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
-"spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-turbo",
-"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
--- | ---------------- | ------- | ---------------------------------------------
------------------------------------------------------------------------ | |
-`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
-supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
-passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
-error if the LLM API returns a malformed response. Otherwise, return the error
-responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
-request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
-When `api` is set to `OpenAI`, the following settings can be defined in the
-`config` dictionary: - `model`: one of the following list of supported models:
-- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
-turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
-- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
-`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
-api.openai.com/v1/completions`. For models requiring the chat endpoint, use
-`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
-[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
-make sure you have installed it first: ```shell python -m pip install
-"minichain>=0.3,<0.4" # Or install with spacy-llm directly python -m pip
-install "spacy-llm[minichain]" ``` Note that MiniChain currently only supports
-Python 3.8, 3.9 and 3.10. Example config blocks: ```ini
-[components.llm.backend] @llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
-[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
-Argument | Type | Default | Description | | -------- | ------------------------
---------------------------------------------------------- | ------- | ---------
--------------------------------------------------------------------------- | |
-`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
-`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
-backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
-Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
-If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
-(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
-for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
-(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
-you have installed it first: ```shell python -m pip install
-"langchain>=0.0.144,<0.1" # Or install with spacy-llm directly python -m pip
-install "spacy-llm[langchain]" ``` Note that LangChain currently only supports
-Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
-@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
-"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
-Default | Description | | -------- | ------------------------------------------
------------------------------------- | ------- | ------------------------------
------------------------------------------------------- | | `api` | `str` | |
-The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
-[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
-`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
-Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
-defaults to `spacy.CallLangChain.v1`. | The default `query`
-(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
-each given textual prompt. #### spacy.Dolly_HF.v1 To use this backend, ideally
-you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
-your virtual environment. This allows you to have the setting `device=cuda:0`
-in your config, which ensures that the model is loaded entirely on the GPU (and
-fails otherwise). You can do so with ```shell python -m pip install "spacy-llm
-[transformers]" "transformers[sentencepiece]" ``` If you don't have access to a
-GPU, you can install `accelerate` and set`device_map=auto` instead, but be
-aware that this may result in some layers getting distributed to the CPU or
-even the hard drive, which may ultimately result in extremely slow queries.
-```shell python -m pip install "accelerate>=0.16.0,<1.0" ``` Example config
-block: ```ini [components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1"
-model = "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description
-| | ------------- | ---------------- | ------- | ------------------------------
------------------------------------------------------------------- | | `model`
-| `str` | | The name of a Dolly model that is supported. | | `config_init` |
-`Dict[str, Any]` | `{}` | Further configuration passed on to the construction
-of the model with `transformers.pipeline()`. | | `config_run` | `Dict[str,
-Any]` | `{}` | Further configuration used during model inference. | Supported
-models (see the [Databricks models page](https://huggingface.co/databricks) on
-Hugging Face for details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-
-v2-7b"` - `"databricks/dolly-v2-12b"` Note that Hugging Face will download this
-model the first time you use it - you can [define the cached directory](https:/
-/huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting
-the environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
+--------------------------- | | `api` | `str` | | The name of a supported API.
+In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
+| Further configuration passed on to the backend. | | `strict` | `bool` |
+`True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
+following settings can be defined in the `config` dictionary: - `model`: one of
+the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
+32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
+`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
+babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
+`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
+For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
+completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
+srush/MiniChain) for the API retrieval part, make sure you have installed it
+first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
+spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
+MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
+blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
+api = "OpenAI" [components.llm.backend.query] @llm_queries =
+"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
+--- | -------------------------------------------------------------------------
+-------- | ------- | ----------------------------------------------------------
+------------------------- | | `api` | `str` | | The name of an API supported by
+MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
+Function that executes the prompts. If `None`, defaults to
+`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
+executes the prompts by running `model(text).run()` for each given textual
+prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
+hwchase17/langchain) for the API retrieval part, make sure you have installed
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
+with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
+that LangChain currently only supports Python 3.9 and beyond. Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
+= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
+- | ---------------------------------------------------------------------------
+--- | ------- | ---------------------------------------------------------------
+--------------------- | | `api` | `str` | | The name of an API supported by
+LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
+that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
+`model(text)` for each given textual prompt. #### spacy.Dolly_HF.v1 To use this
+backend, ideally you have a GPU enabled and have installed `transformers`,
+`torch` and CUDA in your virtual environment. This allows you to have the
+setting `device=cuda:0` in your config, which ensures that the model is loaded
+entirely on the GPU (and fails otherwise). You can do so with ```shell python -
+m pip install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If
+you don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" model =
+"databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
+--------- | ---------------- | ------- | --------------------------------------
+---------------------------------------------------------- | | `model` | `str`
+| | The name of a Dolly model that is supported. | | `config_init` | `Dict[str,
+Any]` | `{}` | Further configuration passed on to the construction of the model
+with `transformers.pipeline()`. | | `config_run` | `Dict[str, Any]` | `{}` |
+Further configuration used during model inference. | Supported models (see the
+[Databricks models page](https://huggingface.co/databricks) on Hugging Face for
+details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` -
+`"databricks/dolly-v2-12b"` Note that Hugging Face will download this model the
+first time you use it - you can [define the cached directory](https://
+huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
+environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
 `torch` and CUDA in your virtual environment. You can do so with ```shell
 python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ``` If you don't have access to a GPU, you can install `accelerate` and
 set`device_map=auto` instead, but be aware that this may result in some layers
 getting distributed to the CPU or even the hard drive, which may ultimately
 result in extremely slow queries. ```shell python -m pip install
```

### Comparing `spacy-llm-0.3.0/pyproject.toml` & `spacy-llm-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 select = [
     "E",    # pycodestyle errors
     "W",    # pycodestyle warnings
     "F",    # Pyflakes
     "Q",    # flake8-quotes
     "T201"  # flake8-print
 ]
+typing-modules = ['spacy_llm.compat']
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 filterwarnings = [
     "error",
     "ignore:^.*pkg_resources.*:DeprecationWarning",
     "ignore:.*function is now available as sqlalchemy.orm.declarative_base().*:",
```

### Comparing `spacy-llm-0.3.0/setup.cfg` & `spacy-llm-0.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.3.0
+version = 0.3.1
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/integration/hf/base.py` & `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/integration/hf/dolly.py` & `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/integration/hf/openllama.py` & `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/integration/hf/stablelm.py` & `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/integration/remote/base.py` & `spacy-llm-0.3.1/spacy_llm/backends/integration/remote/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/integration/remote/langchain.py` & `spacy-llm-0.3.1/spacy_llm/backends/integration/remote/langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/integration/remote/minichain.py` & `spacy-llm-0.3.1/spacy_llm/backends/integration/remote/minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/rest/anthropic.py` & `spacy-llm-0.3.1/spacy_llm/backends/rest/anthropic.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/rest/base.py` & `spacy-llm-0.3.1/spacy_llm/backends/rest/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/rest/cohere.py` & `spacy-llm-0.3.1/spacy_llm/backends/rest/cohere.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/rest/noop.py` & `spacy-llm-0.3.1/spacy_llm/backends/rest/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/rest/openai.py` & `spacy-llm-0.3.1/spacy_llm/backends/rest/openai.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/backends/rest/registry.py` & `spacy-llm-0.3.1/spacy_llm/backends/rest/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/cache.py` & `spacy-llm-0.3.1/spacy_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/compat.py` & `spacy-llm-0.3.1/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/pipeline/llm.py` & `spacy-llm-0.3.1/spacy_llm/pipeline/llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from spacy.tokens import Doc
 from spacy.training import Example
 from spacy.ty import InitializableComponent as Initializable
 from spacy.vocab import Vocab
 
 from .. import registry  # noqa: F401
 from ..compat import TypedDict
-from ..ty import Cache, LLMTask, PromptExecutor, Scorable, Serializable, validate_types
+from ..ty import Cache, Labeled, LLMTask, PromptExecutor, Scorable, Serializable
+from ..ty import validate_type_consistency
 
 logger = logging.getLogger("spacy_llm")
 logger.addHandler(logging.NullHandler())
 
 
 class CacheConfigType(TypedDict):
     path: Optional[Path]
@@ -42,41 +43,45 @@
         "cache": {
             "@llm_misc": "spacy.BatchCache.v1",
             "path": None,
             "batch_size": 64,
             "max_batches_in_mem": 4,
         },
         "save_io": False,
+        "validate_types": True,
     },
 )
 def make_llm(
     nlp: Language,
     name: str,
     task: Optional[LLMTask],
     backend: PromptExecutor,
     cache: Cache,
     save_io: bool,
+    validate_types: bool,
 ) -> "LLMWrapper":
     """Construct an LLM component.
 
     nlp (Language): Pipeline.
     name (str): The component instance name, used to add entries to the
         losses during training.
     task (Optional[LLMTask]): An LLMTask can generate prompts for given docs, and can parse the LLM's responses into
         structured information and set that back on the docs.
     backend (Callable[[Iterable[Any]], Iterable[Any]]]): Callable querying the specified LLM API.
     cache (Cache): Cache to use for caching prompts and responses per doc (batch).
     save_io (bool): Whether to save LLM I/O (prompts and responses) in the `Doc._.llm_io` custom extension.
+    validate_types (bool): Whether to check if signatures of configured backend and task are consistent.
     """
     if task is None:
         raise ValueError(
             "Argument `task` has not been specified, but is required (e. g. {'@llm_tasks': "
             "'spacy.NER.v2'})."
         )
-    validate_types(task, backend)
+    if validate_types:
+        validate_type_consistency(task, backend)
 
     return LLMWrapper(
         name=name,
         task=task,
         save_io=save_io,
         backend=backend,
         cache=cache,
@@ -118,14 +123,25 @@
 
         # This is done this way because spaCy's `validate_init_settings` function
         # does not support `**kwargs: Any`.
         # See https://github.com/explosion/spaCy/blob/master/spacy/schemas.py#L111
         if isinstance(self._task, Initializable):
             self.initialize = self._task.initialize
 
+    @property
+    def labels(self) -> Tuple[str, ...]:
+        labels: Tuple[str, ...] = tuple()
+        if isinstance(self._task, Labeled):
+            labels = self._task.labels
+        return labels
+
+    @property
+    def task(self) -> LLMTask:
+        return self._task
+
     def __call__(self, doc: Doc) -> Doc:
         """Apply the LLM wrapper to a Doc instance.
 
         doc (Doc): The Doc instance to process.
         RETURNS (Doc): The processed Doc.
         """
         docs = self._process_docs([doc])
```

### Comparing `spacy-llm-0.3.0/spacy_llm/registry/normalizer.py` & `spacy-llm-0.3.1/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/registry/reader.py` & `spacy-llm-0.3.1/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/__init__.py` & `spacy-llm-0.3.1/spacy_llm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/lemma.py` & `spacy-llm-0.3.1/spacy_llm/tasks/lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/ner.py` & `spacy-llm-0.3.1/spacy_llm/tasks/ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 @registry.llm_tasks("spacy.NER.v1")
 def make_ner_task(
     labels: str = "",
     examples: Optional[Callable[[], Iterable[Any]]] = None,
     normalizer: Optional[Callable[[str], str]] = None,
-    alignment_mode: Literal["strict", "contract", "expand"] = "contract",  # noqa: F821
+    alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
     """NER.v1 task factory.
 
     labels (str): Comma-separated list of labels to pass to the template.
         Leave empty to populate it at initialization time (only if examples are provided).
@@ -63,15 +63,15 @@
 @registry.llm_tasks("spacy.NER.v2")
 def make_ner_task_v2(
     labels: Union[List[str], str] = [],
     template: str = _DEFAULT_NER_TEMPLATE_V2,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
-    alignment_mode: Literal["strict", "contract", "expand"] = "contract",  # noqa: F821
+    alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
     """NER.v2 task factory.
 
     labels (Union[str, List[str]]): List of labels to pass to the template,
         either an actual list or a comma-separated string.
@@ -110,17 +110,15 @@
     def __init__(
         self,
         labels: List[str] = [],
         template: str = _DEFAULT_NER_TEMPLATE_V2,
         label_definitions: Optional[Dict[str, str]] = None,
         examples: Optional[List[SpanExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
-        alignment_mode: Literal[
-            "strict", "contract", "expand"  # noqa: F821
-        ] = "contract",
+        alignment_mode: Literal["strict", "contract", "expand"] = "contract",
         case_sensitive_matching: bool = False,
         single_match: bool = False,
     ):
         """Default NER task.
 
         labels (List[str]): List of labels to pass to the template.
             Leave empty to populate it at initialization time (only if examples are provided).
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/noop.py` & `spacy-llm-0.3.1/spacy_llm/tasks/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/rel.py` & `spacy-llm-0.3.1/spacy_llm/tasks/rel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Dict, Iterable, List, Optional, Type, Union
+from typing import Callable, Dict, Iterable, List, Optional, Tuple, Type, Union
 
 import jinja2
 from pydantic import BaseModel, Field, ValidationError, validator
 from spacy.language import Language
 from spacy.tokens import Doc
 from spacy.training import Example
 from wasabi import msg
@@ -133,14 +133,18 @@
 
     @classmethod
     def _check_rel_extention(cls):
         """Add `rel` extension if need be."""
         if not Doc.has_extension("rel"):
             Doc.set_extension("rel", default=[])
 
+    @property
+    def labels(self) -> Tuple[str, ...]:
+        return tuple(self._label_dict.values())
+
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=_preannotate(doc),
                 labels=list(self._label_dict.values()),
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/spancat.py` & `spacy-llm-0.3.1/spacy_llm/tasks/spancat.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 @registry.llm_tasks("spacy.SpanCat.v1")
 def make_spancat_task(
     labels: str = "",
     examples: Optional[Callable[[], Iterable[Any]]] = None,
     normalizer: Optional[Callable[[str], str]] = None,
-    alignment_mode: Literal["strict", "contract", "expand"] = "contract",  # noqa: F821
+    alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
     """SpanCat.v1 task factory.
 
     labels (str): Comma-separated list of labels to pass to the template.
         Leave empty to populate it at initialization time (only if examples are provided).
@@ -62,15 +62,15 @@
 @registry.llm_tasks("spacy.SpanCat.v2")
 def make_spancat_task_v2(
     labels: Union[List[str], str] = [],
     template: str = _DEFAULT_SPANCAT_TEMPLATE_V2,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
-    alignment_mode: Literal["strict", "contract", "expand"] = "contract",  # noqa: F821
+    alignment_mode: Literal["strict", "contract", "expand"] = "contract",
     case_sensitive_matching: bool = False,
     single_match: bool = False,
 ):
     """SpanCat.v2 task factory.
 
     labels (Union[str, List[str]]): List of labels to pass to the template,
         either an actual list or a comma-separated string.
@@ -110,17 +110,15 @@
         self,
         labels: List[str] = [],
         template: str = _DEFAULT_SPANCAT_TEMPLATE_V2,
         label_definitions: Optional[Dict[str, str]] = None,
         spans_key: str = "sc",
         examples: Optional[List[SpanExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
-        alignment_mode: Literal[
-            "strict", "contract", "expand"  # noqa: F821
-        ] = "contract",
+        alignment_mode: Literal["strict", "contract", "expand"] = "contract",
         case_sensitive_matching: bool = False,
         single_match: bool = False,
     ):
         """Default SpanCat task.
 
         labels (List[str]): List of labels to pass to the template.
             Leave empty to populate it at initialization time (only if examples are provided).
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/lemma.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/lemma.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/textcat.py` & `spacy-llm-0.3.1/spacy_llm/tasks/textcat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Iterable, List, Optional, Type, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, Union
 
 import jinja2
 from pydantic import BaseModel
 from spacy.language import Language
 from spacy.scorer import Scorer
 from spacy.tokens import Doc
 from spacy.training import Example
@@ -245,14 +245,18 @@
         if self._use_binary and not self._exclusive_classes:
             msg.warn(
                 "Binary classification should always be exclusive. Setting "
                 "the `exclusive_classes` parameter to True."
             )
             self._exclusive_classes = True
 
+    @property
+    def labels(self) -> Tuple[str, ...]:
+        return tuple(self._label_dict.values())
+
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
                 labels=list(self._label_dict.values()),
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.3.1/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/util/serialization.py` & `spacy-llm-0.3.1/spacy_llm/tasks/util/serialization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tasks/util/span.py` & `spacy-llm-0.3.1/spacy_llm/tasks/util/span.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         self._label_definitions = label_definitions
         self._examples = examples
         self._validate_alignment(alignment_mode)
         self._alignment_mode = alignment_mode
         self._case_sensitive_matching = case_sensitive_matching
         self._single_match = single_match
 
+    @property
+    def labels(self) -> Tuple[str, ...]:
+        return tuple(self._label_dict.values())
+
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
                 labels=list(self._label_dict.values()),
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_anthropic.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_cohere.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_cohere.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_dolly.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_langchain.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_minichain.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_openllama.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_rest.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/backends/test_stablelm.py` & `spacy-llm-0.3.1/spacy_llm/tests/backends/test_stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/conftest.py` & `spacy-llm-0.3.1/spacy_llm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.3.1/spacy_llm/tests/pipeline/test_llm.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import sys
 import warnings
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
 import pytest
 import spacy
+from confection import Config
 from spacy.language import Language
 from spacy.tokens import Doc
 from thinc.api import NumpyOps, get_current_ops
 
 import spacy_llm
 from spacy_llm.backends.rest.noop import _NOOP_RESPONSE
 from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import registry
 from spacy_llm.tasks import make_noop_task
 from spacy_llm.tasks.noop import _NOOP_PROMPT
 
 from ...cache import BatchCache
+from ...util import assemble_from_config
 from ..compat import has_openai_key
 
 
 @pytest.fixture
 def noop_config() -> Dict[str, Any]:
     """Returns NoOp config.
     RETURNS (Dict[str, Any]): NoOp config.
@@ -166,14 +168,19 @@
     )
     assert (
         str(record[1].message)
         == "Type returned from `backend` (`typing.Iterable[str]`) doesn't match type "
         "expected by `task.parse_responses()` (`typing.Iterable[float]`)."
     )
 
+    # Run with disabled type consistency validation.
+    nlp = spacy.blank("en")
+    noop_config["validate_types"] = False
+    nlp.add_pipe("llm", config=noop_config)
+
 
 @pytest.mark.parametrize("use_pipe", [True, False])
 def test_llm_logs_at_debug_level(
     nlp: Language, use_pipe: bool, caplog: pytest.LogCaptureFixture
 ):
     with caplog.at_level(logging.INFO):
         if use_pipe:
@@ -221,7 +228,41 @@
     spacy_llm.logger.removeHandler(stream_handler)
 
     doc = nlp("This is a test with no handler")
     captured = capsys.readouterr()
     assert f"Generated prompt for doc: {doc.text}" not in captured.out
     assert "Don't do anything" not in captured.out
     assert f"LLM response for doc: {doc.text}" not in captured.out
+
+
+@pytest.mark.external
+@pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
+def test_pipe_labels():
+    """Test pipe labels with serde."""
+
+    cfg_string = """
+    [nlp]
+    lang = "en"
+    pipeline = ["llm"]
+
+    [components]
+
+    [components.llm]
+    factory = "llm"
+
+    [components.llm.task]
+    @llm_tasks = "spacy.TextCat.v2"
+    labels = ["COMPLIMENT", "INSULT"]
+
+    [components.llm.backend]
+    @llm_backends = "spacy.REST.v1"
+    api = "OpenAI"
+    config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
+    """
+
+    config = Config().from_str(cfg_string)
+    nlp = assemble_from_config(config)
+
+    with spacy.util.make_tempdir() as tmpdir:
+        nlp.to_disk(tmpdir / "tst.nlp")
+        nlp = spacy.load(tmpdir / "tst.nlp")
+        assert nlp.pipe_labels["llm"] == ["COMPLIMENT", "INSULT"]
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.json` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.jsonl` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.yml` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/rel_examples.jsonl` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_lemma.py` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.tokens import Span
 from spacy.training import Example
 from spacy.util import make_tempdir
 
+from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import fewshot_reader, file_reader, lowercase_normalizer
 from spacy_llm.registry import strip_normalizer
 from spacy_llm.tasks.ner import NERTask, make_ner_task_v2
 from spacy_llm.tasks.util import find_substrings
-from spacy_llm.util import assemble_from_config
+from spacy_llm.ty import Labeled, LLMTask
+from spacy_llm.util import assemble_from_config, split_labels
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 TEMPLATES_DIR = Path(__file__).parent / "templates"
 
 
@@ -197,14 +199,26 @@
     component_cfg = dict(orig_config["components"]["llm"])
     component_cfg.pop("factory")
 
     nlp2 = spacy.blank("en")
     nlp2.add_pipe("llm", config=component_cfg)
     assert nlp2.pipe_names == ["llm"]
 
+    pipe = nlp.get_pipe("llm")
+    assert isinstance(pipe, LLMWrapper)
+    assert isinstance(pipe.task, LLMTask)
+
+    labels = orig_config["components"]["llm"]["task"]["labels"]
+    labels = split_labels(labels)
+    task = pipe.task
+    assert isinstance(task, Labeled)
+    assert task.labels == tuple(labels)
+    assert pipe.labels == task.labels
+    assert nlp.pipe_labels["llm"] == list(task.labels)
+
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize(
     "cfg_string",
     [
         "zeroshot_cfg_string",
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_rel.py` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_rel.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 import pytest
 from confection import Config
 from pytest import FixtureRequest
 from spacy.tokens import Span
 from spacy.training import Example
 
+from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.tasks.rel import RelationItem, RELTask
-from spacy_llm.util import assemble_from_config
+from spacy_llm.ty import Labeled, LLMTask
+from spacy_llm.util import assemble_from_config, split_labels
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 
 
 @pytest.fixture
@@ -109,20 +111,31 @@
     return text, gold_relations
 
 
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
 def test_rel_config(cfg_string, request: FixtureRequest):
     """Simple test to check if the config loads properly given different settings"""
-
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = assemble_from_config(orig_config)
     assert nlp.pipe_names == ["ner", "llm"]
 
+    pipe = nlp.get_pipe("llm")
+    assert isinstance(pipe, LLMWrapper)
+    assert isinstance(pipe.task, LLMTask)
+
+    task = pipe.task
+    labels = orig_config["components"]["llm"]["task"]["labels"]
+    labels = split_labels(labels)
+    assert isinstance(task, Labeled)
+    assert task.labels == tuple(labels)
+    assert pipe.labels == task.labels
+    assert nlp.pipe_labels["llm"] == list(task.labels)
+
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
 def test_rel_predict(task, cfg_string, request):
     """Use OpenAI to get REL results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed to be consistent/predictable
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_spancat.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.tokens import Span
 from spacy.training import Example
 from spacy.util import make_tempdir
 
+from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import fewshot_reader, lowercase_normalizer, strip_normalizer
 from spacy_llm.tasks import make_spancat_task_v2
 from spacy_llm.tasks.spancat import SpanCatTask
 from spacy_llm.tasks.util import find_substrings
-from spacy_llm.util import assemble_from_config
+from spacy_llm.ty import Labeled, LLMTask
+from spacy_llm.util import assemble_from_config, split_labels
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 
 
 @pytest.fixture
@@ -83,14 +85,26 @@
 @pytest.mark.parametrize("cfg_string", ["fewshot_cfg_string", "zeroshot_cfg_string"])
 def test_spancat_config(cfg_string, request):
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
+    pipe = nlp.get_pipe("llm")
+    assert isinstance(pipe, LLMWrapper)
+    assert isinstance(pipe.task, LLMTask)
+
+    labels = orig_config["components"]["llm"]["task"]["labels"]
+    labels = split_labels(labels)
+    task = pipe.task
+    assert isinstance(task, Labeled)
+    assert task.labels == tuple(labels)
+    assert pipe.labels == task.labels
+    assert nlp.pipe_labels["llm"] == list(task.labels)
+
 
 @pytest.mark.external
 @pytest.mark.parametrize("cfg_string", ["zeroshot_cfg_string", "fewshot_cfg_string"])
 def test_spancat_predict(cfg_string, request):
     """Use OpenAI to get zero-shot NER results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed to be consistent/predictable
     """
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_textcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.training import Example
 from spacy.util import make_tempdir
 
+from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import fewshot_reader, file_reader, lowercase_normalizer
 from spacy_llm.registry import registry
 from spacy_llm.tasks.textcat import TextCatTask, make_textcat_task_v3
-from spacy_llm.util import assemble_from_config
+from spacy_llm.ty import Labeled, LLMTask
+from spacy_llm.util import assemble_from_config, split_labels
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 TEMPLATES_DIR = Path(__file__).parent / "templates"
 
 
@@ -205,14 +207,25 @@
         overrides["components.llm.task.examples.path"] = examples
 
     cfg_string = request.getfixturevalue(cfg_string)
     orig_config = Config().from_str(cfg_string, overrides=overrides)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
+    pipe = nlp.get_pipe("llm")
+    assert isinstance(pipe, LLMWrapper)
+    assert isinstance(pipe.task, LLMTask)
+
+    labels = split_labels(labels)
+    task = pipe.task
+    assert isinstance(task, Labeled)
+    assert task.labels == tuple(labels)
+    assert pipe.labels == task.labels
+    assert nlp.pipe_labels["llm"] == list(task.labels)
+
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("task", ["binary", "multilabel_nonexcl", "multilabel_excl"])
 @pytest.mark.parametrize(
     "cfg_string",
     [
```

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/test_cache.py` & `spacy-llm-0.3.1/spacy_llm/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.3.1/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm/ty.py` & `spacy-llm-0.3.1/spacy_llm/ty.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,28 +58,36 @@
 @runtime_checkable
 class Scorable(Protocol):
     def scorer(
         self,
         examples: Iterable[Example],
     ) -> Dict[str, Any]:
         """Scores performance on examples."""
+        ...
 
 
 @runtime_checkable
 class LLMTask(Protocol):
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[_Prompt]:
         ...
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[_Response]
     ) -> Iterable[Doc]:
         ...
 
 
 @runtime_checkable
+class Labeled(Protocol):
+    @property
+    def labels(self) -> Tuple[str, ...]:
+        ...
+
+
+@runtime_checkable
 class Cache(Protocol):
     """Defines minimal set of operations a cache implementiation needs to support."""
 
     @property
     def vocab(self) -> Optional[Vocab]:
         """Vocab used for deserializing docs.
         RETURNS (Vocab): Vocab used for deserializing docs.
@@ -164,16 +172,19 @@
         if k not in to_ignore
     }
     assert len(signature) == 2
     assert "return" in signature
     return signature
 
 
-def validate_types(task: LLMTask, backend: PromptExecutor) -> None:
-    # Inspect the types of the three main parameters to ensure they match internally
+def validate_type_consistency(task: LLMTask, backend: PromptExecutor) -> None:
+    """Check whether the types of the task and backend signatures match.
+    task (LLMTask): Specified task.
+    backend (PromptExecutor): Specified backend.
+    """
     # Raises an error or prints a warning if something looks wrong/odd.
     if not isinstance(task, LLMTask):
         raise ValueError(
             f"A task needs to be of type 'LLMTask' but found {type(task)} instead"
         )
     if not hasattr(task, "generate_prompts"):
         raise ValueError(
```

### Comparing `spacy-llm-0.3.0/spacy_llm/util.py` & `spacy-llm-0.3.1/spacy_llm/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: spacy-llm
-Version: 0.3.0
-Summary: Integrating LLMs into structured NLP pipelines
-Author: Explosion
-Author-email: contact@explosion.ai
-License: MIT
-Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
-Project-URL: Source, https://github.com/explosion/spacy-llm
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: minichain
-Provides-Extra: langchain
-Provides-Extra: transformers
-License-File: LICENSE
-
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
@@ -247,20 +215,18 @@
 
 spacy_llm.logger.addHandler(logging.StreamHandler())
 spacy_llm.logger.setLevel(logging.DEBUG)
 ```
 
 > NOTE: Any `logging` handler will work here so you probably want to use some sort of rotating `FileHandler` as the generated prompts can be quite long, especially for tasks with few-shot examples.
 
-
 Then when using the pipeline you'll be able to view the prompt and response.
 
 E.g. with the config and code from [Example 1](##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
 
-
 ```python
 from spacy_llm.util import assemble
 
 
 nlp = assemble("config.cfg")
 doc = nlp("You look gorgeous!")
 print(doc.cats)
@@ -298,20 +264,21 @@
 {'COMPLIMENT': 1.0, 'INSULT': 0.0}
 ```
 
 ## 📓 API
 
 `spacy-llm` exposes a `llm` factory that accepts the following configuration options:
 
-| Argument  | Type                                        | Description                                                                         |
-| --------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
-| `task`    | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
-| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
-| `cache`   | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
-| `save_io` | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`                  |
+| Argument         | Type                                        | Description                                                                         |
+| ---------------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
+| `task`           | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
+| `backend`        | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
+| `cache`          | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
+| `save_io`        | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`.                 |
+| `validate_types` | `bool`                                      | Whether to check if signatures of configured backend and task are consistent.       |
 
 An `llm` component is defined by two main settings:
 
 - A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
 - A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
@@ -321,14 +288,18 @@
 
 Finally, you can choose to save a stringified version of LLM prompts/responses
 within the `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
 `Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM component
 within the spaCy pipeline. Each entry is itself a dictionary, with two keys:
 `prompt` and `response`.
 
+A note on `validate_types`: by default, `spacy-llm` checks whether the signatures of the `backend` and `task` callables
+are consistent with each other and emits a warning if they don't. `validate_types` can be set to `False` if you want to
+disable this behavior.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -683,35 +654,36 @@
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.Lemma.v1"
 examples = null
 ```
 
-| Argument                  | Type                                    | Default                                                   | Description                                                                                                                                           |
-| ------------------------- | --------------------------------------- |-----------------------------------------------------------| ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `template`                | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
-| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                    | Optional function that generates examples for few-shot learning.                                                                                      |
+| Argument   | Type                                    | Default                                                | Description                                                                                                                              |
+| ---------- | --------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
+| `template` | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
+| `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                 | Optional function that generates examples for few-shot learning.                                                                         |
 
 `Lemma.v1` prompts the LLM to lemmatize the passed text and return the lemmatized version as a list of tokens and their
-corresponding lemma. E. g. the text 
+corresponding lemma. E. g. the text
 `I'm buying ice cream for my friends` should invoke the response
+
 ```
 I: I
 'm: be
 buying: buy
 ice: ice
 cream: cream
 for: for
 my: my
 friends: friend
 .: .
 ```
 
-If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized 
+If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized
 by spaCy, no lemmas are stored in the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is updated with
 the lemma suggested by the LLM.
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
 The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
 
 ```yaml
@@ -721,15 +693,15 @@
     - "'m": "be"
     - "buying": "buy"
     - "ice": "ice"
     - "cream": "cream"
     - ".": "."
 
 - text: I've watered the plants.
-  lemmas: 
+  lemmas:
     - "I": "I"
     - "'ve": "have"
     - "watered": "water"
     - "the": "the"
     - "plants": "plant"
     - ".": "."
 ```
```

#### html2text {}

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.0 Summary: Integrating LLMs
-into structured NLP pipelines Author: Explosion Author-email:
-contact@explosion.ai License: MIT Project-URL: Release notes, https://
-github.com/explosion/spacy-llm/releases Project-URL: Source, https://
-github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: minichain Provides-Extra: langchain
-Provides-Extra: transformers License-File: LICENSE [https://explosion.ai/
-assets/img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP
-pipelines [![GitHub Workflow Status](https://img.shields.io/github/actions/
-workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/
-explosion/spacy-llm/actions/workflows/test.yml) [![pypi Version](https://
-img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
+structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
+github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
+(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
+Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/ambv/black) This package
 integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
 featuring a modular system for **fast prototyping** and **prompting**, and
 turning unstructured responses into **robust outputs** for various NLP tasks,
 **no training data** required. - Serializable `llm` **component** to integrate
@@ -153,39 +136,44 @@
 example: Label1, Label2, Label3. Do not put any other text in your answer, only
 one or more of the provided labels with nothing before or after. If the text
 cannot be classified into any of the provided labels, answer `==NONE==`. Here
 is the text that needs classification Text: ''' You look gorgeous! ''' Backend
 response for doc: You look gorgeous! COMPLIMENT ``` `print(doc.cats)` to
 standard output should look like: ``` {'COMPLIMENT': 1.0, 'INSULT': 0.0} ``` ##
 ð API `spacy-llm` exposes a `llm` factory that accepts the following
-configuration options: | Argument | Type | Description | | --------- | --------
------------------------------------ | -----------------------------------------
------------------------------------------- | | `task` | `Optional[LLMTask]` |
-An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks). |
-| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a
-specific LLM API. See [docs](#backends). | | `cache` | `Cache` | Cache to use
-for caching prompts and responses per doc (batch). See [docs](#cache). | |
-`save_io` | `bool` | Whether to save prompts/responses within `Doc.user_data
-["llm_io"]` | An `llm` component is defined by two main settings: - A
-[**task**](#tasks), defining the prompt to send to the LLM as well as the
-functionality to parse the resulting response back into structured fields on
-spaCy's [Doc](https://spacy.io/api/doc) objects. - A [**backend**](#backends)
-defining the model to use and how to connect to it. Note that `spacy-llm`
-supports both access to external APIs (such as OpenAI) as well as access to
-self-hosted open-source LLMs (such as using Dolly through Hugging Face).
-Moreover, `spacy-llm` exposes a customizable [**caching**](#cache)
-functionality to avoid running the same document through an LLM service (be it
-local or through a REST API) more than once. Finally, you can choose to save a
-stringified version of LLM prompts/responses within the `Doc.user_data
-["llm_io"]` attribute by setting `save_io` to `True`. `Doc.user_data["llm_io"]`
-is a dictionary containing one entry for every LLM component within the spaCy
-pipeline. Each entry is itself a dictionary, with two keys: `prompt` and
-`response`. ### Tasks A _task_ defines an NLP problem or question, that will be
-sent to the LLM via a prompt. Further, the task defines how to parse the LLM's
-responses back into structured information. All tasks are registered in spaCy's
+configuration options: | Argument | Type | Description | | ---------------- | -
+------------------------------------------ | ----------------------------------
+------------------------------------------------- | | `task` | `Optional
+[LLMTask]` | An LLMTask can generate prompts and parse LLM responses. See
+[docs](#tasks). | | `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` |
+Callable querying a specific LLM API. See [docs](#backends). | | `cache` |
+`Cache` | Cache to use for caching prompts and responses per doc (batch). See
+[docs](#cache). | | `save_io` | `bool` | Whether to save prompts/responses
+within `Doc.user_data["llm_io"]`. | | `validate_types` | `bool` | Whether to
+check if signatures of configured backend and task are consistent. | An `llm`
+component is defined by two main settings: - A [**task**](#tasks), defining the
+prompt to send to the LLM as well as the functionality to parse the resulting
+response back into structured fields on spaCy's [Doc](https://spacy.io/api/doc)
+objects. - A [**backend**](#backends) defining the model to use and how to
+connect to it. Note that `spacy-llm` supports both access to external APIs
+(such as OpenAI) as well as access to self-hosted open-source LLMs (such as
+using Dolly through Hugging Face). Moreover, `spacy-llm` exposes a customizable
+[**caching**](#cache) functionality to avoid running the same document through
+an LLM service (be it local or through a REST API) more than once. Finally, you
+can choose to save a stringified version of LLM prompts/responses within the
+`Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
+`Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM
+component within the spaCy pipeline. Each entry is itself a dictionary, with
+two keys: `prompt` and `response`. A note on `validate_types`: by default,
+`spacy-llm` checks whether the signatures of the `backend` and `task` callables
+are consistent with each other and emits a warning if they don't.
+`validate_types` can be set to `False` if you want to disable this behavior.
+### Tasks A _task_ defines an NLP problem or question, that will be sent to the
+LLM via a prompt. Further, the task defines how to parse the LLM's responses
+back into structured information. All tasks are registered in spaCy's
 `llm_tasks` registry. Practically speaking, a task should adhere to the
 `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py). It needs to define
 a `generate_prompts` function and a `parse_responses` function. Moreover, the
 task may define an optional [`scorer` method](https://spacy.io/api/
 scorer#score). It should accept an iterable of `Example`s as input and return a
 score dictionary. If the `scorer` method is defined, `spacy-llm` will call it
 to evaluate the component. #### function `task.generate_prompts` Takes a
@@ -441,148 +429,148 @@
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
 [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
 "Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
 = "rel_examples.jsonl" ``` #### spacy.Lemma.v1 The `Lemma.v1` task lemmatizes
 the provided text and updates the `lemma_` attribute in the doc's tokens
 accordingly. ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
-examples = null ``` | Argument | Type | Default | Description | | -------------
------------- | --------------------------------------- |-----------------------
-------------------------------------| -----------------------------------------
+examples = null ``` | Argument | Type | Default | Description | | ---------- |
+--------------------------------------- | -------------------------------------
+----------------- | -----------------------------------------------------------
+----------------------------------------------------------------------------- |
+| `template` | `str` | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) |
+Custom prompt template to send to LLM backend. Default templates for each task
+are located in the `spacy_llm/tasks/templates` directory. | | `examples` |
+`Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
+generates examples for few-shot learning. | `Lemma.v1` prompts the LLM to
+lemmatize the passed text and return the lemmatized version as a list of tokens
+and their corresponding lemma. E. g. the text `I'm buying ice cream for my
+friends` should invoke the response ``` I: I 'm: be buying: buy ice: ice cream:
+cream for: for my: my friends: friend .: . ``` If for any given text/doc
+instance the number of lemmas returned by the LLM doesn't match the number of
+tokens recognized by spaCy, no lemmas are stored in the corresponding doc's
+tokens. Otherwise the tokens `.lemma_` property is updated with the lemma
+suggested by the LLM. To perform few-shot learning, you can write down a few
+examples in a separate file, and provide these to be injected into the prompt
+to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+`.yaml`, `.json` and `.jsonl`. ```yaml - text: I'm buying ice cream. lemmas: -
+"I": "I" - "'m": "be" - "buying": "buy" - "ice": "ice" - "cream": "cream" -
+".": "." - text: I've watered the plants. lemmas: - "I": "I" - "'ve": "have" -
+"watered": "water" - "the": "the" - "plants": "plant" - ".": "." ``` ```ini
+[components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"lemma_examples.yml" ``` #### spacy.NoOp.v1 This task is only useful for
+testing - it tells the LLM to do nothing, and does not set any fields on the
+`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
+Backends A _backend_ defines which LLM model to query, and how to query it. It
+can be a simple function taking a collection of prompts (consistent with the
+output type of `task.generate_prompts()`) and returning a collection of
+responses (consistent with the expected input of `parse_responses`). Generally
+speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
+but specific implementations can have other signatures, like `Callable[
+[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
+`llm_backends`. If no backend is specified, the repo currently connects to the
+[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
+accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
+third-party libraries in addition to a native REST backend and which should > I
+choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
+prompt management, integration of many different LLM > APIs, and other related
+features such as conversational memory or agents. `spacy-llm` on the other hand
+emphasizes > features we consider useful in the context of NLP pipelines
+utilizing LLMs to process documents (mostly) independent > from each other. It
+makes sense that the feature set of such third-party libraries and `spacy-llm`
+is not identical - > and users might want to take advantage of features not
+available in `spacy-llm`. > > The advantage of offering our own REST backend is
+that we can ensure a larger degree of stability of robustness, as > we can
+guarantee backwards-compatibility and more smoothly integrated error handling.
+> > Ultimately we recommend trying to implement your use case using the REST
+backend first (which is configured as the > default backend). If however there
+are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
+> backend of a third-party library - and easy to customize the prompting
+mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
+to get an API key from openai.com, and ensure that the keys are set as
+environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
+OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
+`requests` and a simple retry mechanism to access an API. ```ini
+[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
+= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
+Default | Description | | ----------- | ---------------- | ------- | ----------
 -------------------------------------------------------------------------------
------------------------------ | | `template` | `str` | [lemma.jinja](./
-spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM
-backend. Default templates for each task are located in the `spacy_llm/tasks/
-templates` directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
-| `None` | Optional function that generates examples for few-shot learning. |
-`Lemma.v1` prompts the LLM to lemmatize the passed text and return the
-lemmatized version as a list of tokens and their corresponding lemma. E. g. the
-text `I'm buying ice cream for my friends` should invoke the response ``` I: I
-'m: be buying: buy ice: ice cream: cream for: for my: my friends: friend .: .
-``` If for any given text/doc instance the number of lemmas returned by the LLM
-doesn't match the number of tokens recognized by spaCy, no lemmas are stored in
-the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is
-updated with the lemma suggested by the LLM. To perform few-shot learning, you
-can write down a few examples in a separate file, and provide these to be
-injected into the prompt to the LLM. The default reader
-`spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
-```yaml - text: I'm buying ice cream. lemmas: - "I": "I" - "'m": "be" -
-"buying": "buy" - "ice": "ice" - "cream": "cream" - ".": "." - text: I've
-watered the plants. lemmas: - "I": "I" - "'ve": "have" - "watered": "water" -
-"the": "the" - "plants": "plant" - ".": "." ``` ```ini [components.llm.task]
-@llm_tasks = "spacy.Lemma.v1" [components.llm.task.examples] @misc =
-"spacy.FewShotReader.v1" path = "lemma_examples.yml" ``` #### spacy.NoOp.v1
-This task is only useful for testing - it tells the LLM to do nothing, and does
-not set any fields on the `docs`. ```ini [components.llm.task] @llm_tasks =
-"spacy.NoOp.v1" ``` ### Backends A _backend_ defines which LLM model to query,
-and how to query it. It can be a simple function taking a collection of prompts
-(consistent with the output type of `task.generate_prompts()`) and returning a
-collection of responses (consistent with the expected input of
-`parse_responses`). Generally speaking, it's a function of type `Callable[
-[Iterable[Any]], Iterable[Any]]`, but specific implementations can have other
-signatures, like `Callable[[Iterable[str]], Iterable[str]]`. All built-in
-backends are registered in `llm_backends`. If no backend is specified, the repo
-currently connects to the [`OpenAI` API](#openai) by default, using the built-
-in REST protocol, and accesses the `"gpt-3.5-turbo"` model. > :question: _Why
-are there backends for third-party libraries in addition to a native REST
-backend and which should > I choose?_ > > Third-party libraries like
-`langchain` or `minichain` focus on prompt management, integration of many
-different LLM > APIs, and other related features such as conversational memory
-or agents. `spacy-llm` on the other hand emphasizes > features we consider
-useful in the context of NLP pipelines utilizing LLMs to process documents
-(mostly) independent > from each other. It makes sense that the feature set of
-such third-party libraries and `spacy-llm` is not identical - > and users might
-want to take advantage of features not available in `spacy-llm`. > > The
-advantage of offering our own REST backend is that we can ensure a larger
-degree of stability of robustness, as > we can guarantee backwards-
-compatibility and more smoothly integrated error handling. > > Ultimately we
-recommend trying to implement your use case using the REST backend first (which
-is configured as the > default backend). If however there are features or APIs
-not covered by `spacy-llm`, it's trivial to switch to the > backend of a third-
-party library - and easy to customize the prompting mechanism, if so required.
-#### OpenAI When the backend uses OpenAI, you have to get an API key from
-openai.com, and ensure that the keys are set as environmental variables:
-```shell export OPENAI_API_KEY="sk-..." export OPENAI_API_ORG="org-..." ```
-#### spacy.REST.v1 This default backend uses `requests` and a simple retry
-mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
-"spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-turbo",
-"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
--- | ---------------- | ------- | ---------------------------------------------
------------------------------------------------------------------------ | |
-`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
-supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
-passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
-error if the LLM API returns a malformed response. Otherwise, return the error
-responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
-request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
-When `api` is set to `OpenAI`, the following settings can be defined in the
-`config` dictionary: - `model`: one of the following list of supported models:
-- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
-turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
-- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
-`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
-api.openai.com/v1/completions`. For models requiring the chat endpoint, use
-`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
-[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
-make sure you have installed it first: ```shell python -m pip install
-"minichain>=0.3,<0.4" # Or install with spacy-llm directly python -m pip
-install "spacy-llm[minichain]" ``` Note that MiniChain currently only supports
-Python 3.8, 3.9 and 3.10. Example config blocks: ```ini
-[components.llm.backend] @llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
-[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
-Argument | Type | Default | Description | | -------- | ------------------------
---------------------------------------------------------- | ------- | ---------
--------------------------------------------------------------------------- | |
-`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
-`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
-backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
-Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
-If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
-(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
-for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
-(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
-you have installed it first: ```shell python -m pip install
-"langchain>=0.0.144,<0.1" # Or install with spacy-llm directly python -m pip
-install "spacy-llm[langchain]" ``` Note that LangChain currently only supports
-Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
-@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
-"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
-Default | Description | | -------- | ------------------------------------------
------------------------------------- | ------- | ------------------------------
------------------------------------------------------- | | `api` | `str` | |
-The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
-[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
-`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
-Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
-defaults to `spacy.CallLangChain.v1`. | The default `query`
-(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
-each given textual prompt. #### spacy.Dolly_HF.v1 To use this backend, ideally
-you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
-your virtual environment. This allows you to have the setting `device=cuda:0`
-in your config, which ensures that the model is loaded entirely on the GPU (and
-fails otherwise). You can do so with ```shell python -m pip install "spacy-llm
-[transformers]" "transformers[sentencepiece]" ``` If you don't have access to a
-GPU, you can install `accelerate` and set`device_map=auto` instead, but be
-aware that this may result in some layers getting distributed to the CPU or
-even the hard drive, which may ultimately result in extremely slow queries.
-```shell python -m pip install "accelerate>=0.16.0,<1.0" ``` Example config
-block: ```ini [components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1"
-model = "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description
-| | ------------- | ---------------- | ------- | ------------------------------
------------------------------------------------------------------- | | `model`
-| `str` | | The name of a Dolly model that is supported. | | `config_init` |
-`Dict[str, Any]` | `{}` | Further configuration passed on to the construction
-of the model with `transformers.pipeline()`. | | `config_run` | `Dict[str,
-Any]` | `{}` | Further configuration used during model inference. | Supported
-models (see the [Databricks models page](https://huggingface.co/databricks) on
-Hugging Face for details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-
-v2-7b"` - `"databricks/dolly-v2-12b"` Note that Hugging Face will download this
-model the first time you use it - you can [define the cached directory](https:/
-/huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting
-the environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
+--------------------------- | | `api` | `str` | | The name of a supported API.
+In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
+| Further configuration passed on to the backend. | | `strict` | `bool` |
+`True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
+following settings can be defined in the `config` dictionary: - `model`: one of
+the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
+32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
+`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
+babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
+`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
+For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
+completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
+srush/MiniChain) for the API retrieval part, make sure you have installed it
+first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
+spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
+MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
+blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
+api = "OpenAI" [components.llm.backend.query] @llm_queries =
+"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
+--- | -------------------------------------------------------------------------
+-------- | ------- | ----------------------------------------------------------
+------------------------- | | `api` | `str` | | The name of an API supported by
+MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
+Function that executes the prompts. If `None`, defaults to
+`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
+executes the prompts by running `model(text).run()` for each given textual
+prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
+hwchase17/langchain) for the API retrieval part, make sure you have installed
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
+with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
+that LangChain currently only supports Python 3.9 and beyond. Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
+= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
+- | ---------------------------------------------------------------------------
+--- | ------- | ---------------------------------------------------------------
+--------------------- | | `api` | `str` | | The name of an API supported by
+LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
+that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
+`model(text)` for each given textual prompt. #### spacy.Dolly_HF.v1 To use this
+backend, ideally you have a GPU enabled and have installed `transformers`,
+`torch` and CUDA in your virtual environment. This allows you to have the
+setting `device=cuda:0` in your config, which ensures that the model is loaded
+entirely on the GPU (and fails otherwise). You can do so with ```shell python -
+m pip install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If
+you don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" model =
+"databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
+--------- | ---------------- | ------- | --------------------------------------
+---------------------------------------------------------- | | `model` | `str`
+| | The name of a Dolly model that is supported. | | `config_init` | `Dict[str,
+Any]` | `{}` | Further configuration passed on to the construction of the model
+with `transformers.pipeline()`. | | `config_run` | `Dict[str, Any]` | `{}` |
+Further configuration used during model inference. | Supported models (see the
+[Databricks models page](https://huggingface.co/databricks) on Hugging Face for
+details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` -
+`"databricks/dolly-v2-12b"` Note that Hugging Face will download this model the
+first time you use it - you can [define the cached directory](https://
+huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
+environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
 `torch` and CUDA in your virtual environment. You can do so with ```shell
 python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ``` If you don't have access to a GPU, you can install `accelerate` and
 set`device_map=auto` instead, but be aware that this may result in some layers
 getting distributed to the CPU or even the hard drive, which may ultimately
 result in extremely slow queries. ```shell python -m pip install
```

### Comparing `spacy-llm-0.3.0/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.3.1/spacy_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.3.1/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.3.1/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.3.1/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/ner_minichain_openai/run_pipeline.py` & `spacy-llm-0.3.1/usage_examples/ner_minichain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.3.1/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.3.1/usage_examples/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.3.1/usage_examples/tests/test_usage_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.0/usage_examples/textcat_openai/run_pipeline.py` & `spacy-llm-0.3.1/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

